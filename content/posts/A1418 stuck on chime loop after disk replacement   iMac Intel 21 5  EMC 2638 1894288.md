---
title: "You Won't Believe What Happened After This Simple Disk Replacement on an iMac - A1418 Stuck on Endless Chime Loop!"
ShowToc: true 
date: "2023-02-11"
author: "Sylvester Moses"
---
*****
# You Won't Believe What Happened After This Simple Disk Replacement on an iMac - A1418 Stuck on Endless Chime Loop!

If you're experiencing an endless chime loop after replacing the drive on your iMac A1418, fear not, you're not alone. The good news is that you can quickly fix this issue with a few simple steps. In this article, we'll show you what happened and how you can resolve it.

## What Happened?

Before we dive into the solution, let's discuss what happened. The endless chime loop occurs when the iMac is unable to find a bootable OS on the hard drive. It continues to chime as it repeatedly attempts to boot up the computer. Your iMac will remain stuck in this state until a bootable drive is detected.

Many users experience the endless chime loop after replacing their iMac's hard drive. In these scenarios, the issue usually arises from a misconfiguration of the hard drive. However, there are other underlying factors that can cause this problem.

## Solution

If you are experiencing the endless chime loop, here are the steps you need to take to resolve it.

### 1. Perform a PRAM reset

The PRAM (Parameter Random Access Memory) stores information about your iMac's settings, including the boot drive. To reset the PRAM, shut down your iMac, turn it on again, and immediately press the `Command + Option + P + R` keys.

Hold down these keys until you hear the startup sound twice. Once the sound is heard twice, release the keys, and allow the iMac to boot up.

If the PRAM reset doesn't resolve the issue, proceed to the next step.

### 2. Verify the drive's configuration

Verify that your iMac's hard drive is correctly configured. A wrong configuration can cause issues when booting up the system.

Here is how you can check the drive's configuration:

- Shut down the iMac.
- Press the power button to turn it on and immediately, press and hold the `Command + R` keys until you see the Apple logo.
- If prompted, enter your Wi-Fi network password to connect to the internet.
- Once you're in the macOS Utilities window, select `Disk Utility` and click Continue.

If you can't see the hard drive, click on `View` and select `Show All Devices`. 

- Select the iMac's primary hard drive and click `Partition`. 
- Choose `1 Partition` under the Partition Layout section, followed by `MacOS Extended (Journaled)`.

Click `Apply` to execute the changes. Once the process is complete, restart the iMac and check if the problem persists. If it does, proceed to the next step.

### 3. Reinstall macOS

If your iMac is still stuck on the endless chime loop, you may need to reinstall macOS. This process will help you create a bootable USB drive that you can use to reinstall the operating system.

- Boot up your iMac while holding down the `Command + R` keys to boot from the recovery partition.
- Select `Reinstall macOS` and follow the on-screen instructions to reinstall the operating system.

## Conclusion

The endless chime loop issue on an iMac can be frustrating. However, we hope this guide has helped you resolve the issue. If you're still experiencing issues after following these steps, you may need to seek further assistance from Apple's support team.

{{< youtube sw_eLa9Kwdc >}} 



## Chosen Solution
 Hi Everyone,
I’ve replaced the HDD on my Late 2013 21.5” iMac A1418 (EMC 2638).
After installing the new HDD the iMac on power up showed the folder with question mark, I’ve inserted USB with High Sierra 10.13 created with TransMac after started install it showed Apple logo and was stuck 10minutes, I’ve pressed the power button, after power up again the iMac is stuck on chime reboot (5 sec) tried to boot in Safe Mode, tried PRAM reset (pressing the Option, Command & P + R keys before pressing power button) any ideas?
Best Regards

 OK, so you swapped the HDD with a new formatted one. Assuming this drive is in perfect condition and correctly connected, The reason why after the chime (the sound) the folder with the question mark shows up is because the system does not find a bootable drive (I think EFI doesn’t have set up to boot from USB drives by default).
So It’s most likely that you don’t boot from the USB drive or even that USB bootable copy was not correctly made.
Try to start up with the drive attached and pressing and holding the Option (⌥) key immediately upon hearing the startup chime. Release the key when the StartupManager appears, showing you two possible options: your internal HDD and the install USB drive.
Hope this helps!

 Lets try this, Instead of booting up under the USB thumb drive or using Option, Command & P + R.
Lets use the built-in Internet recovery service again.
With your system connected to the internet (Ethernet or WiFi) follow this Apple T/N Reinstall from macOS Recovery.
This time lets just run Command (⌘)-R




