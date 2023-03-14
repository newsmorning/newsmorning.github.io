---
title: "Root horror: Samsung Galaxy S7 Edge rendered useless after accidental OEM unlock disable!"
ShowToc: true 
date: "2022-11-21"
author: "Eva Sabatino"
---
*****
Title: Root horror: Samsung Galaxy S7 Edge rendered useless after accidental OEM unlock disable!

Intro: The Samsung Galaxy S7 Edge has been one of the most popular Android smartphones, but a recent incident has highlighted the dangers of tinkering with the device's settings.

Body:

When a young tech enthusiast named John accidentally disabled the OEM (Original Equipment Manufacturer) unlock on his Samsung Galaxy S7 Edge, he never imagined the horror that would follow.

With OEM unlock disabled, John lost access to his device's bootloader, which is responsible for loading the Android operating system (OS) and other system-level software. This meant that he could not install custom ROMs or kernels, which allow users to modify the OS and add new features.

John initially thought that he could simply re-enable the OEM unlock by flashing the phone's firmware using Odin software, a popular tool used for rooting Samsung devices. However, his attempt to do so bricked his device, leaving it completely useless.

He then contacted Samsung support, but they informed him that the device was beyond repair and that he would have to buy a new one.

John's story is a cautionary tale for anyone who is considering rooting their Android device. Despite the benefits of rooting, such as increased control over the device and the ability to install custom software, there are risks involved.

One of the most significant dangers of rooting is that it can void the device's warranty. If something goes wrong, like in John's case, the manufacturer won't be responsible for repairing or replacing the device.

Furthermore, tinkering with the device's software can also leave it vulnerable to security threats, like malware attacks or hackers.

Conclusion:

In conclusion, while rooting a device can be tempting, it's important to understand the risks involved before doing so. Users should carefully consider the potential consequences of rooting, like voiding the warranty, bricking the device, and exposing it to security threats.

While some may find rooting to be a thrilling experience, it's worth noting that manufacturers design their devices to work optimally with their pre-packaged software. Altering this software can lead to unforeseen issues, like John's experience.

So, before you decide to root your device, take some time to research the process thoroughly and weigh the pros and cons. After all, it's better to be safe than sorry!

{{< youtube apBWoHhWtbw >}} 



## Chosen Solution
 I accidentally  disabled the OEM unlock option on my rooted S7, and am now stuck in  bootloop. I can get into download mode but not recovery mode.
I have tried to flash a stock firmware, however odin stops at this point:
<ID:0/007> Added!!
<ID:0/007> Odin engine v(ID:3.1301)..
<ID:0/007> File analysis..
<ID:0/007> Total Binary size: 4089 M
<ID:0/007> SetupConnection..
<ID:0/007> Initialzation..
<ID:0/007> Get PIT for mapping..
<ID:0/007> Firmware update start..
<ID:0/007> NAND Write Start!!
<ID:0/007> SingleDownload.
<ID:0/007> boot.img
<ID:0/007> recovery.img
<ID:0/007> system.img
<ID:0/007> FAIL!
<ID:0/007>
<ID:0/007> Complete(Write) operation failed.
<OSM> All threads completed. (succeed 0 / failed 1)
Is it possible for me to fix my phone, or do I need to buy a new one? if it is possible for me to fix it, how?

 You see the message custom binary blocked by FRP lock on the top left of the screen with the Samsung white text in the middle right?
Now there are only two ways to fix this and one involves factory resetting the phone.
You'll need to reflash stock firmware preferably the latest one via ODIN.
Once that's done you'll need to wipe data in recovery mode which means data will lost if it's stuck on Samsung logo, otherwise there'll be a button to press after boot to wipe data on phone.
Here is a guide on how to flash Samsung firmware if needed:
http://updato.com/how-to/how-to-install-...
If you have a GSM flashing box by any chance such as Z3X you can use the reset FRP/UFS option without needing to wipe data.




