---
title: "Devastating liquid damage causes MacBook Pro 15 Touch Bar to short circuit and connector destroyed!"
ShowToc: true 
date: "2023-02-26"
author: "Frederick Haydon"
---
*****
Title: "The Nightmare of Liquid Damage on MacBook Pro 15 Touch Bar: How it Short Circuits and Destroys Connectors"

Introduction:

Macbooks are the preferred choice for many people, especially professionals, for their sleek design, excellent functionalities and overall productivity. However, these sophisticated machines are not immune to damages and accidents, especially when it comes to liquid damage. Liquid damage is a common yet devastating issue, which can seriously affect the performance and lifespan of your MacBook. In this article, we will discuss how liquid damage can cause MacBook Pro 15 Touch Bar to short circuit and destroy connectors.

Body:

MacBook Pro 15 Touch Bar is a powerful machine, with a host of advanced features such as Touch Bar, Retina display, and high-performance processors. However, these features are housed within a compact and tightly built structure and any damage to this structure can lead to serious problems. Liquid spills are one of the most common causes of damage to MacBooks, and they can result in short-circuiting, corrosion, and permanent damage to the components.

When liquid spills on a MacBook Pro 15 Touch Bar, it can penetrate the gaps and crevices in the keyboard, touchpad, and other openings, thereby reaching the internal components. The liquid contains minerals and salts, which can cause corrosion and oxidation of metal components, leading to the formation of rust, and eventually, a short circuit. Short circuiting is caused due to the flow of electric current in unintended directions or paths, and can cause the MacBook to shut down or stop working altogether.

In addition to short circuiting, liquid damage can also destroy the connectors in a MacBook Pro 15 Touch Bar. Connectors are essential components that help in the transfer of power and data between different parts of the machine. When liquid reaches the connectors, it can erode the metal contacts, leading to the loss of connection or even permanent damage. In such cases, the damaged connectors need to be replaced, which can be an expensive and time-consuming proposition.

Conclusion:

In conclusion, liquid damage is a serious issue that can cause irreversible damage to your MacBook Pro 15 Touch Bar. If you spill liquid on your MacBook, it is essential to take immediate action by turning off the machine, unplugging it from the power source, and wiping away the liquid. However, if you notice any symptoms such as malfunctioning, overheating, or unusual sounds, it is best to seek professional help. Regular maintenance and care can also go a long way in preventing liquid damage, such as the use of protective covers or avoiding liquids near your MacBook. Remember, prevention is always better than cure, when it comes to your MacBook's well-being.

{{< youtube VB8RrxbNqU8 >}} 



## Chosen Solution
 Hi,
I have a 2017 Macbook Pro with minor liquid damage to the board. The board has been cleaned, however it appears that the pad for pin 22 on J4402, the Touch Bar connector, has vanished and left a fairly decent sized  crater where the via for pin 22 would’ve been. After an exhaustive search I finally managed to identify/locate a suitable connector to use for replacement (if anyone else finds themselves in this situation, the connector can be harvested from an ipad air 1 or ipad air 2, it’s the rear camera connector).
I don’t have any schematics for this, so I’m not sure where I should be running a wire. The only pad that was damaged is pin 22 and the machine appears to be in an S0 state (the fans run but there’s no chime, no display, no caps lock key activation, no usb power out present, etc.  I see 18-19 volts on my meter and  the machine seems to be steadily puling approximately 2.9 amps. I suppose there isn’t much else to test at this point until address the issue with reconnecting pin 22.
This particular board schematic is not available, however 820-00281-A appears nearly identical to this model. I found a component that is incredibly hot, U8209, and it looks like this is a switch for PP5V_S0.  I’m hoping that if I can run a jumper from pin 22 to connect to PP5V_S0 somewhere , I might just be able to make this Macbook boot up again?
Any advice, direction or input is very much appreciated!
I’m going to take some pics so I can upload them to give a better understanding of the situation.
Added some pictures - the mounting hole/bracket thing was already missing when I received the board. I have no idea how it could’ve even been broken off in that spot.

 Yes, the connector is gone!
You also lost the mounting stud for the metal plate that helps hold the connector down. hopefully you can recover it (still with the plate?)
To remount the stud don’t clean off the remaining fiberglass from the stud! Carefully protect the area so you don’t get any flux or flux cleaning solvent into the damaged well on the logic board when you pull off and mount the new connector. Using a sprayer with a non-residue cleaner clean the stud and the area on the logic board. The trick here is the rough surface of the break will help hold the stud back on better.
You want to use a gel Cyanoacrylate glue. To help speed up the set use your breath which has moisture within it. You may also need a new Touch Bar if the cable connector is damaged MacBook Pro 15" Retina (Late 2016-2017) Touch Bar Assembly

 I have that same issue with my a1707 preciesely, I’ve seen it 3 times so far, always the same pin in the same connector involved.  This has to be a design issue.)
It won’t let me post the schematic or brd but if you google 820-00239 its not exact same board but extremely similar, it has helped me!  Also, there is a current regulator involved, and from what I’ve heard it’s on the back side of the board.




