---
title: "You won't believe what happened to this Macbook Pro 13! Liquid damage and SMC IO failure cause mind-blowingly slow performance!"
ShowToc: true 
date: "2023-03-27"
author: "Pedro Tobar"
---
*****
---

# You Won't Believe What Happened to This MacBook Pro 13!

## Liquid Damage and SMC IO Failure Cause Mind-Blowingly Slow Performance!

If you're a MacBook Pro 13 user, you probably know how disheartening it is to experience slow performance. There are numerous factors that can be responsible for this issue, including malware or adware, an outdated operating system, or even insufficient RAM. However, there's one reason that's often overlooked, and that's liquid damage.

In this article, we'll discuss the case of a MacBook Pro 13 that experienced liquid damage and SMC IO failure, which caused it to become frustratingly slow.

## The Case of the Damaged MacBook Pro 13

The MacBook Pro 13 in question belonged to a college student who accidentally spilled coffee on it. Despite quick action to dry it off, some liquid seeped into the machine. At first, it seemed like everything was okay, but then the student began to experience performance issues.

The MacBook was incredibly slow, with programs taking forever to launch, webpages taking ages to load, and the fan running non-stop. The student tried troubleshooting the issue by running several diagnostics, but nothing seemed to work.

## The Diagnosis

After several unsuccessful attempts to fix the problem, the student decided to take the MacBook to an Apple service center. The technicians conducted a thorough diagnosis, and the results were mind-blowing.

The liquid had caused significant damage to the logic board, including the SMC (System Management Controller). The SMC is responsible for the communication between the different hardware components of the MacBook, and when it fails, it can cause a variety of issues, including slow performance.

The technicians replaced the logic board and cleaned the MacBook to remove any remaining liquid residue. They also updated the operating system, which had been neglected, and added more RAM to improve the overall performance.

## The Result

After the repairs, the MacBook Pro 13 was running like new again. The sluggishness was gone, and the programs launched almost instantly. The fan stopped running constantly, and webpages loaded without any delays.

The student was delighted with the outcome and relieved that their MacBook was still salvageable. They learned a valuable lesson about the importance of protecting their MacBook from liquid damage and ensuring that it's maintained correctly.

## Conclusion

If you're experiencing slow performance on your MacBook Pro 13, don't panic. There are numerous reasons why this could be happening, but liquid damage is a common one that's often overlooked. If you've spilled any liquid on your MacBook or suspect that it may have been exposed to moisture, take it to a professional for a thorough diagnosis.

Remember, prevention is always better than cure. Protect your MacBook from liquid damage by using a keyboard cover, keeping liquids away from the machine, and avoiding using it in humid environments. Maintaining your MacBook correctly and addressing any issues promptly can help you avoid expensive repairs in the future.

{{< youtube YucFR_WGI88 >}} 



## Chosen Solution
 I left my Macbook in my backpack and I guess my water bottle somehow opened and managed to get my Macbook wet. At first I wasn't getting any signs of life so I performed these steps on it to try to revive it:
1. Dropped the logic board into an ultrasonic cleaner to clean off corrosion. Afterwards, I submerged the motherboard into 99% isopropyl alcohol to displace the water and left it to dry overnight
*At this point, my Macbook is able to turn on but I notice that the fan kicks in at full speed and it's unbearably slow
2. I ran ASD on it and was able to get an "SMC IO Fail" error underneath TN1D. I did a bit of research and found out that TN1D represents the MCP 0 Die Temp.
It sounds to me like it's a faulty sensor. However, I don't know where this is on the motherboard. I have the schematics and boardview for it but it doesn't mention anything about MCP 0 Die.
3. I measured the resistors around the sensors and they all measured as they're supposed to. I checked the voltage rails too and they are measuring correctly as well.
4. I reflowed the SMC chip with an hot air gun but still the same result.
I'm am now stuck. Could someone please point me in the right direction?
UPDATE:
I looked at the schematic again and found MCP T-Diode Thermal Sensor. I ended up taking off this chip and putting it back on and it then it passed the ASD test! However after a few minutes, I ran the test again and it failed.
I ended up ordering a new MCP Thermal Sensor chip for the board. I'll replace it once I get it. Hopefully this works.
UPDATE:
Replacing the SMC Thermal Diode did not seem to work. It still gives me the same error which is the TN1D error. Does anyone have any suggestions?

 The MCP Thermal Sensor/Diode is inside the MCP chip itself. MCP_THMDIODE_P  and MCP_THMDIODE_N are the two data lines that connect U5535 to the MCP. The chip that connects the thermal diode to the SMC: connects to a thermal diode inside the MCP (called MCP Die), and also houses a separate thermal sensor called MCP Proximity.




