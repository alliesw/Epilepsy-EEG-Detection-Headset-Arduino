# Wireless-EEG-Headset
IOT based wireless EEG transmission system 

Biomedical Field: Measuring brain activity for Epilepsy - EEG 
Description: System accurately measure brain activity and provides detailed readings of your brainwaves, heart rate, attention, pressure level

< Project 1: Hack a MindFlex EEG Headset using Arduino >
< Updated for 4.0.1 Processing > 

Hardware Components:
1. Mindflex EEG headset (must have a nerosky brand control board inside to run code)
2: Arduino (with the Arduino Brain Library installed and running)
3: Usb cable
4: A computer
5: Screwdriver, multimeter, wire-snips
6: Soldering iron

Hardware Steps:
1. Remove headset battery > Unscrew the four screws on the left side of the headset > open it up
2. Find the smaller circuit board [6 pins sticking out with denoted label "NeuroSky"] > solder a wire to the pin that is labeled T 
> solder a wire to the pin on the bigger board [has a black wire connecting to it].
3. Hook up the wire soldered to the T pin to the RX pin on the Arduino > hook up the pin soldered to the black wire to GND on the Arduino
4. Screw the headset back together > zip tie the Arduino to the mindflex headset > put batteries back in headset.

Since you're using this with a hacked MindFlex, you'll need the Arduino Brain Library installed and running on your Arduino. 

Software Steps: 
1. Download the Arduino Brain library (ZIP file):
2. Open the Arduino IDE and click to the "Sketch" menu and then Include Library > Manage Libraries.
Scroll through the list of libraries > select the Brain library ZIP you downloaded > install lib 


Disconnect the RX pin wire > upload the brain serial out example code > run code while 
the Arduino is connected to your computer > plug the RX pin back in > turn on the headset.

Open the serial monitor > get csv data from the headset

Download processing 4.0.1 code here: 

https://processing.org/download/ 

Download the main brain grapher code here:

https://github.com/kitschpatrol/BrainGrapher/blob/master/BrainGrapher/BrainGrapher.pde