---
title: "iPhone 5 Users Beware: Display Replacement Could Disable Vital Home and Power Buttons!"
ShowToc: true 
date: "2023-04-10"
author: "Robert Russell"
---
*****
Title: iPhone 5 Users Beware: Display Replacement Could Disable Vital Home and Power Buttons!

Are you an iPhone 5 user experiencing display issues? It's important to know that replacing your display could render your home and power buttons useless. This is because the replacement display is not an official Apple product and may not be compatible with certain features on your iPhone.

The home button and power button are essential to operating your iPhone. The home button is used to return to the home screen, activate Siri, and more. Meanwhile, the power button is used to turn your phone on and off, activate the lock screen, and take screenshots.

By having a faulty home or power button, your iPhone will become incredibly difficult to use. You may find yourself unable to turn on your phone, take screenshots, or even return to the home screen.

According to reports from Apple's support forums, some iPhone 5 users have experienced similar issues after replacing their display with a non-Apple screen. This is because third-party displays are not calibrated to work with the home and power buttons on the iPhone 5. Moreover, the display replacement process itself could damage the cables that connect the home and power button to the phone's logic board.

It's important to remember that even if you purchase an official Apple display, the repair process could still result in damage to your phone's cables. The iPhone 5's display replacement is not particularly easy and requires some level of expertise.

So, what should you do if you're experiencing display issues on your iPhone 5? Firstly, seek out a legitimate Apple repair service provider. This will minimize the risk of causing damage to your phone during the repair process. Secondly, backup your data before going in for repairs as a precautionary measure.

In conclusion, if you're an iPhone 5 user experiencing display issues, be mindful that replacing your display could cause further problems. Unofficial screens may not be compatible with your phone's home and power buttons, rendering them useless. Seek out a legitimate Apple repair service provider and backup your data before repairs take place to avoid any further discontent.

{{< youtube hIs6vLdHHKI >}} 



## Chosen Solution
 Hello,
I just replaced the display from my iPhone 5.
But after the replacement, mine home button + power button doens't work.
Weird is that my mute button + volume buttons does work.
Please someone sollution?
Thank you

 I do stateside board-level pry damage repairs like these via mail-in service--located in NY. Contact via my profile---this is straightforward if I happen to have a donor board, or for the parts commonly available on mouser.
To the discussion, I can add that the directionality of the U3 component is important---if it is installed upside down the phone will not power on.
Also important are R20 and R22 on either side of U3--required for home/power button circuit
I can confirm that this repair does restore the normal function of the power and home buttons.
UPDATE:
U3 chip is not available anywhere.  However, I've figured out that you can substitute a couple different low power buffer chips from the iPhone 3G logic board---U35_AP for example.  Proven working solution 100%
Do any of the dozen or so people that I've helped with this repair want to upvote this so this answer is closer to the top?  I am getting a lot of tentative 'can you really fix this?' emails about it, so I've added the repair service to my website:
http://www.mommyfixit.com/iPhone_5_Pry_D...

 See image content:

 Hey mate,
Do the buttons work if you replace the original damaged screen? If so, you need to return the screen you purchased. I would hazard to guess that this could be the issue. If not, let me know.
Cheers.

 Anyone have any more info on this? I'm running into this problem as well...same symptoms and missing two IC's  in the area shown in the posted picture. I'm game for trying to replace them, but I can't find any information on the specs for those IC's.
UPDATE:
I spent a lot of time last night digging around the web, and thought I'd post some info that may be helpful to folks in the future. First of all, a complete schematic of the IC's on the iPhone 5 logic board can be found here:
https://www.dropbox.com/s/0tmxaxb5n3x8em...
I have no idea how long that link will work, so no guarantees there. The password for the .RAR file that downloads is "rn325", without the quotes of course.
The three IC's highlighted by a previous poster are Q7, Q3, and U3 moving from left to right.
Q3 and Q7 seem to have something to do with power circuitry, so those specifically may have something to do with power button functionality, although it's not explicitly mentioned in the schematic. I don't happen to be missing those IC's, so I didn't dig into those any further.
I do happen to be missing U3, which definitely plays a role in the functionality of the home button and power button according to the schematic. I found a data sheet for the IC, which seems to be manufactured by NXP:
http://www.nxp.com/documents/data_sheet/...
I also happen to be missing the iC just to the right of U3, which is DZ101_RF. This IC has something to do with SIM card detection, which makes sense in my case because the phone never recognizes that it has no SIM card, nor will it read a SIM card when one is inserted. This part seems to be manufactured by Texas Instruments:
http://www.ti.com/lit/ug/slvu702/slvu702...
Now my problem is...how do I get my hands on these parts. Obviously, these are typically purchased in very large quantities, so I'm thinking that finding just one, or even a reasonable amount, is going to be impossible. The only option might be to find a non-functional iPhone 5 logic board somewhere and use these particular parts.
If anyone has any advice on where to find these replacement IC's, I would appreciate it very much!

 hi, look de solution for U3:
http://i40.tinypic.com/hv3odw.jpg
short (1->6) and (3->4)
solution of DZ101_RF (SIM CARD):
http://i39.tinypic.com/6ssahu.jpg
:)
br.
Mario Yunis

 Just to clarify this very confusing thread:-) the parts that everyone is referring to by their designators are as follows:
Q7 is manufacturer # RV1C002UN and it is a Nch 20V 150mA Small Signal MOSFET
Q3 is manufacturer # RV1C001ZP and it is a Pch -20V -100mA Small Signal MOSFET
U3 is manufacturer # 74AUP2G34GN and it is a Low-power dual buffer. That one is available [ http://www.nxp.com/products/logic/buffer...|from here.] Q3 and Q7 should be available from places like Mouser.com or Digikey.com. Be aware that Q7 and Q3 are a 0806 package. That means the size of the component is 2.0mm X1.6mmX1.6mm. Not an easy task to solder that. U3 is a SOT1115 package, measuring 0.9 x 1.0 x 0.35 mm with 0.3 mm pitch. So, unless one really knows how to solder and has the right tools, I would suggest to find somebody to do the replacement. Hope this helps, good luck

 Try to pluging it in to the charger this should take it out of sleep mode

 I can confirm that those chips on the photo of oliveira2013 do indeed render the home button+power button inactive if they are displaced/removed. Had the same problem and was fixed after having a repair shop replacing the chips on the board.
Update
@mjlegiralde & adem: sadly I don't know, I gave the phone to a repair shop to do the work on the logicboard.

 Great, thanks. Is your iPhone 5 a CDMA version? If so, that would explain why it still works even though DZ101_RF is missing. That particular IC seems to have a function relating to SIM card detection, so a CDMA iPhone would not necessarily need that ability to still be able to use the cell network...at least as I understand it.
U3 is some sort of buffer, so the behavior you're seeing (not turning on with power button, not waking after a few minutes, etc.) makes sense to me, at least from an empirical standpoint.

 I know this Problem... If the powerbutton activate Siri then u3 is not good placed on the solderpads. After correction the problem was solved..

 Hello,
I found here a lot of usable information about the same problem I have as well.
Here are my 2 cents, hope this can help many of you due to the availability of U3. It is possible there are even more replacement alternatives but I found some which are available widely enough. The original part 74AUP2G34GN from NXP can be directly replaced by 74AUP2G34FW3-7 from DIODES. This part is available from DigiKey - it is cheap enough and there are lots of it on stock DigiKey link
Below are 2 other alternatives which are not perfect replacement due to 0.35mm pitch instead of the original 0.3mm. Still, persons with good skills may use these if DigiKey is not an option. The parts are: 74AUP2G34FW4-7 (DIODES) and SN74AUP2G34DSFR (TI) - both on stock at Mouser - the DIODES part and the TI part.
Regards
Pavel

 @jessabethany  where can I find the U35_AP chip on the iphone 3g? (I mean, which part of the logic board). I will really appreciate your help.

 One of the two little copper pins from the home button got bent and is no longer making contact with the contact area located on the underside of the screen unit. Just bend them back into shape. Look underneath the  digitizer to align.




