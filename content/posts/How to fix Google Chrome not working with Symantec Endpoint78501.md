---
title: "Discover the Quick and Easy Fix to Make Google Chrome and Symantec Endpoint Play Nice Together!"
ShowToc: true 
date: "2023-06-16"
author: "Nancy Alonzo"
---
*****
# Discover the Quick and Easy Fix to Make Google Chrome and Symantec Endpoint Play Nice Together!

Are you having trouble with Google Chrome and Symantec Endpoint not working together? It's a common problem that can be frustrating to deal with. But don't worry, there's an easy fix that will have your web browsing running smoothly in no time.

# The Problem

The issue arises when Symantec Endpoint, an antivirus software, blocks Google Chrome from accessing certain websites or web applications. This can cause Chrome to crash, freeze or simply not work properly, leaving you unable to fully utilize its features. Common sites that have experienced issues include Gmail and Google Drive.

# The Solution

The solution to this problem is straightforward. You need to add Google Chrome to the list of trusted applications in Symantec Endpoint. This will allow Chrome to bypass the antivirus software's checks and allow access to all websites and applications without interruption. There are a few steps to follow to enable this feature.

1. Open Symantec Endpoint on your device.

2. Select the "Firewall" tab from the left-hand menu.

3. Go to the "Program Control" section and click the "Add" button at the bottom.

4. Find the Google Chrome application on your computer and select it.

5. Set the "Access" setting to "Allow".

6. Click "OK" to save the changes.

And that's it! You've successfully added Google Chrome to the list of trusted applications in Symantec Endpoint. You can now browse the web freely without worry of any interruptions from the antivirus software.

# Conclusion

It can be frustrating when Google Chrome and Symantec Endpoint don't work together seamlessly. Fortunately, adding Chrome to the trusted applications list in Symantec Endpoint is an easy fix. Don't let this issue continue to hinder your web browsing experience – take the time to follow these steps and enjoy the full capabilities of Google Chrome.

{{< youtube 3lcTkTyAlU0 >}} 



In October 2019, users started posting on the Symantec support forum about an Aw Snap error that arises in Chrome when they start the browser.
 
 
 
- Download DriverFix (verified download file).
 - Click Start Scan to find all problematic drivers.
 - Click Update Drivers to get new versions and avoid system malfunctionings.

 
- DriverFix has been downloaded by 0 readers this month.

 
The Aw Snap crash error isn’t something new. However, in this case, it occurs because Chrome 78 and 79 are not compatible with Symantec Endpoint Security software versions.
 
The incompatibility issue arises on any Windows platform that includes a Symantec Endpoint version that predates 14.2 RU2 MP1.
 
The issue largely pertains to Windows 2016 and Windows 10 RS1 platforms with SEP and Google Chrome browsers installed. Note, however, that Edge Chromium 78 and 79 are also incompatible with Symantec Endpoint Protection.
 
## How can I fix Chrome’s incompatibility with Symantec Endpoint?
 
### 1. Update Symantec Endpoint Protection
 
Symantec’s official fix for SEP’s Chrome incompatibility is to update Symantec Endpoint to the latest 14.2 version.
 
You can get the latest patch update for Endpoint Protection (build 5569) from the RU2 MP1 client-only patches page. That page includes instructions for how you can download the latest patch and update the software with it.
 

 
### 2. Deactivate Chrome’s renderer code
 
- Right-click Google Chrome’s desktop shortcut and select Properties.
 - Select the Shortcut tab.
 - Then enter the following line in the Target text box as shown directly below:
 - -disable-features=RendererCodeIntegrity
 - Select the Apply option.
 - Click the OK button.

 
If you’re tired of Google Chrome’s incompatibilities, check out this article for some good alternatives
 
- -disable-features=RendererCodeIntegrity

 
### 3. Edit the registry
 
- Press the Windows key + R hotkey, which opens Run.
 - Input ‘regedit’ in the Open box and press Enter to open the Registry Editor.
 - Go to this registry key: HKLM > Software > Policies > Google Chrome.
 - Double-click the RendererCodeIntegrityEnabled DWORD on the right of the window.
 - Change its value to 0 in the Edit Dword window.
 - Click the OK option.

 
If you have issues opening the Registry Editor, check out this detailed guide for some quick fixes.
 
### 4. Launch Chrome with no sandbox
 
- Right-click a shortcut icon for Chrome on the desktop and select Properties.
 - Click the Shortcut tab on the window that opens.
 - Then add –no-sandbox to end of the Target box as below
 - Select the Apply option.
 - Click the OK button.

 
### Edit Chrome’s exe file title
 
- Launch File Explorer with the Windows key + E keyboard shortcut.
 - Open the folder that includes Chrome’s EXE file.
 - Right-click Chrome’s EXE and select Rename.
 - Enter Chrome as the new file title, but don’t change the EXE format at the end.

 
Those are a few of the resolutions confirmed to fix Google Chrome’s Aw Snap incompatibility error with Symantec Endpoint.
 
Remember, however, that you can always switch to browsers that don’t have any compatibility issues with Endpoint Protection, such as Firefox or Opera.
 
Which one of the many solutions listed above fixed the issue for you? Let us know by leaving a message in the comment scetion below.
 
If the advices above haven't solved your issue, your PC may experience deeper Windows problems. We recommend downloading this PC Repair tool (rated Great on TrustPilot.com) to easily address them. After installation, simply click the Start Scan button and then press on Repair All.
 
Still having issues? Fix them with this tool:
 
SPONSORED
 
- Google Chrome Errors

 
Email * 
 

Commenting as .
Not you?

 
Comment 





