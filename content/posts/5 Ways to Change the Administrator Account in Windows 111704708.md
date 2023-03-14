---
title: "Unlock Hidden Features: 5 Sneaky Ways to Switch Up Your Windows 11 Admin Account!"
ShowToc: true 
date: "2023-04-10"
author: "Justin Spiegel"
---
*****
# Unlock Hidden Features: 5 Sneaky Ways to Switch Up Your Windows 11 Admin Account!

As an administrator, you are likely using your Windows 11 admin account for a variety of tasks. But did you know that there are several hidden features that can help you work more efficiently? In this article, we will explore five sneaky ways to switch up your Windows 11 admin account and unlock some powerful features.

## 1. Use the Quick Links Toolbar

The Quick Links Toolbar is a handy feature that allows you to access frequently used admin tools quickly. To enable it, right-click the taskbar and select "Show Taskbar Toolbar." Next, choose "New Toolbar" and type in the following path: `%ProgramData%\Microsoft\Windows\Start Menu\Programs\Administrative Tools`. This will create a Quick Links toolbar that provides one-click access to all your admin tools.

## 2. Customize the Start Menu

The Start Menu is one of the most important features in Windows 11, and you can customize it to suit your needs. Right-click the Start button and select "Settings." In the Settings menu, choose "Personalization." From there, you can change the Start Menu layout, create custom folders, and add or remove specific apps.

## 3. Set Up Virtual Desktops

Virtual Desktops are a powerful tool that allows you to create multiple workspaces on your computer. To enable this feature, press "Windows + Tab" to enter the Task View. From there, you can choose to create a new Desktop and switch between multiple workspaces. This can help you stay organized and productivity by keeping different tasks separate.

## 4. Use PowerToys

PowerToys is a set of utilities that can be used to unlock many hidden features in Windows 11. Some of the features included in PowerToys include a window manager, a keyboard shortcut manager, and a file renamer. To install PowerToys, visit the official Microsoft download page and click on the latest installer.

## 5. Customize the File Explorer

File Explorer is an essential tool for any administrator, and you can customize it to make it more efficient. Right-click on the File Explorer icon in the taskbar and select "Properties." In the Properties menu, you can choose to open File Explorer to This PC, show or hide the Navigation pane, and even set up custom shortcuts.

In conclusion, there are many hidden features in Windows 11 that can help you work more efficiently as an admin. By using the Quick Links Toolbar, customizing the Start Menu, setting up Virtual Desktops, using PowerToys, and customizing the File Explorer, you can unlock powerful admin tools and switch up your Windows 11 admin account. Give these tips a try and see how they can improve your workflow!

{{< youtube MUZ1jpnr71w >}} 



There are multiple user types on Windows, each with different permissions. Out of all available groups, the administrator group has the most privileges. Sometimes, to make certain changes on your PC, you need to have the maximum rights. 
 
## Simple and surefire ways to get administrative rights on your PC
 
- To change the administrator in Windows 11, you just need to modify some user account settings from the Settings app.
 - Various built-in applets can be used to adjust your Windows account settings.
 - You may also change the administrative account from command line in both PowerShell and Command Prompt.

 

 


 
- Download Restoro PC Repair Tool that comes with Patented Technologies (patent available here).
 - Click Start Scan to find Windows 11 issues that could be causing PC problems.
 - Click Repair All to fix issues affecting your computer's security and performance

 
- Restoro has been downloaded by 0 readers this month.

 
If you want to change your current account settings and give it additional privileges, this is possible in Windows 11 and the process isn’t that much different when compared to the one of making yourself an administrator in Windows 10. 
 
## Why don’t I have admin rights on Windows 11?
 
If you don’t have admin rights on Windows 11, it might be because you are using a standard account instead of an administrator account.
 
Also, if you are using a PC owned by your company, the admin rights might be disabled by your organization.
 
### Should I use an administrator or a standard account?
 
Administrators have full and unrestricted access to system files, and they can install applications. However, this isn’t without security concerns.
 
If your PC were to get infected by malware, it would be able to spread with almost no restrictions and perform whatever it wants if it infects a user with maximum access rights.
 
By using a standard account, the malware won’t be able to run without extra permissions, so the chance to get infected is smaller.
 
Therefore, many experts recommend using a Windows 11 local account and enabling the administrator account only when necessary.
 
Some PC issues are hard to tackle, especially when it comes to corrupted repositories or missing Windows files. If you are having troubles fixing an error, your system may be partially broken. We recommend installing Restoro, a tool that will scan your machine and identify what the fault is.Click here to download and start repairing.
 
Expert tip:
 
SPONSORED
 
Even more, for an extra layer of protection, we highly recommend installing a Windows 11 compatible antivirus.
 
## How can I change the administrator account in Windows 11?
 
### 1. Use the Settings app
 
- Click the Start button in the Taskbar.
 - Select Settings.
 - Now go to the Accounts section and choose Family & other users.
 - Select the account that you want to change to administrator and click on Change account type.
 - Set the Account type to Administrator and click OK to save changes.

 
If the Settings app fails to work, you can fix the issue by using the command-line tool and running a few commands, as described in this guide on what to do if the Settings app crashes in Windows 11.
 
### 2. Use Control Panel
 
- Click the Search icon in the Taskbar.
 - Type control panel and select Control Panel from the list of results.
 - Now select Change account type.
 - Choose the account that you want to change.
 - Now select Change the account type.
 - Choose Administrator and click on Change account type.

 
### 3. Use the netplwiz command
 
- Press Windows key + R and enter netplwiz. Press Enter.
 - Double-click the account that you want to change.
 - Navigate to the Group Membership tab. Now select Administrator and click on Apply and OK.

 
### 4. Use the lusrmgr command
 
- Press Windows key + R, enter lusrmgr.msc, and hit Enter.
 - Select your user account and double-click it.
 - Navigate to the Member Of tab and click on Add.
 - Enter Administrators in the input field and click on Check Names. The input will now change if the name is good. Click OK.
 - Select Users and click on Remove. Now click Apply and OK to save changes.

 
### 5. Use Terminal
 
#### 5.1. On PowerShell
 
- Press Windows Key + X and choose Windows Terminal (Admin) from the list.
 - Run the following command to add the user account to the Administrator group:add-LocalGroupMember -Group “Administrators” -Member “WR_Test”
 - Optional: To remove a user from the administrator group, use the following command:remove-LocalGroupMember -Group “Administrators” -Member “WR_Test”

 
#### 5.2. On Command Prompt
 
- Start Windows Terminal by pressing Windows Key + X and choosing the Windows Terminal (Admin) from the list.
 - Click the down arrow and select Command Prompt.
 - When the Command Prompt window opens, run this command:net localgroup Administrators "WR_Test" /add
 - Optional: To remove an account from the Administrators group, run this command:net localgroup Administrators "WR_Test" /delete

 
These are some of the methods on how to change the administrator account on Windows 11 on a Lenovo laptop and other PCs. All our solutions are relatively simple, but we suggest using the Settings app since it’s the most straightforward.
 
- How to create a local account on Windows 11
 - How to remove local users in Windows 11
 - Windows 11 Map Network Drive Missing: 3 Quick Fixes
 - Show All Apps by Default in Windows 11 Start Menu [2 Tips]
 - How to Enable or Disable Copy Paste in Application Guard
 - How to Hide a Partition in Windows 11 [Easy Steps]

 
However, if you’re an advanced user and you want to quickly add a user account to the administrator group, then using the Terminal might be the right for you because it only takes a few seconds. 
 
If you want to know how to delete an administrator or local account on Windows 11, check our guide to do it quickly.
 
What is your favorite method of changing the system administrator? Let us know in the comments section below.
 
- administrator accountWindows 11

 
Email * 
 

Commenting as .
Not you?

 
Comment 





