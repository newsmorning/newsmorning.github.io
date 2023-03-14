---
title: "You'll never believe how this one gadget can revolutionize your electronics set-up: The Acurite Digital Readout Power Supply now available with Radioshack's 22 510 Switching Power Supply!"
ShowToc: true 
date: "2023-06-30"
author: "James Deltoro"
---
*****
You'll Never Believe How This One Gadget Can Revolutionize Your Electronics Set-up: The Acurite Digital Readout Power Supply Now Available with Radioshack's 22-510 Switching Power Supply!

Technology has continued to advance in ways we never thought possible, making our lives simpler, more enjoyable, and convenient. The electronics industry is not left behind, as it is an ever-evolving industry that introduces newer, more advanced gadgets regularly. One of such devices that can revolutionize your electronics set-up and elevate your experience is the Acurite Digital Readout Power Supply. Now, combine it with Radioshack's 22-510 Switching Power Supply, and you'll be amazed at the possibilities you can achieve.

Acurite Digital Readout Power Supply is a cutting-edge, easy-to-use digital power supply designed to help you power your electronic devices. It is an all-in-one device that features a built-in voltmeter, ammeter, and wattage meter with a high-resolution LED display, making it easy to monitor and adjust the output voltage, current, and wattage according to your requirements.

Moreover, the Acurite Digital Readout Power Supply comes with an adjustable voltage regulator and built-in protection circuits. This means that you can not only set the voltage to your desired level, but you can also rest assured that your device is protected from over-voltage, over-current, and short-circuits. It features a sleek and compact design that takes up little space in your work area.

Now, combine this amazing gadget with Radioshack's 22-510 Switching Power Supply, and you'll discover a world of new possibilities. The 22-510 is a versatile power source designed to deliver a constant, regulated voltage and current to your devices. With an output voltage range of 1.5V to 12V and a current output range of up to 1.5A, this power supply can power up to two devices simultaneously, making it ideal for powering a wide range of electronics, from small devices to larger ones.

The combination of the Acurite Digital Readout Power Supply and Radioshack's 22-510 Switching Power Supply creates a perfect pairing for powering and monitoring your electronic devices. You can use it to power your Arduino Projects, Raspberry Pi, LED lovers or any other electronics that require a stable and regulated power supply. You'll be amazed at the level of precision, control, and accuracy you can achieve with this powerful duo.

In conclusion, the Acurite Digital Readout Power Supply, combined with Radioshack's 22-510 Switching Power Supply, is a game-changer for anyone looking to elevate their electronics set-up. It offers accurate and precise power monitoring and control, versatile power output, and built-in protection, all in a compact and easy-to-use design. Get yours today, and experience the convenience and benefits it brings to your electronics set-up!


## Chosen Solution
 Hope someone can help.
I could not find a listed device even close.
The primary windings of the transformer have gone (open circuit). I am trying to find the secondary voltage so I can purchase a new transformer. There are no markings on the transformer. One of the first components after the rectifier on the pcb is an LM340T5780P+ voltage regulator (wired as fixed output). Is it possible to work out it’s supply voltage and hence input voltage from other components from the pcb?
Spec sheet says Vout - 5,12,15. Vin - 10,19,23. Are these just test voltages for the specs or are they the only 3 operating voltages?
It is connected to 2 capacitors with markings - K5R 334K & 105 +25K.




The transformer connects to the two pins.
There is no model number - Acurite Millmate.

The only numbers on the board are; 387575-6033 (printed) and 7-19   570702   1-29-90 (hand written) and ACU-RITE 387575-6034 ASSM. REV A (printed).
There does not appear to be a thermal fuse within the transformer. It has 4 primary windings and a single secondary winding.
The transformer is connected to the two pins shown in photos 1 and 3.
Is it possible to workout the supply voltage from the voltage regulator and the components around it - capacitors and resistors?
Do you mean the tiny capacitors near the regulator that I gave the numbers for, or the electrolytic capacitors?
The main transformer is connected directly to a RMS401L rectifier (Max 35V). The rectifier is connected directly to some electrolytic capacitors, the LM340T5 voltage regulator, an IC - TL494 and the small capacitors associated with the LM340T5 as listed above. The electrolytic capacitors are rated at 16V, the IC is rated at 7-40Vand the regulator is rated at 5V out and 5 to 18V in.
If I had to take a guess, it would be 12V supply to the board. Would that be correct? Could I damage anything with 12V - Would 10V be better?
Can anyone help
Kind Regards
Jeremy

 Hi @jwa2 ,
I assume that the faulty transformer is connected to the J4 connector on the board in image 3, is this correct?
Long shot maybe but try gently removing the insulation covering the windings on the transformer as some transformers have a cutout thermal fuse inserted in the transformer. Not sure if it is on the primary or the secondary or even if it is buried within the windings and not on the top under the insulation, but maybe worth a look.
If there is one there and it is blown you could try replacing it (hopefully its rating is stamped on it) and then check if the primary winding is OK and if so connect power to it and measure the output voltage on the secondary. You may have to be quick in case the fuse blows again due to an internal fault in the transformer
Knowing the output voltage is one thing as you still need to know the secondary output current required as well so that you can get the correct replacement or a suitable alternate supply.
The input voltage and current for the device is shown in the specs in the  user manual (see Sect 5-1)
Update (03/08/2022)
Hi @jwa2 ,
Did you check all the primary windings, you never said?
Here’s an image to show how you might be able to still use it perhaps.

(click on image to enlarge)
If it tests open circuit between terminals A - E as shown in the image try between B - E, C - E and D - E and check if there is a reading at all.
If there is no continuity between D - E then unfortunately the main part of the primary winding is open circuit so it can’t be used but if it is only open between A - B or A - C or A - D, you can use the other windings as the primary input e.g. B - E, C - E or D - E
The specs in the user manual list 4 AC input values so presumably they connect 240VAC across A - E, 220VAC across B - E, 120VAC across C - E & 100VAC across D - E so depending where the problem is in the primary winding you may be able to supply the appropriate AC input voltage across the working section of the primary.
If the transformer can’t be used, I would try connecting 10V AC first and check if the device functions normally and is still accurate,

 Hi James
Acurite had no idea what the secondary windings were meant to be.
I checked all the component specifications around the transformer connection to the pcb. Ie. the power supply section for maximum and minimum voltage requirements. All indicated that around 6V should be ok, so I found a 6.3V transformer - see photo. Obviously, if you are in the US you need a 110V primary. It has been working for around 8 months now.
So, if you have no other faults, maybe this is for you. I measured the output of my old transformer and it was 0V.
Your board looks different to mine, so a component voltage check would be advisable - in particular, the Voltage regulator (small black component with 3 pins). I think the output was 5V and 6.3V was within the input range of the one on my board. I can send more photos or go into more detail if required.
Many electronic component stores should be able to supply. I got mine from Jaycar - not sure if it is in the US.
Hope this helps.

 @jwa2 the voltages are very specific and would not be test voltages but actual operating voltages. We really would need to see more of the device etc. where this transformer is part off. Post some pictures of the whole setup with your question. I suppose you could try and get the voltages needed by designing your own voltage regulator circuitry or really try to hunt for a matching transformer (or at least something that comes close). It all depends on the requirements for the PSU and this transformer. By using the LM340t5 you know that the working amperage would be relatively low as well (~1A)Adding images to an existing question

 Hi, I also have a broken ACU-RITE Millmate. I believe that the transformer is defective form what I can tell. Any idea where I might be able to find a replacement. The numbers printed on the side are: 387575-600. Rev. A, Foster. 15576,  9251S. Any help where I might find. I would appreciate it very much. I will also try to send some pictures of the board it sets on. Thanks, James




