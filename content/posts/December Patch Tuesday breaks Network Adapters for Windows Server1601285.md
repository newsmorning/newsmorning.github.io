---
title: "You Won't Believe How December Patch Tuesday Disrupts Windows Server Network Adapters!"
ShowToc: true 
date: "2023-05-22"
author: "Donny Bluhm"
---
*****
Title: You Won't Believe How December Patch Tuesday Disrupts Windows Server Network Adapters!

Introduction:

Patch Tuesday is a regular event that takes place on the second Tuesday of every month when Microsoft releases security patches and bug fixes for its products. December Patch Tuesday reportedly brought in six critical updates for Windows Server operating systems. However, while the update was meant to fix bugs and increase security, it caused more problems than it actually solved. Specifically, the update disrupted network adapters on Windows servers.

Body:

The update caused chaos following numerous reports of servers losing their network connections following the installation of the update. The issue is attributed to a bug in the update. Since various devices connect to Windows servers such as laptops, printers, scanners, and other peripherals, the failure of the network adapters seriously hindered the smooth running of operations in affected organizations.

Microsoft has identified the problem and has recommended some remedial measures to overcome it, such as manually installing an update, tweaking the Local Security Policy Editor, or using a Group Policy to disable kernel updates. Suppose your organization does not have a dedicated IT support team. In that case, it is essential to keep up to date with these patches and monitor the updates for glitches that may disrupt essential operations.

Conclusion:

December Patch Tuesday disruption was not only annoying but also frustrating as it impacted the productivity of businesses that are relying on technology. Microsoft acknowledged the issue in a blog post and is working on a fix. Microsoft also issued a preview for the January 2021 Security Updates to address the issue. To ensure the smooth running of operations, vigilance is required on a frequent basis, especially when using various devices for operations. Therefore, it is essential to monitor updates and seek timely support from IT specialists to tackle any issues that may arise.

{{< youtube L8tdPYqFV7E >}} 



By now, you are undoubtedly aware that Microsoft rolled out Patch Tuesday updates to various Windows versions just a couple of days ago. 
 
- Microsoft acknowledged that the latest Patch Tuesday rollout broke features in Windows Server.
 - Users were getting errors when creating a new Network Adapter, or Network Interface Card (NIC).
 - The issue has been officially fixed by Microsoft, so you no longer have to worry about this at all.

 
While, as usual, some of them have brought along new features and known issues, other annoying problems have also popped up. 
 
That being said, know that today, Microsoft has confirmed that the process to create Network Adapters on some Hyper-V hosts is broken in Windows Server.
 
If you feel like you have been affected by this issue, this article will help you have a better understanding of the issue.
 
## The December 2022 Patch Tuesday brings more problems 
 
In a recent update on the health dashboard, the tech giant notes that customers who install the KB5021249 update might be treated to issues concerning Hyper-V hosts on Windows Server installations. 
 
To give you a better understanding, an error will be thrown when creating a new Network Adapter, or Network Interface Card (NIC) joined to a virtual machine (VM) network. 
 
Of course, this may also occur when creating a new VM with a Network Adapter joined to a VM network, just so you know. 
 
Thus, the bug only affects new NICs and existing ones should work fine post-KB5021249 update, so keep that in mind. 
 
As you would have expected, this issue will interrupt the workflow on Hyper-V hosts managed by Software Defined Networking (SDN) configured System Center Virtual Machine Manager (VMM).
 
We are also going to show you exactly the errors you can face when encountering the problem, so that you won’t be taken by surprise:
 
- When creating a new VM or a new network adapter on an existing VM, you might receive, vmName failed to modify device ‘Ethernet Connection
 - Software-defined networking (SDN) software load balancer service might fail, and you might receive, SLBVMName failed to modify device ‘Ethernet Connection’ error
 - SDN RAS Gateway service might fail, and you might receive, GatewayVMName failed to modify device ‘Ethernet Connection’ error

 
Please note that, for now, the mitigation that Microsoft has offered is to run the following commands on PowerShell running with administrator privileges:
 
$lang = (Get-WinSystemLocale).Name

C:\Windows\system32\wbem\mofcomp.exe C:\Windows\system32\wbem\$lang\VfpExt.mfl

C:\Windows\system32\wbem\mofcomp.exe C:\Windows\system32\wbem\VfpExt.mof
 
If large-scale installations are your concern, these commands can also be integrated as a post-install script through the guide that Microsoft has prepared.
 
The Redmond company has assured customers that it is working on a fix but has not hinted at how long it will take to patch the problem. 
 
The good news is that Microsoft has released out-of-band (OOB) updates today that resolve the issue. For Windows Server 2022, it is KB5022553, while for Server 2019, it is KB5022554.
 
This non-security update includes quality improvements. When you install this KB:
 
This update addresses a known issue that affects Hyper-V hosts that use software-defined networking (SDN) and are managed by System Center Virtual Machine Manager (VMM). 
 
Now, however, you can say goodbye to receiving an error for workflows that involve:
 
- Creating a new network adapter for an existing virtual machine (VM) that is joined to a VM network
 - Creating a new VM that has a network adapter that is joined to a VM network.

 
Keep in mind that Windows Server wasn’t the only platform affected by Patch Tuesday bugs as Windows 10 is experiencing hidparse BSODs.
 
Be aware that the issue only affects Windows Server 2019 and Windows Server 2022, so client installations of Windows are unaffected.
 
Have you also run across this nasty error? Let us know in the comments section located just below.
 

 
If the advices above haven't solved your issue, your PC may experience deeper Windows problems. We recommend downloading this PC Repair tool (rated Great on TrustPilot.com) to easily address them. After installation, simply click the Start Scan button and then press on Repair All.
 
Still having issues? Fix them with this tool:
 
SPONSORED
 
- windows server

 
Email * 
 

Commenting as .
Not you?

 
Comment 





