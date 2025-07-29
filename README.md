# Unschuled dissasembly a 3lb "meltybrain" combat robot

This is a 3lb combat robot that me and luke have designed. this is a special type of robot thats way more complcated then normal bots, normal bots just have normal wheels and then the spinning weapon right well this bot is the weapon, the two hugely overpowered motors act as drive motors set to spin oppisite directions from eachother so the enitre 3lb mass of the robot is the weapon for a greater moi and impact. this can be achieved by using a microcontroller like a arduino nano or in my case a adafruint itsybitsy 32u4 and hooking it to the reciever and allowing it to act as a controller for the motor escs instead of the reciever and what is then does is edit the pwn that the escs get to allow translational drift to happen which is when even when the entire robot is spinning at 5000 rpm it can still go in a mostly stright line. 

# About this project 
This project includes a custom pcb for all the wiring of motors, escs, adafruit and the accelerometer. the pcb also acts as a power distrubution board which i struggled with for a while because of the amount of power going throught it, the back pads of the escs are going to be filled with solder to help conduct the electricity better and allow for more heat disspation. all the vias are also going to be filled to the brim with solder. i also created a reverse polarity protection circuit for the electronics other then the escs using a mosfet. the weapons are going to be made out of ar500 steel for the strength to weight ratio. the pcb is going to cost extra because it has to be 2oz copper, this was a fun and painful project to learn how to make pcbs on. i know buying spares of parts is frowned opon but its the same price without the spare weapon, i also left the carbon fibre out of the bom because theres not enough time to get it quoted.



<img width="1240" height="718" alt="image" src="https://github.com/user-attachments/assets/351e054c-3a8f-429b-8e1f-a2853ed640db" />
<img width="1920" height="722" alt="471334013-767f2554-9c21-4e59-9d07-b84de258acd2" src="https://github.com/user-attachments/assets/17f9eb64-4beb-436a-8c96-fd9ac90e0d2a" />
<img width="1443" height="881" alt="image" src="https://github.com/user-attachments/assets/ac9372a2-50bf-4f83-9960-8640fa336449" />
<img width="1033" height="580" alt="image" src="https://github.com/user-attachments/assets/e36d1495-88ba-4be9-b40e-7bf34643fc17" />

| Parts                  | r | Cost   | Total Cost | Weight     | Total Weight | Provider        |                                                                |
|------------------------|---|--------|------------|------------|--------------|-----------------|----------------------------------------------------------------|
|                        |   |        |            |            |              |                 |                                                                |
| Drive/Weapon motor     | 2 | $34.59 | $69.18     | 156        | 312          | HobbyKing       | PROPDRIVE v2 3542 1250KV Brushless Outrunner Motor             |
| ESC                    | 2 | $30.00 | $60.00     | 13.9       | 27.8         | Amazon          | HGLRC Specter 90A 8S BLheli32 Single ESC                       |
| Battery                | 1 | $62.99 | $62.99     | 370        | 370          | Amazon          | OVONIC 4S LiPo Battery 3500mAh 14.8V 130C                      |
| Reciever               | 1 | $5.67  | $5.67      | 0.9        | 0.9          | Aliexpress      | FS2A 4CH AFHDS 2A                                              |
| Power switch           | 1 | $12.50 | $12.50     | 3          | 3            | Repeat Robotics | Lynx Anti-Spark Switch                                         |
| MCU                    | 1 | $9.95  | $9.95      | 2.6        | 2.6          | Adafruit        | Adafruit ItsyBitsy 32u4 - 5V 16MHz                             |
| xt90 connector         | 1 | $12.99 | $12.99     | 18         | 36           | Amazon          | xt90 connector                                                 |
| Buck Converter         | 1 | $3.55  | $3.55      | 3.85       | 3.85         | Amazon          | Micro voltage regulator                                        |
| N-Channel mosfet       | 1 | $7.99  | $7.99      | negligible | negligible   | Amazon          | N-Channel Enhancement-Mode MOSFET Transistor 60V 115mA,SOT-23. |
| Accelerometer          | 1 | $25    | $25        | Unknown    | Unknown      | Adafruit        | Adafruit H3LIS331 Ultra High Range Triple-Axis Accelerometer   |
| Pin headers            | 1 | $5.73  | $5.73      | negligible | negligible   | Amazon          | 40 pin Breakable Pin Header                                    |
| P-Channel mosfet       | 1 | $2.83  | $2.83      | negligible | negligible   | Aliexpress      | SUM110P06-07L-E3 p channel mosfet                              |
| Blue LED               | 1 | $6     | $6         | 2.8        | 2.8          | Amazon          | Clear blue LED Diode Lights                                    |
| Zener Diode            | 1 | $6     | $6         | negligible | negligible   | Amazon          | 15v zener diode                                                |
| Resistor set           | 1 | $7     | $7         | negligible | negligible   | Amazon          | 0805 Chip Resistor Assortment Kit                              |
| Ceramic Capacitor 47uf | 1 | $2.62  | $2.62      | negligible | negligible   | Aliexpress      | 0805 47UF 25V X7R M                                            |
| Electrolytic Capacitor | 1 | $9     | $9         | 33         | 33           | Amazon          | 4700uF 35V 18x30mm Electrolytic Capacitor                      |
| Weapon                 | 3 | $10    | $31        |            |              | SendCutSend     | ar500 steel weapon                                             |
| PCB                    | 1 | $27.50 | $27.50     |            |              | JLCPCB          | pcb for power distrubution and connections to mcu and escs     |
|                        |   |        |            |            |              |                 |                                                                |
| Body                   | 1 | $0.00  | $0.00      | $0.00      | $384.00      |                 |                                                                |
|                        |   |        | $367.82    |            | 1175.95      |                 |                                                                |

