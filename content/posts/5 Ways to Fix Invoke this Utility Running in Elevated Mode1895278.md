---
title: "You Won't Believe These 5 Simple Hacks to Fix Your Elevated Mode Woes!"
ShowToc: true 
date: "2023-02-11"
author: "Lisa Mclaughlin"
---
*****
# You Won't Believe These 5 Simple Hacks to Fix Your Elevated Mode Woes!

## Introduction

If you are a Windows user, you might have come across the elevated mode, also known as administrator mode. This feature is meant to give you full access or control over your computer so that you can perform certain actions that normal users can't do. However, sometimes, things can go wrong, and you might find yourself unable to access elevated mode. Don't worry, though, in this article, we will provide you with five simple hacks to get you back on track.

## Hack 1: Disable UAC

User Account Control (UAC) is a feature that prompts you for confirmation whenever you try to execute an action that requires elevated mode access. Although UAC is an essential security feature, it can sometimes interfere with the process of accessing elevated mode. To disable UAC, follow these steps:

1. Press the Windows key + R to open the Run dialogue box.

2. Type in "Control Panel" and press Enter.

3. Click on "User Accounts" and then "User Accounts" again.

4. Click on "Change User Account Control settings."

5. Drag the slider down to "Never Notify" and apply the changes.

6. Restart your computer.

## Hack 2: Use Command Prompt

Another way to solve elevated mode woes is by using the command prompt. Follow these steps:

1. Press the Windows key + X and click on "Command Prompt (Admin)."

2. Type in "net user administrator /active:yes" and press Enter.

3. Close the command prompt and log out of your account.

4. Log in to the newly created administrator account.

5. Right-click on the Start button and click on "Command Prompt (Admin)."

6. Type in "net user administrator /active:no" and press Enter.

7. Close the command prompt and log out of the administrator account.

8. Log in to your account, and elevated mode should be working again.

## Hack 3: Use System Restore

If the above two options don't work, you can try using system restore. Here's what you need to do:

1. Press the Windows key + R to open the Run dialogue box.

2. Type in "rstrui.exe" and press Enter.

3. Select the restore point you wish to use and follow the on-screen instructions.

4. After the restore process is complete, try accessing elevated mode again.

## Hack 4: Check Group Policy

Group Policy is a feature that allows a network administrator to control user environments. However, if you are not in a network environment, Group Policy can cause elevated mode access problems. To solve this, follow these steps:

1. Press the Windows key + R to open the Run dialogue box.

2. Type in "gpedit.msc" and press Enter.

3. Go to "Computer Configuration" > "Windows Settings" > "Security Settings" > "Local Policies" > "Security Options."

4. Scroll down to "User Account Control: Only elevate UIAccess applications that are installed in secure locations" and double-click on this option.

5. Select "Disabled" and click on "Apply" and "OK."

6. Restart your computer and try accessing elevated mode again.

## Hack 5: Check Your Anti-Virus Settings

Sometimes, your anti-virus software can cause elevated mode access problems. To solve this, follow these steps:

1. Open your anti-virus software.

2. Navigate to the settings or options menu.

3. Look for any options that relate to elevated mode access or UAC.

4. Disable these options and save the changes.

5. Restart your computer and try accessing elevated mode again.

## Conclusion

Elevated mode access is an essential feature of Windows. However, sometimes, this feature can malfunction, causing inconvenience to users. In this article, we have provided five simple hacks to help you fix your elevated mode access woes. These hacks range from disabling UAC to checking your anti-virus settings. We hope these tips will be helpful to you.

{{< youtube kchzoy1lO-Y >}} 



The You have to invoke this utility running in elevated mode and ensure the disk is unlocked error message is not new to experienced Windows users who regularly use the Command Prompt.
 
## Follow our steps in order to resume your Command Prompt work
 
- The You have to invoke this utility running in elevated mode and make sure the disk is unlocked error occurs when you don't have the necessary privileges to run a command.
 - Certain Command Prompt commands will not run unless you are logged in as an administrator.
 - This is a security measure that makes sure strangers can't change your important files and data.

 

 
- Download Restoro PC Repair Tool that comes with Patented Technologies (patent available here).
 - Click Start Scan to find Windows issues that could be causing PC problems.
 - Click Repair All to fix issues affecting your computer's security and performance

 
- Restoro has been downloaded by 0 readers this month.

 
This is how one user on the Microsoft Answers forum described the problem:
 
If you’ve encountered (or you’re encountering) this error and are in the dark about how to fix it, this post will show you practical solutions.
 
I have received this message:
 
“Access denied as you do not have sufficient privileges or the disk may be locked by another process You have to invoke this utility running in elevated mode and make sure the disk is unlocked”. How can I resolve this problem. Thank you
 
## What does You have to invoke this utility running in elevated mode and make sure the disk is unlocked mean?
 
The functionality of the Command Prompt changes significantly depending on whether it is run typically or with administrator privileges; thus, specific commands won’t be able to run with regular user privileges. 
 
It explains why you need to launch the CMD program in elevated mode, which translates to having administrator capabilities on the system. The error message can also appear as You do not have sufficient privileges to run system configuration.
 
As you can see, a clear solution is to run Command Prompt as an administrator so that you can gain the privileges needed.
 
This is because doing so would mean that a guest user on your computer would be able to make significant changes to your computer, which is not recommended.
 
Some PC issues are hard to tackle, especially when it comes to corrupted repositories or missing Windows files. If you are having troubles fixing an error, your system may be partially broken. We recommend installing Restoro, a tool that will scan your machine and identify what the fault is.Click here to download and start repairing.
 
Expert tip:
 
SPONSORED
 
## How do I fix the You have to invoke this utility running in elevated mode error?
 
### 1. Run Command Prompt as an administrator
 
- Press Windows, enter cmd, and select the Run as administrator option under the result on the right side.
 - After that, try running the desired commands and check if the problem still appears.

 
### 2. Repair your PC’s registry
 
- Shut down your computer and boot into Safe Mode. Even though the guide linked is for Windows 11, the steps are similar in Windows 10.
 - Once your PC has booted, press the Windows key, then enter cmd and open the Command Prompt result as an administrator by selecting this option under the result on the right side.
 - Next, enter the following command and press Enter: sfc /scannow
 - Wait for the scanning process to complete, and then restart your computer. All corrupted files will be replaced on reboot. The You have to invoke this utility running in elevated mode and make sure the disk is unlocked error will be solved.

 
### 3. Run the CHKDSK command
 
- Press the Windows keyboard button, enter cmd and choose the Run as administrator option from the right panel.
 - When Command Prompt opens, enter the Command below, but replace the X with your drive (it’s usually C), then hit the Enter key: chkdsk /f X:
 - Follow the prompts and then restart your computer.

 
### 4. Take ownership of the drive partition
 
- Press Windows + E to open File Explorer, then go to This Pc.
 - Next, right-click the target drive partition and select Properties.
 - Go to the Security tab, then click Advanced.
 - Click the Change link beside the Owner label.
 - Type your user account under the Enter the object name to select pane, then click OK.
 - Go back to the Security tab. Click the Edit button. Select your user, set the permissions to Full control, then click OK to apply the changes made.

 
### 5. Change the current user to an administrator account
 
- Press Windows + I, then go to Accounts.
 - Go to Family and other users. Then, select the account owner name, and click Change account type.
 - Under Account type, select Administrator and click OK.
 - Afterward, sign in with the new administrator account.

 
### How do I fix CHKDSK Access Denied?
 
To fix access denied issues, you will need to execute Command Prompt as an administrator, just as we did previously. To do this, stick to our instructions, which are laid out above and are pretty easy to understand.
 
- Fix: Can’t run Command Prompt as admin
 - How to open a file / folder in Command Prompt [CMD guide]
 - How to Make Yourself an Administrator in Windows 10

 
Check out our guide on what to do if you can’t run Command Prompt as admin, so you can also fix this issue.
 
Alternatively, we have prepared an article on how to fix Access denied in Windows 10/11 that you can visit for more potential solutions.
 
We hope you resolved the You have to invoke this utility running in elevated mode and make sure the disk is unlocked error message. If so, you can share your experience with us by commenting below.
 
- windows 10 fix

 
Email * 
 

Commenting as .
Not you?

 
Comment 





