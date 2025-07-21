---
title: "3lb MeltyBrain"
author: "Dylan and Luke"
description: "This is going to be a 3lb meltybrain that has a custom pcb to control pwm movement"
created_at: "2025-28-6"
---
# Total Time Spent 0hr

# June 28th: Researching parts, weight, and costs

Today is the start of the next bot, today will mainly consist of making a basic BOM, researching how to connect everything, and how to start designing the pcb for it. We also decided on the name of the bot... unscheduled dissasembly. Dylan worked on making the BOM and looked into what would need to be done to make the pcb. Luke sat on call with dylan and helped out with the BOM. After being on call for one hour we came up with the tenative BOM.

![image](https://github.com/user-attachments/assets/64e6b240-3704-41b0-bd76-19129e2d1823)

With this BOM we have two 3536 drone motors as our main drive motors and two 90a esc's that Dylan found a good deal on. We also decieded on running the bot on a 3500 mah 4s battery, on lukes suggestion we are going to run carbon fiber for top and bottom plates with ar500 or s7 tool steel teeth somehow screws into a tpu body. 

**Total Time Spend 1.5hr**

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

**Total time spend 5hr**


