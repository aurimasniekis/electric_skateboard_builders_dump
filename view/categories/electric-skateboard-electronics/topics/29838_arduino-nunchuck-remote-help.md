# Arduino/Nunchuck Remote Help

### Replies: 9 Views: 995

## \#1 Posted by: bcarr Posted at: 2017-08-06T02:57:18.577Z Reads: 76

```
Hi Everyone, I'm in the final stages of my electric longboard build after working on and off for the past year. My parts list is as follows:

4x - 3s 5000mAh Lipo battery wired in series for a total of 12s
RotorStar 120A HV (4~14S) ESC [Link](https://hobbyking.com/en_us/rotorstar-120a-hv-4-14s-brushless-speed-controller-opto.html)
Turnigy Aerodrive SK3 149kv Brushless Outrunner Motor [Link](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-149kv-brushless-outrunner-motor.html)

For the remote I have an Arduino Pro Mini 3.3v sending a PWM signal to the ESC. With some brief test code I can run the motor and change speeds from a potentiometer in my test setup. However, this is while having the Arduino powered from a USB cable to an FTDI breakout board responsible for programming the Arduino. In my final setup I want to power the Arduino from a 3s lipo battery and a 3.3v regulator separate from the batteries running the motor. When I wire this configuration, the motor will not arm or make any noises, indicating that it is receiving the PWM signal from the Arduino. Trying to diagnose the problem, I have tried many different power sources including 9v battery, 18650 cells, and the balancing leads from the batteries powering the motor(all of these tested to the RAW pin on the arduino and additionally to the 3.3v regulator and the vcc pin) and none of these will run the motor. The only configuration I can get the motor to run is from a USB port(either from computer, iPhone charging brick, or power bank) to the FTDI breakout board and then finally to the Arduino. 

I have tried everything I can think of to fix this issue but I can't figure it out. Any advice would be greatly appreciated!


My second issue arrises when I try to use the Nyko Kama wireless wii nunchuck to control the board. The control is now very unreliable, only sometimes arming the motor and controlling it, other times nothing will happen at all and I will have to restart everything. Also, when it does work the acceleration is very jerky and it seems the motor will get choked up sometimes. Has anyone had success using the Nyko Kama to control their board? If so what nunchuck library were you using and what did your setup look like.


Thanks for reading this! I could use any help I can get. I'm trying to get this board up and running in the next 3 weeks so I can use it to get around at college.
```

---
## \#2 Posted by: bmcm Posted at: 2017-08-07T18:17:08.187Z Reads: 55

```
Sounds like the 3v regulator is the variable that hasn't been tested, and so therefore, might be the culprit? Have you tried another type of regulator? Bench power supply? Voltage divider using resistors?
```

---
## \#3 Posted by: Der6FingerJo Posted at: 2017-08-07T19:16:19.030Z Reads: 49

```
The simplest thing that comes to my mind is a proper ground connection between arduino and ESC. Sorry if that is too obvious but i sometimes forget this too.
```

---
## \#4 Posted by: bcarr Posted at: 2017-08-07T19:25:44.628Z Reads: 49

```
How would I go about establishing a proper ground connection? Currently I have the brown wire from the ESC connected to a ground pin on the Arduino and the orange signal wire connected to the PWM pin. The red wire from the ESC is left unused.
```

---
## \#5 Posted by: bcarr Posted at: 2017-08-07T19:30:29.523Z Reads: 43

```
The RAW pin on the Arduino can accept up to 12 volts so I have already tried without the 3v regulator. The only reason why I would like to use an external regulator is because I have fried a few Arduino's powering from the RAW pin before. I currently don't have access to a bench power supply so that isn't an option. How would I go about setting up the voltage divider using resistors?
```

---
## \#6 Posted by: Der6FingerJo Posted at: 2017-08-07T19:50:00.663Z Reads: 37

```
Ok i meant hat. Do you have any access to oscilloscopes to see what the arduino does? 
maybe a long shot, but you could measure the outputs of the esc (from the signal wire and +5V and ground), i once had a esc with reversed wires.
```

---
## \#7 Posted by: bmcm Posted at: 2017-08-07T20:29:35.840Z Reads: 35

```
So did you plug in the 3S (11.1V nominal) battery into the arduino 12V input without anything in between (regulator/resistor), and the arduino still didn't boot up? 

If you need a voltage divider (which may not be a solution to your problem), this site is useful: http://www.ohmslawcalculator.com/voltage-divider-calculator
```

---
## \#8 Posted by: bmcm Posted at: 2017-08-07T20:41:13.242Z Reads: 34

```
Can you post a photo of your wiring setup? It may be just something stupid simple that's wrong (or the opposite).
```

---
## \#9 Posted by: bcarr Posted at: 2017-08-10T03:18:14.605Z Reads: 35

```
This is a diagram of the wiring setup that WILL work. 

<img src="/uploads/db1493/original/3X/7/f/7f1dfadec431c490e2c8faa54443156f47b666d3.jpg" width="500" height="500">

While running this code.

    #include <SoftwareServo.h>

    int sensorPin = A0;
    int sensorValue = 0;
    SoftwareServo esc;

    void setup() {
      esc.attach(10);
      esc.setMinimumPulse(800);
      esc.setMaximumPulse(2000);
    }

    void loop() {
      sensorValue = analogRead(sensorPin);
      sensorValue = map(sensorValue, 0, 1023, 0, 180);
      SoftwareServo::refresh();
      esc.write(sensorValue);
    }

When I try to replace the FTDI board and USB with any different power source this setup no longer works.
```

---
