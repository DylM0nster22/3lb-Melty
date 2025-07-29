---
title: "3lb MeltyBrain"
author: "Dylan and Luke"
description: "This is going to be a 3lb meltybrain that has a custom pcb to control pwm movement and distrubte power"
created_at: "2025-28-6"
---
# Total Time Spent 38.75hr

# June 28th: Researching parts, weight, and costs

Today is the start of the next bot, today will mainly consist of making a basic BOM, researching how to connect everything, and how to start designing the pcb for it. We also decided on the name of the bot... unscheduled dissasembly. Dylan worked on making the BOM and looked into what would need to be done to make the pcb. Luke sat on call with dylan and helped out with the BOM. After being on call for one hour we came up with the tenative BOM.

![image](https://github.com/user-attachments/assets/64e6b240-3704-41b0-bd76-19129e2d1823)

With this BOM we have two 3536 drone motors as our main drive motors and two 90a esc's that Dylan found a good deal on. We also decieded on running the bot on a 3500 mah 4s battery, on lukes suggestion we are going to run carbon fiber for top and bottom plates with ar500 or s7 tool steel teeth somehow screws into a tpu body. 

**Total Time Spent 1.5hr**

# June 29th: making the cad and trying to make the pcb

Today luke designed the enitre meltybrain robot while on a call with dylan. Dylan started trying to make the pcb and tried different ideas and custom things but completly failed at all of them. Luke spent around 8hr making the meltybrain cad and its mostly done, dylan had no progress to speak of other than deciding on a plan.

![image](https://github.com/user-attachments/assets/e41fcb9e-9832-4c37-90cd-c68255b39981)
![image](https://github.com/user-attachments/assets/263007fa-38ad-49f9-9e12-a08b5cc27c43)
![image](https://github.com/user-attachments/assets/aeae5ecb-53cc-4c41-926c-c87c14aa5500)

**Total time spent 8hr**

# July 18th: Starting the PCB

Today Dylan started the design of the pcb and got pretty close to finishing the schematic, he added the mcu which is a xiao esp32 breakout board, the mcu an h3lis311 breakout board, the reciever which is a fs-2a, the led, the xt60, and he still needs to add things like voltage regulator pads and other various things. tommorow will most likely consist of mainly wiring the pcb.

![image](https://github.com/user-attachments/assets/ae449426-af5a-4c87-ad0e-6ca301b02cf3)

**Total time spent 6hr**

# July 20th: Getting closer to wiring the PCB

Dylan didnt have time to work on the PCB yesterday and today he learned he wasnt even close to done with the schematic, the mcu that was being used was the wrong type so that was switched to an Adafruit ItsyBitsy 32u4 - 5V 16MHz because its the correct architecture for the opensource code were using/editing called openmelt2. He also learned that a xt60 wasnt nearly big enough for this so the bot is now going to use a xt90 which supports up to 90a. tommorow will consist of adding resistors, diodes, cap's, etc, then maybe after all that wiring the PCB. oh and a buck converter was also added to keep everything at 5v. Most of the time was spent remakeing things and relizing nothing works.

![image](https://github.com/user-attachments/assets/65da2628-63cd-44c1-8b85-a7690f9aad56)

**Total time spent 5hr**

# July 21st: added the rest of things to schematic

Today dylan worked on the schematic and added things like caps, resistors, mosfets, and diodes, he also added everything that is needed into the bom, the price might be over 350$ so luke might need to split the extra. the big main mosfet is for in case the power gets applied backwards all the electronics dont die, the diode is to help reduce noise.

![image](https://github.com/user-attachments/assets/5f6904a4-4b80-426b-9970-d34f1ce15626)

**Total time spent 3hr**

# July 22nd: starting the pcb part

Today dylan spent too long to count looking for footprints before relizing that he has to make some of them himself or find ones close enough then edit them, he placed most of the components in a way that might work but might have to change it later, he also made the boundey of 48x128mm which is how big the current comparment of the bot is. 

![image](https://github.com/user-attachments/assets/ecefd59d-47b6-43b0-bab3-d6088a5bcd57)

**Total time spent 4hr**

# July 23rd: Continuing on the PCB

Today Dylan finally started getting into the grove of how kicad works after spending too many hours on it, he also learned that 90a on 16.4v is alot of power and needs thick traces, about 10mm with 2oz copper and solder all over those 10mm lines so that fun. he also relized that the current boundries were too small for both the normal bot componenets and the pcb so the pcb is now 28 mm longer yay more room. he had fights with the mcu footprint and the accelarometer footprint for a while because neither of them were working correctly with pins and whatnot until he changed the pins in the footprint which took him hours to learn. overall most of the placement is decided, this bot is going to be spinning stupid fast around 300mph, for the acceloreter to not be oversatured it needs to be exactly in the ceneter, even 10mm out from the center could reach almost 5000 g's. there is too much open space in the pcb perfect for some art.

![image](https://github.com/user-attachments/assets/313ae2f6-6445-4a53-8417-81a9940b3905)

**Total time spent 3hr**

# July 27th: Finishing the PCB and editing the CAD

Today luke didnt exist so dylan did everything, the start of today was routing the pcb and figureing out how to make those big traces i was talking about, routing took a bit because i had to remember how to flip wires on the underside of the board and figure out how to make the big traces. i learned instead of normal traces what i needed was zones of copper, and to make it so everything was easier to route i make those zones on the bottom of the board. during the routing process i relized that where i had the pins for the reciever to the mcu set wrong so i had to change that. on the Cad side of things i had to make the space changes i talked about earlier to make the pcb fit and i also learned luke wasnt as done with the cad as i though. I added things like more support for the center of the bot, mounting holes for the weapons, wheels and rims, making the whole things 6mm taller, adding the escs, and adding screw holes to the bottom plate. tommorow i will need to make a way to mount the tires to the rims and add screw holes to the top lid and do some final weight calculations and hope that im not somehow out of weight, oh and i also learned that i am overbudget by a good amount so thats fun. while i was typing this big paragraph i was letting fusion render the cad so thats nice.

![image](https://github.com/user-attachments/assets/587d3e10-3455-4d4e-ab22-b6c65ada1be3)
![image](https://github.com/user-attachments/assets/767f2554-9c21-4e59-9d07-b84de258acd2)
![image](https://github.com/user-attachments/assets/cc086c95-5261-4a39-8bf9-6529ee81a07c)
![image](https://github.com/user-attachments/assets/e95d2aff-6e03-483b-81df-baa9032a1f29)
![image](https://github.com/user-attachments/assets/5247cdd4-f1bb-4297-a058-7f1654979a7d)

**Total time spent 8hr**

# July 28th: spent some time on finishing touches and weight calculations

Today didnt consist of much just some small things like adding screw holes to the top. send cut send is really fun with pricing see the images below which is why theres three weapons instead of just two. i think this is the end of it, time to submit and hope for the best. there is carbon fibre needed but were going to buy it separately.

![image](https://github.com/user-attachments/assets/dd17807b-7a73-46b5-828c-13e41d4d3d83)
![image](https://github.com/user-attachments/assets/4f24199f-9d35-4e4d-ace8-8fb3252dcc75)
![image](https://github.com/user-attachments/assets/b3bd89a2-dc25-4741-b53a-229dbfaabac8)

**Total time spend 45 min**
