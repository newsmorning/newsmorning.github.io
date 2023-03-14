---
title: "Revolutionize Your Lenovo Yoga 720 with This Quick Trick to Boost Your PC Performance - Changing from RAID to AHCI"
ShowToc: true 
date: "2022-11-24"
author: "Maria Stewart"
---
*****
Revolutionize Your Lenovo Yoga 720 with This Quick Trick to Boost Your PC Performance - Changing from RAID to AHCI

The Lenovo Yoga 720 is a powerful laptop that's designed for versatility and high-performance computing. With its super-fast SSD storage, powerful processor, and stunning display, this laptop is a favorite among tech enthusiasts and productivity lovers alike. However, even the most powerful PCs can be slowed down by the wrong storage settings. Many Lenovo Yoga 720 users may not know that simply changing their storage controller mode from RAID to AHCI can dramatically improve their PC's performance.

What is RAID?
This technology stands for Redundant Array of Independent Disks. RAID enables users to combine two or more hard drives to store data together. By doing this, it improves performance and readers, and in case of a disk drive fails, the loss of data will be avoided.

What is AHCI?
AHCI stands for Advanced Host Controller Interface, which is a protocol that governs how storage devices communicate with the computer's CPU. Unlike RAID, which is designed to combine multiple hard drives, AHCI is focused on optimizing the transfer of data between the computer and single drives. By changing from RAID to AHCI mode, your Lenovo Yoga 720 can achieve faster data transfer speeds, leading to improved PC performance.

What are the benefits of switching from RAID to AHCI mode?
When you change from RAID to AHCI mode, you can unlock several benefits that directly contribute to your Lenovo Yoga 720's performance. Firstly, your PC can experience faster boot and load times. This is because AHCI mode is designed to optimize drive connectivity and performance, leading to quicker data access speeds. Secondly, your Lenovo Yoga 720 can handle multitasking more efficiently, leading to smoother and more efficient performance when running multiple programs. Lastly, changing from RAID to AHCI mode can improve battery life, meaning you can get more out of your laptop without having to recharge as often.

How to switch from RAID to AHCI mode
If you're ready to boost your Lenovo Yoga 720's performance by switching from RAID to AHCI mode, the process is relatively simple. Here's how to do it:

1. Before you begin, make sure you have a backup of your important data. Changing the storage controller mode can sometimes cause data loss unless precautions are taken beforehand.

2. Go to your computer's BIOS settings by restarting your PC and pressing the designated key on your keyboard. On most Lenovo Yoga 720 models, this key is F2.

3. In the BIOS, navigate to the storage options menu, and change the storage controller mode from RAID to AHCI.

4. Save your changes and exit the BIOS. Your Lenovo Yoga 720 will restart, and the new settings will take effect.

In conclusion, switching from RAID to AHCI mode can significantly enhance your Lenovo Yoga 720's performance. By optimizing data transfer speeds, improving multitasking capabilities, and extending battery life, this quick trick can revolutionize the way you use your PC. So, if you're looking to get the most out of your Lenovo Yoga 720, changing from RAID to AHCI mode is a must-try!

{{< youtube pu5IbAlw1Nk >}} 



## Chosen Solution
 I barely know anything about these to things except for that RAID is causing a problem with linux. I'm pretty sure you are supposed to use RAID with at least 2 storage devices while my laptop only has a single SSD. would I break something doing this? I know I lose my stuff doing this so beforehand I will backup.
@danj @nick

Can't call me out for taking a picture of my screen this time! you try taking a screenshot in the UEFI!

 If you turn RAID off in the BIOS, the rule has historically been that also requires a OS reinstallation. The problem with Windows is it does not like that setting being changed. Windows 10 likely isn't much different.
Because Lenovo was caught with Superfish and LSE, they had to promise not to ship 3rd party bloatware on their laptops to keep their sales. You likely have a Signature Edition system and part of the requirements to be a Signature Edition laptop is Microsoft requires your laptop has to boot up in RAID.
If you're booting from other installation media, then you'll need to switch from RAID to AHCI temporarily. Once you do what you need, it needs to be switched back to RAID.

 You can't RAID a single drive! RAID also requires two or more drives of the same I/O speed and the channel connection needs to be the same in I/O as well.

 My Lenovo Yoga 720-I3KB came with a tiny SSD installed, so I swapped it for a 1TB Intel SSD. In order for the system to recognize the drive I had to change the SATA Controller mode from RAID to AHCI. Also, 6 months later a Lenovo automatic firmware update overwrote this setting and caused my system to crash on boot....thankfully, I remembered about this controller mode change.




