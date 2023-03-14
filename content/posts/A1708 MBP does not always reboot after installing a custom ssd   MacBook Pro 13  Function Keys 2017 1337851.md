---
title: "SHOCKING: New Macbook Pro glitch leaves users unable to reboot after custom SSD installation!"
ShowToc: true 
date: "2023-01-06"
author: "Brenda Jones"
---
*****
Title: SHOCKING: New Macbook Pro glitch leaves users unable to reboot after custom SSD installation!

Subheading: Apple faces heat over a grave MacBook Pro issue that's been causing serious problems to numerous users worldwide.

Introduction:

For several months now, Apple has been receiving an increasing number of complaints from MacBook Pro users over a critical glitch. The glitch is associated with customers who have installed custom high-capacity SSD upgrades in their new MacBook Pros, resulting in an inability to boot the device. Apple's failure to address the issue has caused outrage among consumers who are demanding immediate action. In this article, we will examine the extent of the problem and the potential solutions.

Body:

The MacBook Pro is a high-end laptop that comes with impressive features such as a high-resolution Retina display, Touch Bar, Touch ID, fast processing speeds, and impressive graphics performance, among others. It is no wonder that it has become the preferred device for many professionals and tech enthusiasts worldwide. However, this glitch makes it unusable, especially for those who have a custom SSD installed, as it causes the device to go into an infinite loop, rendering it impossible to boot.

The problem appears to originate from the latest versions of Apple's T2 chip. This chip is responsible for various functions such as system security, storage and power management, among others. The T2 chip also oversees the storage control, which explains the glitch’s origin in SSDs. According to Apple, the issue affects third-party drives installed on the new MacBook Pro, and Apple has not released any fix or update to address the problem.

The issue has been frustrating MacBook Pro users, mostly tech enthusiasts who perform upgrades themselves frequently. Many have taken to social media platforms to express their frustration and demand a solution. Some have even reported having to replace their new MacBook Pros, which is not only an inconvenience but also an unnecessary expense.

However, there are reports of a temporary solution to the glitch. According to online forums and user reviews, users who are experiencing the issue can boot their device by resetting their NVRAM, a chip that stores system settings. This method works for some users initially, but the problem reoccurs after subsequent reboots.

Conclusion:

The MacBook Pro is one of Apple's flagship products, and it is unacceptable for customers to experience such a severe issue. Apple's failure to address the problem has spurred outrage among users, forcing them to resort to online forums for a solution. While resetting the NVRAM is a temporary solution, Apple needs to find an immediate and permanent fix to its T2 chip, ensuring that users have a seamless experience when upgrading their MacBook Pros. Until this happens, dozens of users worldwide will have to put up with the glitch, causing unnecessary inconvenience and expense.

{{< youtube 6Ij9PiehENA >}} 



## Chosen Solution
 Hey guys!
A few days ago I swapped the factory-installed 128GB SSD for a Sabrent 1TB Rocket NVMe PCIe M.2 2242 SSD on my 2017 MacBook Pro without a touchbar. The installation itself went without any problems and the new SSD was recognized immediately.
With the help of an external recovery stick, I first formatted the new SSD as APFS and in the GUID partition scheme and then installed Big Sur. During the installation where the MacBook had to restart several times, I noticed that the MacBook shuts down, but then I had to restart it manually because it didn't do this by itself. Big Sur is now fully installed and I have all my data back via a Time Machine backup, but it still seems to have a problem when restarting:
It switches off, takes about 15 seconds, then switches on again and then shows the folder symbol with the question mark - it does not seem to recognize the hard drive.
If I then manually shut it down again and then boot into recovery mode with cmd + R (sometimes it is the Internet recovery and sometimes the system-internal recovery, booting into recovery mode from usb drive works as well) and then shutdown the macbook in this mode and then start it again, the macbook booted without exception and without any problems always normal to MacOS.
After this procedure when I am in the operating system, the following appears in the error report:
 MCA Error Report  CPU Machine Check Architecture Error Dump (CPU: Intel (R) Core (TM) i5-7360U CPU @ 2.30GHz, CPUID: 0x806E9) CATERR detected! No MCA data found.
Strangely, if I shut down the macbook normally and then turn it on again, this problem does not occur, so that the mac then boots normally into MacOS.
Things I've already tried to solve the problem:
SSD completely erased again, reformatted, installed the factory-installed MacOS Mojave and updated from there up to BigSurPRAM / NVRAM & SMC resetdeactivated FileVault and restartedstarted in safe and verbose moderapaired the ssd in disk utility tool several timeswith 'bless -mount "/ Volumes / Macintosh HD" -setBoot' set the hard disk again as the start volume and restarted, here I have deactivated SIP beforehand, because this command otherwise failed with "Could not set boot device property: 0xe00002bc"tested MacBook with apple diagnosis (held D key at startup), ended with ADP000 - No issues found.adjusted power management settings with pmset command to counteract the rapid discharge of the battery
All of these attempts were unfortunately unsuccessfull.
I'm really desperate. Does anyone know a solution?

 Sadly, your SSD replacement is giving you problems ;-{
Time for a replacement of either the carrier or the M.2 SSD its self or both!
While its more expesive (sadly) you might want to get a real Apple SSD Custom Apple 1 TB SSD

 I have the same problem, and I have not found any valid solution.
The problems I usually have and the solution I have used are:
1. When you get an update and the computer needs to reboot, it doesn't reboot automatically. I have to have the power cord disconnected and hit it manually when it won't boot.
2. When the computer is connected to the power and I open it, it usually does not start and the folder icon appears with the question mark. The solution is to hold the power button, turn it off and turn it on by disconnecting the power cord.

 I'm very late to the party but here goes.I just did this upgrade. Sabrent Rocket 1TB 2242 NVMe paired to the same NFHK N-1708A adapter. I did not experience any significant issues. Of course, I read this entire stack of replies (plus a LOAD of other threads and videos) but it appears to be hit and miss for a lot of people. I seem to have hit square on with write @ 18k and read and 21k. This is a 3x write increase over the 128GB Apple SSD, so I'm very happy. I don't think I did anything unusual...? What I did is not any different to you and to be honest, I think you have a dud SSD. It's either that or it's an OSX compatibility issue which are the only things I can think of. Here's what I did...a. Obvious prep to get ready for the new SSD, backup etc etc1. Installed the SSD and left the bottom off just in case. Plugged everything back in.2. Booted the machine up and got the question mark folder. Uh oh... what did I do wrong?3. Command R, reboot and the machine didn't recognize the drive. $@$*... am I done? 4. Plugged it in, PRAM reset - audible chime difference. That's interesting...5. Command R again, Disk Util - and the unit recognizes the drive!! YES!6. Expand directories and Format + rename drive to GUID as per usual.7. Reboot again, PRAM reset again, SMC reset as well. Load Command R and get the screen where you can choose... go to the spinning globe.8. Chose a fresh install for High Sierra and waited. If this works, I know I'm good to go.9. Sure enough, it loaded just fine and the drive was now registered and operational. 10. Noticed some random warnings about this:
MCA Error Report
CPU Machine Check Architecture Error Dump (CPU: Intel(R) Core(TM) i5-7360U CPU @ 2.30GHz, CPUID: 0x806E9)
CATERR detected! No MCA data found.11. Slight panic but the computer isn't acting strange at all - everything seems totaly fine - so I'm ignoring it. 12. Upgrade from High Sierra to Catalina through a target disk via USB.13. Trouble shoot some bugs and Enable TRIMFORCE just in case as I don't want Apple thinking I'm doing anything dodgy. It is my machine after all, isn't it?14. Check the battery drain and write/read speeds - everything seems really good so far! Got 9 hours from my first charge and seems stable at 17 to 19k write 20 to 21k read. BUT... I am noticing some fade/dropoff/wilt/leak of the write speed. It will hit 19k for a few cycles on Blackmagic and then drop through the floor to 1000 or under... and then shoot back up again while read stay consistently at < 20k ... I wonder why that is???15. Backed up from my Catalina file and all is well! I have not really had a single issue I couldn't fix so I would suggest it may be a hardware fault OR it is something to do with the firmware you're trying to upgrade from perhaps? Try doing the PRAM reset first as soon as you want to start it up, make sure it is plugged in and then do it a couple of times before going Command R and looking for Dick Util so you can go from there. Once you hit Disk Util you are basically 90% of the way finished and it's a bit tedious to that point but from my perspective well worth it.

 I’ve had issues with my iMac restarting while not using it and this “CATERR detected! No MCA data found” has been occurring a lot lately. I am on Big Sur 11.2.1. I have a 3rd party SSD (Samsung) and I have a Sabrent Thunderbolt 3 dock, and a thunderbolt sound card (UAD).
I am keeping the sound card off for now, but it’s interesting the name Sabrent is something we have in common.

 I don't think anyone has an answer to this problem the Sabent 1TB drive that I was using was a real energy hog so I stopped using it and went back the the original 256 GB drive. I think these laptops are too old now to upgrade or waste anytime figuring out the problems. It's time to upgrade to a new Mac unfortunately. Good luck.

 The key is choosing right SSD and Adapter.
Pick one with Silicon Motion Controller, and 99.99% you will be fine. Other controller like Phison, WD, Samsung, etc not always playing nice with A1708.
If you happen to face the question mark upon reboot. Key is, not to reboot, but shutdown instead. It will detect the SSD just fine when turning on.

 my “restart” problem happens  on Mojave and  Catalina both OS.  i have not tried BigSur.
i had sabrent 2Tb and sintech adaptor ( and another no brand adaptor ) on A1708, 2017 MBP no function key.
i sent back the ssd and going to get refund  for adaptor.
i found couple of SSD ( looked like combined 2240 ssd + adaptor ) with working guaranty for A1708 on eBay US but up to 1TB, since i need 2TB, I ‘m using external USB case with my old 2012 MBP 2.5’SSD (mojave ), it takes little longer to start up but no issue.
right now i ‘m not travelling , so this external system is ok but for the future when the pandemic goes down i will travel a lots like before and i will need decent internal system, i ‘m still looking for solutions.
i don’t know who is making 2240 ssd 2TB beside sabrent. and all adaptors looked same on amazon and eBay.

 I was facing same problem but with apple original ssd if I downgrade the OS from BiG Sur to High Sierra. Then I reinstall Bigsur and now working fine for

 have some one solve that problem now? i have exactly the same problem

 It’s really hard to say what fixed mine but suffice to say it rarely reboots anymore. My system actually seems more stable on Monterey and has been substantially better on 11.3+. Of course I have other issues but they are likely unrelated. All I can say is try a PRAM reset as that seems to help get boot issues fixed.

 Also having issues with the same errors after upgrading to a 2TB Sabrent M.2 2242  (via Sintech M.2 NVMe SSD Adapter).
Upgraded from stock 128GB to the 2TB above and installed Big Sur to match my Time Machine backup. OEM SSD was on Big Sur so decided to install the same to be safe even though Monterey / MacOS 12.x is out.
Struggling to understand where the issue is coming from. SSD firmware? That, at least, would make sense.

 Hi guys,
Last Monday I upgraded my MacBook Pro’s 2017 A1708 SSD because the original one died. I purchased an OWC Aura Pro NT 240gb SSD because it was I think the most compatible solution I could think of. By the time I upgraded i’m experiencing the following problems.
My machine cannot execute a restart (I restart the MacBook and it takes about 30 seconds to boot back again and when it opens it displays a windows indicating that My computer was restarted because of a problem)When the machine is shut (with closed lid) I connect the power cord and I get no charging sound, when I open the lid in order for the Mac to boot to the OS I get a folder with a question mark.
My guess is that anything besides the original Apple SSD will not operate normal in Macbook’s. Is there any possible solution to this issue?

 People always said that Sintech & Sabrent is the best combo, while for most of cases in A1708, it's not. Well, in fact for most of cases Sintech is no longer relevant, since other makers already catch up with the wiring map, and do even better with the PCB cutting and connector plating.
for A1708 (or even A1502, A1398, A1465 and A1466) the key is always on the SSD Controller and Firmware. The one with custom/in house controller like Samsung and Western Digital will have more tendency to have compatibility problem compared to the one using a more universally adopted controller (named Silicon Motion and/or Phison), combined with the firmware, will decide whether those SSD can provide sleep and power management on your macOS or not. The one using less popular controller (like Realtek - mostly used by ADATA) might also causing issues.
I've been using this SSD bellow for around 3 years, and so far having no issues related to sleep, energy drain, restart, update (installed it back in Catalina days, and am on Monterey now) or elses. The specs said that it use Silicon Motion Controller along with Micron TLC NAND. That being said, it might or might not available in your countries, since the maker is one of my country local brand.

It sleep when the lid is closed, and uses around 0,0x Watt (0,09W in screenshot above - i previously tried ADATA, and SAMSUNG and none of their SSD manage to get bellow 0,5W ) of energy during idle, and the temp hovering around 30-60 degree celcius. Normally am using iStat menus app to monitor all stats of my hardware.

 Just update it last night. Never thought people will reply this post after a long time. Mine is Sabrent 1TB Rocket NVMe PCIe M.2 2242.
My adapter is this one:
https://shopee.tw/Macbook-Pro-NVMe-M.2-N...
What's your adapter? Is this one?
https://www.taobao.com/list/item/3735499...
I watched a youtube video that he use this adapter without any issues.
https://www.youtube.com/watch?v=7n-NcROd...
I'm so curious why your write and read is way high speed? Mine is 400-500@write and 1800@read. Any tricks did you do for your mac?
It's easy to installed the SSD in physical, but hard to install the OS in software. I experienced the question mark folder !&&*.....finally I installed the MacOS mojave successfully then upgrade to monterey. Then use time machine to recovery all my status in my previous setup.
And it did become as a power consuming monster. It dried the battery very quickly.
Also notice when it reboots, it may go to question folder screen. Seems it will happen while rebooting. So prepare to get used to it. :)
Anyone experienced deep sleep issue with this SSD? How to prevent it?
OR any other setup need to be adjusted?

 My current Write/Read speed after a couple of weeks is still 17k/20k. I am not sure why others are having such serious issues. :/Now... my 14" M1 Max 10/24/32 on the other hand... holy crap0la @____@!!

 Kioxia Exceria Plus.




