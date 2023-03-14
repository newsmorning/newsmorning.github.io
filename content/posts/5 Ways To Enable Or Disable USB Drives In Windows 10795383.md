---
title: "You Won't Believe How Easy It Is To Control USB Access In Windows 10 With These 5 Simple Steps!"
ShowToc: true 
date: "2023-04-12"
author: "Justin Amin"
---
*****
Title: You Won't Believe How Easy It Is To Control USB Access In Windows 10 With These 5 Simple Steps!

Are you often worried about the security of your confidential data when you transfer them via USB devices? With the increasing cases of data breaches, it's important to ensure that only authorized users have access to your data. Windows 10 provides a built-in feature that allows you to control USB access to your device. In this article, we'll guide you through the simple steps you can take to control USB access in Windows 10.

Step 1: Open Group Policy Editor

Press the Windows key + R on your keyboard to open the Run dialog box. Type "gpedit.msc" and hit Enter. This will open the Group Policy Editor window.

Step 2: Navigate to the "Administrative Templates" Folder

On the left-hand side of the Group Policy Editor window, navigate to the "Administrative Templates" folder.

Step 3: Open the "System" Folder and Locate "Removable Storage Access"

Under the "Administrative Templates" folder, select "System" and scroll down until you find "Removable Storage Access."

Step 4: Select "Removable Disks: Deny Execute Access" Policy

Double-click on "Removable Disks: Deny Execute Access" Policy, located on the right-hand side of the window.

Step 5: Set the Policy to Enabled

In the Policy Properties dialog box, select the "Enabled" option and click "OK" to save the changes.

Congratulations! You have successfully enabled USB access control in Windows 10. Now, any unauthorized USB devices that are plugged into your computer won't be able to execute any files, making it difficult for hackers to access your data.

In conclusion, USB access control is an important security measure that you should consider implementing to protect your confidential data. By following these simple steps, you can easily enable USB access control in Windows 10 and enjoy peace of mind knowing that your data is safe from unauthorized access.

{{< youtube MbuGcnYcHkQ >}} 



Do you want to protect the data on your Windows 10 computer by blocking USB drives or disabling USB drives on your PC? In this guide, we will cover the five easy ways out there to enable or disable USB drives in Windows 10.
 
Blocking USB drives in Windows 10 can be done in many ways. You can use the Registry, BIOS or third-party utilities to enable or disable USB drives in Windows 10.
 









 
In no particular order, following are the five ways to enable or disable USB drives in Windows 10.
 
Method 1 of 5
 
## Enable or disable USB drives in Windows 10 via Registry
 
If you are comfortable making changes to Windows Registry, you can enable or disable USB drives in Windows 10 by manually editing the Registry. Here is how to do that.
 
Step 1: Open the Registry Editor by typing Regedit.exe in the Start/taskbar search and then pressing Enter key.
 
Click Yes button if you see the User Account Control prompt.
 
Step 2: Navigate to the following key:
 
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\ Services\USBSTOR
 
Step 3: Now, on the right-side, double-click on Start DWORD value and change its value to 4 to disable USB drives and USB storage devices on your Windows 10 PC. Change the Start DWORD value back to 3 to enable USB drives and storage devices on your PC.
 
Method 2 of 5
 
## Enable or disable USB ports via Device Manager
 
Did you know that you can disable all USB ports via Device Manager? By disabling USB ports, you are preventing users from using USB ports to connect to USB drives to your PC.
 
When you disable USB ports, USB ports on your PC will not function, and hence no one can connect USB drives. You will need to enable USB ports again to connect a device via USB. Here is how to enable or disable USB ports via Device Manager.
 
IMPORTANT: We recommend you create a system restore point before disabling USB ports so that you can easily enable them again when you want.
 
Step 1: Right-click on the Start button on the taskbar and then click Device Manager to open the same.
 
Step 2: Expand Universal Serial Bus Controllers. Right-click on all entries one-after-another and then click Disable device option. Click Yes button when you see the confirmation dialog.
 
Method 3 of 5
 
## Use USB Drive Disabler to enable or disable USB drives
 
If you don’t want to edit the Registry manually, you can use a free tool called USB Drive Disabler to quickly enable or disable USB drives on your PC. Simply download USB Disabler, run the same, and then select Enable USB drives or Disable USB drives to enable or disable USB drives on your PC.
 
Download USB Drive Disabler
 
Method 4 of 5
 
## Disable or enable USB ports in BIOS
 
Some manufacturers offer an option in BIOS/UEFI to disable or enable USB ports. Boot into BIOS/UEFI and check if there is an option available to disable or enable USB ports. Check your PC’s user manual to know if an option to enable or disable USB ports is present in the BIOS/UEFI.
 
Method 5 of 5
 
## Enable or disable USB drives with USB Guard
 
Nomesoft USB Guard is another free utility out there to block USB drives on PCs running Windows 10 and earlier Windows versions. You must this program as administrator to enable or disable USB drives.
 
Download Nomesoft USB Guard



