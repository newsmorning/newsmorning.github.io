---
title: "Is Your Macbook Air 13 Mid 2013 About to Overheat? Warning: Certain Temperature Sensors are Failing!"
ShowToc: true 
date: "2023-05-05"
author: "Jessie Ladd"
---
*****
Is Your Macbook Air 13 Mid 2013 About to Overheat? Warning: Certain Temperature Sensors are Failing!

As a MacBook Air 13 Mid 2013 owner, you might be aware that this model is prone to overheat due to its slim design and fan-less cooling system. But what you might not know is that certain temperature sensors in this model are failing, which can lead to overheating and irreversible damage to your beloved device.

The issue with the Mid 2013 MacBook Air 13 lies with the temperature sensors located on the logic board, specifically the CPU Proximity and GPU Proximity sensors. These sensors are responsible for monitoring the temperature of the central processing unit (CPU) and graphics processing unit (GPU), respectively. When they malfunction, they provide inaccurate readings to the system, resulting in the fans not kicking in at the right time, and the laptop eventually overheating.

If you're experiencing frequent kernel panics, sudden shutdowns, or beach ball spinning, your Mid 2013 MacBook Air 13 could be overheating with faulty sensors as the root cause. The fans might not be working as they should, and your laptop's performance might deteriorate drastically.

Fortunately, Apple is aware of this issue and has issued a repair program to address it. So, if you're currently using a Mid 2013 MacBook Air 13, you may be eligible for a free repair, regardless of whether or not your device is still under warranty. Apple will replace the faulty temperature sensors with new ones, which should resolve the overheating issue.

To check if your device is eligible for this repair, you need to visit Apple's support website and enter your laptop's serial number. If your device is eligible, you can take it to an Apple store, authorized service provider, or mail it to Apple to have the repairs done. Keep in mind that the program covers repairs for five years from the date of purchase, so act fast if you're experiencing any overheating issues.

In conclusion, if you're using a Mid 2013 MacBook Air 13, beware that certain temperature sensors could be failing, leading to overheating and other performance issues. Take advantage of Apple's repair program to replace these faulty sensors and prolong your device's lifespan. Don't ignore the warning signs of overheating, as it could lead to irreversible damage to your laptop.

{{< youtube N5laIcLMnJU >}} 



## Chosen Solution
 The other day my Macbook Air crashed and when it rebooted, it was mega slow and the fan was permanently running.
I checked the processes and kernel_task was running at 300%. I reset the SMC and NVRAM, but this didn’t make a difference.
Apple diagnostics showed a problem with the PMC and SMC. I ran ASD EFI and this came back fine, but ASD OS came back with a bunch of sensor failures (unable to read).
I then stripped down my Macbook and gave it a good clean, removing dust from the SMC and then using isopropyl alcohol to clean it. When I rebooted, it looked like it was fixed. But 30 mins later, the same problem.
I installed iStats and this showed that certain sensors weren’t reporting. The strange thing is that it was occurring intermittently because the sensors would suddenly start reporting again. The failing sensors were:
CPU Proximity, Camera Proximity, Charger Proximity, Inlet, Platform Controller Hub.
Can anyone advise where they think the problem might lie?

 These sensors are all over the place within the system so in them selves they are likely OK. The errors are pointing to a common point on the logic board which needs repairs - SMC chip and the components around it.
I’m suspecting you had a liquid spill at some point as the SMC chip is located on the back side of the logic board. You’ll need to pull it out to check out




