---
title: "Desperate DIYer seeks circuit wizardry - Can you solve this audio amplifier mystery?"
ShowToc: true 
date: "2022-12-26"
author: "Paula Blackard"
---
*****
+++ 
title = "Desperate DIYer seeks circuit wizardry - Can you solve this audio amplifier mystery?" 
date = 2021-07-21T20:56:47+08:00 
tags = ["audio amplifier", "DIY", "electronics"] 
author = "John Doe" 
description = "A desperate DIYer seeks help in fixing his audio amplifier circuitry. Can you help him solve this audio amplifier mystery?" 
+++

As an avid DIYer with a passion for electronics, I have always enjoyed tinkering with circuits and building my own gadgets. Recently, I decided to take on an audio amplifier project that I had been planning for a while. The project involved building a simple audio amplifier circuit using a LM386N IC and a few basic components.

To my dismay, the circuit did not seem to be functioning as expected. Despite careful soldering and following the circuit tutorial to the tee, my audio amplifier was producing no sound. I tried replacing the IC, triple-checking the wiring, and testing each component individually, but nothing seemed to work.

At this point, I realized that I had hit a dead end and required the help of a more experienced circuit wizard. As such, I decided to reach out to the online electronics community for assistance.

To my surprise, I received several responses from fellow DIYers and electronics enthusiasts, offering to help me fix my audio amplifier circuit. One individual, in particular, provided me with a list of possible causes for the issue I was experiencing.

According to this kind-hearted individual, there were several potential causes for my audio amplifier's lack of functionality. These ranged from faulty individual components to incorrect wiring of the IC's inputs and outputs.

 Armed with this knowledge, I decided to go back to the drawing board and start from scratch. I eventually found that I had made an error in the wiring of the IC's inputs, and the correction of that mistake enabled the circuit to produce excellent sound quality.

In conclusion, my experience with this audio amplifier project taught me the importance of seeking help from the online electronics community when facing technical difficulties. I learned that there are many passionate and knowledgeable individuals out there who are always ready to offer assistance and guidance to fellow DIYers.

As for the audio amplifier, it is now working perfectly, and I have gained a brand new sense of appreciation for the power of collaborative problem-solving. I now know that even the most perplexing electronics projects can be successfully completed with a little help from others.


## Chosen Solution
 I attached a schematic of a circuit I am troubleshooting.  In red, I have marked where I should be seeing 1.6V on the negative side of two capacitors, but I am getting 0V. What would cause this to happen? The capacitors themselves are good, the + side is getting the appropriate voltage, but I am not getting the 1.6V on the - side.

thank you in advance for your help!

 Hi,
Just querying if you're measuring for AC voltage with a signal injected into the amplifier?
They’re both coupling capacitors which allow the AC component of the signal (-ve  and  +ve going transients) to pass through but not the straight DC. They are directly connected to the R & L, V inputs of U16.
Did you measure at pins 3 & 6 on the IC?
Are the U16 voltages i.e. VCC1A, VCC1B, VCC2 & VDD, all OK.
Here’s the datasheet for the IC.




