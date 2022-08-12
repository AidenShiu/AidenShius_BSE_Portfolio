# Gesture-Controlled Car with Accelerometer
In this project, I build a car that can be controlled by my hand movements!

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Aiden Shiu | Lowell High School | Mechanical Engineering | Incoming Senior

![Project](https://i.ibb.co/XFLxJ90/IMG-8334.jpg)
![Me](https://i.ibb.co/qrV6TLp/Me.jpg)
![BlueStamp Engineering](https://static.wixstatic.com/media/d1d841_095ca2fd341e499988531cbf9bc9d2fe~mv2.png/v1/fill/w_1000,h_318,al_c,usm_0.66_1.00_0.01/d1d841_095ca2fd341e499988531cbf9bc9d2fe~mv2.png)
![Schematic](https://i.ibb.co/yXN41xk/Schematic-V1.png)
![CAD](https://i.ibb.co/0yPRhBd/CAD-V1.png)

Bill of Materials (Tools: soldering kit (+ filament), screwdriver, Arduino IDE):
- Arduino Uno, Arduino Micro
- HC 05 Bluetooth Module x2
- Wires x34
- 10k ohm resistors x7
- Breadboard x2
- 5v/1A mobile phone charger x2
- L298N motor driver
- MPU 6050 accelerometer
- Battery holder (AA battery x4)
- USB Cable A to B Cord
- USB Micro
- LED
- Tape
- Screws x14
- Nuts x14
- Screw mounting spacers x6
- Wheels x4
- Motors x4
- Car frame x2, motor tabs x8

# Final Milestone

My final milestone was the completion of my gesture-controlled car. I managed to connect the Bluetooth modules and transfer data using code that read and wrote gyroscope data. The car unit's code read that and started/stopped the motors accordingly. Some challenges were letting data get transferred from one module to the other and the motors stopping while trying to start. I solved the data transfer by supplementing the text data transfer code for HC05 communication into if statements to both units' codes: the motors would start if the gyroscope data was within a certain range. The motors stopping was solved by making the stop command activate on the condition of all values other than those covered by the directions (all values less than the directions being registered to stop the motors).

<iframe width="560" height="315" src="https://www.youtube.com/embed/z79fxv7lb4Q" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


Demo Night Presentation: https://docs.google.com/presentation/d/1ZVHzbN6flsaTkyChQDTGXWUFQCs_jenud-zdLmrFD3s/edit?usp=sharing

# Second Milestone

My second milestone was getting the accelerometer/gyroscope to work and produce values in the serial monitor. I also did the breadboard configurations for Bluetooth modules and am taking steps to connect them. Challenges that often came up were not selecting the right board or port in Arduino IDE or putting the wrong pins/wires for SCL and SDA pins. I learned a lot over this week about wiring/circuits -> had to make resistors in a 1:2 ratio (since I used 10kohm resistors I put two in parallel on the car unit breadboard to make a 1:2 ratio with the other 10kohm resistor—R_eq=(((1/10,000)+(1/10,000))^(-1))=5,000ohms). Also, I learned about the code for Arduinos, libraries, and the MPU 6050. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/pNDEMt8qtAY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


# First Milestone
  
My first milestone was setting up all four car motors and spinning them all simultaneously with an Arduino connected to an L298N motor driver. I ran into some trouble with the wires falling out, which was solved by screwing them into place. Also, the motors wouldn't all spin at the same time so I needed to fiddle with the code and Arduino pins until they all did. I learned a lot over this week. I had to solder the wires onto the motors and use Arduino IDE to make the motors spin.

<iframe width="560" height="315" src="https://www.youtube.com/embed/3ywsrFl8mXY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


# Tutorial Links Used

https://create.arduino.cc/projecthub/shubhamsuresh/how-to-make-a-gesture-control-robot-at-home-a3f4a4

https://create.arduino.cc/projecthub/ryanchan/how-to-use-the-l298n-motor-driver-b124c5

https://create.arduino.cc/projecthub/MissionCritical/mpu-6050-tutorial-how-to-program-mpu-6050-with-arduino-aee39a

https://create.arduino.cc/projecthub/RucksikaaR/interfacing-the-hc-06-bluetooth-module-with-arduino-f9c315

https://docs.google.com/document/d/129GrxjuClSyWmbEPe6VwU3c2hFJH28iS/edit?rtpof=true
