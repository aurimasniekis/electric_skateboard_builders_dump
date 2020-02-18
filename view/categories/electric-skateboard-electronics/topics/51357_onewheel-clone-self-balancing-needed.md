# Onewheel clone. Self-balancing needed

### Replies: 11 Views: 2077

## \#1 Posted by: CCU Posted at: 2018-04-05T23:25:41.214Z Reads: 205

```
Hi everybody 

Do you know of anyone who has successfully created a Onewheel like board with a build guide? 
I am really curious about that type of board and since the self-balancing part of the board is the only thing i´m missing, it would be really cheap to just try it out. 

Best regards Casper
```

---
## \#2 Posted by: evoheyax Posted at: 2018-04-05T23:53:41.166Z Reads: 200

```
Not that hard to do, just will take a lot of tweaking. Get an arduino, a 3axis gyroscope, and a weight sensor and wire I into a vesc through the uart port and boom!
```

---
## \#3 Posted by: b264 Posted at: 2018-04-06T00:39:19.493Z Reads: 193

```
Yep, a little C code, and some falling on your face, and you can build it.  The hard part will be dismounting.  How does it know when to balance and when to not balance?
```

---
## \#4 Posted by: pennyboard Posted at: 2018-04-06T00:53:38.665Z Reads: 181

```
Do you have experience with dynamic controls systems? Easiest way to create a controller for a one wheel is to have something like an arduino or a teensy run the ESC (i.e. output PWN signal from the arduino to the ESC in order to control the motor), then have the gyro and any other sensors feed data to the ESC and find the transfer function of the system and then use a program like Matlab to design a closed loop controller for the system that will be run on the arduino (which is programmed in arduino language which is basically C++).
```

---
## \#5 Posted by: Bor.inc Posted at: 2018-04-06T05:44:25.365Z Reads: 137

```
A person on the internet called 'xenonjohn' has done things with onewheel (and is just the balanching god of diy electric vehicles)

this person has a helpful blog about it: http://transistor-man.com/flying_nimbus.html
```

---
## \#6 Posted by: CCU Posted at: 2018-04-06T08:19:01.257Z Reads: 127

```
I was actually worried that the Arduino wouldn´t have enough power to calculate the self-balancing algorithm constantly. 
So it would be nice to see someone else doing it that way. Also it would be my first Arduino project, so it would be nice to know it could be done that way before i buy the parts and rip my hair out trying to find out why it wouldn´t work.
```

---
## \#7 Posted by: CCU Posted at: 2018-04-06T08:24:47.349Z Reads: 122

```
That is also one of the reasons i want to see what someone else has done. Maybe someone found a great way of programming it
```

---
## \#8 Posted by: CCU Posted at: 2018-04-06T08:37:34.081Z Reads: 126

```
I have experience with PLC systems, Matlab simulations and other similar things. 
But it would be my first time implementing it on something like an Arduino.

I figured I would use a PPM signal from the Arduino and replace the input signal from the remote receiver.
And let it Arduino look after the pressure pads
```

---
## \#9 Posted by: CCU Posted at: 2018-04-06T08:39:29.867Z Reads: 118

```
Thank you so much! Bin trawling all over google for something like this without any luck
```

---
## \#10 Posted by: evoheyax Posted at: 2018-04-06T15:46:35.030Z Reads: 106

```
I've just recently starting messing with arduinos. The mega is what you would want for this project, more power, more space, and more tx/rx's for multiple speed controllers if needed.

Certain ports can receive the pwm signal. It'll give number between 1000-2000 with 1500 being nothing, 1000 being brake, and 2000 full throttle. It's as simple as an if else statement, and just one wire, the white wire, to the arduino. And just one command to get the data.
```

---
## \#11 Posted by: m303625 Posted at: 2018-12-10T23:30:45.883Z Reads: 61

```
refer to this thread, lastest is to use cheap flight controller because it has all the necessary hardware inc 32bit processor and an off the shelf Vesc etc.
https://www.electric-skateboard.builders/t/onewheel-skateboard/15901/76
```

---
