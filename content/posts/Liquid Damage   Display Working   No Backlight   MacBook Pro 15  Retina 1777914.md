---
title: "You won't believe how this Macbook Pro survived liquid damage - with a working display but no backlight!"
ShowToc: true 
date: "2023-04-09"
author: "Evelyn Wisneski"
---
*****
Title: You Won't Believe How This Macbook Pro Survived Liquid Damage - With a Working Display but No Backlight!

Introduction:
Accidents happen all the time, and some of them can be disastrous, especially when it comes to electronic gadgets. However, there are some instances where devices survive damage beyond our expectations. One such incredible case is the Macbook Pro that survived liquid damage, with a working display but no backlight! Yes, you read that right. This miraculous incident demonstrates the durability and resilience of Apple's premium devices.

Body:
The incident occurred when a Macbook Pro owner accidentally spilled water on his device while working on an important project. He immediately turned off the laptop and dried it using a towel. However, as he turned it back on, he realized that the display was working, but the backlight was not. He tried all the tricks in the book - from resetting the SMC to adjusting the brightness - but nothing seemed to work.

Desperate to fix his beloved device, the owner took it to an Apple Authorized Service Provider (AASP) to get it checked. After a thorough inspection, the service provider informed him that the backlight chip on the logic board was entirely burnt due to liquid damage. This revelation shattered the hopes of the owner, who was convinced that his Macbook Pro was beyond repair. However, the service provider promised to fix it and asked for a few days to get the necessary parts.

A few days later, the service provider called the Macbook Pro owner and informed him that his device was repaired and ready for pickup. The owner rushed to the AASP, apprehensive about the outcome. After a small fee, the owner received his precious device, hoping that everything was okay.

To his amazement, the Macbook was in perfect condition, and it displayed everything without any problem. Still, he realized that the backlight was not working even after replacing the backlight chip. The service provider explained that the diode that powers the backlight chip might have also been burned due to liquid damage, which he fixed as well. The owner was thrilled to have his beloved device back, considering he only had to pay a mere fraction of the cost of a new Macbook Pro.

Conclusion:
The incredible story of the Macbook Pro that survived liquid damage, with a working display but no backlight, is a testament to the durability of Apple products. It also reaffirms the notion that proper care and quick action can save gadgets from irreparable damage. For anyone who encounters a similar accident, remember to turn off and dry the device immediately and take it to an authorized service provider as soon as possible. You never know; your device might just be as resilient as this Macbook Pro!

{{< youtube SKejJwQ3MGU >}} 



## Chosen Solution
 I have recently obtained an Early 2013 MBP 15-inch Retina, 2.4 / 8GB / 256 SSD.  The person that donated the laptop informed me that she spilled some liquid into the machine and that it no longer works.  Come to find out the machine boots and runs fine, display works through thunderbolt -> HDMI or HDMI port and LCD, however, there is no backlight.
I checked the fuse labeled "P" below the right fan with a multimeter and I do have continuity.  The liquid sensor is tripped under what I believe is the LVDS connector.
Can anyone provide next steps for troubleshooting this bad boy?
Thanks!
Matt
EDIT:  Board is 820-3332-A

 Of course there is no LVDS on this machine since it uses displayport, so no need to check a non-existent connector. Replace the LCD connector since pin 1 is burned, and make sure there is no short to ground when you plug the LCD cable back in. This didn't happen on its own, you spilled something or replaced the screen so check for whatever caused this.
Pin 1 of the LCD connector is the fuse on retinas, the fuse never blows.  On 820-3787 they fixed this stupid $@$* but 820-3332 melts the LCD connector without fail every time.




