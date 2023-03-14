---
title: "Say Goodbye to Slow Windows 10 in 5 Easy Steps - Fix 100% Disk Usage Today!"
ShowToc: true 
date: "2023-02-17"
author: "James Campbell"
---
*****
# Say Goodbye to Slow Windows 10 in 5 Easy Steps – Fix 100% Disk Usage Today!

If you are experiencing slow response from your Windows 10 device, then you're not alone. The performance issues on Windows 10 are a common issue encountered by many users. One problem that stands out is the struggle with extremely high disk usage. Finding and fixing the issue is a daunting task, but it doesn't have to be.

In this article, we will outline some of the most effective actions you can take to solve the problem of high disk usage on Windows 10.

## 1. Disable Windows Search

Windows Search is a handy feature, but it can become a burden on the system resources. Windows 10's search indexing service can run continuously, resulting in high disk usage. Disabling this feature can be an effective way to free up your system resources.

To disable the feature, follow these steps:

* Press the Windows key + R to bring up the Run dialog box.
* Type "services.msc" and press Enter.
* Look for "Windows Search" and double-click it.
* Click on "Stop" to stop the service.
* Under "Startup type," select "Disabled."
* Click OK to save the changes.

## 2. Disable Superfetch

Superfetch is a feature that is designed to speed up your system by preloading frequently used applications into memory. While it is a helpful feature, it can cause high disk usage and slow down your system in some cases.

To disable Superfetch, follow these steps:

* Press the Windows key + R to bring up the Run dialog box.
* Type "services.msc" and press Enter.
* Look for "Superfetch" and double-click it.
* Click on "Stop" to stop the service.
* Under "Startup type," select "Disabled."
* Click OK to save the changes.

## 3. Disable the Windows Tips feature

The Windows Tips feature is an attractive feature for Windows 10 users, but it can impact your system performance. Turning it off can help reduce the high disk usage.

To disable Windows Tips, follow these steps:

* Open the Settings app using the Windows key + I.
* Click on "System."
* Click on "Notifications & actions."
* Turn off "Get tips, tricks, and suggestions as you use Windows" under "Notifications."

## 4. Run the Windows Troubleshooter

The Windows Troubleshooter is a built-in feature of Windows 10 that can help detect and fix problems with the system. Running it can be a quick and easy way to identify and solve disk usage issues.

To run the troubleshooter, follow these steps:

* Open the Settings app using the Windows key + I.
* Click on "Update & Security."
* Click on "Troubleshoot."
* Select "Power troubleshooter" and click "Run the troubleshooter."

## 5. Restore Windows 10 to its default settings

If you're still facing slow performance or high disk usage issues after attempting the previous steps, consider restoring Windows 10 to its default settings. This will delete your files, but you will be left with a clean slate that can help restore your system to its previous performance levels.

To restore Windows 10 to its default settings, follow these steps:

* Open the Settings app using the Windows key + I.
* Click on "Update & Security."
* Click on "Recovery."
* Under "Reset this PC," click "Get started."
* Select "Remove everything" and follow the prompts.

Conclusion

By following these simple steps, you can fix the high disk usage issue on Windows 10 and boost your system performance. Disabling features such as Windows Search and Superfetch, turning off Windows Tips, running the Windows Troubleshooter, and restoring your Windows 10 to its default settings can help free up your system resources and restore your device's performance to its former glory.

{{< youtube Enh3gPc3HVs >}} 



Is your brand-new Windows 10 computer lagging? Well you are not the only one! Recently, many users reported that their Windows 10 disk utilization reaches to 100%, leading to lagging and unresponsive system.
 
So, in this tutorial, we are providing 5 tips to fix the issue of 100 percent disk usage problem in Windows 10.
 
## How To Fix 100% Disk Usage On Windows 10
 
### 1.    Disable Windows Search
 
To fix, 100% disk usage in Windows 10, firstly, you must disable Windows search temporarily and check if the computer speeds up. In case the problem still not resolved then move to disable Windows search permanently.
 
- Disable Windows Search (Temporarily)

 
Windows search allows you to search files on your computer faster. However, if you do not use it, you can disable it. Once you will disable the service it will stop the indexing of all files.
 
However, when you reboot your computer the Windows search will start again.
 
- Press Windows logo key and X in a combination and select Command Prompt (Admin).
 - Click Yes at the User Account Control window prompt.
 - In the Command Prompt window, type “net.exe stop “Windows search”” and press Enter.

 
Check if disk usage of your computer improved. If this step worked, then you must disable Windows Search permanently as shown below.
 
- Disable Windows Search(Permanently)
 - Press Windows logo key and R in a combination, a box will open->type “services.msc” and press Enter.
 - Scroll down and find “Windows Search” and right-click on it and click on Properties.
 - Change the Startup type to Disabled. Then click Apply and OK to save your change.

 
### 2.    Disable SuperFetch Service
 
In Windows 10, it has been identified that SuperFetch service is causing a disk performance issue. Disabling SuperFetch decreases boot time and speeds up the computer. Here’s how to stop SuperFetch service:
 
- Press Windows logo key and X in a combination and select Command Prompt (Admin) and allow its user account control.
 - In the Command Prompt window, type “net.exe stop superfetch” and hit Enter.

 
Wait for few moments to check if your computers performance better.
 
### 3.    Reset Virtual Memory
 
Virtual memory is a memory which is used as an extension of your computer’s physical memory. When RAM is not having an enough memory to perform a task then Windows temporarily stores files in virtual memory to complete the task and switch back to RAM again. Unnecessary, virtual memory allocation may lead to high disk usage.
 
You can reset virtual memory using the steps below:
 
1)  Press Windows logo key and Pause/ Break key in a combination. Then select Advanced System Settings on the left panel.

 
2) Tap Advanced tab, then click Settings.

 
3) Now, tap Advanced tab again, and select Change… under Virtual memory.

 
4) Make sure the Automatically manage paging file size for all drives checkbox is unchecked.


 
5) Select your Windows drive, the hard drive or partition that has Windows installed on it. In our case it is C:, now enter an Initial size and Maximum size for your virtual memory:
 
- Initial size – This value can vary and it depends on your computer. If you’re not sure what value to enter, just enter from the Recommended category.
 - Maximum size – use the size 1.5 times the size of your physical RAM. e.g. If your computer has 4 GB (4096 MB) of RAM then you should have to enter 6,144 MB virtual memory not more than that.
 - Once you’ve entered values, click Set, then click OK to continue.

 
6) Now, clear all your ‘temp’ files on your PC. To do so, press Windows logo key and R in a combination, a Run box will open, type temp and press Enter. This will open Windows Explorer with all the temp files on your PC.

 
7) Select all the files in the Temp folder and delete them.
 
Wait for few moments to check if your 100% disk usage is fixed.
 
### 4.    Fix your StorAHCI.sys driver
 
If you have tried all above solutions and the problem is still not resolved, then you can try this. It has been found that 100% disk usage issue might be caused by some Advanced Host Controller Interface PCI-Express (AHCI PCIe) models running with the inbox StorAHCI.sys driver due to a firmware bug.
 
Here’s how to check and how you can fix it:
 
Check if you are running the inbox AHCI driver (StorAHCI.sys)
 
- Press Windows logo key and R in a combination, a Run box will open, type “devmgmt.msc” and press Enter.
 - Under IDE ATA/ATAPI Controllers, right-click Standard SATA AHCI Controller and choose Properties.
 - Now, tap on Driver tab and click Driver Details. If you see storahci.sys in the list i.e. you are running the driver.

 
Now Disable MSI for the controller in the registry
 
- Close the driver files details window, now go to the Details tab and select “Device instance path from the drop-down menu. Note down the path starts from PCI\VEN.
 - Now, press Windows logo key and R in a combination, a Run box will open, type regedit and press Enter.
 - Follow the following path to HKEY_LOCAL_MACHINE\System\CurrentControlSet\Enum\PCI\<AHCIController>\Device Parameters\Interrupt Management\MessageSignaledInterruptProperties, where <AHCI Controller> refers to the device instance path you noted in the above step. Then change its value of the MSISupported key from 1 to 0.

 
Re-start your computer and check whether this step has been worked to fix the issue.
 
### 5.    Use Disk SpeedUp Tool
 
If the all above solutions did not help, it is mandatory having a check of your hard drive. You can do this by using Disk Speedup developed by Systweak. It is used to defragment the hard drive. Download Here.
 
It securely defrags the hard disk, restoring hard disk storage efficiency and giving a major performance boost. It scans through the whole system to find the data and files which lie haphazardly fragmented on the hard disk, and brings them together to reduce the data access time.
 

 
This should be done periodically to maintain consistency and stability in system’s performance.
 
That’s all folks!Hope that you have fixed 100 percent disk usage issue in Windows 10. If you have any question or suggestions, please feel free to share them in the comments section below.
 
##  People Who Read This Post Also Like 



