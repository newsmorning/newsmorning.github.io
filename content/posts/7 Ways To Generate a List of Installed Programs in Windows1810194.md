---
title: "You Won't Believe How Easy It Is To Find All Installed Programs On Windows In Just 7 Simple Steps!"
ShowToc: true 
date: "2023-01-21"
author: "Robert Garner"
---
*****
# You Won't Believe How Easy It Is To Find All Installed Programs On Windows In Just 7 Simple Steps!

If you're an avid PC user or a tech enthusiast, you already know how important it is to have a well-organized computer system. Having unnecessary programs installed on your computer can take up valuable storage space, slow down your system performance and cause other issues. Among many reasons, finding installed programs on Windows is necessary for uninstalling them, updating them or organizing them in a particular manner. In this article, I will walk you through seven simple steps to find all installed programs on your Windows computer.

## Step 1: Open the Start menu

The first step to finding all installed programs on your Windows computer is to open the start menu. You can do this in several ways, but the easiest way is to click on the Windows icon located on the lower-left corner of your screen. Alternatively, you can press the Windows key on your keyboard to open the start menu.

## Step 2: Click on the Settings icon

Once you've opened the start menu, click on the gear-shaped icon located just above the power icon. This icon represents the Settings app on your computer.

## Step 3: Select "Apps"

In the Settings app, you'll find different options to customize your PC settings. To find all installed programs, scroll down and click on the "Apps" option.

## Step 4: Click on "Apps & features"

Once you've clicked on the "Apps" option, you'll find several sub-options. Simply click on "Apps & features," which will show you all the programs installed on your computer.

## Step 5: Scroll down the list

After clicking on "Apps & features," you'll see a list of all apps installed on your Windows computer. The list might be lengthy, depending on how many programs you've installed. To find a specific program, you can either scroll down the list or use the search box located on the top-right corner of the window.

## Step 6: Sort your apps

If you want to organize your apps in a particular manner, you can do so by clicking on the "Sort by" option located just above the list. You can sort the programs by name, size, and date, among other options.

## Step 7: Uninstall or update your apps

Once you find the app you're looking for, click on it to reveal the "Uninstall" or "Modify" options. You can uninstall an app that you no longer need, or modify it if you want to update or change its features.

In conclusion, finding all installed programs on your Windows computer is an easy task that helps keep your system organized and running efficiently. By following these seven simple steps, you can easily find and manage all the programs installed on your Windows computer.

{{< youtube 4T6aOHC_A7U >}} 



If you own a Windows PC, you’ll likely have a list of go-to software that you use all the time, whether it’s Chrome, Outlook, or Steam. Outside of these favorites, there’ll be other programs you’ve forgotten about or have never even used. That can be problematic—forgotten software takes up disk space and can be a security risk.
 
We absolutely recommend you properly uninstall programs on Windows that you don’t use, but that doesn’t help you if you don’t know what software you have installed, especially if you’re managing multiple PCs at once. Here are several ways to generate a list of installed programs in Windows 10.
 
## Using The Windows PowerShell (Get-RemoteProgram)
 
If you want a list of installed programs in Windows 10 that you can export, the best solution is to use a built-in tool to create it. Few tools exist to do this, but one option is to use the Windows PowerShell (or command prompt, if you’re feeling old school).
 

 
For those who don’t know, the PowerShell has largely replaced the command prompt as the default terminal on Windows PCs. A script exists for PowerShell users to automatically list all installed programs called Get-RemoteProgram. This queries the Windows registry for a full and complete list of installed software on your PC.
 
- You’ll need to download the Get-RemoteProgram script for the PowerShell from the Microsoft TechNet website first. Download this, then place the file in your C:\Windows\System32 folder.

 
- Next, you’ll need to open a PowerShell window. You can do that by right-clicking the Windows Start menu and pressing Windows PowerShell (Admin) to open a new PowerShell window.

 
- You’ll need to make sure that Windows can run scripts like this—type Set-ExecutionPolicy Unrestricted to ensure that you can, hit enter, then press A to confirm. If that is successful, type Get-RemoteProgram to run the script, then hit enter. If you want to export the list to a file, type Get-RemoteProgram > list.txt instead.

 
## Using The Windows PowerShell (WMIC)
 
You can use either the PowerShell or cmd to run the Windows Management Instrumentation Command-Line Utility (WMIC) to generate a list of installed programs in Windows 10. As the PowerShell is the default command-line tool for Windows 10 users, we’ll be using that here.
 
Using the WMIC tool to view or export a list of your installed Windows software will create a similar list to the Get-RemoteProgram script.
 
- In an open PowerShell window or command line terminal with administrative privileges, type wmic. Once the WMIC prompt opens, type /output:C:\list.txt product get name, version then hit enter. You can replace C:\list.txt with another file name or output directory.

 
- Type exit to close the WMIC tool once you’re done. A list of your installed software should be available in the text file at the location you provided for the output file.

 
## Using Print Screen (Apps & Features)
 
If you want a visual list of your installed software, you could use the print screen key to take a screenshot in Windows of the Apps & Features menu in Windows Settings, where Windows displays a list of your installed software for you to modify or remove.
 
- To access this menu, right-click the Windows Start menu and press Settings. From here, press Apps > Apps & features. A list of your installed software will be visible in a scrollable list.

 
It’s unlikely that your installed PC software will fit in just one screenshot. You’ll need to press the PrtScrn button on your keyboard (or use third-party screenshot tools like Snagit), then paste your screenshots into a third-party image editor to save (or into a Word document).
 
You’ll need to scroll through the list and repeat this step to make sure you save the full and complete list of installed software on your PC.
 
## Using NirSoft UninstallView
 
NirSoft UninstallView is a quick, third-party alternative that can help you generate a list of installed programs in Windows 10. Like the Get-RemoteProgram script, it will query the Windows registry for a complete list of installed software.
 
- To start, download NirSoft UninstallView and extract the ZIP file (the 64-bit version is recommended). Once that’s done, run the extracted UninstallView.exe file.

 
- UninstallView will scan your PC for installed software. Once that process has completed, the full list of software will be available in the UninstallView window. To export the list, press View > HTML Report – All Items.

 
- A file called report.html will be created in the same folder as the UninstallView.exe file, showing a formatted list of your installed software. Pressing HTML Report – All Items will open this file in your default web browser.

 
## Using Belarc Advisor
 
Belarc Advisor has been a must-have tool in the arsenal of local PC repair shops for years, and it remains a useful tool for Windows 10 users. It generates a breakdown of your PC software, hardware, settings, installed updates, and more to allow you to fully audit your Windows installation.
 
Like UninstallView, this will be visible in a formatted HTML file that you can export elsewhere.
 
- To start, download Belarc Advisor and install it. Once it’s installed, Belarc Advisor will begin an immediate audit of your PC—this will take a few moments to complete.

 
- Your default web browser will open once Belarc has finished its audit of your PC. To view a list of your installed software, press the Software Versions and Usage link in the side menu, or scroll to that section manually. This file will be available in the C:\Program Files (x86)\Belarc\BelarcAdvisor\System\tmp folder, should you wish to export it.

 
## Using Geek Uninstaller
 
Geek Uninstaller is a third-party tool for uninstalling software. Like UninstallView, however, it also allows you to view and export a list of your installed programs in Windows 10.
 
- Download Geek Uninstaller to begin—you can choose the free version or the paid, Pro version. It comes as a ZIP file, so unzip the contents, then run the geek.exe file to launch the tool.

 
- The Geek Uninstaller window will show your installed software in an alphabetical list. To export the list, press File > Export to HTML or press Ctrl + S on your keyboard.

 
- Geek Uninstaller will ask you where to save the file—choose a location and a filename, then press Save to save the file.

 
- The generated list of your installed software will be saved, with the file automatically opened in your default web browser for you to view.

 
## CCleaner (Last Resort Option)
 
There are plenty of reasons why you shouldn’t download CCleaner anymore. Once a go-to and essential piece of maintenance software for Windows users, many of its core features have been rendered useless or ineffective due to Windows changes, or have been incorporated into Windows itself (or into other, better third-party apps).
 
CCleaner also suffered a rather unfortunate incident back in 2017, when a malware-injected version of the CCleaner installer was uploaded and installed by millions of users. For most users, the trust is gone and the message is clear—avoid CCleaner.
 
However, CCleaner can export a list of installed programs, but we’re not going to recommend downloading it to do so. This is a last resort option, but if you already have CCleaner installed, you could use it to generate and export a list of your installed programs. That is, of course, before you rush to remove it.
 
- To do that, open CCleaner and press the Tools tab on the left, then click Uninstall. At the bottom of the window, press the Save to text file button. This will allow you to export a list of your installed software.

 
- Choose a location and filename for your exported list, then press Save to save it.

 
This will export your installed files as a file formatted using tab delimiters. Opening the file using Microsoft Excel will allow you to view the list in a more manageable way.
 
## Removing Or Updating Windows Software
 
If you prefer to stay organized, or if you have too many PCs to maintain, generating a list of installed programs in Windows 10 can help you find the software you need to remove or update to give you more disk space and improve your security. 
 
If you don’t need to remove it, make sure you find ways to keep your software updated automatically to get the latest security patches and bug fixes. You may end up with software that you just don’t want on your PC, however. If that’s the case, be sure to remove unwanted software from your PC as soon as you find it.



