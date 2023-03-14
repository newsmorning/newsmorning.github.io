---
title: "Warning: Macbook Pro 13 Retina Display Early 2015 owners must read this! A1502 LCD screen malfunction causes video blackout during wakeup with backlight still on!"
ShowToc: true 
date: "2023-03-24"
author: "Karen Macdonald"
---
*****
Title: Warning: MacBook Pro 13 Retina Display Early 2015 Owners Must Read This! A1502 LCD Screen Malfunction Causes Video Blackout during Wakeup with Backlight Still On!

If you own a MacBook Pro 13 Retina Display from early 2015, you may want to read this before you take any further action with your device. A1502 LCD screen malfunction causes video blackout during wakeup with backlight still on, and this is a problem that has been reported by many MacBook users.

The MacBook Pro 13 Retina Display is a popular device that is widely used by people across the world. It is a sleek and powerful machine that is designed to cater to the needs of professionals and students alike. However, the A1502 LCD screen malfunction can cause a major inconvenience to the users of the device.

The problem appears to be caused by a faulty component on the LCD screen that causes the backlight to stay on, even when the device is in sleep mode. This results in a video blackout when the device is woken up from sleep, but the backlight remains on.

The good news is that Apple has recognized the problem and has launched a repair program to address the issue. If you are experiencing this problem with your MacBook Pro 13 Retina Display, you can take your device to an Apple store or an authorized repair center to get it fixed for free.

It is important to note that not all MacBook Pro 13 Retina Display devices from early 2015 are affected by this problem. Only those that were sold between October 2014 and February 2015 are eligible for the repair program.

If you are unsure about whether your device is eligible for the repair program or not, you can check the serial number of your MacBook Pro 13 Retina Display on the Apple website. If your device is eligible, you can arrange a repair appointment with Apple or an authorized repair center.

In conclusion, the A1502 LCD screen malfunction is a serious problem that can cause a major inconvenience to the users of MacBook Pro 13 Retina Display from early 2015. However, the good news is that Apple has recognized the problem and has launched a repair program to address the issue. If you are experiencing this problem with your device, make sure to take it to an Apple store or an authorized repair center to get it fixed for free.

{{< youtube SKejJwQ3MGU >}} 



## Chosen Solution
 I am trying to fix an early 2015 13" MBP.
Got it working (mostly) except on wake from sleep (or when rebooting during an install) I lose video output on the LCD. Backlight is on (verified by turning bringhtness all the way up, I get a light vertical display output from second lvds channel)
If I don't close the clamshell, use screen saver with "never sleep" timeout, it works fine (except needing hard power down if I update OS)
Unfortunately due to cats who love walking on keyboards, I need to close the lid.
I have tried:
SMC and P/N VRAM resetunplug/replug battery (battery is "normal")safe modebooting external SSD (same problem)reinstalling OSgoogling many hours for answers
I suspect something with LCD voltage rails coming out of sleep, but I need to find the schematics and board view to check.
I will try an external hdmi monitor, which I suspect will work, but that does not help with getting sleep working.
Any/all help much appreciated,
Bill

 @mikronauts - Let’s back up here a bit… What happened on your repair journey? You talk about your cat loves walking across your computer is it possible it marked your system?
As far as your video retina systems use iDP signaling while the cable is similar to the older LVDS cable the signals are very different like the older analog TV and our current digital TV signaling both use an antenna so we can’t assume the conduit is the same just like how water and gas both use pipes.
As far as what the external display uses. It uses either DP or Thunderbolt connection (the video in both is DP)
The logic board uses a MUX to spilt out the video to the internal and Thunderbolt ports. If you are getting a good external image via both TB ports then we know the issue is strictly within the internal displays path if it doesn’t offer a good image.
As far as wake/sleep that is a different circuit which would need to be independently tested and repaired. While from the use perspective they do fit hand to glove they are not one in the same.




