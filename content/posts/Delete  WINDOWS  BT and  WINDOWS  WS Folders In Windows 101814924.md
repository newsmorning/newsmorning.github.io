---
title: "Say Goodbye to Useless Junk: Learn How to Delete Windows BT and Windows WS Folders in Windows 10 Now!"
ShowToc: true 
date: "2023-05-15"
author: "Lawrence Clouse"
---
*****
#Say Goodbye to Useless Junk: Learn How to Delete Windows BT and Windows WS Folders in Windows 10 Now!

Are you tired of seeing those pesky Windows BT and Windows WS folders on your desktop? Do you find them taking up valuable storage space in your hard drive? If yes, then it's time to learn how to delete those useless junk folders in your Windows 10 operating system.

Here's how to do it using easy-to-follow steps:

**Step 1: Open Administrative Command Prompt**

The first step is to open the Administrative Command Prompt on your PC by pressing the Windows Key + X and selecting "Command Prompt (Admin)" from the list.

**Step 2: Disable the Automatic Update**

Once you have opened the Administrative Command Prompt, stop the automatic update service by typing "net stop wuauserv" and pressing Enter.

**Step 3: Delete the Windows BT Folder**

After disabling the automatic update service, navigate to the Windows BT folder by typing "cd C:\Windows\10Upgrade" and pressing Enter. Once you are in this folder, type "rmdir /S /Q Windows BT" and press Enter to delete the folder.

**Step 4: Delete the Windows WS Folder**

After deleting the Windows BT folder, navigate to the Windows WS folder by typing "cd C:\Windows\WS" and pressing Enter. Once you are in this folder, type "rmdir /S /Q Windows WS" and press Enter to delete the folder.

**Step 5: Enable the Automatic Update**

After deleting the Windows BT and Windows WS folders, enable the automatic update service by typing "net start wuauserv" and pressing Enter. 

**Congratulations! You have successfully deleted the Windows BT and Windows WS folders from your Windows 10 operating system.**

By deleting these useless junk folders, you can create more space on your hard drive, allowing you to store more important files and folders. This process also helps speed up your PC's performance and improve its overall efficiency.

In conclusion, it's important to take control of your PC's storage space by regularly deleting unnecessary files and folders. By following the steps outlined in this article, you can easily delete the Windows BT and Windows WS folders, creating more space on your hard drive and enhancing your PC's performance.

{{< youtube rdmrgwxtihM >}} 



The $WINDOWS.~BT and $WINDOWS.~WS folders are located at the root of the system drive, which is usually “C” drive. These folders are hidden by default. You need to configure the File Explorer to see them.
 
The $WINDOWS.~BT and $WINDOWS.~WS folders are created on your Windows 10 PC when you upgraded your Windows 10 installation to the latest version. For instance, these folders get created when you upgrade from Windows 10 Creators Update to Windows 10 Fall Creators Update.
 









 
The $WINDOWS.~BT folder contains files from the previous version of Windows 10 which are required to go back to the previous version. Installation files used by Windows setup or Media Creation Tool are saved in $Windows.~WS folder.
 
If your system drive is running out of free space, you can free up some good amount of space by deleting these folders. But how to safely delete $WINDOWS.~BT and $WINDOWS.~WS folders in Windows 10?
 
## Is it safe to delete $WINDOWS.~BT and $WINDOWS.~WS folders?
 
Since $WINDOWS.~BT and $WINDOWS.~WS folders are system folders and contain crucial files, many people wonder if it’s safe to delete these folders. The answer is, you can safely delete these folders only if you don’t want to go back to the previous Windows installation or version. That is, once you delete these folders, you cannot go back to the previous version of Windows 10.
 
If you are happy with the current version of Windows 10, you can delete them free up drive space. You will need to use the built-in Disk Cleanup tool to delete $WINDOWS.~BT and $WINDOWS.~WS folders safely. Here is how to do just that.
 
Important: You won’t be able to go back to the previous Windows installation after deleting these folders.
 
## Delete $WINDOWS.~BT and $WINDOWS.~WS folders
 
Step 1: Open up This PC. Right-click on the drive where Windows 10 is installed and then click Properties to open the properties dialog.
 
Step 2: Under the General tab, click the Disk Cleanup button. This will open the Disk Cleanup tool.
 
Step 3: When you see the following dialog of Disk Cleanup, click Clean up system files button.
 
Step 4: Finally, select Previous Windows installation(s) and Temporary Windows installation files. Click Ok button.
 
When you see the confirmation dialog, click Delete Files button. The Disk Cleanup tool will now delete $WINDOWS.~BT and $WINDOWS.~WS folders, and all files in these folders.
 
It’s worth noting that selecting Previous Windows installation(s) deletes $Windows.~BT and Windows.old folders. Similarly, select Temporary Windows installation files option to delete $Windows.~WS folder. Select both options to delete $WINDOWS.~BT and $WINDOWS.~WS folders.
 
Remember that Windows 10 will automatically create these folders again next time when you upgrade Windows 10 to the newest version. Repeat these steps again to delete them.



