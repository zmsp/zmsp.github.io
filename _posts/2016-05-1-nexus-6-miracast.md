---
title: "Miracast on Nexus 6"
excerpt: "Enable Miracast on Nexus 6"
header:
  teaser: "/images/nexus6-cast.jpg"
  overlay_color: "#8d9eba"
categories:
  - How-To & Guides
tags:
  - Android
  - Tutorial
  - adb
  - screenmirroring
---

**TL;DR:**

1. Connect your device to your PC.
2. Go to recovery mode (AKA TWRP recovery).
3. Mount your system by going to mount and check system.
4. Open ADB on your PC.
5. Run the following commands each line one by one on your ADB shell.

### How to Enable Miracast on Nexus 6 on Android N Preview

Miracast is a wireless display standard designed for mirroring a smartphone, tablet, or PC's screen to a television without requiring any physical HDMI cables. The Nexus 6 hardware supports Miracast. For some reason, Google decided to disable it. I recently bought a Miracast-enabled device but couldn’t project my Nexus 6 screen on my TV. I went on a quest to enable Miracast on Nexus 6. After searching, it seemed that people enabled Miracast on different devices by editing build.prop. However, it seemed that Google has disabled editing that file even when you have root enabled. So apps like BuildProp Editor can’t do it. Without further ado, here is how to enable it.

This process should work on Nexus (P/X) as well as other devices.

#### Prerequisites:

1. Rooted phone.
2. TWRP recovery installed on the phone.
3. Android Debugging Tool (ADB) installed.
4. Device-specific driver installed (PC sees your device).

#### The Process:

1. Connect your device to your PC.
2. Go to recovery mode (AKA TWRP recovery).
3. Mount your system by going to mount and check system.
4. Open ADB on your PC.
5. Run the following commands each line one by one on your ADB shell:

```bash
adb shell # Launches shell inside your phone.
su root # Gives your user root permission.
cp /system/build.props /sdcard/tmp/ # Keep a backup copy of build.prop in tmp.
echo "persist.debug.wfd.enable=1" >> /system/build.props # Appends this line to the file.
chmod 644 /system/build.props # Change permission of build.props.
reboot
```

Now you can go to your Nexus 6 > Settings > Display > Cast > and Enable wireless display.

![nexus 6 miracast cast](/images/nexus6-cast.jpg "Miracast on nexus 6")

