---
title:  "Creating a shared directory for a group of users"
excerpt: "Shared directories and file permission management on unix"
header:
  teaser: https://i.imgur.com/R7CbUmn.jpg
  og_image: https://i.imgur.com/R7CbUmn.jpg
  overlay_image: https://i.imgur.com/R7CbUmn.jpg
categories:
  - devops
tags:
  - devops
  - unix
  - linux
  

---

TLDR: the following command creates a group and adds two users. We, then, link the group to the
directory and set permissions. Users (userone/usertwo) now will have access to read/write/execute
permission to the directory. Newly created folder and files will be assigned to the same parent group. 

```shell
groupadd sharedgroup
usermod -a -G sharedgroup userone
usermod -a -G sharedgroup usertwo

mkdir shareddir
chgrp -R sharedgroup ./shareddir
chmod -R g+rwx  ./shareddir/
chmod g+s shareddir
```

## Notes:
* The best way to get permission is to assign permissions to groups of users instead of to individuals.
* Permissions are assigned in World Permissions, Group Permissions, and Owner Permissions.
* The three numbers that are shown in the `ls -l` output are the owner's permissions, group permissions, and world permissions respectively, in that order.
* You must be the owner of blob to change its permissions. Enter `ls -la` to see who has file permissions.
* Directory Permission sets default permission for the files and folders created in the directory.



## Setting directory permissions 
The command `chmod <permission> <directory>`is used to set permissions for the files and folders. 
For instance to set a file permission to be readable by others but only modifiable by the owner of the file, 
you could issue:
```
chmod 755 myfile.txt
```
Few common permission codes from [Wikipedia](https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation)
```
Symbolic    Numeric Description
----------	0000	no permissions
-rwx------	0700	read, write, & execute only for owner
-rwxrwx---	0770	read, write, & execute for owner and group
-rwxrwxrwx	0777	read, write, & execute for owner, group and others
---x--x--x	0111	execute
--w--w--w-	0222	write
--wx-wx-wx	0333	write & execute
-r--r--r--	0444	read
-r-xr-xr-x	0555	read & execute
-rw-rw-rw-	0666	read & write
-rwxr-----	0740	owner can read, write, & execute; group can only read; others have no permissions
```
A POSIX (Portable Operating System Interface for Unix) file permission model is used, with the
  first digit representing file type, and permissions for read (4), write (2), and execute (1). [Read more](https://www.guru99.com/file-permissions.html)
