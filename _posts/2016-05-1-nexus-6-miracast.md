---
title:  "Miracast on nexus 6"
excerpt: "Enable miracast on nexus 6"
header:
    teaser: "/images/nexus6-cast.jpg"
    overlay_color: "#8d9eba"
categories: 
  - hardware
tags:
  - nexus 6
  - miracast
  - android
---
tldr:

1.  Connect your device to your PC

2.  Go to recovery mode (AKA twrp recovery)

3.  Mount your system by going to mount and check system

4.  Open adb on your PC

5.  Run




### How to Enable Miracast on Nexus 6 on Android N Preview

Miracast is a wireless display standard designed for mirroring a smartphone, tablet, or PC's screen to a television without requiring any physical HDMI cables. Nexus 6 hardware wise supports miracast. For some reason however, Google decided to disable quite a few different features including miracast. I recently bought a Miracast enabled device but couldn’t project my nexus 6 screen on my TV. I went my one night quest to enable Miracast on nexus 6. After searching it seemed that people enabled Miracast on different devices by editing build.prop. However, it seemed that Google has disabled editing that file even when you have root enabled. So apps like BuildProp Editor can’t Without further due here is how to enable it –

This process should on Nexus (P/X) as well as other devices.

Prerequisites:

1.  Rooted phone

2.  TWRP recovery installed on the phone

3.  Android debugging tool (ADB installed)

4.  Device specific driver installed (PC sees your device)

The Process:

1.  Connect your device to your PC

2.  Go to recovery mode (AKA twrp recovery)

3.  Mount your system by going to mount and check system

4.  Open adb on your PC

5.  Run the following each line one by one on your ADB shell:

```
adb shell # launches shell inside your phone
su root # gives your user root permission
cp /system/build.props /sdcard/tmp/ # keep a backup copy build props in tmp
echo "persist.debug.wfd.enable=1" >> /system/build.props #appends this line to the file
chmod 644 /system/build.props # change permission of build.props
reboot
```

Now you can go to your nexus 6 > Settings> Display> Cast> and Enable wireless display

![nexus 6 miracast cast](/images/nexus6-cast.jpg "Miracast on nexus 6")

