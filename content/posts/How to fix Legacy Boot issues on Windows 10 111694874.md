---
title: "Say Goodbye to Annoying Legacy Boot Problems Forever with This One Simple Fix for Windows 10 & 11!"
ShowToc: true 
date: "2023-01-10"
author: "Linda Limerick"
---
*****
Say Goodbye to Annoying Legacy Boot Problems Forever with This One Simple Fix for Windows 10 & 11!

If you're a Windows user who has experienced annoying boot problems on your PC, you're not alone. Legacy boot issues have long plagued the Windows operating system, causing headaches for users and IT professionals alike. But there's good news: there's a simple fix that can help you bypass these problems and get your system up and running quickly and smoothly.

The solution is known as Unified Extensible Firmware Interface (UEFI) boot mode. UEFI is a newer type of boot mode that replaces legacy BIOS, which has been used for decades. One of the biggest advantages of UEFI is faster boot times, but it also offers a number of other benefits, including enhanced security, larger disk support, and improved system performance.

To switch your Windows PC to UEFI boot mode, the first step is to check if your computer supports UEFI. You can do this by following these steps:

1. Press the Windows key + R to open the Run dialog box.

2. Type "msinfo32" into the dialog box and click OK.

3. In the System Information window that opens, look for the "BIOS Mode" entry. If it says "Legacy," then your computer is currently using legacy boot mode.

If your computer supports UEFI, you can switch to UEFI mode by following these steps:

1. Restart your computer and enter the UEFI settings. The key to enter UEFI mode varies depending on the manufacturer, but it's usually F1, F2, F10, or Del.

2. Once you're in the UEFI settings, look for the option to switch to UEFI boot mode. The exact location of this option varies depending on the manufacturer and the model, but it's usually found in the Boot or Security menu.

3. Enable UEFI boot mode and save your changes.

4. Restart your computer and let it boot up in UEFI mode.

Once you've switched to UEFI boot mode, you should notice faster boot times and fewer boot problems. However, if you do encounter issues with UEFI, you can always switch back to legacy BIOS mode by following the same steps.

In conclusion, if you want to say goodbye to annoying legacy boot problems forever, switching to UEFI boot mode is a simple and effective solution. Not only will it help you get your PC up and running faster, but it also offers a number of other benefits, such as enhanced security and improved system performance. So, give it a try and see the difference of UEFI boot mode.

{{< youtube F8OLhUAPDq0 >}} 



There are two options when it comes to BIOS firmware. You might go for the more-recent firmware UEFI or stick with the Legacy BIOS. Your choice depends on various factors but we won’t suggest meddling with firmware if you don’t have enough experience.
 
 
 
- Download DriverFix (verified download file).
 - Click Start Scan to find all problematic drivers.
 - Click Update Drivers to get new versions and avoid system malfunctionings.

 
- DriverFix has been downloaded by 0 readers this month.

 
The common issue is switching from one to another option, as some users are unable to boot with the Legacy boot. There are multiple reasons for that and we provided some solutions below.
 
## What to do if Legacy Boot won’t work
 
### Solution 1 – Disable Raid On and Secure Boot
 
If you’re unable to boot with the Legacy boot and, for some reason, need to avoid UEFI, our first suggestion is to disable both RAID and Secure boot in boot settings. Once you’ve done that, reboot your PC and try booting again. Of course, make sure that Legacy boot is enabled in boot settings.
 
If you’re not sure how to access BIOS settings on Windows 10, follow these steps:
 
- Restart your PC 3 time forcibly to access the Advanced Recovery menu.
 - Choose Troubleshoot.
 - Select Advanced options.
 - Choose UEFI Firmware settings.
 - And finally, click Restart.
 - Once in BIOS/UEFI Settings, disable Secure Boot and RAID On (enable AHCI).

 
### Solution 2 – Repair or rebuild bootloader
 
Issues with booting with the Legacy BIOS might lie in the bootloader corruption. Instead of MBR, which runs with UEFI, we’ll need you to repair GPT. For this, you’re going to need the Windows 10 installation media created with Media Creation Tool. After you’ve successfully made a bootable drive, follow the steps we listed below:
 
- Boot with the bootable media.
 - Click Repair.
 - Choose Startup repair.
 - Enter the following commands and press Enter after each:
 - diskpart
 - list disk
 - select disk 0
 - list partition
 - select partition 1
 - active
 - exit
 - Now, just type bcdboot C:windows and press Enter.
 - Exit the command line and restart your PC.

 
### Solution 3 – Convert HDD to GPT
 
Finally, if you’ve previously used UEFI boot firmware to install a system on your HDD, you won’t be able to boot into a legacy mode. This drive is probably using MBR which won’t boot as it requires GPT. This can be resolved but, sadly, it requires formatting your drive in order to convert it to GPT partition.
 
- diskpart
 - list disk
 - select disk 0
 - list partition
 - select partition 1
 - active
 - exit

 
- Can’t Download Anything on Windows 10: How to Fix It
 - Looks Like You’re Stranded: How to Fix This Xbox App Error
 - A Device Which Does Not Exist Was Specified: 5 Easy Fixes
 - How to Fix Canon Printer Reset Error B203 [Quick Guide]
 - Windows Live Mail Attachments Not Showing: 6 Easy Fixes

 
Here’s what you need to do:
 
- Open Command Prompt from the Advanced Recovery menu.
 - In the command line, type the following commands and press Enter after each:
 - diskpart
 - list disk
 - Now, remember the number alongside the volume you want to convert. The easiest way to determine which is which is to check the storage space. We’ll use 1 as an example below.
 - In the command line, type the following commands and press Enter after each:
 - select disk 1
 - clean
 - convert mbr
 - Reboot PC and try installing Windows 10 again.

 
With that said, we can conclude this article. In case you have any questions or suggestions, feel free to tell us in the comments section below.
 
- diskpart
 - list disk

 
- select disk 1
 - clean
 - convert mbr

 

 
- windows 10 fix

 
Email * 
 

Commenting as .
Not you?

 
Comment 





