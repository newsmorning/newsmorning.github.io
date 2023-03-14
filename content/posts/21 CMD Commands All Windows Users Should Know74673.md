---
title: "Are You Ready to Unlock The Secrets of Your PC? 21 Must-Know Cmd Commands for Windows Users!"
ShowToc: true 
date: "2023-02-22"
author: "Wendy Santiago"
---
*****
Title: Are You Ready to Unlock the Secrets of Your PC? 21 Must-Know Cmd Commands for Windows Users!

Introduction:

Windows operating system is the most widely used system in the world, loved by millions of people for its ease-of-use, versatility, and user-friendly interface. However, what many people don't know is that there is a hidden world just beneath the surface of Windows, full of powerful tools, and features that can make your life easier.

This hidden world is known as the Command Prompt, or Cmd for short. It's a powerful tool that can help you diagnose problems with your computer, tweak its settings, and perform all sorts of tasks that would otherwise be impossible. So, if you're ready to take your Windows experience to the next level, read on to discover 21 must-know Cmd commands for Windows users.

Body:

1. Ipconfig

The Ipconfig command is one of the most useful commands for networking. It allows you to view your computer's IP address, the subnet mask, and the default gateway.

2. Ping

The Ping command is a networking tool that allows you to test the connectivity of a device. It sends a packet of data to the IP address you specify and waits for a response.

3. Tracert

Tracert is a tool that helps you determine the route that your traffic takes to reach a destination. It shows you all the routers between your computer and the destination.

4. Netstat

The Netstat command allows you to view active connections on your computer, including the IP address, port, and protocol used.

5. Tasklist

The Tasklist command allows you to view a list of all the processes running on your computer, including their process ID, memory usage, and CPU time.

6. Taskkill

The Taskkill command allows you to terminate a process that is causing problems on your computer. It's a useful tool for troubleshooting.

7. Shutdown

The Shutdown command allows you to shut down, restart, or log off your computer quickly.

8. Systeminfo

The Systeminfo command provides the complete configuration of your computer, including the hardware and OS details.

9. Driverquery

The Driverquery command allows you to view a list of all the drivers installed on your computer, including their versions and dates.

10. Sfc

The Sfc command allows you to scan for and repair corrupted system files. It's a useful tool for keeping your computer running smoothly.

11. Dism

Dism is a tool that allows you to repair the Windows installation, including offline correction and image repairs.

12. Netsh

The Netsh command is a powerful networking tool that allows you to configure and manage network settings.

13. Cipher

The Cipher command allows you to securely delete files and folders, ensuring that they cannot be recovered.

14. System File Checker

The System File Checker command allows you to scan your system files and repair them if necessary.

15. Ipconfig/flushdns

The Ipconfig/flushdns command allows you to clear the DNS cache, which can help resolve network-related issues.

16. Net User Command

Net user command allows you to manage user accounts on your computer and change their passwords.

17. Netstat-aon

This command allows you to view all the active connections on your computer, including their IP addresses, protocols, and port numbers.

18. Robocopy

Robocopy is a tool that allows you to copy large files and folders quickly and efficiently. It's a useful tool for backups and data transfers.

19. Fsutil

Fsutil is a tool that allows you to manage file and disk operations, including managing file permissions and NTFS compression.

20. Diskpart

Diskpart is a tool that allows you to manage disk partitions, including creating partitions and formatting them.

21. Sc.exe

The Sc.exe command allows you to manage Windows services, including starting and stopping them.

Conclusion:

There you have it, 21 must-know Cmd commands for Windows users. With these powerful tools at your disposal, you'll be able to diagnose problems, tweak your settings, and perform all sorts of tasks that would otherwise be impossible. So, if you're ready to take your Windows experience to the next level, start exploring the powerful world of the Command Prompt today!

{{< youtube Jfvg3CS1X3A >}} 



The Windows command prompt is a feature that’s been a core
part of the Windows operating system for a long time. There are some CMD
commands that are so useful and easy to use that even regular users see the
Windows command prompt as a key part of the operating system.
 
There are always rumors that it will be phased out at some
point, but that’s unlikely to happen any time soon. 
 
The following are 21 of the best CMD commands you should know if you want to have more control over your Windows PC.
 

 
Also, be sure to check out our YouTube video where we go over the commands listed in this article:
 
## 1. ASSOC: Fix File Associations
 
One of the most powerful tools in the CMD command library is
the ASSOC command. 
 
Your computer associates certain file extensions with
certain programs. This is how your computer knows to open Adobe when you double
click a PDF file, or Microsoft Word when you double click a DOC file. 
 
You can view all the file associations your computer knows
about by typing ASSOC in the command
window. You’ll see the file extension and the program it’s associated with.
 
You can set the association by typing something like assoc .doc=Word.Document.8.
 
## 2. FC: File Compare
 
Sometimes when files are changed over time, it’s hard to
remember what the differences were between versions. You may not know that a
CMD command offers the ability to compare files and see all differences, but
it’s true.
 
The FC command
performs either an ascii or a binary file comparison and will list all of the
differences that it finds.
 
Fc /a File1.txt
File2.txt will compare two ascii files.
 
Fc /b Picture1.jpg
Picture2.jpg will do a binary compare on two images.
 
## 3. IPCONFIG: IP Configuration
 
Network troubleshooting is never simple, but one command
that makes it much easier is IPCONFIG.
 
Using this command in the CMD command prompt returns detailed
information about your current network adapter connection including:
 
- Current IP AddressSubnet MaskDefault Gateway IPCurrent domain

 
This information can help you troubleshoot router issues and
other connection issues you could be having with your network adapter.
 
## 4. NETSTAT: Network Statistics
 
Concerned that you could have malware running on your
computer that’s connecting to internet locations without you knowing about it? 
 
If you run a NETSTAT
command in the command prompt, you can get a list of all active TCP connections
from your computer.
 
## 5. PING: Send Test Packets
 
An IT Analyst’s best friend is the PING command.  Running this
command sends test packets over the network to the target system.
 
You can use the PING command to test whether your computer
can access another computer, a server, or even a website. It can help with
revealing network disconnections. It also provides transit time for the packets
in milliseconds, so it also reveals a bad network connection as well.
 
## 6. TRACERT: Trace Route
 
TRACERT is a
fascinating Windows Command to use. If you’re ever curious to see the path your
internet traffic takes to get from your browser to a remote system like Google
servers, you can use TRACERT to see it.
 
The command stands for “Trace Route”, which sends packets
out to a remote destination (server or website), and provides you with all of
the following information:
 
- Number of hops (intermediate servers) before
 - getting to the destinationTime it takes to get to each hopThe IP and sometimes the name of each hop

 
TRACERT can reveal how the routes of your internet requests
change depending where you’re accessing the web. It also helps with
troubleshooting a router or switch on a local network that may be problematic.
 
## 7. POWERCFG: Power Configuration
 
Are you frustrated with how quickly your laptop seems to run
out of power? It could be that your power settings are configured as
efficiently as possible. There’s a windows CMD command called POWERCFG (power configuration) that can
help. Run the command prompt as an administrator and type powercfg – energy to get a full power efficiency report.
 
The process can take up to about a minute, but when it’s done,
you’ll see whether there are any warnings or errors that might help you improve
the power efficiency of your system.
 
View the energy-report.html file to see the details of those
errors and warnings.
 
## 8. SHUTDOWN: Turn Off Computer
 
The SHUTDOWN
command is a pretty versatile command that lets you shutdown the computer but
control the behavior of that shutdown. It’s commonly used as a scheduled task
or part of an IT batch job after patches have been applied to a computer
system.
 
Typing shutdown /i
from the command prompt will initiate a shutdown, but it’ll upon a GUI to give
the user an option on whether to restart or do a full shutdown. If you don’t
want to have any GUI pop up, you can just issue a shutdown /s command. 
 
There is a long list of other parameters you can use to do a
log off, hibernate, restart, and more. Just type shutdown without any arguments to see them all.
 
## 9. SYSTEMINFO: System Information
 
If you need to know what brand of network card you have,
processor details, or the exact version of your Windows OS, the SYSTEMINFO command can help.
 
This command polls your system and pulls the most important
information about your system. It lists the information in a clean format
that’s easy to read.
 
## 10. SFC: System File Checker
 
If you’re ever concerned that a virus or some other software
might have corrupted your core system files, there’s a Windows command that can
scan those files and ensure their integrity.
 
You need to launch CMD as administrator (right click and
choose Run as Administrator). Typing
SFC /SCANNOW will check the integrity of all protected system files. If a
problem is found, the files will be repaired with backed-up system files.
 
The SFC command also lets you:
 
- /VERIFYONLY:
 - Check the integrity but don’t repair the files./SCANFILE:
 - Scan the integrity of specific files and fix if corrupted./VERIFYFILE:
 - Verify the integrity of specific files but don’t repair them./OFFBOOTDIR:
 - Use this to do repairs on an offline boot directory./OFFWINDIR:
 - Use this to do repairs on an offline Windows directory./OFFLOGFILE:
 - Specify a path to save a log file with scan results.

 
The scan can take up to 10 or 15 minutes, so give it time.
 
## 11. NET USE: Map drives
 
If you want to map a new drive, you could always open File
Explorer, right click on This PC, and go through the Map Network Drive wizard.
However, using the NET USE command,
you can do the same thing with one command string.
 
For example, if you have a share folder on a computer on
your network called \\OTHER-COMPUTER\SHARE\, you can
map this as your own Z: drive by typing the command:
 
Net use Z: “\\OTHER-COMPUTER\SHARE”
/persistent:yes
 
The persistent
switch tells your computer that you want this drive remapped every time you log
back into your computer.
 
## 12. CHKDSK: Check Disk
 
While the SFC command only checks the integrity of core
system files, you can use the CHKDSK
command to scan an entire drive.
 
The command to check the C: drive and repair any problems,
launch the command window as an administrator and type CHKDSK /f C:. 
 
This command checks for things like:
 
- File fragmentationDisk errorsBad sectors

 
The command can fix any disk errors (if possible). When the
command is finished, you’ll see a status of the scan and what actions were
taken.
 
## 13. SCHTASKS: Schedule Tasks
 
Windows comes with a wizard for creating scheduled tasks.
For example, maybe you have a BAT file stored on C:\temp that you want to run
every day at noon. 
 
You’d have to click through the Scheduled Task wizard to
configure this. Or you can type a single SCHTASKS
command to set it up.
 
SCHTASKS /Create /SC
HOURLY /MO 12 /TR Example /TN c:\temp\File1.bat
 
The scheduled switch accepts arguments like minute, hourly,
daily, and monthly. Then you specify the frequency with the /MO command.
 
If you typed the command correctly, you’ll see the response,
SUCCESS: The scheduled task “Example”
has successfully been created.
 
## 14. ATTRIB: Change File Attributes
 
In Windows, you can change file attributes by right clicking
on a file and finding the right property to change. However, instead of hunting
around for the file attribute, you can use the ATTRIB command to set the file attributes.
 
For example, if you type: ATTRIB +R +H C:\temp\File1.bat, it’ll set File1.bat as a hidden,
read-only file.
 
There is no response when it’s successful, so unless you see
an error message, the command worked.
 
## Other Windows CMD Commands
 
As you can see, there are some powerful and useful things
you can do with the Windows command prompt, if you know the right commands.
 
Believe it or not, there are even more commands that will
give you the ability to do some things you probably never realized just by
typing a simple command.
 
- BITSADMIN:
 - Initiate upload or download jobs over the network or internet and monitor the
 - current state of those file transfers.COLOR:
 - Change the background color of the command prompt window.COMP:
 - Compare the contents of any two files to see the differences.FIND/FINDSTR:
 - Search for strings inside of any ASCII files.PROMPT:
 - Change the command prompt from C:\> to something else. TITLE:
 - Change the title of the command prompt window.REGEDIT:
 - Edit keys in the Windows registry (use with caution).ROBOCOPY:
 - A powerful file copy utility built right into Windows.

 
If you’re interested in learning more, Microsoft offers a full list of all of the Windows CMD commands included in the latest version of the Windows OS.



