---
title: "Say Goodbye to Remote Desktop Woes: 5 Game-Changing Solutions to Get Your Copy and Paste Function Back Up and Running!"
ShowToc: true 
date: "2023-02-25"
author: "Norman Sugar"
---
*****
Say Goodbye to Remote Desktop Woes: 5 Game-Changing Solutions to Get Your Copy and Paste Function Back Up and Running!

Working remotely has become the norm for many people around the world. With the rise of remote work, the use of remote desktops also increased, allowing workers to access their work computers from any location. Remote desktops offer flexibility, convenience, and ease of access, but they can also be frustrating at times, especially if your copy and paste function is not working correctly.

If you've faced this problem, you know how frustrating it can be. You can't copy and paste files, text, or even images between your local and remote desktops. Fortunately, there are solutions to resolve this common remote desktop issue. In this article, we will discuss five game-changing solutions that will get your copy and paste function back up and running in no time.

1. Update Your Remote Desktop Software

The first solution to fix the copy and paste problem is to update your remote desktop software. Sometimes, outdated remote desktop software can cause various issues, including the copy and paste function not working correctly. So, make sure to keep your remote desktop software updated to the latest version to fix any glitches.

2. Restart Remote Desktop Services

If updating your remote desktop software doesn't resolve the issue, try restarting the remote desktop services. To do this, open the services manager by typing "services.msc" in the Start menu. Once you've located Remote Desktop Services, right-click on it, and select Restart. This will temporarily stop the service and restart it, which will often solve the copying and pasting issue.

3. Check Your Clipboard Settings

Another reason why the copy and paste function might not be working correctly could be due to the clipboard settings. By default, remote desktops disable the clipboard sharing option for security reasons. However, you can enable this option by selecting the local resources tab in the remote desktop connection settings and checking the clipboard box.

4. Use Clipboard Managers

Clipboard managers are third-party software that can help you solve the copy and paste issue. These tools can store multiple items that you've copied in your clipboard, allowing you to easily access them at any time. Examples of clipboard managers include Ditto, ClipX, and Clipboard Master.

5. Use Cloud-Based File-Sharing Services

When all else fails, another option is to use cloud-based file-sharing services. These services, such as Dropbox, OneDrive, or Google Drive, allow you to share files between your local and remote desktops by simply uploading the file to the cloud and accessing it from the remote desktop. This method is also an excellent solution if you need to share large files.

In conclusion, if you're experiencing issues with your remote desktop copy and paste function, you have several solutions to get it back up and running. Updating your remote desktop software, restarting remote desktop services, checking your clipboard settings, using clipboard managers, and using cloud-based file-sharing services are all excellent solutions to this problem. So, try these solutions, and you'll be back to being productive in no time!

{{< youtube L29nzSzWdGM >}} 



Remote desktop connections allow users to view and transfer files from one local machine to another. 
 
## Some settings in Remote Desktop may prevent you from copy pasting
 
- Users often experience difficulty while doing copy-paste between your system and RDP.
 - It often occurs due to some issues like if you didn't allow copy-pasting in your Remote Desktop app properties.
 - This issue can be easily resolved by updating the permissions of RDP or by doing clipboard redirection.

 

 
- Download Restoro PC Repair Tool that comes with Patented Technologies (patent available here).
 - Click Start Scan to find Windows issues that could be causing PC problems.
 - Click Repair All to fix issues affecting your computer's security and performance

 
- Restoro has been downloaded by 0 readers this month.

 
The inability to use copy and paste in RDP is one of the most annoying Windows issues.
 
Users of RDP often report that they are unable to copy text or files from their local computer and paste them on the remote computer, or vice versa.
 
This is one of the most prevalent issues that users have with RDP software.
 
This guide will provide you with a number of different solutions for the issue of copy and paste not functioning while using a remote desktop connection.
 
## Why does Remote Desktop not allow copy and paste?
 
Troubleshooting must be performed when a Windows desktop’s connection to its host through the remote desktop protocol fails. 
 
This may include examining firewall settings, security certificates, and other such items.
 
Network outages, difficulties with SSL certificates, authentication challenges, and storage constraints are just a few of the obstacles. These issues are faced by administrators while using remote desktop connections.
 
Other common reasons why you cannot copy paste in Remote Desktop are:
 
- Issues with the Credential Security Support Provider (CredSSP) protocol
 - Connectivity issues due to exceeded infrastructure capacity
 - Remote desktop connectivity issues

 
After knowing the common reasons for this problem, let’s head toward the solutions to fix it.
 
## What can I do if remote desktop computer is not allowing copy-paste?
 
### 1. Run the RDP from Task Manager
 
- Turn off the RDP, click the File tab in the Task Manager, and select Run New Task.

 
- Now type rdpclip.exe (your RDP name) and click OK.

 
- Now, you will probably face no trouble in copying and pasting the text from a remote computer.

 
### 2. Enable copy-paste functions from RDP connection properties
 
- Click on Show Options on the RDP connection window.

 
- Click on the option labeled Local Resources.

 
- Make sure the Clipboard option is selected and click More.

 
- Select the Drives option. Click OK.

 
- Now click Connect.

 
By making these adjustments, you have successfully enabled the ability to copy and paste between the local and remote computers.
 
### 3. Enable Remote Desktop Clipboard Redirection on the client’s computer
 
- To open a Run dialogue box on the client computer, simultaneously press the Windows + R.
 - Type regedit in the text box of the dialogue box and click OK to open the Registry Editor.

 
- In Registry, go to the following path: HKEY_LOCAL_MACHINE\Software\Microsoft\Terminal Server Client
 - Now, Ensure that the value data of the DisableClipboardRedirection is set to 0. If the value is 1, change it to 0, then close the Registry Editor.
 - Restart your PC and then see if the copy/paste function in RDP is working or not.

 
### 4. Fix Remote Desktop copy-paste not working in Registry
 
- Open the command box by pressing Window + R, type regedit, and press Enter.
 - In the Registry Editor, go to the two places below and change the value of the fDisableClip REG DWORD to 0. HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Terminal Server\Wds\rdpwd and HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Terminal Server\WinStations\RDP-Tc
 - Restart after making the change, and then check the copy-and-paste function in the Remote Desktop.

 
### 5. Enable copy-paste in Remote Desktop through Group Policy
 
- To launch the Run dialogue box, press both the Windows and R keys simultaneously on your keyboard.

 
- Type gpedit.msc into the text field of the dialogue box and click OK open the Group Policy Editor.

 
- In the Local Group Policy Editor, go to the following path: Computer Configuration\Administrative Templates\Windows Components\Remote Desktop Services\Remote Desktop Session Host\Device and Resource Redirection

 
- Open the Do not allow Clipboard redirection on the right.

 
- Select the Disabled option and then click OK.

 
- Close the Group Policy Editor application.
 - Open Command Prompt as Administrator and enter the following command to change the group policy or restart the machine and you are good to go. gpupdate /force

 
Copy-pasting problem is very common in RDP, but obviously, if there is a problem then there is a solution too.
 
We hope that the above solutions helped you in fixing the Remote Desktop copy-paste not working problem. 
 
Now, you should also check out our guide with quick fixes to use if Remote Desktop Connection is not working.
 
Do let us know using the comments section below which of the above methods worked for you. Also, feel free to ask any related questions that you may have. 
 
If the advices above haven't solved your issue, your PC may experience deeper Windows problems. We recommend downloading this PC Repair tool (rated Great on TrustPilot.com) to easily address them. After installation, simply click the Start Scan button and then press on Repair All.
 
Still having issues? Fix them with this tool:
 
SPONSORED
 
- Remote Desktop Connection

 
Email * 
 

Commenting as .
Not you?

 
Comment 





