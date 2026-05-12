## 1/25/2026 Project Start
-Created a public GitHub Repository

## 1/27/26 Project Definiton 
-Wrote the project definition 
-Started creating block diagrams and the parts needed 
-looking into parts needed to make it work in its environment  

## 2/1/26 Finish block diagram
-looking for sensors that will get here fast and are cheap

##Componet selection 2/2/26
-For our proof of concept, we decided to use an arduino one kit with a sensor that can mimic the functionality that we want since we have it available. This will allow a fast prototype. 


## 2/2/26 Component selection.
- battery  18650 li ion battery popular use and small
-2 pushbuttons for input
-esp32-S3-N16 microcontroller: reason: cheap and functional
-A PIR sensor for more accurately detecting a person
fairly cheap SR602

## 2/12/26 prototype plan 
Using the Arduino kit to make the POC prototype since we have it available. don’t have to wait for the new ESP32


## 2/19/26 startKicad
-Bringing the block diagram into Kicad to start schematics. 

## 2/25/26 New components 
-MLX90640 for the detection, the iFR camera can detect humans better
-USB to USART to program the ESP32-S3
-Had to change the LED driver, which wasn't powerful enough. CN5711 is being used
## 3/7/26 Power SChematic
-working on the power for the schematic, this is a battery usbc for Chagrin
-A MOSFET and a Schottky diode so that we can use it while it's charging. (Found a project that had the schematics for this)
##3 /21/26 Programing schematic
-Worked on the USB-USBART(This part wanst necessary but I was working on it so i left it the 6 pin header would have been better may remove)
-Also worked on the ESP32 and the MLX90640 sensor 
-Learned the LED drivers can't be connected to the GPIO pins, need to redo led schematic. 

## 3/28/26 PCB Layout
-Start working the PCB layout(Some footprint were not working since i worked from a laptop to the PC some are not being found have to download them again and add them)

## 4/10/26 Reveiws
-Ran DRC for PCB review, a lot of errors with the ESP-32 pads and thermal vias in the center
-Changed properties of the vias and connected them to gnd, but this doesn't save every time I run DRC review; it erases, and I have to add them to the gnd net. 

## 4/17/26
-double-checking components, I realized I installed the wrong footprint for the LED, and had to fix that.

## 4/18/26
-Had reviews with other group members so they can take a look and do a revision of both PCB and schematic. 

## 4/30/26
Group review feedback LEDs for charging statues were added.
Start working on the presentation and compiling everything for the report.
 
## Lessons learned
-Don't use GPIO pins to drive LED drivers. 
-Double-check what footprints you are installing. 
-Using Outlook Cloud to work from different computers can lead to problems with the files.
-Sometimes simpler is better. 
-Double-check polarity on diodes when wiring. 
