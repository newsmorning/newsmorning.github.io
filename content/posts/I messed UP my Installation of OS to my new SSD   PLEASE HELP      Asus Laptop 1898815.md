---
title: "Disaster Strikes! How I Botched My OS Installation on a Brand New Asus Laptop - Desperate for Help!"
ShowToc: true 
date: "2023-01-25"
author: "Lindsey Fuller"
---
*****
+++
title = "Disaster Strikes! How I Botched My OS Installation on a Brand New Asus Laptop - Desperate for Help!"
date = "2022-06-21"
author = "Your Name"
tags = ["computer", "troubleshooting", "installation"]
+++

It was supposed to be a simple task - installing a new operating system (OS) on my brand new Asus laptop. I had done this before on other computers, so I thought this would be a breeze. But disaster struck, and I botched up the installation, leaving me desperate for help.

Everything started out fine. I had downloaded the latest version of Ubuntu, the OS I intended to use, and created a bootable USB drive. I inserted the USB drive into my laptop, pressed F2 to enter the BIOS, and changed the boot order so that the USB drive would be the first option. So far, so good.

But when I restarted the computer, things started to go wrong. Instead of booting from the USB drive, the laptop displayed an error message saying "No bootable device found." I tried again, but the same message appeared. Panic started to set in.

I turned to Google for help and found a forum where someone had encountered the same problem. The suggested solution was to disable the Secure Boot feature in the BIOS, which supposedly caused conflicts with certain bootable drives. I tried this, but it didn't work. The error message persisted.

I was at a loss. I had followed all the instructions, but something wasn't right. I was desperate for help. I called a friend who was more tech-savvy than I was, but he couldn't offer much assistance beyond suggesting that I try to reinstall the OS.

I was about to give up when I stumbled upon a YouTube video that showed how to troubleshoot bootable device errors. The video suggested that I check the USB drive's partition scheme and ensure it was compatible with my laptop's BIOS. I checked, and sure enough, the USB drive was formatted using the wrong partition scheme.

I recreated the USB drive using the GUID Partition Map, which was compatible with my Asus laptop's BIOS. This time, the laptop booted up from the USB drive without any problems. I began the installation process again, and this time, it worked like a charm.

The whole ordeal was a humbling experience. I had underestimated the complexity of installing an OS, especially on a new laptop with unfamiliar hardware. I learned that even seemingly simple tasks could become complicated if you lacked the necessary knowledge and experience.

In conclusion, if you're ever in a similar situation where disaster strikes during an OS installation, don't panic. Take a deep breath, reach out for help, and scour the internet for troubleshooting tips. With patience and persistence, you'll eventually find a solution. My advice would be to familiarize yourself with the hardware you're working with, double-check everything, and don't be afraid to ask for assistance. Good luck!

{{< youtube MCjaoBuun34 >}} 



## Chosen Solution
 Here’s what happens:  (apologies for my bad english first.)
Got new SSD -> plugged it in on my laptop immediately -> installed Win10 on the SSD  BUT WITHOUT REMOVING /UNPLUGGING MY OLD HDD  after that, I’ve encountered the problem:
1. Everytime I turn on my Laptop, the BIOS won’t recognize any boot devices. Turn on laptop -> after 10-15 secs, automatically goes to BIOS showing this


and this is the boot list which is empty IDK why?


2.  now everytime this happens, I JUST ALWAYS HARD PRESS THE POWER BUTTON TO SHUTDOWN THE LAPTOP  and just turn it on again. But this time it recognizes now the old HDD, as per checking in the BIOS here is the image


Here is now the boot list (the first attempt was empty,  but now it has the HDD but SSD is nowhere to be found, weird):


3. after that, I close the BIOS and the screen will go like this, having 2 volumes of different OS

volume 2 is SSD and the other is the old HDD
4.  I select the first choice and then I can normally use my SSD, sure I can use it just fine but I KNOW THAT THERE IS SOMETHING WRONG, I feel that this shouldn’t be my everdyay process of booting up my laptop. Please help ME guys..
lastly, this is the DISK MANAGEMENT PARTITION SCREENSHOT

 Help me please kind sirs…




