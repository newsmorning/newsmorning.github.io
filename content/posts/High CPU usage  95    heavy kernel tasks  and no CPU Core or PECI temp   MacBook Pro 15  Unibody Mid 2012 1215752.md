---
title: "Is Your Macbook Pro Overheating? Shocking High CPU Usage And Heavy Kernel Tasks Revealed With No Temperature Readings!"
ShowToc: true 
date: "2023-01-31"
author: "Ingrid Mancuso"
---
*****
Title: Is Your Macbook Pro Overheating? Shocking High CPU Usage And Heavy Kernel Tasks Revealed With No Temperature Readings!

If you're a Macbook Pro user, you might notice that your device is getting hotter and hotter over time. You might also notice that the fan is spinning faster and louder than before. If you've checked the temperature readings, you might be surprised to find that there are no readings available.

This is a common problem for Macbook Pro users, and it can be caused by several factors, including high CPU usage, heavy kernel tasks, and a faulty temperature sensor. In this article, we'll explore these factors in detail and provide some solutions to keep your Macbook Pro from overheating.

High CPU Usage

Your Macbook Pro's CPU (Central Processing Unit) is responsible for executing instructions and processing data. If a software application is using a lot of CPU power, it can cause your device to overheat. To check which applications are using the most CPU power, launch the Activity Monitor application and click on the CPU tab.

You can sort the list by CPU usage to see which applications are using the most power. If you notice that one application is using a lot of CPU power, you can try quitting or uninstalling it. You can also check for updates to the application, as newer versions may be more efficient and use less CPU power.

Heavy Kernel Tasks

The kernel is the core of your Macbook Pro's operating system, and it manages system resources such as memory and disk storage. If there are heavy kernel tasks running, it can cause your device to overheat. To check for heavy kernel tasks, launch the Activity Monitor application and click on the Memory tab.

You can sort the list by Memory usage to see which tasks are using the most memory. If you notice that a task is using a lot of memory, you can try stopping or disabling it. However, be careful when stopping kernel tasks, as you may cause system instability if you stop a critical task.

Faulty Temperature Sensor

If your Macbook Pro's temperature sensor is faulty, it may not provide accurate temperature readings. This can make it difficult to determine if your device is overheating. You can try resetting the System Management Controller (SMC) to see if it resolves the problem. To reset the SMC, follow these steps:

1. Shut down your Macbook Pro.
2. Press and hold the Shift, Control, and Option keys on the left side of the keyboard.
3. Press and hold the Power button for 10 seconds.
4. Release all keys and turn on your Macbook Pro.

If resetting the SMC doesn't work, you may need to have your temperature sensor replaced by a professional technician.

Conclusion

If your Macbook Pro is overheating, it can be a frustrating problem to deal with. However, by checking for high CPU usage, heavy kernel tasks, and a faulty temperature sensor, you can identify the issue and take steps to resolve it. By following the tips in this article, you can keep your Macbook Pro cool and prevent it from overheating.

{{< youtube FZjELZBq7WU >}} 



## Chosen Solution
 I have a Mid 2012, 15” MacBook Pro (A1286 - with 820-3330B logic board).
The problem is that the macOS can’t read the CPU PECI or CORE TEMPS. The fans are running at full throttle, kernel task reaching 600% and CPU usage is 95%, making the system super slow and unusable.
Checked all the sensors using ASD, all sensors read OK, test passed, apart from the TIM test 75%GB test failing which I believe is a false error on these MacBooks.
Ran “iStat” and “MacFanControl” to realize that I have no CPU Core or CPU PECI temps being read.
But, if I boot  the system from the Windows 10 partition, the fans are still high, but the system is completely fine. The CPU usage is normal and the system works as intended, but with just the fans always on high. Ran “MacFanControl” in windows, still no core temps, but ran “core temp software”, which showed all the CPU temps in control and within limits.
To my understanding, I guess the SMC is not able to read the CPU Core or CPU PECI temps.
Please help, thanks!

 Did you have a liquid spill at some point?Did you try using an external bootable drive (with a clean OS install) to see if your internal drives OS has a problem?
Most likely you'll need to inspect the logic board both sides following this guide: MacBook Pro 15" Unibody Mid 2012 Logic Board Replacement and look carefully around the SMC chip for corrosion damage.




