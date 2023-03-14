---
title: "Unlock Security Secrets: Discover 5 Simple Ways to Enable/Disable TLS on Your Windows Server Today!"
ShowToc: true 
date: "2023-06-02"
author: "Vernon Segura"
---
*****
Title: Unlock Security Secrets: Discover 5 Simple Ways to Enable/Disable TLS on Your Windows Server Today!

TLS or Transport Layer Security is a protocol that is used to secure communications between applications and servers or devices. It uses encryption to protect the content of messages sent over a network. Enabling TLS on your Windows Server can help protect against cyber-attacks, but disabling it can cause compatibility issues with certain applications. In this article, we will discover 5 simple ways to enable/disable TLS on your Windows Server today.

1. Enable TLS using Group Policy:

Group Policy is a powerful tool that enables administrators to manage policies and settings across a network. To enable TLS using Group Policy, follow these steps:

a. Open the Group Policy Editor.

b. Navigate to Computer Configuration > Administrative Templates > Windows Components > Internet Explorer > Internet Control Panel > Advanced Page.

c. Enable the “Turn off Encryption Support” policy.

d. Select the “TLS 1.0”, “TLS 1.1”, and “TLS 1.2” checkboxes.

e. Click Apply and then OK.

2. Enable TLS using the Registry Editor:

The Registry Editor is a built-in tool on Windows that enables users to view and modify the system registry. To enable TLS using the Registry Editor, follow these steps:

a. Open the Registry Editor.

b. Navigate to the following path: HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client.

c. Create a new DWORD value named “DisabledByDefault” and set its value to “0”.

d. Create a new DWORD value named “Enabled” and set its value to “1”.

3. Disable TLS using Group Policy:

To disable TLS using Group Policy, follow these steps:

a. Open the Group Policy Editor.

b. Navigate to Computer Configuration > Administrative Templates > Windows Components > Internet Explorer > Internet Control Panel > Advanced Page.

c. Enable the “Turn off Encryption Support” policy.

d. Clear the checkboxes for “TLS 1.0”, “TLS 1.1”, and “TLS 1.2”.

e. Click Apply and then OK.

4. Disable TLS using the Registry Editor:

To disable TLS using the Registry Editor, follow these steps:

a. Open the Registry Editor.

b. Navigate to the following path: HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client.

c. Create a new DWORD value named “DisabledByDefault” and set its value to “1”.

d. Create a new DWORD value named “Enabled” and set its value to “0”.

5. Enable/Disable TLS using PowerShell:

PowerShell is a powerful command-line tool that enables administrators to automate Windows tasks. To enable/disable TLS using PowerShell, follow these steps:

a. Open PowerShell as an administrator.

b. To enable TLS 1.2, run the following command: Set-ItemProperty -Path 'HKLM:\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client' -Name 'Enabled' -Value '1'

c. To disable TLS 1.2, run the following command: Set-ItemProperty -Path 'HKLM:\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client' -Name 'Enabled' -Value '0'

Conclusion:

Transport Layer Security is an essential protocol for securing communications between servers, devices, and applications across networks. Enabling or disabling TLS can greatly impact your network's security and compatibility with various applications. Using the methods mentioned above in this article, you can easily enable/disable TLS on your Windows Server today. Remember, it is essential to keep your network security up-to-date, and TLS is an essential tool in achieving that goal.

{{< youtube 8q9qJzteBn8 >}} 



If you were wondering how to enable or disable TLS (Transport Layer Security) on Windows Server, you are at the right place. 
 
## TLS is critical for data encryption between the client and a web server
 
- To ensure maximum security, it's important to enable TLS on Windows Server properly.
 - Modifying a couple of values in your registry is the simplest way to do that.
 - If you prefer using the command line, you can enable this feature using PowerShell.

 

 
- Download Restoro PC Repair Tool that comes with Patented Technologies (patent available here).
 - Click Start Scan to find Windows issues that could be causing PC problems.
 - Click Repair All to fix issues affecting your computer's security and performance

 
- Restoro has been downloaded by 0 readers this month.

 
Transport Layer Security 1.0 hasn’t been supported for a while, so what you also want to do, besides enabling the latest TLS 1.2, is disabling the older version as well. 
 
For security reasons, it’s necessary to have the latest security protocol on your Windows Server and not the outdated version that has vulnerabilities.
 
Therefore, in this guide, we’re going to show you how to properly enable and disable TLS.
 
## How do I know if TLS 1.2 is enabled on Windows Server?
 
- Press the Windows key + R to start Run, type regedit, and press Enter or click OK.
 - Now go to the following key and check it. If it’s present, the value should be 0: HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client\DisabledByDefault
 - Also, check the following key. If you find it, its value should be 1: HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client\Enabled
 - If you can’t find any of the keys or if their values are not correct, then TLS 1.2 is not enabled.

 
#### How does TLS work?
 
TLS is a cryptographic protocol that encrypts the data between the client and a web server, thus protecting it from being viewed by a third party.
 
It also provides you with authentication and integrity protection, ensuring that the data and both the server and client are genuine.
 
There are four versions of TLS available, with the latest and safest one being 1.3, so be sure to use it along with reliable antivirus for Windows Server for maximum protection.
 
#### How do I enable TLS 1.0 on Windows Server?
 
- Press Windows key + R and enter regedit. Now press Enter.
 - Navigate to the following key: HKLM\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols
 - Right-click the right pane, expand the New section and select Key.
 - Name the new key TLS 1.0 and move to it.
 - Create a new key called Client and move to it.
 - Now right click the right pane, and select DWORD (32-bit) Value from the New menu.
 - Name the new DWORD Enabled and double-click it to open its properties.
 - Set the Value data to 1 and click OK to save changes.

 
Although the solution above helps you with this old version we recommend the Windows Server disable TLS 1.0 and get the newer version.
 
## How can I enable TLS on Windows Server?
 
### 1. Enable TLS 1.2 on Windows Server by modifying the registry
 
- If you are running Windows Server 2008, check this Microsoft’s article regarding the necessary update in order to enable TLS 1.2. Once you’ve installed updates, move to the steps below.
 - Open Registry Editor by pressing Windows key + R and entering regedit.
 - Since we are dealing with registry, we strongly suggest backing up the current registry state. Incorrect changes to the registry might have detrimental effects on your system.
 - Once we’ve dealt with that, follow this path:Computer\HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols
 - Right-click on the empty space in the right pane and choose New and then Key.
 - Name the new key TLS 1.2 and click to expand it.
 - Navigate to TLS 1.2, click on the empty space in the right pane and add two new keys. Name the first one Client and the second one Server. It should look like this.
 - Now, select the Client key, right-click in the right pane and select New and then DWORD (32-bit) Value.
 - Name the DWORD DisabledByDefault, and double-click it.
 - Ensure that the Base is Hexadecimal and the value is 0 (zero).
 - Create a new DWORD and name it Enabled and double-click it.
 - Ensure that the Base is, again, Hexadecimal and the Value is set to 1.
 - Repeat this for the Server key with the exactly the same DWORDS and values.
 - Close the Registry Editor and reboot your server.
 - If you want to revert back to the initial settings, just restore the Registry state from the backup.

 
To avoid any unplanned issues, it might be a good idea to use reliable backup software for Windows Server.
 
Some PC issues are hard to tackle, especially when it comes to corrupted repositories or missing Windows files. If you are having troubles fixing an error, your system may be partially broken. We recommend installing Restoro, a tool that will scan your machine and identify what the fault is.Click here to download and start repairing.
 
Expert tip:
 
SPONSORED
 
### 2. Enable TLS 1.2 with Powershell on Windows Server
 
- Press Windows key + X and select Windows PowerShell (Admin) from the menu.
 - When PowerShell opens, run the following commands:New-Item 'HKLM:\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server' -ForceNew-Item 'HKLM:\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client' -ForceNew-ItemProperty -Path 'HKLM:\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server' -name 'Enabled' -value '1' –PropertyType 'DWORD'New-ItemProperty -Path 'HKLM:\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server' -name 'DisabledByDefault' -value '0' –PropertyType 'DWORD'New-ItemProperty -Path 'HKLM:\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client' -name 'Enabled' -value '1' –PropertyType 'DWORD'New-ItemProperty -Path 'HKLM:\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client' -name 'DisabledByDefault' -value '0' –PropertyType 'DWORD'

 
So, by applying these commands you trigger Windows Server to enable TLS 1.2 using PowerShell.
 
### 3. Disable TLS 1.0 and TLS 1.1
 
- Open Registry Editor. To do that, press Windows key + R and enter regedit.
 - Navigate to Computer\HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols
 - Select Protocols and in the right pane, right-click the empty space. Now choose New and select DWORD (32-bit) Value.
 - Create a new key as already explained, and name it TLS 1.1. You can create the one named TLS 1.0 as well.
 - Navigate to the TLS 1.1 key and create a new key called Client. You can also create a Server key if you want
 - Navigate to the key you created, and make a new DWORD named Enabled.
 - Dobule-click the Enabled DWORD. Set its value to 0 and confirm changes.

 
### Is there any tool to enable TLS 1.2 on Windows Server?
 
- Download ISS Cryptio GUI.
 - Once you download the application, run it.
 - Check TLS 1.2 and click on Apply.

 
### How to enable TLS 1.3 on Windows Server?
 
- Make sure you’re using Windows Sever 2022.
 - Press Windows key + S and enter command prompt. Select Run as adminsitrator.
 - Run the following command: reg add "HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\services\HTTP\Parameters" /v EnableHttp3 /t REG_DWORD /d 1 /f

 
### Is TLS 1.2 enabled on Windows Server 2016?
 
The good news is that starting with Windows Server 2016, TLS 1.2 is supported by default for WSUS. 
 
- How To Add An User To Windows Server [2008, 2012 & 2016]
 - What is Active Directory Account Lockout and How to Prevent It

 
In other words, there is no need to enable TLS 1.2 on Windows Server 2016 or Windows Server 2019.
 
Therefore, you only need to update TLS 1.2 on Windows Server 2012 and Windows Server 2012 R2 WSUS servers.
 
That’s how to enable or disable TLS on Windows Server. With those steps, TLS 1.2 is enabled and TLS 1.0 disabled with ease. 
 
All of these solutions require you to modify your registry, so be sure to create a backup beforehand. Also, we advise you to check our guide on how to restore Windows registry without a backup for more information.
 
What method do you use to enable TLS 1.2 on Windows Server? Let us know in the comments section below.
 
- TLSwindows server

 
Email * 
 

Commenting as .
Not you?

 
Comment 





