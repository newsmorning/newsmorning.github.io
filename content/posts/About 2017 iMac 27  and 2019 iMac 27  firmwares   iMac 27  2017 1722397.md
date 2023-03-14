---
title: "Unveiling the shocking truth about the 2017 and 2019 iMac 27 firmwares - you won't believe the differences!"
ShowToc: true 
date: "2023-03-11"
author: "Esther Martineau"
---
*****
Unveiling the Shocking Truth about the 2017 and 2019 iMac 27 Firmwares – You Won't Believe the Differences!

Mac has been in the forefront of the computing world ever since its inception. Known for its reliability and sleek design, Mac computers have taken the world by storm. Among the many models in their lineup, iMac has made a name for itself by being one of the most versatile all-in-one computers out there. With its 27-inch display, powerful processor, and user-friendly features, it's no wonder why it enjoys a massive following.

However, as the saying goes, "with great power comes great responsibility." One such responsibility that's often overlooked is firmware. The firmware is a piece of software responsible for controlling a computer's hardware components. It's an essential aspect of a computer's performance and stability. Therefore, it's necessary to make sure that the firmware is always up-to-date.

In 2017, Apple released the iMac 27 with firmware version number 114.0.0.0.0. It was a significant update, and users around the world were excited to try out its new features. However, it came with some issues that were later discovered. Many users complained of a bug that caused the computer to freeze randomly. Other users reported that the computer would shut down unexpectedly, which was frustrating, to say the least.

Apple acknowledged the issue and rolled out an update in 2018, which fixed the bug. The updated version number was 141.0.0.0.0. However, despite fixing the bug, the firmware had a new problem. The 2018 update reduced the iMac 27's performance by 5-10%, raising concerns among users.

Fast forward to 2019; Apple released the new iMac 27, which came with a firmware version number of 155.0.0.0.0. Users were happy to hear that the new firmware addressed the performance issue. However, the excitement was short-lived as users discovered a new issue with the 2019 firmware. The new firmware caused the iMac 27 to crash randomly, making it unusable for some users.

Apple, yet again, rolled out an update in 2020, which fixed the bug. The updated version number was 170.0.0.0.0. Despite the new bug fixes, users noted that the performance had dropped once again by 5-10%.

It's incredible how much the firmware updates affect the iMac 27's performance in just a few years. With every update, the iMac 27's performance fluctuates, making it hard for users to trust the product. Users are worried that the performance will continue to drop with every new update, causing them frustration and making them hesitant to purchase the product.

In conclusion, firmware is an essential aspect of any computer's performance, and it's necessary to ensure that it's always up-to-date. The iMac 27 has had its fair share of firmware issues, with every update affecting its performance. While Apple has rolled out bug fixes, the constant fluctuations in performance have made users hesitant to trust the product. Apple needs to address these issues and ensure that the iMac 27's performance is consistent and stable, making it easy for users to trust the product.

{{< youtube HPg9N_HiLMg >}} 



## Chosen Solution
 Well as far as I could check through online research both the 2017 and 2019 models have the same hardware: same CPU socket, same GPU (ok, 580 vs 580pro, minor change) and same PSU however the 2017 model would not work with the same i9 9900 CPUs available for the 2019 models and I want to know why.
Could it be just a firmware restriction in the known 'Apple way' of planned obsolescence considering the hardware is the same therefore shouldn't be any technical reason? Would the 2017 model run with the i9 9900 CPUs if its firmware were to be flashed with 2019 firmware? Could the firmware even be actually flashed just like that…?
I would really like to know more than just assumptions ?

 Apple’s approach is to use the same firmware within a given ID Series so in your case the iMac17,1 and the iMac19,1
Late 2015 - Skylake
I5-6500I5-6600I7-6700K
2019  - Coffee Lake
I5-8500I5-8600I5-9600K
These are very different Intel CPU series which use very different micro-code. Apple does not load up their EFI with multiple micro-code builds.
Bottom line: You are limited to what the given series offered in some rare cases (very rare) you might have an option. Sadly not here.

 You cannot use Coffee Lake CPU's (as in what the 2019  uses) on the 2017 for two (very) major reasons:
(1) The 2017 uses an LGA 1151 rev 1 socket, and the 2019 has the LGA 1151 rev 2.
(2) The chipsets on each logic board are very different: z170 vs z370
LGA 11551 rev1 vs rev2: Not same sockets: the pin allocations are different Second revision of the LGA 1151 socket for Coffee Lake CPUs:
"While physical dimensions remain unchanged, the updated socket reassigns some reserved pins, adding power and ground lines to support the requirements of 6-core and 8-core CPUs. The new socket also relocates the processor detection pin, breaking compatibility with earlier processors and motherboards. As a result, desktop Coffee Lake CPUs are officially not compatible with the 100 (original Skylake) and 200 (Kaby Lake) series chipsets."
----------------------------------------
Edit:
In fact, there's a VERY detailed comparison of Kirby Lake/Coffee Lake pinouts (i.e. on the interface betwwen CPU and socket). And it explains the very big differences between the two. It even says a firmware upgrade would not be able to address it. The only (remote) possibility would be on some motherboards a z270 chipset is used, whicxh is closer to the z370. But iMac went from z170 to z370 directly.
Kabylake vs Coffee Lake LGA1151 Pinout Differences Revealed
Anadtech discusses it too:
Differences from Coffee Lake to Kaby Lake Physical Design: Pin Outs
------------------------------------------
Chipsets: The 2017 logicboard has the z170 chipset, whereas the 2019 has the z370.
Here's a nice link on the differences between the chipsets (look under LGA 1151 rev1 and rev2).
List of Intel Chipsets
The z170 is quite different from the z370 in terms of what it supports.
And note that there was an intermediate z270 chipset in-between them, that is very close to the z370 (specs are very close here).
Intel says that the z170 cannot support the Coffee Lake CPU's (used in 2019 iMac):
LGA 1151
Look under the LGA 1151 rev1 and rev2 tables.
Can see that the z170 is not forwards compatible, and the z370 not backwards compatible, and even the z270 won't support Coffee Lake CPU's.
And this is part speculation on my end, but I think the EFI chips/firmware difference is not really an issue. You can both back-up and re-flash these chips on the board. And re-soldering one is no big deal: are simple chips, and you can buy them.

 @danj  Just got my first 12 core 2013 Mac Pro yesterday.  Will have a couple of questions on it for you later on, been a while since I had a new toy to play with.  Simply Mac going under has really helped business, I'm actually making a living again.




