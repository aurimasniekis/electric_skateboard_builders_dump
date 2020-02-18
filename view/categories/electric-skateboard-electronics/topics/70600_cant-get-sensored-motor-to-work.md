# Can&rsquo;t get sensored motor to work

### Replies: 27 Views: 943

## \#1 Posted by: silvor11 Posted at: 2018-10-08T21:24:42.776Z Reads: 140

```
Hello community. 

After lots of reading on this forum, I recently build my first esk8 board. I use a hobbyking 6364 245KV sensored motor in combination with a flipsky 4.12 VESC (and battery etc.).The problem is the motor. When I use the motor UNsensored it is running fine. But when I choose sensored in the VESC tool settings, the hall sensors don't get recognized. In BLDC I get the error: "Unknown hall error: 255" and when I use FOC mode I get: "Bad Detection Results Received". I searched similar topics but couldn't find a solution. Things I tried:

-Different combinations of phase wires
-Increasing duty cycle value

Is there anyone who has or had the same problem and knows a solution to this problem or has some insights? I would really appreciate it.
```

---
## \#2 Posted by: Silverline Posted at: 2018-10-08T21:40:13.673Z Reads: 125

```
You need to be sure , that +5v and GND is in the right place, sometimes you need to re-arrange the order of the wires in the jst
```

---
## \#3 Posted by: jasonbhuynh Posted at: 2018-10-08T21:46:24.365Z Reads: 123

```
Is the sensor cable damaged?
```

---
## \#4 Posted by: silvor11 Posted at: 2018-10-08T21:47:26.179Z Reads: 115

```
Okay, but how do I know the layout of the hall sensors from the motor? And the layout of the flipsky vesc?
```

---
## \#5 Posted by: silvor11 Posted at: 2018-10-08T21:48:07.245Z Reads: 111

```
[quote="jasonbhuynh, post:3, topic:70600, full:true"]
Is the sensor cable damaged?
[/quote]

No, cable is not damaged
```

---
## \#6 Posted by: jasonbhuynh Posted at: 2018-10-08T21:50:09.833Z Reads: 110

```
the flipsky 4.12 should be a clone of the original VESC hardware, if it's not labeled on the vesc then look up the pinout for vesc 4.12, it should be the same as all of the others. The hall sensor +5v should be red and the GND should be black, if the cables are switched in the connector then move them to the right place
```

---
## \#7 Posted by: silvor11 Posted at: 2018-10-08T22:05:48.053Z Reads: 106

```
[quote="jasonbhuynh, post:6, topic:70600, full:true"]
the flipsky 4.12 should be a clone of the original VESC hardware, if it’s not labeled on the vesc then look up the pinout for vesc 4.12, it should be the same as all of the others. The hall sensor +5v should be red and the GND should be black, if the cables are switched in the connector then move them to the right place
[/quote]

I checked. The 5v is indeed red and GND black. They are in the right place.
```

---
## \#8 Posted by: jasonbhuynh Posted at: 2018-10-08T22:18:21.080Z Reads: 95

```
Did you remove the belt before performing detection? afaik you shouldn't have any load on the motor when doing motor or sensor detection. 

Other than this, I can't think of why it would fail except for a faulty sensor/cable
```

---
## \#9 Posted by: silvor11 Posted at: 2018-10-08T22:27:03.932Z Reads: 93

```
[quote="jasonbhuynh, post:8, topic:70600, full:true"]
Did you remove the belt before performing detection? afaik you shouldn’t have any load on the motor when doing motor or sensor detection.

Other than this, I can’t think of why it would fail except for a faulty sensor/cable
[/quote]

I removed the belt. I only left the small 16 teeth pulley on. Don't think that could be the problem but I can always try to take it off and give it a go.
```

---
## \#10 Posted by: mynamesmatt Posted at: 2018-10-08T23:06:10.266Z Reads: 87

```
is it an sk3 or sk8
```

---
## \#11 Posted by: briman05 Posted at: 2018-10-09T00:59:50.210Z Reads: 87

```
Only the sk8 is sensored. The wire colors may be different because different factory may have different wire

![Capture|690x445](upload://ncItWMvKlbxiTwVgFC8Xdg53xg2.PNG) https://www.electric-skateboard.builders/uploads/db1493/original/3X/a/2/a2a205e7c0abb613a56b20ac950bc367af6d685e.PNG

That is the pin out on the vesc
```

---
## \#12 Posted by: mynamesmatt Posted at: 2018-10-09T01:03:04.239Z Reads: 83

```
ignore me i was half asleep
```

---
## \#13 Posted by: silvor11 Posted at: 2018-10-09T10:02:39.195Z Reads: 79

```
[quote="mynamesmatt, post:10, topic:70600, full:true"]
is it an sk3 or sk8
[/quote]

It is a sk8. This one: https://hobbyking.com/en_us/turnigy-sk8-6364-245kv-sensored-brushless-motor-14p.html. 

Does somebody know of they have a different wiring scheme? Or  has other ideas. Much appreciated.
```

---
## \#14 Posted by: silvor11 Posted at: 2018-10-09T10:09:54.997Z Reads: 77

```
![Hall%20sensor%20wires|666x499](upload://ry3AnffSgOTpDxGvl7jBGvfPuAR.jpeg) ![12|666x499](upload://4ATdLn3DUUZ4kRWLiNvfadJiJAZ.jpeg) 

I made a photo. The wire colors are right. Possible that they switch them?
```

---
## \#15 Posted by: briman05 Posted at: 2018-10-09T11:37:46.197Z Reads: 69

```
I would say not.  Does the motor detection work but not the sensor detection? Are you running bldc or foc. If bldc try doing foc that is what I had to do for my racerstar motors.
```

---
## \#16 Posted by: silvor11 Posted at: 2018-10-09T11:47:15.390Z Reads: 68

```
I had contact with hobbyking and they confirmed that the wires are in the right order. I have tried BLCD and FOC. BLDC gives hall error: 255. The first 5 sec of the detection in FOC mode is working, the motor spins a little, however, after those 5 sec it stops working and I get also an error in FOC mode.
```

---
## \#17 Posted by: briman05 Posted at: 2018-10-09T11:57:31.407Z Reads: 66

```
What is the error. Go to the terminal and type fault and see if anything comes up
```

---
## \#18 Posted by: silvor11 Posted at: 2018-10-09T12:19:45.945Z Reads: 63

```
When I type in fault, nothing comes up. No errors.
```

---
## \#19 Posted by: Andy87 Posted at: 2018-10-09T12:24:26.545Z Reads: 64

```
it´s a stupid question but just to be 100% sure.
You pluged the sensors in the Nr1 port, not Nr4, right?
do you have a other esc laying around to check if it´s issue with the motor or the esc?
If no, maybe a friend can help you out?
```

---
## \#20 Posted by: silvor11 Posted at: 2018-10-09T14:33:28.678Z Reads: 64

```
[quote="Andy87, post:19, topic:70600"]
ensors in the Nr1 port, not Nr4, right?
do you have a other esc laying around to che
[/quote]

Thank you for your reaction. I plugged it in the right port. Unfortenately I don't have another esc or another motor laying around to check. This is my problem in FOC mode while detecting: https://www.youtube.com/watch?v=-ju8t0SaPXI

Vesc shuts down and error on the bottom right side saying: bad detection result received
```

---
## \#21 Posted by: Andy87 Posted at: 2018-10-09T17:00:13.885Z Reads: 53

```
Can you flash the firmware new?
I think everything else you already tried.
```

---
## \#22 Posted by: silvor11 Posted at: 2018-10-09T21:27:21.683Z Reads: 52

```
I have already firmware 3.40 according to the Vesc-tool. Should I maybe downgrade and use old BLDC tool? Is that possible?
```

---
## \#23 Posted by: silvor11 Posted at: 2018-10-09T22:04:15.520Z Reads: 52

```
This is a photo of results after BLDC detection:

 ![BLDC%20detection%20results|666x499](upload://sNll0WWUqXEngbWW3Q95AoHQnQI.jpeg) 

Could a bad soldered phase wire have influence on this? Sensorless it's working with those same soldered connections.
```

---
## \#24 Posted by: CarlCollins Posted at: 2018-10-09T22:28:19.979Z Reads: 49

```
@silvor11
Can you double check the following?
Make sure all of your sensor wire's are not broken, sometimes those tiny wires broke within the insulation.
Use a multimeter to check it.
You can use a 1s battery connected to the system and a multimeter.
When you rotate the motor by your hand every wire should have to give 0V-5V value 

Also try increasing the detection current a little bit in VESC tool.
Because your sensor values looks fine
```

---
## \#25 Posted by: Andy87 Posted at: 2018-10-10T09:11:11.169Z Reads: 42

```
I mean just flash it once again with the same firmware you already have on it.
```

---
## \#26 Posted by: dareno Posted at: 2018-10-10T10:27:44.418Z Reads: 41

```
That sk8 motor has a bad sensor on the pcb or a fault in the wiring.   Happened to me on a 192 kv.  Unplug the sensor wire and use it unsensored.  Get in touch with HK and get a replacement.
```

---
## \#27 Posted by: silvor11 Posted at: 2018-10-13T14:03:57.236Z Reads: 34

```
I want to thank you all for the input. I contacted Hobbyking and will send the motor back. They will check if the hall sensors work correctly.
```

---
