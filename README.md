# Arduino Laser Trip Wire Project

## Description
For this project, I designed a device that detects when someone or something passes it by. Using two lasers that point at light detecting devices (LDRs) and a speaker attachment, the device greets guests upon their entry to my apartment and bids them farewell upon their exit. There are no limitations to what the speaker will play (e.g., Seinfeld baseline upon entry). As a result, the device can be used for a variety of situations in which one may want to communicate with a passersbyer.
  
## Mechanical/Electronic description
The device is split into two parts: the lasers and the detection and speaker system. For the lasers, I use a 9V wall adapter connected through a breadboard to power two generic laser diodes. To prevent the diodes from overheating, I use a small voltage regulator that cuts the power output from the wall adapter down to 5V. The detection part of the system is a bit more interesting. Two photoresistors (LDRs) aligned in series detect the light from the lasers and pass a value corresponding to the light intensity to an Arduino board. A time module keeps track of the current date and time. That is all the input. The MP3 music player module loaded with a micro SD card and connected to a speaker compose the sound system (the output). The module connects to the Arduino through the digital pins. Two 10k Ω resistors ensure that power, coming from a USB cable, flows appropriately to all the connected inputs. 

![Arduino Lazer picture](https://user-images.githubusercontent.com/33380363/56870551-39366380-69df-11e9-9b1a-94f73e4972d0.png)


