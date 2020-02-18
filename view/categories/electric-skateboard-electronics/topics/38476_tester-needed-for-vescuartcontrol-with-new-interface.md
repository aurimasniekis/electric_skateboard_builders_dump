# Tester needed for VescUartControl with new Interface

### Replies: 31 Views: 2358

## \#1 Posted by: RollingGecko Posted at: 2017-11-16T02:35:47.789Z Reads: 279

```
Hi,,

The Interface on the Vesc changed with the new firmware. I already adapted the necessary changes and merged also some change requests. But: I have currently no VESC to test this stuff. So I was wondering if somebody is out there using the VescUartControl and wants to test the changes for the community so I can merge the stuff in the master and bring out a new release. The changed interface was already tested and also the pull requests. But not all stuff together.

You can find the newest version in this branch: https://github.com/RollingGecko/VescUartControl/commits/VESC6
I opened also an issue for this help request:https://github.com/RollingGecko/VescUartControl/issues/15

Would be great if you could participate.

Andy
```

---
## \#2 Posted by: Der6FingerJo Posted at: 2017-11-16T12:28:06.658Z Reads: 254

```
Just to get this clear, would it also help to test it with 4.12 Hardware and new Firmware? I think i should be able to test it tomorrow, but it will be while until i get some VESC 6's.
```

---
## \#3 Posted by: RollingGecko Posted at: 2017-11-17T02:59:55.653Z Reads: 230

```
It is only about the new firmware. So 4.12 would be fine!
```

---
## \#4 Posted by: Eboosted Posted at: 2017-11-17T06:19:48.279Z Reads: 208

```
I have 4.12 hardware runing and latest firmware from the latest VESC tool.

I'm your man! (no gay comment implied)
```

---
## \#5 Posted by: Der6FingerJo Posted at: 2017-11-17T13:51:59.579Z Reads: 193

```
Alright i will do some testing as soon as i get the chance (still away from home...)
Can't wait to use the library again for my next remote and board!
```

---
## \#6 Posted by: RollingGecko Posted at: 2017-11-17T14:17:11.521Z Reads: 183

```
Waiting for your test results guys!
```

---
## \#7 Posted by: Vanarian Posted at: 2017-11-17T17:59:37.170Z Reads: 170

```
I'm guinea pig I'll do it too! ... when I successfully reinstall my arduino on computer ! Damn installation is gruesome !
```

---
## \#8 Posted by: niktwo17 Posted at: 2017-11-25T14:05:40.672Z Reads: 152

```
I gave it a try today but i can neither get my esk8.de vesc or 1.1 controller (both running 3.28fw) to work with the new code.
Old version still works for controlling the motor besides theres no telemetry.
```

---
## \#9 Posted by: RollingGecko Posted at: 2017-11-26T03:52:49.532Z Reads: 150

```
True,true. ArduBoardControl was not yet adapted to the changes in the library. Added now SetSerialPort also to ArduBoardControl. Now it should work...I hope. 

Please give it another try. You will find the changes in this branch: https://github.com/RollingGecko/ArduBoardControler/tree/V6

Chears 

Andy
```

---
## \#10 Posted by: niktwo17 Posted at: 2017-11-26T17:29:17.505Z Reads: 138

```
Thanks. ill give it a try tomorrow. But im not sure this will change anything as im just using your library and created my own rx&tx code. I did already add the changes from your initional post to my library.
Maybe I messed up when I merged the codes together as i had to remove the multiple serial ports part (using an arduino nano)
```

---
## \#11 Posted by: RollingGecko Posted at: 2017-11-26T23:19:57.508Z Reads: 131

```
Guys it makes no sense to test a library that you changed. The test is not representative at all.

The code is backwards compatible. The functions are overloaded. Once without setting the serial port to use and once without. Like before. The only thing you have to add is a SetSerialPort(&Serial) to your code in the setup part. Then normal a Serial.begin(xxx). Same with SetDebugSerialPort if required.
```

---
## \#12 Posted by: niktwo17 Posted at: 2017-11-29T19:45:17.619Z Reads: 125

```
ok maybe i wasnt clear enough. i updated the library based on your instructions at first place but didnt manage to establish a connection to the vesc at all. then i tried to make it work but no success so far.
```

---
## \#13 Posted by: Der6FingerJo Posted at: 2017-12-02T15:34:29.217Z Reads: 128

```
i FINALLY had the chance to test it!
and look at that:
<img src="/uploads/db1493/original/3X/4/5/4524c2068d4b4cc0bd70fb88a71809fbc6099cff.png" width="492" height="500">
It works!

Tested with 4.12HW 3.34 FW VESC

Thanks @RollingGecko, you make my projects possible! :heart_eyes: 

(btw does it matter that i didn't try sending stuff to the vesc? didn't have a spare motor to connect to it)
```

---
## \#14 Posted by: niktwo17 Posted at: 2017-12-02T18:53:42.753Z Reads: 116

```
Nice work!
Still doesnt work for me :/ old version with 2.28 firmware is just fine but with the updated version  I can get my Arduino to the VESC
Can you try to connect a Nano? Cause there are 2 Options right now: Code doesnt work with Nano or i messed sth up(more likley :joy:)
```

---
## \#15 Posted by: Der6FingerJo Posted at: 2017-12-02T19:28:07.978Z Reads: 114

```
Have tried only with mega, might find time to test with nano tomorrow. 
My uart settings were standard 115200 baud. 
But next time I want to use nanos for my project, oh well.
```

---
## \#16 Posted by: Der6FingerJo Posted at: 2017-12-03T10:07:43.543Z Reads: 108

```
Alright i gave it a quick try with the Nano. My Method was reading the data via the example sketch and storing the input voltage in EEPROM. Then i read the EEPROM using another Sketch. Unfortunately the Number in the EEPROM stayed 0.00. 
However, this isn't the best way to check this and i can't say that it's impossible that i made a mistake as i did this in a hurry, so it would be great if you could try to test this with something like softwareserial.
```

---
## \#17 Posted by: niktwo17 Posted at: 2017-12-03T11:35:39.741Z Reads: 111

```
Tanks.
Im sending the data to my remote and display it on an oled screen. Same problem, every number stays zero. 
Another weird thing is that it appears that my nano "stops" when it tries to communicate with the VESC.
I will  "borrow" an arduino that supports multiple serial ports from school tomorrow and give it another try.
```

---
## \#18 Posted by: Der6FingerJo Posted at: 2017-12-10T13:01:48.836Z Reads: 105

```
Any updates on the nano? My next remote project really depends on this so i might need to track down a small mega as an alternative.
```

---
## \#19 Posted by: niktwo17 Posted at: 2017-12-10T15:53:25.406Z Reads: 94

```
Unfortunately theres no mega or similar in my school. 
but will get one from a friend by monday. so next week i should be able to try it next week
```

---
## \#20 Posted by: Der6FingerJo Posted at: 2017-12-10T19:51:36.358Z Reads: 94

```
We know that it works on the mega, it would be more interesting to see if you could get it working with the Nano :smile:
```

---
## \#21 Posted by: niktwo17 Posted at: 2017-12-10T21:10:41.324Z Reads: 89

```
exactly but i cant figure out why it doesnt work so far on nano so I first want to make sure that exactly the same code works/doesnt work on mega
starts to get annoying and even students dont have unlimited time :joy:
```

---
## \#22 Posted by: Pedrodemio Posted at: 2017-12-10T21:41:40.106Z Reads: 92

```
I’m almost finishing my board and will try on the nano plus VESC 6 this week or next weekend
```

---
## \#23 Posted by: Der6FingerJo Posted at: 2017-12-11T09:10:01.035Z Reads: 90

```
hah alright i could have guessed as much myself, thanks for your effort :D[quote="Pedrodemio, post:22, topic:38476, full:true"]
I’m almost finishing my board and will try on the nano plus VESC 6 this week or next weekend
[/quote]

That would be great, i wanna use the exact same setup!
```

---
## \#24 Posted by: RollingGecko Posted at: 2017-12-11T11:46:26.990Z Reads: 86

```
Hi,

I tested the example and get telemetry data. But  with the ArduoBoardControl I have the same issues. 
I started reassemble a test hardware again based on a mega, so that I can debug all the stuff. Struggling at the moment to establish the NRF on the mega. Hope that my ship is still OK. 

Keep you updated.

Andy
```

---
## \#25 Posted by: RollingGecko Posted at: 2017-12-15T21:36:09.197Z Reads: 87

```
OK Guys,

Hardware works but now i need a bit of swarm intelligence.
I debuged the send packages on both sides. The VescUartControl works. I get correct telemetry. But when I send the struct VescUartMeasures in the Ack-Message, I does not receive the full message. 

On Rx Site:
avgMotorCurrent:	-0.20
avgInputCurrent:	0.00
avgId:			0.00
avgIq:			0.00
dutyNow:			0.00
rpm:				0
inpVoltage:		23.50
ampHours:		0.00
ampHoursCharged:	0.00
tachometer:		3
tachometerAbs:	3
faultCode:		0

On Tx-Site 

mpFetFiltered:	28.80
tempMotorFiltered:-73.30
avgMotorCurrent:	-0.20
avgInputCurrent:	0.00
avgId:			0.00
avgIq:			0.00
dutyNow:			0.00
rpm:				0
inpVoltage:		23.50
ampHours:		0.00
ampHoursCharged:	0.00
tachometer:		3
tachometerAbs:	3
faultCode:		0


For example inpVoltage is not sended. I have no idea why!

Next problem: The NunChuck control message is send to the vesc. But the motor does not work. Also at the moment no idea. 

I hope somebody can jump in here. Because I have no capacity left for much investigation.

Andy
```

---
## \#26 Posted by: Der6FingerJo Posted at: 2017-12-15T22:57:24.939Z Reads: 85

```
I'm not sure if i understand correctly. The Communication between the VESC and Arduino (Nano?) is fully working, but the data transfer between NRF modules isn't? So you're talking about the ArduBoardControl sketch?
And also the Nunchuck Commands do not work. 

Right now i don't have much time to investigate as well, but after Christmas i have some free time for a while which i will use to make my remote. I'll keep you guys updated if i run into problems and try to fix them. I can also try the ArduBoardControl code as well.
```

---
## \#27 Posted by: Pedrodemio Posted at: 2018-02-09T16:57:46.967Z Reads: 69

```
I'm testing right now

At the moment i confirmed that the NRF communication is working, wasn't sure since it's a new arduino and new NRF with a other stuff connected but not implemented yet, i still haven't managed to talk to the VESC 6

I will try now just send some fixed value and ditch all NRF related stuff from the code

EDIT: i'm also on nano, i was comparing the current commands in the oficial fork with the vesc 6 library branch and the previous versions of the library. Apparently the VESC expect the two joysticks, two buttons and 3 acceleration values, the VESC 6 branch is sending 6 acceleration values, i will try to remove that

EDIT2: It's pretty obvious that the serial communication is not working since the leds in D0 and D1 are off (or very very dim), why is the question


EDIT3: confirmed the serial problem, rolling back to the previous version of the library and works fine (but can't comunnicate with 3.XX since the protocol changed)
```

---
## \#28 Posted by: topazwishes Posted at: 2018-03-02T05:18:48.256Z Reads: 60

```
Is there any way to get the sketch to work on Arduino Uno? I've been trying everything but it still doesn't work!
```

---
## \#29 Posted by: ZackoryCramer Posted at: 2018-03-02T05:36:51.507Z Reads: 55

```
Arduino uno has only one serial port, you will need an Arduino Mega or a supported board with more than one serial port to be able to read the Vesc input and print it over serial on IDE. I used a Bluetooth module which doesn't require a serial port to send data to an app I made and it worked on the Mini. :8ball:
```

---
## \#30 Posted by: Der6FingerJo Posted at: 2018-03-02T08:55:48.086Z Reads: 53

```
It works on pro mini and Nano, so the 1 Port limit shouldn't be the problem. You just have to debug using a software serial port. I recommend the altsoftserial library, it's much more fleshed out than the regular one.
```

---
## \#31 Posted by: Deckoz Posted at: 2018-04-25T18:21:32.622Z Reads: 39

```
I've got this working on a pro-mini, using an HM10(MetR module) only on the vesc. With a standalone pro-mini, and hm05 in slave.

Trying to decide on a screen. Will be using this for telemetry only, and have commented out the controls. I've ordered a handful of SPI oled screens. And going to be working on trying to make a thin glove backpack for Sector 9 leather gloves. 

Think my goal here is to use standard hardware on the board, i.e. normal ppm receiver and Bluetooth module, without any extras on board. No special receivers, basically a standalone system, so you can either connect your phone like normal, or use the glove backpack.

Likely I'll start out with the backpack design, once I have a few screens in hand, so I can pick the screen and make the size of the backpack thin and small. Then start on the display UI after the hardware prototype is done.

Thanks for sharing your updates @RollingGecko
```

---
