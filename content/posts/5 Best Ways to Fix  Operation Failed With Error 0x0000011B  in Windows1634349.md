---
title: "Discover the 5 Foolproof Methods to Fix the Dreaded Error 0X0000011B and Get Your Windows Running Smoothly Again!"
ShowToc: true 
date: "2023-02-15"
author: "Angel Davis"
---
*****
# Discover the 5 Foolproof Methods to Fix the Dreaded Error 0X0000011B and Get Your Windows Running Smoothly Again!

If you're a Windows user, you're no stranger to error messages. One of the most frustrating errors that can pop up is the Error 0X0000011B. This error message can appear out of nowhere and can make your computer completely unusable. Luckily, there are a few foolproof methods that you can use to fix this error and get your Windows running smoothly again. In this article, we will discuss the 5 most effective methods.

## Method 1: Restart your Computer

This may seem obvious, but sometimes a simple restart can fix the error. The Error 0X0000011B is often caused by conflicting drivers or programs, and a simple restart can clear up any issues. When you restart your computer, it will reboot all the drivers and programs and can fix any conflicts.

## Method 2: Uninstall Recently Installed Programs or Drivers

If you have recently installed a new program or driver, this could be the cause of the error. You can try uninstalling the program or driver and see if the error disappears. To uninstall a program, go to Control Panel > Programs and Features, and select the program you want to uninstall. To uninstall a driver, go to Device Manager, locate the driver, right-click, and select Uninstall.

## Method 3: Update your Operating System

Sometimes the Error 0X0000011B can be caused by an outdated operating system. Windows regularly releases updates to fix bugs and errors, and updating your operating system can fix the error. To update your operating system, go to Settings > Update & Security, and click on Check for updates.

## Method 4: Run a System File Checker (SFC) Scan

Another potential cause of the Error 0X0000011B is a corrupted system file. You can run a SFC scan to check for and fix any corrupted files. To run an SFC scan, open the Command Prompt as an administrator and type "sfc /scannow." This will scan your system files and fix any issues.

## Method 5: Run a Disk Check

If your hard drive is damaged, it can cause the Error 0X0000011B. You can run a disk check to see if your hard drive is the issue. To run a disk check, go to the Command Prompt as an administrator and type "chkdsk C: /f /r /x." This will scan your hard drive and fix any errors.

In conclusion, the Error 0X0000011B can be incredibly frustrating, but it's not impossible to fix. By using one of these 5 foolproof methods, you can get your Windows running smoothly again. If none of these methods work, it may be time to contact a professional to diagnose the issue.


A recent Windows 10 Security update is causing printers shared over the network to throw the 0x0000011B error code. The good news is that the problem is easily fixable, and we will show you how.

 
From uninstalling the problematic update to manually installing the printer using a local port, we will review every method to get your network printer working again. Here are all the ways to fix the 0x0000011B error in Windows.

 
## Fix 1: Update Windows

 
While it was a Windows Update that initially caused the issue, another update will likely fix it.

 

 
Windows Updates are notorious for creating weird bugs and conflicts, but Microsoft is also quick to roll out a hotfix for any such problems. Simply installing the latest update will usually fix the 0x0000011B error.

 
- To check for updates, head to the Start Menu and open Settings.

 
- Switch to the Windows Update tab and click the Check for updates button.

 
- Any available packages are displayed as Updates available. Use the download now button to download and install the update.

 
Restart your computer after the update is installed to apply the new changes. If you still get an “Operation Failed With Error 0x0000011B” message, move on to the next fix.

 
## Fix 2: Uninstall the Problematic Update

 
In Windows 10 (and Windows 11), you can uninstall recent updates. This lets you roll back malfunctioning updates to get your computer working correctly.

 
On Windows 11, you can find the option to remove updates by searching Uninstall Updates in the Start Menu.

 
In all versions, you can also locate this setting through the Control Panel.

 
- Open Control Panel by searching for it in the Start menu.

 
- Select Programs.

 
- This opens Programs and Features with the option to View installed updates. Click on it.

 
- A new settings window displays all recently installed Windows updates with the option to uninstall them. Check the dates of these updates and uninstall the one that started your problem.

 
Removing the update will fix the issue, though it is a temporary solution. Wait until the next update, as that usually implements bug fixes.

 
## Fix 3: Restart the Print Spooler Service

 
The print spooler service is responsible for managing all print jobs created on the computer and is often the root of any printer-related bugs. Simply restarting the print spooler service can usually fix the 0x0000011B error.

 
- Search for Services in the Start menu and open it.

 
- The app lists all services—running or not—on your computer. As the listing is alphabetical, scroll down to find the Print Spooler service.

 
- Right-click on the service and select Restart.

 
- Windows immediately restarts the service.

 
If the problem was caused by a temporary glitch, this should fix it. Otherwise, try another method.

 
## Fix 4: Manually Install the Printer

 
A workaround for getting a network printer functioning again is to install it manually. This often allows the system to use the device without a 0x0000011B error message.

 
Note that in earlier versions of Windows, you’d find this option in the Control Panel, while Windows 10 and Windows 11 have relocated it to the Printers & Scanners section of Settings. The steps are still mostly the same, just with an updated UI.

 
- Open Settings by clicking the gear icon on the Start menu. (In older versions of Windows, open the Control Panel instead.)

 
- Switch to the Bluetooth & Devices tab in Settings, then select the Printers & Scanners option. (Or, in the Control Panel, select the View devices and printers option under Hardware and Sound.)

 
- Click Add device to try to detect the printer automatically.

 
- After a few seconds of scanning, you will be presented with the option to Add manually. (The corresponding Control Panel option reads The printer that I want isn’t listed.)

 
- Now you have two ways to go about this. You can add the printer using its IP address or create a local port and manually install the right drivers.

 
- If you choose the Add a local printer or network printer with manual settings option, you can create a new local port. Give it a name and manually install the printer drivers, allowing you to use the network printer through that connection.

 
- The easier option is to Add a printer using an IP address or hostname. You just need to specify the type of printer and enter its IP address.

 
Manual printer installation is a complicated process, with a lot of room for small errors that ruin the whole anyway. If you manage it, however, it is almost guaranteed to work without any 0x0000011B errors.

 
## Fix 5: Disable CVE-2021-1678 Mitigation

 
The whole issue has been caused by a recent Windows Update addressing a security vulnerability posed by network printers. If nothing else works, you can perform a registry edit to shut this new feature down.

 
While the edit is simple enough, registry editing always comes with some risk of messing things up, so the usual warnings apply. Do not fiddle with registry values beyond what is outlined in the following steps, and create a registry backup before you proceed.

 
- First, open the Registry editor by searching for it in the Start menu.

 
- Despite its scary reputation, the registry editor is actually quite easy to use. On the left side is the folder structure containing all registry entries sorted by their respective categories, and on the right, you will see the keys themselves.

 
- Navigate to HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\Print by clicking through the folders or just copy-pasting the path in the address bar.

 
- Right-click in the empty space in the right panel and select New > DWORD (32-bit) value.

 
- Name it as RpcAuthnLevelPrivacyEnabled. Note that this is case-sensitive, so copy-paste the name instead of typing it out yourself.

 
- Registry keys usually start with a default value of zero, but it is a good idea to check anyway. Right-click on the new DWORD you created and select Modify.

 
- Make sure that the Base is set to Hexadecimal and the Value is 0.

 
- Restart your computer to apply the changes. Your network printer should now work without any issues.

 
## What Is the Best Way to Fix the 0x0000011B Printer Error in Windows?

 
The only permanent solution to the 0x0000011B error is to install the latest Windows Update which fixes the issue. For now, you can try uninstalling the update or disabling the problematic security feature from the Registry.

 
Other workarounds include installing the printer manually. You can do this by configuring a new local port with the printer drivers, or using the IP address of the network printer to help the PC establish a connection.

 
Before you try all these methods, however, make sure you are suffering from a 0x0000011B error. If you cannot see the network printer in File Explorer, you might be using the wrong workgroup or just not connected properly.




