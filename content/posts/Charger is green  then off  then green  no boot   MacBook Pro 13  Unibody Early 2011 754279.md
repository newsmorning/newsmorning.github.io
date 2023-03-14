---
title: "Is Your Macbook Pro Dying? Find Out Why Its Charger Keeps Blinking Green and Black!"
ShowToc: true 
date: "2022-12-24"
author: "Vernon Yankee"
---
*****
Title: Is Your MacBook Pro Dying? Find Out Why Its Charger Keeps Blinking Green and Black!

Introduction

MacBook Pro is one of the high-end devices from Apple Inc., known for its quality features and a longer lifespan. However, even the best of devices comes with some warning signs that indicate it's dying. One such indication is the blinking green and black light on the charger. A flickering green light on your MacBook Pro's charger may be an alarming indication that something's wrong with your MacBook. In this article, we'll explore why this occurs and what you can do to troubleshoot and resolve the issue.

Reasons why the charger keeps blinking green and black

1. Battery Life is in Danger

The battery is one of the primary components of any device, and if it fails, the device is rendered practically useless. When your MacBook Pro's battery life is in danger, you'll notice the charger blinking a green and black light. This is a sign that the battery is not getting charged, and you need to take immediate action.

2. Corroded Connectors or Dead Battery

If your MacBook Pro has been in use for a long time, the connectors or battery could become corroded or dead, respectively. If you see a green and black flickering light on your charger, it could indicate that the battery or connectors are not working correctly. Check the battery health to see if it's dead or corroded, and replace it or clean the connectors, respectively.

3. Damaged Charger or Adapter

Another reason for the blinking green and black light could be that the charger or adapter has been damaged. If the wire is broken or kinked, the charger will not work correctly, and you'll see the green and black light flashing. Try to replace the damaged parts with a new one, and see if the problem persists.

How to fix your MacBook Pro's blinking green and black charger issue

1. Check Battery Health

One of the first things you should do when the charger light is flashing a green and black light is to check the battery health. Open the Apple menu and select About This Mac, then click System Report. Now click Power, then check the Cycle Count under Health Information. If the cycle count is high, it's possible that the battery has run out of its lifespan and needs replacing.

2. Clean Connectors

If the connectors are corroded, you can clean them with a cotton swab dipped in rubbing alcohol. This should remove any dirt, grime, or residue that may have accumulated on the connectors.

3. Use a New Charger or Adapter

If your charger or adapter is damaged, replace it with a new one. This should fix the problem.

Closing Remarks

In conclusion, if your MacBook Pro's charger keeps blinking a green and black light, it's a warning sign that there's something wrong with your device. As we've explained, the blinking light can be caused by various issues. However, these can all be resolved by examining and fixing the root cause. If you're unsure of what to do, consult an expert, or contact Apple support for assistance. Don't ignore this warning, as failure to take corrective action could end up costing you a lot more in the long run.

{{< youtube itzOoqAq0JA >}} 



## Chosen Solution
 Hi all.
I’m quite new at trying to troubleshoot logic boards, and have very little knowledge, but I’m trying to learn. So, I received a MBP 13” Early 2011. I don’t even know the conditions of the battery as it’s clearly drained and it won’t charge.
If I disconnect the battery, keep the power button pushed, connect charger, connect battery, release and push again the power button, the machine turns on, the display as well (white screen, no apple no nothing, chimes, fans spinning like crazy and that’s it. Reset SMC, machine dead again. Repeating the procedure and resetting PRAM after the chime also leads nowhere.
I removed the board. Upon connection of a magsafe (Apple original 85W), the light is green for some seconds, then goes off, then returns green and so on looping. Fans: same behaviour. When the green light appears, fans spin. Then they stop spinning (and the green llight goes off) and so on forever.
Following Louis Rossman’s videos and reading a few forums I started taking some measures, and here they are:
F6905 - 16.8V
U6900
Pin 1 - SMC_BC_ACOK_VCC - reads 3.48Pin 4 - SYS_ONEWIRE - reads 2.91Pin 5 - ADAPTER_SENSE - reads 2.90
U6901
Pin 1 - SMC_BC_ACOK - reads 2.36Pin 2 - SMC_BC_ACOK - reads 2.36Pin 4 - SMC_BC_ACOK_VCC - reads 3.48Pin 5 - PP3V42_G3H - reads 3.48C6908 - Pin 1 - PP3V42_G3H - reads 3.47
U7000
Pin 2 - CHGR_DCIN - reads 16.5Pin 3 - CHGR_ACIN - reads 3.9
L7030’s reading goes up and down from 12.5 to 3.4, continuously
I then started taking some measures of a bunch of resistors and really got puzzled. I’ll explain why.
R7012 - 0.99 (should be 1)
R7010 - 28,3 (should be 30.1)
R7011 - 9.22 (should be 9.31)
R7013 - missing (should be 1)
R7015 - 100.2 (should be 100)
The issue here is the missing R7013. On the schematic there’s a row of 8 components (caps and res), but on the board… instead of said resistor I find two spots, and no trace of solder. It’s not the only case. R7002 seems to be missing as well, and R5011 too. It actually looks as if they were never there so I’m really puzzled. Here are a pic and a screen of the schematic.


Any help is really appreciated.

 So lets go through the diagnostic process:
Phase-1: What is the symptoms the customer is encountering. What happened to the system just before the failure and and additional background like liquid spills or alterations (RAM or Storage). Review the MagSafe charger being used is it a real Apple charger OEM MagSafe Chargers vs Cheap Imposters: Teardown for Truth & Real vs Fake Magsafe 2 Charger Macbook Pro is the cord and the connector in good shape? Apple Portables: Troubleshooting MagSafe adapters Also make sure its the correct wattage for the system. What is the color of the MagSafe LED a bright Amber or Green? Is the LED a dim Green?
If you have any question on the MagSafe try a known good unit {FYI: I have five different units just for testing). You could also get a good power supply and take a MagSafe power cord wired up for testing. But thats mostly useful after you’ve taken the board out.
Phase-2: Inspection & basic clean - Inspect the MagSafe connector on the system (DC-In board)are the pins clean and shiny?
Pop the bottom cover off, do you see any staining or wet areas, is there a lot of dust on the backside of the cover and the logic board. Use a 1” soft paint natural brush to scrub the surfaces to loosen the dust and dirt, use can’ed or compressed (oil-less) air to blow out the dust (don’t forget the fans) use care not to over power the fans (short blasts). Do you see any damaged components? Look for corrosion or off color solder joints.
If nothing is visible at this point fully remove the logic board to inspect the other side. Again, look for staining on the uppercase (liquid seepage) dust off the board, look for damaged components. Make note of areas impacted. Remount logic board and cables (not the battery). If needed replace the DC-Inboard before mounting logic board.
Phase-3: Power - With the battery disconnected connect the MagSafe charger. Did the system boot up? What is the color of the MagSafe (it should be Amber). Did the Fan startup?
So what did you find following this process? At this point you should have an idea where you need to focus in on.
Given the age of the system the battery will likely need replacing but without having a working system it’s not possible to test. You could create a power extension cable so you could leverage another working MacBook Pro as a test bed. This could be useful if you plan to work on a lot of this series.
From what you’ve described I would focus on the power logic. Focus on the MOSFET’s first, did you test them? Is the voltage on the power rails correct?
If they are correct then you know what the issue is don’t you ;-}




