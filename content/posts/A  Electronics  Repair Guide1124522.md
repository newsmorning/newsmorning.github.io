---
title: "Revive your Dead Devices with this One-of-a-Kind Electronics Repair Guide - Save Hundreds of Dollars on Repairs!"
ShowToc: true 
date: "2022-12-05"
author: "Bryan Shaw"
---
*****
# Revive your Dead Devices with this One-of-a-Kind Electronics Repair Guide - Save Hundreds of Dollars on Repairs!

Tired of constantly buying new devices when your old ones stop working? Sick of shelling out hundreds of dollars for repairs from professionals? Look no further than this one-of-a-kind electronics repair guide to revive your dead devices and save yourself a ton of money in the process.

Whether it's a broken phone screen, a malfunctioning laptop, or a dead battery in your game controller, this guide has got you covered with step-by-step instructions and detailed diagrams to help you troubleshoot and fix the problem yourself.

One of the great things about this guide is that it covers a wide range of devices and brands, so you can use it for all your repair needs. It even includes sections on repairing your television and home theater system, so you can enjoy your favorite shows and movies without having to pay for costly repairs or replacements.

Another advantage of this guide is that you don't need to have any prior technical knowledge or skills to use it. The instructions are simple and easy to follow, and the guide includes a glossary of terms to help you understand any technical jargon you may come across.

But perhaps the best part of all is the money you'll save. Repairing your devices yourself can cost just a fraction of what it would cost to have a professional do it. In fact, some repairs can be done for as little as a few dollars in parts and supplies.

And let's not forget the environmental impact. By repairing your devices instead of throwing them out and buying new ones, you're having a positive impact on the environment by reducing waste and conserving resources.

In conclusion, if you're tired of constantly buying new devices or paying hefty repair bills, this one-of-a-kind electronics repair guide is a game-changer. Not only will it save you hundreds of dollars on repairs, but it also empowers you to take control of your devices and extend their lifespan. So why wait? Revive your dead devices today and start saving money and the planet.

{{< youtube lBSD6Ni2ZUI >}} 







Difficulty
 



Moderate         
 








Steps
 
13
 



Time Required
 

Suggest a time??
            
 


Sections
 
1
 
- A. Electronics
 - 13 steps

 




Flags
 
#### Member-Contributed Guide
 
An awesome member of our community made this guide. It is not managed by iFixit staff.
 
- BackBLV MGN Cube
 - Full Screen
 - Options

 
- History
 - Save to Favorites
 - Download PDF
 - Edit
 - Translate
 - Get Shareable Link
 - Embed This Guide
 - Notify Me of Changes
 - Stop Notifications

 
## Introduction
 
I did not modify the original wiring in anyway with the exception of the endstops. If there is a middle wire cut the wire and remove it.
 
I’ve you’ve seen my previous builds you know I put a lot of effort into making things look clean. Personally I would’ve made some of the wires longer and some shorter. But with this type of kit you need the flexibility. This is the reason why the wiring isn’t clean.
 
There are 3x push button switches. 1 momentary switch for power and 2x 24v latching switches. 1 of the latching switches is for the LEDs. The 2nd switch can be used for additional LEDs, fans, etc.
 
This is the way I did it based off the information I had and my experience. If you know of a better way or want to share some feedback feel free to contact me directly over Facebook.
 
## What you need
 
## Featured Document
 
## 

Step 1

                  Electronic Mounting               


 
- 
 - Mount the PSU with 5x M3x6 button head screws. The output voltage terminals will be facing up.
 - 
 - Mount the Duet by first screwing in 4 M3x6 button head screws on the inside of the printer through the back panel, into 4x M3x15mm standoffs. Mount the Duet with 4x M3x6 button head screws to the standoffs. The WiFi antenna will be facing up.
 - 
 - Mount the SSR with 2x M4x10 button head screws and 2x M4 nuts. The SSR will be upside down.(Terminals 3 and 4 will be facing up)
 - 
 - There wasn't really a good place to put the Wago connector for the LEDs. I used some 2 sided tape and taped it to the side of the PSU

 
Mount the PSU with 5x M3x6 button head screws. The output voltage terminals will be facing up.
 
Mount the Duet by first screwing in 4 M3x6 button head screws on the inside of the printer through the back panel, into 4x M3x15mm standoffs. Mount the Duet with 4x M3x6 button head screws to the standoffs. The WiFi antenna will be facing up.
 
Mount the SSR with 2x M4x10 button head screws and 2x M4 nuts. The SSR will be upside down.(Terminals 3 and 4 will be facing up)
 
There wasn't really a good place to put the Wago connector for the LEDs. I used some 2 sided tape and taped it to the side of the PSU
 
1024
 
## 

Step 2

                  Power Plug               


 
- 
 - The orange arrow is the Load(AKA hot/power) wire. It connects to the Load input on the power supply and to the Load wire on the momentary power button
 - 
 - The green arrow is the Neutral wire. It connects to terminal 2 on the SSR along with the green wires of the momentary power button
 - 
 - The black wire is ground or earth. It connects to the Negative input on the power supply and the black wire of the momentary power button
 - 
 - NOTE-The FYSETC wiring said to connect the Black wire from the momentary push button switch to Neutral. This is incorrect. It should be connected to Negative

 
The orange arrow is the Load(AKA hot/power) wire. It connects to the Load input on the power supply and to the Load wire on the momentary power button
 
The green arrow is the Neutral wire. It connects to terminal 2 on the SSR along with the green wires of the momentary power button
 
The black wire is ground or earth. It connects to the Negative input on the power supply and the black wire of the momentary power button
 
NOTE-The FYSETC wiring said to connect the Black wire from the momentary push button switch to Neutral. This is incorrect. It should be connected to Negative
 
## 

Step 3

                  PS_ON/SSR               


 
- 
 - SSR pin 3(+) > Duet pin 3 (3.3v)
 - 
 - SSR pin 4(-) > Duet PS_ON
 - 
 - SSR pin 1 > neutral in from power plug + yellow wire from power button
 - 
 - SSR pin 2 > neutral to board + green wire from power button
 - 
 - In order for PS_ON to work you have to have M80 in config.g and hold the power button down for 1-2 seconds. When M80 is ran, PS_ON becomes grounded. This is what powers the SSR

 
SSR pin 3(+) > Duet pin 3 (3.3v)
 
SSR pin 4(-) > Duet PS_ON
 
SSR pin 1 > neutral in from power plug + yellow wire from power button
 
SSR pin 2 > neutral to board + green wire from power button
 
In order for PS_ON to work you have to have M80 in config.g and hold the power button down for 1-2 seconds. When M80 is ran, PS_ON becomes grounded. This is what powers the SSR
 
## 

Step 4

                  PSU Output               


 
- 
 - On the PSU the 3 terminals on the left(Orange) are + and the 3 on the right(Green) are -
 - 
 - Connect 1 + and 1- from the PSU output to the Duet Input paying attention to the polarity

 
On the PSU the 3 terminals on the left(Orange) are + and the 3 on the right(Green) are -
 
Connect 1 + and 1- from the PSU output to the Duet Input paying attention to the polarity
 
## 

Step 5

                  BLTouch Wiring               


 
- 
 - Connect the White wire to Z_PROBE_IN
 - 
 - Connect the Black wire to GND
 - 
 - Connect the Red wire to Pin 1 5v
 - 
 - Connect the Brown wire to Pin 2 GND
 - 
 - Connect the Orange wire to Pin 8 HEATER3

 
Connect the White wire to Z_PROBE_IN
 
Connect the Black wire to GND
 
Connect the Red wire to Pin 1 5v
 
Connect the Brown wire to Pin 2 GND
 
Connect the Orange wire to Pin 8 HEATER3
 
## 

Step 6

                  PanelDue               


 
- 
 - Connect the 10 pin ribbon cable to CONN_SD on the Duet to the Panel Due

 
Connect the 10 pin ribbon cable to CONN_SD on the Duet to the Panel Due
 
## 

Step 7

                  BLV NeoPixel Board               


 
- 
 - Connect the white/black wire from the NeoPixel board to the PanelDue port on the Duet
 - 
 - Connect the +/- from the NeoPixel board to the PSU output. Make sure you pay attention to polarity.
 - 
 - Connect the 3x 3 wire NeoPixel rings to the NeoPixel board
 - 
 - I didn't like the long 2 wire cable going back to the Duet.  A simple modification you can do if you have the ability to crimp new connectors is you can connect the BLV NeoPixel board to the side of the PanelDue
 - 
 - Connect the White(RX) wire from the BLV NeoPixel board to the TX porton the PanelDue.
 - 
 - Connect the Black(GND) wire from the BLV NeoPixel Board to the GND port on the PanelDue
 - 
 - The BLV NeoPixel board is supposed to work with the Duet 3. However I've not been able to get it to work correctly. There's speculation the transmission levels are too low for the BLV board. We're currently investigating.

 
Connect the white/black wire from the NeoPixel board to the PanelDue port on the Duet
 
Connect the +/- from the NeoPixel board to the PSU output. Make sure you pay attention to polarity.
 
Connect the 3x 3 wire NeoPixel rings to the NeoPixel board
 
I didn't like the long 2 wire cable going back to the Duet.  A simple modification you can do if you have the ability to crimp new connectors is you can connect the BLV NeoPixel board to the side of the PanelDue
 
Connect the White(RX) wire from the BLV NeoPixel board to the TX porton the PanelDue.
 
Connect the Black(GND) wire from the BLV NeoPixel Board to the GND port on the PanelDue
 
The BLV NeoPixel board is supposed to work with the Duet 3. However I've not been able to get it to work correctly. There's speculation the transmission levels are too low for the BLV board. We're currently investigating.
 
## 

Step 8

                  Stepper Wiring               


 
- 
 - First put a jumper over each stepper channel in the 2nd Z port in Drive 2
 - 
 - Pay attention to the Drive layout. They do not go in numerical order
 - 
 - Connect the Extruder (E0) to Drive 3
 - 
 - Connect the X stepper(Top Left stepper) to Drive 0
 - 
 - Connect the Y stepper(Top Right) to Drive 1
 - 
 - Connect the Z1 (Left Z stepper) to Drive 4
 - 
 - Connect the Z2 (Right Z stepper) to Drive 2

 
First put a jumper over each stepper channel in the 2nd Z port in Drive 2
 
Pay attention to the Drive layout. They do not go in numerical order
 
Connect the Extruder (E0) to Drive 3
 
Connect the X stepper(Top Left stepper) to Drive 0
 
Connect the Y stepper(Top Right) to Drive 1
 
Connect the Z1 (Left Z stepper) to Drive 4
 
Connect the Z2 (Right Z stepper) to Drive 2
 
## 

Step 9

                  LEDs               


 
- 
 - I used different LEDs than what were in the kit but they are installed in the exact same way.
 - 
 - The wiring is pretty straight forward. The important thing to remember is with the Wago connectors one side is input and the other side is output. Make sure you do not cross the polarity
 - 
 - The Black wire on the push button latching switching goes to the Negative - terminal on the PSU output
 - 
 - The Yellow wire on the push button latching switch goes to the positive + side of the PSU output.
 - 
 - The Green and Red wire on the push button latching switch goes into one of the contacts on the Wago connector. This will be the Positive + side
 - 
 - The single Black wire in the kit goes from the Negative terminal on the output side of the PSU to the open contact on the same side as the Green/Red wire.
 - 
 - The both Red Positive + wires of the LEDs will go in the opposite side of the Green/Red wires
 - 
 - Both Black Negative - wires of the LEDs will go in the opposite side of the Black Negative - wire

 
I used different LEDs than what were in the kit but they are installed in the exact same way.
 
The wiring is pretty straight forward. The important thing to remember is with the Wago connectors one side is input and the other side is output. Make sure you do not cross the polarity
 
The Black wire on the push button latching switching goes to the Negative - terminal on the PSU output
 
The Yellow wire on the push button latching switch goes to the positive + side of the PSU output.
 
The Green and Red wire on the push button latching switch goes into one of the contacts on the Wago connector. This will be the Positive + side
 
The single Black wire in the kit goes from the Negative terminal on the output side of the PSU to the open contact on the same side as the Green/Red wire.
 
The both Red Positive + wires of the LEDs will go in the opposite side of the Green/Red wires
 
Both Black Negative - wires of the LEDs will go in the opposite side of the Black Negative - wire
 
## 

Step 10

                  X Carriage               


 
- 
 - The X Carriage wiring is pretty straight forward. Polarity of E0 Therm, E0 Heater and Bed Therm is irrelevant.
 - 
 - The 2 4010 Blower fans are wired together so you only need 1 set of wires going back to the board.
 - 
 - To make the connector I soldered the 2 + wires together and the 2 - wires together. I than cut the length I needed from the original 5015 blower fan and soldered the wires together.
 - 
 - Make sure you remove the middle wire of the endstops.

 
The X Carriage wiring is pretty straight forward. Polarity of E0 Therm, E0 Heater and Bed Therm is irrelevant.
 
The 2 4010 Blower fans are wired together so you only need 1 set of wires going back to the board.
 
To make the connector I soldered the 2 + wires together and the 2 - wires together. I than cut the length I needed from the original 5015 blower fan and soldered the wires together.
 
Make sure you remove the middle wire of the endstops.
 
## 

Step 11

                  Heated Bed               


 
- 
 - The wiring for the 24v DC bed is pretty straight forward. Make sure you pay attention to the polarity of the +/-.

 
The wiring for the 24v DC bed is pretty straight forward. Make sure you pay attention to the polarity of the +/-.
 
## 

Step 12

                  Wiring               


 
- 
 - The wiring didn't turn out as well as I would've liked. Because this is supposed to be an all in one kit I didn't want to modify the wiring. After all is said and done I'll probably do some re-wiring and put in cable raceways
 - 
 - Use some small zip-ties to bundle the wires together.
 - 
 - As you can see with the back panel it's definitely not my cleanest wiring. Normally I'll make my own cables to they're the length I want.

 
The wiring didn't turn out as well as I would've liked. Because this is supposed to be an all in one kit I didn't want to modify the wiring. After all is said and done I'll probably do some re-wiring and put in cable raceways
 
Use some small zip-ties to bundle the wires together.
 
As you can see with the back panel it's definitely not my cleanest wiring. Normally I'll make my own cables to they're the length I want.
 
## 

Step 13

                  Jumpers               


 
- 
 - Make sure your jumpers are set correctly.
 - 
 - V_FAN: This is where you select the voltage for the 5 fan ports. You want the jumper on VIN (pins 2 & 3) to set the fans to run on the voltage that is supplied to the Duet 2 WiFi(24v). If you set it to 5v(pins 1 & 2) the fans won't turn on.
 - 
 - 5v Selection: You need to select if 5v is provided by the onboard regulator(24v to 5v) or from an external 5v source.
 - 
 - Only use INT 5V EN or EXT 5V EN.
 - 
 - INT 5V EN: Most builds you will have the jumper placed here.
 - 
 - EXT 5V EN: Place a jumper here if you want to use an external PSU to provide 5v to the board.
 - 
 - If desired you need to connect the external 5v source to the +5V and GND pins on EXT 5V header
 - 
 - Erase Jumper: Used to erase the firmware

 
Make sure your jumpers are set correctly.
 
V_FAN: This is where you select the voltage for the 5 fan ports. You want the jumper on VIN (pins 2 & 3) to set the fans to run on the voltage that is supplied to the Duet 2 WiFi(24v). If you set it to 5v(pins 1 & 2) the fans won't turn on.
 
5v Selection: You need to select if 5v is provided by the onboard regulator(24v to 5v) or from an external 5v source.
 
Only use INT 5V EN or EXT 5V EN.
 
INT 5V EN: Most builds you will have the jumper placed here.
 
EXT 5V EN: Place a jumper here if you want to use an external PSU to provide 5v to the board.
 
If desired you need to connect the external 5v source to the +5V and GND pins on EXT 5V header
 
Erase Jumper: Used to erase the firmware
 

Cancel: I did not complete this guide.

 

                                                                                          5 other people completed this guide.                                             
 
### Attached Documents
 
- 
 - BLV接线图
 - PDF - 47.52 mb
 - View

 

 
BLV接线图
 
PDF - 47.52 mb
 
### 
Author

 

                                          with 1 other contributor 
 
#### 

                        David Husolo                     

 
Member since: 06/16/2021
 
7,245 Reputation
 

                                          28 Guides authored                  
 


                           Badges:
                           14


 


                                                            +11 more badges                           




