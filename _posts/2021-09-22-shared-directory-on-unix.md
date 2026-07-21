---
title: "Unix Shared Directories"
excerpt: "A quick guide to managing file permissions for group collaboration."
header:
  teaser: /assets/images/overlays/grayscale-pond-grass.webp
  og_image: /assets/images/overlays/grayscale-pond-grass.webp
  overlay_image: /assets/images/overlays/grayscale-pond-grass.webp
categories:
  - How-To & Guides
tags:
  - DevOps
  - Unix
  - Linux
toc: true
---

Managing a shared directory in a multi-user Unix environment can be tricky. By default, files created by a user belong to their primary group, and permissions are dictated by their personal `umask`. This often leads to "Permission Denied" errors when another team member tries to edit a file you just created.

This guide covers how to set up a robust shared folder where everything "just works."

## The Quick Setup (TLDR)

The following commands create a group, add users, and set the `setgid` bit on the directory so that all new files inherit the group ownership.

```shell
# 1. Create the group
sudo groupadd sharedgroup

# 2. Add users to the group
sudo usermod -a -G sharedgroup userone
sudo usermod -a -G sharedgroup usertwo

# 3. Create the directory and set ownership
mkdir shareddir
sudo chgrp -R sharedgroup ./shareddir

# 4. Set permissions and the SGID bit
sudo chmod -R 2775 ./shareddir/
```

> **Note:** The `2` in `2775` sets the **setgid** (Set Group ID) bit.

---

## Core Concepts

### 1. The Magic of the SGID Bit
On a directory, the `setgid` (set group ID) bit tells the OS: *"Any file created inside this folder should inherit the group of the folder itself, rather than the primary group of the user who created it."*

- **Command:** `chmod g+s <dir>` or `chmod 2xxx <dir>`
- **Why it matters:** Without this, `userone` creates a file as `userone:userone`. With this, they create it as `userone:sharedgroup`.

### 2. The Umask Problem
Even if the group ownership is correct, the permissions might still be too restrictive. Most Linux systems have a default `umask` of `0022`, which creates files with `644` (rw-r--r--) permissions. This means the group can **read** the file but not **edit** it.

To fix this globally, users need a `umask` of `002`, but changing global umasks can be risky.

### 3. The Modern Solution: ACLs (Access Control Lists)
If your filesystem supports it (most modern Linux distros do), **ACLs** are the most reliable way to handle shared directories. They allow you to set "Default ACLs" that are forced onto every new file, regardless of the user's umask.

```shell
# Set default permissions for the group to rwx
sudo setfacl -d -m g:sharedgroup:rwx ./shareddir

# Set current permissions
sudo setfacl -m g:sharedgroup:rwx ./shareddir
```

---

## Permission Reference Table

Unix permissions are calculated by adding values: **4 (Read), 2 (Write), 1 (Execute)**.

| Symbolic | Numeric | Description |
| :--- | :--- | :--- |
| `rwx------` | `0700` | Full access for owner only |
| `rwxrwx---` | `0770` | Full access for owner and group |
| `rwxr-xr-x` | `0755` | Everyone can read/execute, only owner can write |
| `rw-rw-r--` | `0664` | Owner/Group can read/write, others read-only |
| `rwxrwsr-x` | `2775` | SGID set: Group inheritance + group write access |

---

## Best Practices
* **Avoid 777:** Never give "World" write permissions (`777`) unless you absolutely have to. It's a significant security risk.
* **Sticky Bit:** If you want users to be able to create files but **not delete** each other's files, add the sticky bit: `chmod +t <dir>` or `chmod 1xxx <dir>`.
* **Group Membership:** Remember that users must log out and back in for new group assignments (`usermod -a -G`) to take effect.

For more deep dives into POSIX models, check out the [Linux Documentation Project](https://tldp.org/LDP/lame/LAME/linux-admin-made-easy/local-user-administration.html).

