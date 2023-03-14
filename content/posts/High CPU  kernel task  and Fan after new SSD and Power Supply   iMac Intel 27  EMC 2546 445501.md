---
title: "Is Your iMac Going Crazy? Discover the Shocking Cause of High CPU Kernel Task and Fan After Upgrading to New SSD and Power Supply!"
ShowToc: true 
date: "2023-02-10"
author: "Donna Harris"
---
*****
Is Your iMac Going Crazy? Discover the Shocking Cause of High CPU Kernel Task and Fan After Upgrading to New SSD and Power Supply!

Have you recently upgraded your iMac's hard drive to a solid-state drive (SSD) or replaced its power supply and noticed that your iMac's CPU kernel task is running at high percentages and the fan is running at full blast? You might be wondering what is causing this, and you are not alone.

Many Mac users who have upgraded their iMac's components have experienced this phenomenon. There are several reasons why your iMac's CPU kernel task is running at high percentages and your fan is running at full blast. 

One of the primary reasons for this issue is that the heat sink on the CPU is not properly seated when you reassembled the computer. When replacing the power supply or installing a new SSD, you need to open up the computer and remove various components. Sometimes, in the process, the heat sink on the CPU gets knocked out of position. This misalignment can cause the CPU to overheat and trigger your iMac's fan into overdrive.

Another reason that your iMac's processor might be running hot and causing the fan to turn on is that the thermal paste that conducts the heat away from the CPU has dried up or even wiped clean accidentally. If thermal paste is not applied or applied improperly, it can cause your CPU to overheat and your fan to spin continuously.

Finally, there is a chance that your newly installed SSD is not compatible with your iMac. This can cause issues like high CPU usage, system crashes, and unexpected shutdowns.

How to Fix the Problem?

If you are experiencing Kernel task high CPU usage and a loud fan on your iMac after upgrading to a new SSD or power supply, there are several steps you can take to resolve the issue. 

First, you can try reseating the heat sink on the CPU. This requires removing the CPU from the motherboard and reapplying thermal paste. Reseating the heat sink on the CPU correctly can reduce the temperature of the CPU by up to 5°C.

Secondly, consider replacing the current thermal paste with a fresh, high-quality paste. This will eliminate any dried-up or wiped-off paste that might be interfering with the heat transfer from the CPU to the heat sink.

Lastly, verify that your new SSD complies with Apple's specifications. While most SSDs are compatible with Macs, some have different firmware that can cause issues. You can check the specifications of your new SSD by visiting the manufacturer's website or contacting the manufacturer's support team.

In conclusion, if you've experienced high CPU usage and noisy fans after upgrading your iMac's hard drive or its power supply, there is a way to get your iMac running efficiently once again. Re-seating the heat sink, replacing the thermal paste, and confirming the SSD are some of the ways you can troubleshoot and solve the problem. Once you've done this, your iMac will be back to operating as usual, and you can continue enjoying the benefits of your updated system.

{{< youtube 41gq76SIjf8 >}} 



## Chosen Solution
 Hello all,
I’ve probably read just about every post on the internet regarding my issue and cannot find an answer so I am hoping the ifixit community can help.
I had issues with my late 2012 iMac randomly powering off, and the culprit of this seems to be a broken power supply. So I ordered a new LiteOn powersupply through ifixit and decided that if I am opening the iMac, I might as well change my 3TB HDD drive, with a 2TB SSD to speed up my old Mac. I purchase the Crucial MX500 2TB SSD.
Installation was not nearly as difficult as I expected, and had no problem installing all the items based on the guides provided. As suggested, I installed the thermal adapter on the SSD as well.
Hooked everything back up, installed Catalina and my computer all of a sudden was SLOW and super loud fan noise. Thinking it might be that Catalina doesn’t run on my old iMac, I reformatted the drive, and installed what came with my iMac, Mountain Lion, then updated to Mojave (which I ran on the old Hard drive). Neither Mountain Lion nor Mojave have affected the speed. It still runs super slow.
So, I bought a case for my old hard drive, plugged that in and booted the computer using the old hard drive using USB 3.0 to rule out the SATA cable. No change in speed. It’s even slower.
I have enabled TRIM, reset PRAM, reset SMC, tried to boot apple diagnostic pressing d or Shift + D but my computer is no longer supported, start up in safe mode using shift but there is no change.
Checked the activity monitor for both the HDD and SSD and the kernal_task is running extremely high. It never falls below 600%. This is on a clean install. Besides Mac Fan Control to lower the fan speed (it’s set to take the temperature from the SSD which seems to work), there isn’t really anything I have installed on the computer.
I’m attaching the EtreCheck, and some screenshots but hoping someone can point me in the right direction. Willing to open my iMac back up, but not sure what to do.
Really appreciate the help in advance
Sandra


hope this pastes ok.
EtreCheck version: 5.5.5 (5111)
Report generated: 2020-06-13 15:19:49
'''Download EtreCheck from https://etrecheck.com'''
Runtime: 16:57
Performance: Poor
Sandbox: Enabled
Full drive access: Disabled

Problem: Computer is too slow

Major Issues:
    Anything that appears on this list needs immediate attention.

    No Time Machine backup - Time Machine backup not found.
    Runaway process - A process is using a large percentage of your CPU.
    Poor performance - EtreCheck report shows poor performance. This is unusual.
    Software performance problems - Software seems to be causing performance problems.

Minor Issues:
    These issues do not need immediate attention but they may indicate future problems or opportunities for improvement.

    32-bit Apps - This machine has 32-bits apps will not work on macOS 10.15 "Catalina".
    Limited drive access - More information may be available with Full Drive Access.

Hardware Information:
    iMac (27-inch, Late 2012)
    iMac Model: iMac13,2
    3.4 GHz Intel Core i7 (i7-3770) CPU: 4-core
    24 GB RAM - Upgradeable
        BANK 0/DIMM0 - 8 GB DDR3 1600
        BANK 1/DIMM0 - 8 GB DDR3 1600
        BANK 0/DIMM1 - 4 GB DDR3 1600
        BANK 1/DIMM1 - 4 GB DDR3 1600

Video Information:
    NVIDIA GeForce GTX 680MX - VRAM: 2 GB
        iMac 2560 x 1440

Drives:
    disk0 - CT2000MX500SSD1 2.00 TB (Solid State - TRIM: Yes)
    Internal SATA 6 Gigabit Serial ATA
        disk0s1 - EFI (MS-DOS FAT32) [EFI] 210 MB
        disk0s2 [APFS Container] 2.00 TB
            disk1 [APFS Virtual drive] 2.00 TB (Shared by 4 volumes)
                disk1s1 - I****x (APFS) (Shared - 16.38 GB used)
                disk1s2 - Preboot (APFS) [APFS Preboot] (Shared)
                disk1s3 - Recovery (APFS) [Recovery] (Shared)
                disk1s4 - VM (APFS) [APFS VM] (Shared - 2.15 GB used)

Mounted Volumes:
    disk1s1 - I****x
        2.00 TB (Shared - 16.38 GB used, 1.98 TB free)
        APFS
        Mount point: /

    disk1s4 - VM [APFS VM]        2.00 TB (Shared - 2.15 GB used, 1.98 TB free)        APFS        Mount point: /private/var/vm

Network:
    Interface Bluetooth-Modem: Bluetooth DUN
    Interface en0: Ethernet
    Interface en1: Wi-Fi
        802.11 a/b/g/n
    Interface en2: Bluetooth PAN
    Interface bridge0: Thunderbolt Bridge

System Software:
    macOS Mojave 10.14.6 (18G103)
    Time since boot: About an hour

Notifications:
    Notifications not available without Full Drive Access.

Security:
    Gatekeeper: Enabled
    System Integrity Protection: Enabled

    Antivirus software: Apple

32-bit Applications:
    One 32-bit app

System Launch Agents:
    [Not Loaded] 15 Apple tasks
    [Loaded] 180 Apple tasks
    [Running] 105 Apple tasks

System Launch Daemons:
    [Not Loaded] 38 Apple tasks
    [Loaded] 178 Apple tasks
    [Running] 118 Apple tasks
    [Other] One Apple task

Launch Daemons:
    [Running] com.crystalidea.macsfancontrol.smcwrite.plist (Ilya Parniuk - installed 2020-06-13)

User Internet Plug-ins:
    User Internet Plug-ins need Full Drive Access

Audio Plug-ins:
    AppleTimeSyncAudioClock: 1.0 (Apple - installed 2019-09-20)
    BluetoothAudioPlugIn: 6.0.14 (Apple - installed 2019-09-20)
    AirPlay: 2.0 (Apple - installed 2019-09-20)
    AppleAVBAudio: 760.6 (Apple - installed 2019-09-20)
    BridgeAudioSP: 5.52 (Apple - installed 2019-09-20)
    iSightAudio: 7.7.3 (Apple - installed 2019-09-20)

User Audio Plug-ins:
    User Audio Plug-ins need Full Drive Access

User iTunes Plug-ins:
    User iTunes Plug-ins need Full Drive Access

Time Machine:
    Time Machine Not Configured!
    One local snapshot
    Oldest local snapshot: 2020-06-13 12:50:32
    Last local snapshot: 2020-06-13 12:50:32

Performance:
    System Load: 13.00 (1 min ago) 13.45 (5 min ago) 13.52 (15 min ago)
    Nominal I/O speed: 1.16 MB/s
    File system: 121.53 seconds (timed out)
    Write speed: 112 MB/s
    Read speed: 137 MB/s

CPU Usage Snapshot:
    Type Overall
    System: 85 %
    User: 5 %
    Idle: 10 %

Top Processes Snapshot by CPU:
    Process (count) CPU (Source - Location)
    Other processes 705.26 % (?)
    EtreCheck 9.32 % (App Store)
    Activity Monitor 5.45 % (Apple)
    Macs Fan Control 0.28 % (Ilya Parniuk)
    Dock 0.10 % (Apple)

Top Processes Snapshot by Memory:
    Process (count) RAM usage (Source - Location)
    EtreCheck 453 MB (App Store)
    Finder 84 MB (Apple)
    Spotlight 68 MB (Apple)
    accountsd 68 MB (Apple)
    NotificationCenter 60 MB (Apple)

Top Processes Snapshot by Network Use:
    Process Input / Output (Source - Location)
    Other processes 97 KB / 13 KB (?)
    SystemUIServer 0 B / 64 B (Apple)
    mdworker_shared 0 B / 0 B (Apple)
    backgroundtaskmanagementagent 0 B / 0 B (Apple)
    cfprefsd 0 B / 0 B (Apple)

Virtual Memory Information:
    Physical RAM: 24 GB

    Free RAM: 17.06 GB
    Used RAM: 4.04 GB
    Cached files: 2.91 GB

    Available RAM: 19.96 GB
    Swap Used: 0 B

Software Installs (past 30 days):
    Install Date Name (Version)
    2020-06-12 OS X (10.8.5 (12F45))
    2020-06-12 macOS Mojave (14.6.01)
    2020-06-12 SU_TITLE (10.14.6.1.1.1569030045)
    2020-06-13 XProtectPlistConfigData (2123)
    2020-06-13 CompatibilityNotificationData (1.0.6)
    2020-06-13 Gatekeeper Configuration Data (181)
    2020-06-13 MRTConfigData (1.62)
    2020-06-13 EtreCheck (5.5.5)

Diagnostics Information (past 7-30 days):
    Directory /Library/Logs/DiagnosticReports is not accessible.
    Enable Full Drive Access to see more information.

End of report

 In hopes that this will ease someone else’s frustration, here is an update:
After running out of ideas to fix my computer, I took my iMac to a local repair shop, who confirmed that the PowerSupply I purchased is not compatible with a late 2012 iMac 27”. Opposite of what the product information states from ifixit, the one send is only good for a 2015-2017 iMac. He also confirmed that the SSD Thermal Sensor I installed had shorted. He said I was lucky to not kill my logic board.
Overall, had it been the correct power supply, the install instructions from this website were on point and would’ve fixed my computer.




