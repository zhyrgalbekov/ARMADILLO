# ARMADILLO 
OBSTACLE AVOIDING CAR
## Installation 
The minimum programming knowledge needed to program the operations of our product is as follows:

First of all, you need to download the Arduino and install the driver for your laptop/computer/app in order to master the programming part 
To do this type in your browser Arduino.com and go to the [software section](https://www.arduino.cc/en/software) select the option your notebook requires (e.g. DOWNLOAD OPTIONS: Win 7 and newer, Windows app Win 8.1 or 10, Linux 32 bits, Mac OS X 10.10 or newer). 

[Web-version of Arduino](https://create.arduino.cc/editor/zhyrgalbekovadiz/b121ed27-0e92-4f0a-b8bf-bedd418a29d0):The Arduino Web Editor allows you to write code and upload sketches to any official Arduino board from your web browser (Chrome, Firefox, Safari, and Edge). 
If you prefer to use the web version of the Arduino software, follow the requirements below: To do this type in Arduino.com in your browser and go to the web editor. This is all you need to start writing code in the web editor.
## Library

Before uploading the code you have to install the necessary library.
### [Adafruit Motor library](https://learn.adafruit.com/adafruit-motor-shield/library-install)
### [NewPing Library](https://github.com/livetronic/Arduino-NewPing) 
### [Servo Library](https://github.com/arduino-libraries/Servo.git)
 To Install the libraries go to sketch >> Include Library >> Add .ZIP File >> Select the Downloaded ZIP files From the Above links
 
 To instal them go to sketch >> Include Library >> Manage Labraries..
 
 ## define
.The motor shield can drive up to 4 DC motors bidirectional. That means they can be driven forwards and backwards

'''#define TRIG_PIN A0 // Pin A0 on the Motor Drive Shield soldered to the ultrasonic sensor

'''#define ECHO_PIN A1 // Pin A1 on the Motor Drive Shield soldered to the ultrasonic sensor

'''#define MAX_DISTANCE 300 // sets maximum useable sensor measuring distance to 300cm

The speed ranges from 0(stopped)  to 255 (full speed)/ 

#define MAX_SPEED 160 // sets speed of DC traction motors to 150/250 or about 70% of full speed - to get power drain down.

#define MAX_SPEED_OFFSET 40 // this sets offset to allow for differences between the two DC traction motors

#define COLL_DIST 30 // sets distance at which robot stops and reverses to 30cm

#define TURN_DIST COLL_DIST+20 // sets distance at which robot veers away from object

'''C
NewPing sonar(TRIG_PIN, ECHO_PIN, MAX_DISTANCE); // sets up sensor library to use the correct pins to measure distance.
This initializes NewPing to use pin 12 for trigger output, pin 11 for echo input, with a maximum ping distance of 200cm


