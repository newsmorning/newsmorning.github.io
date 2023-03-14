---
title: "You won't believe why this Acer laptop only works on VGA and not its own screen!"
ShowToc: true 
date: "2022-11-30"
author: "Thomas Garvin"
---
*****
Title: You Won't Believe Why This Acer Laptop Only Works on VGA and Not Its Own Screen!

Intro:

Acer laptops are known to be reliable and efficient machines that cater to the needs of a wide range of users, from students to professionals. Nonetheless, some Acer laptop users have experienced an unexpected issue where their device only works on VGA and not its own screen.

In this article, we will delve into why this issue occurs, how to fix it, and prevent it from happening again.

What is VGA and how does it work?

VGA stands for Video Graphics Array. It is an analog interface used to transmit video signals from a computer to a display or projector. It has been available since the 1980s and, surprisingly, is still used today in some modern devices such as laptops.

VGA works by transmitting analog signals through a 15-pin connector. The connector is connected to the VGA port on a computer and the VGA port on a display or projector. Once connected, the display or projector will receive the video signal and project it onto the screen.

The issue:

Now that we understand what VGA is and how it works let's get back to the Acer laptop issue. If you own an Acer laptop and the device only works on VGA and not its own screen, chances are there's an issue with the graphics card.

The graphics card is the component that outputs the visual display to the screen. If the graphics card is damaged or not functioning correctly, it can prevent the laptop from projecting the video display onto its own screen, causing the screen to remain black.

This issue can arise for several reasons, such as a hardware malfunction, outdated drivers, or an improper connection to the screen. Let's dive deeper into these potential causes and how to fix them.

How to fix the issue:

1. Update the drivers:

The first step in fixing the issue is to update the graphics card drivers. Outdated drivers can cause the graphics card to malfunction and prevent the display from working correctly. To update the drivers, follow these steps:

a) Open the device manager by pressing the Windows key + X and selecting the device manager option.

b) Expand the Display adapters option and right-click the graphics card.

c) Select the update driver option, and follow the prompts to update the drivers.

2. Check the connections:

Another reason why the laptop may not project the visual display onto its own screen is due to a loose or improper connection between the screen and the graphics card. To check the connections, follow these steps:

a) Shut down the laptop and disconnect it from the power source.

b) Remove the battery from the laptop.

c) Locate the graphics card and check the connections between the card and the screen.

d) Ensure the connection is tight and secure.

3. Hardware malfunction:

If the above steps do not resolve the issue, it may be due to a hardware malfunction. In this case, we recommend consulting a professional technician who can diagnose and repair the problem.

Preventing the issue from happening again:

Preventing the issue from happening again requires maintaining the device and keeping the drivers up to date. Here are some ways to prevent the issue from recurring:

a) Regularly perform a maintenance check on your laptop.

b) Keep your drivers up to date by checking for available updates regularly.

c) Avoid installing third-party software and programs on your laptop that could interfere with the graphics card's function.

Conclusion:

The Acer laptop issue of only working on VGA and not its own screen can be caused by several reasons, such as outdated drivers, a loose connection, and hardware malfunctions. It's essential to keep the device maintained, keep drivers up to date, and avoid installing third-party software to prevent the issue from occurring in the future. If the issue persists, consult with a professional technician to diagnose and repair the problem.

{{< youtube NWVMMGfUKno >}} 



## Chosen Solution
 Hello to all,
I have problem with Acer Aspire 5520. Laptop is working only on external display connected on VGA port but internal screen don’t show anything, no backlight, not even picture under the light on that screen.
I have try with another motherboard-screen flat cable, also have tried another panel, light inverter but nothing showed, dead. Computer boot and work fine on VGA connected monitor but on internal nothing show up from powering on pc- bios - windows, nothing.
Internal monitor also not detected in windows, when I open graphical properties there is no second screen only one (VGA monitor), so there is no option only second scree or similar, one screen is available only.
We can skip suggestion like reinstall drivers, FN key for monitor change, hold power off without battery and that kind of stuff or similar because BIOS is not showing on the internal screen. RAM, HDD, are tested and 100% working. Any suggestions?

 Hi @shule88 ,
I don’t know the answer but here’s a link to the motherboard schematics. At least I think that it is the correct one. Check the motherboard’s board number (printed on motherboard) to verify.
On p.2 the circuit block diagram shows how the internal screen (LVDS) and external screen (CRT) connect back to the chipset IC
On p.7 it shows how the video signals and controls are sent from different sections of the chipset IC (see LVDS and DAC sections)
Something is telling it not to connect video from the LVDS section of the IC but from the DAC section is OK. I don’t know enough about how chipsets function down at this level though to know how it switches between the outputs
I realize that you said not to reinstall the drivers but have you checked that the chipset drivers (supplier example only) are OK and are the latest available, just in case?
I would also try removing the cmos battery (soldered on board top right hand corner) and removing the main battery and then doing a hard reset as a corrupted setting may be being held in BIOS by it and preventing the switch over of the outputs from the chipset. You haven’t got much to lose by trying everything first before delving into board level repairs
Otherwise you may have to check the components and power supplies around the chipset IC (also see p.19)
Just what I would try.




