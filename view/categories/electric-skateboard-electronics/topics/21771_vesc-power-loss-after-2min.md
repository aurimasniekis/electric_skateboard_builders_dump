# Vesc power loss after 2min

### Replies: 25 Views: 1435

## \#1 Posted by: TheManShaker Posted at: 2017-04-25T20:08:37.687Z Reads: 141

```
Hello,
First my setup:
Motor: 6374 192kv single
VESC: Vedder 4.xx
Battery: 10s4p Diy 20A/cell
Wheel: 83mm
Gears: 12/36

I finished my build 1 month ago, but the skate has lost power immidiatly after starting. I saw that the vesc is hovering always around 105-107 degrees (BLDC tool) so i turned it up to max 120C°, lowered battery max to 20A and put some heatsinks on. Still same problem after first 20meters. Now i changed the gear to 12/36 but it still only lasts to 30-50m untill it looses power and after 100m it had no power at all.
What can I do?
Motor max is 40
Voltage cutoff is ok at 57_34_32
Motor detection and test was ok too.
```

---
## \#2 Posted by: TheManShaker Posted at: 2017-04-25T20:14:46.322Z Reads: 132

```
I am around 100kg and I tested on flat ground.
I am pretty sure the vesc is overheating, but that should not be with this gearing.
The Motor never got hot by touch and neighter the Vesc.
Also i never shorted the motor wires.
```

---
## \#3 Posted by: Blasto Posted at: 2017-04-25T20:15:39.706Z Reads: 132

```
[quote="TheManShaker, post:1, topic:21771"]
I saw that the vesc is hovering always around 105-107 degrees (BLDC tool)
[/quote]

This is even before use?
```

---
## \#4 Posted by: Guacamoleface Posted at: 2017-04-25T20:18:23.837Z Reads: 126

```
Where is the vesc from? I heard a while ago about a bad batch of vescs that had the problem with temperature being insanely high eventhough not used.
```

---
## \#5 Posted by: TheManShaker Posted at: 2017-04-25T21:36:32.245Z Reads: 125

```
Vesc is from diyelectricskateboard.
Yes it was from start. I could only use itbwith remote if i set max temp from 100 to 120.
```

---
## \#6 Posted by: Guacamoleface Posted at: 2017-04-25T21:48:04.751Z Reads: 120

```
Ok, Guy I know including one other thread got a bad batch(from what I heard) from there with temperature problems. 
When did u order it ?`

@hannesr Same problem as you had on your Diy Vesc?
```

---
## \#7 Posted by: TheManShaker Posted at: 2017-04-25T22:02:05.860Z Reads: 122

```
I ordered it on the 10/03/17 from the US.
Are this the sames
```

---
## \#8 Posted by: sl33py Posted at: 2017-04-25T23:04:30.917Z Reads: 115

```
Connect it to BLDC tool, run real-time detection and see if you can duplicate the issue?  Then go to terminal and type in "faults" (iirc) - to see what is going on specifically.

GL!
```

---
## \#9 Posted by: evoheyax Posted at: 2017-04-26T00:52:52.674Z Reads: 106

```
In a video which vedder showed a comparison of the VESC v6 and a VESC v4.12, he showed that the v4 VESC can do 27 amps continuous before it will start to rise in temperature uncontrollably. Basically, if your pumping less than 27 amps continuous, the VESC should not being having heat issues. (Knock a few amps off if you don't have good airflow, but also add a few for the heatsink)

Have you modified the firmware?

Another idea, it could be a bad temp sensor. If you have any laser thermometers, I would suggest double checking that the FETs are actually at the temperature that the VESC claims they are. The temp sensor is on the 3rd FET between the FET and UART port.

Either way, I would suggest sending it back to DIY if you can cause it sounds fishy. My (chaka) VESCs sits at around 94-95 degrees Fahrenheit with 20 amps max going through each vesc. When I first turn it on, it sits at around 70-75 degrees (room temperature). I can do 20 con. with heatsinks and no ventilation, without issue. And I run 4 together.
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2017-04-26T01:06:20.195Z Reads: 99

```
@TheManShaker please contact @torqueboards, I'm pretty sure he know about those issue

@evoheyax and @sl33py it has been confirm a few time that DIY got a bad batch of VESC... the problem is most likely to be hardware.

https://www.electric-skateboard.builders/t/vesc-problem-red-flashing-light/19018/60?u=johnnymeduse
```

---
## \#11 Posted by: evoheyax Posted at: 2017-04-26T01:53:51.148Z Reads: 89

```
ahhh, I thought it was likely a temp sensor issue.

Glad to see Torqueboards stepping up, owning the problem, and fixing it! Great Work!
```

---
## \#12 Posted by: Guacamoleface Posted at: 2017-04-26T06:35:40.323Z Reads: 76

```
I think that was about the time span he ordered his aswell, Contact Diyelectric and ask. It most likely seem to be an unlucky batch that causes your problem.
```

---
## \#13 Posted by: TheManShaker Posted at: 2017-04-26T07:10:17.381Z Reads: 75

```
I'll contact them. Thanl you for all the help.
```

---
## \#14 Posted by: TheManShaker Posted at: 2017-05-04T13:05:40.281Z Reads: 66

```
I baught a new Vesc and did set it up. It's working now. It was the Mosfets fault.
```

---
## \#15 Posted by: TheManShaker Posted at: 2017-05-07T17:23:15.963Z Reads: 60

```
Today (the second day i took out the board) my board blocked completly at full speed and sent me flying twice. I checked the remote, but it was still.connected. what can I do? I don't trust the board anymore...
```

---
## \#16 Posted by: Ackmaniac Posted at: 2017-05-07T18:12:11.065Z Reads: 58

```
Sounds like your remote isn't binded correctly.
When the receiver looses connection to the remote then it uses a default pulse width. You can change that default pulse width during the binding process.
First you should test it by watching the ppm signal when you turn the remote off. When this goes way below 50% then it is braking when it looses the connection. To fix this just add the bind cable to the receiver and remove the bind cable again while leaving the throttle in the idle position. Then the receiver knows that it should send this signal when it looses the connection.
```

---
## \#17 Posted by: jmasta Posted at: 2017-05-07T18:26:14.906Z Reads: 58

```
[quote="TheManShaker, post:7, topic:21771, full:true"]
I ordered it on the 10/03/17 from the US.
Are this the sames
[/quote]

Well there's your problem.  Ordering VESCs from the future has been shown to corrupt the hardware.  Something must be broken with the time-traveler. Ask Marty
```

---
## \#18 Posted by: TheManShaker Posted at: 2017-05-07T19:39:59.683Z Reads: 54

```
Damn, i got 88mph mixed up with km/h. Ill try again. Btw, i´m European, so it was 10th March 2017.
```

---
## \#19 Posted by: TheManShaker Posted at: 2017-05-07T19:40:26.973Z Reads: 52

```
I´ll try tomorrow. Thx!
```

---
## \#20 Posted by: TheManShaker Posted at: 2017-05-14T16:12:35.486Z Reads: 45

```
That fixed my Problem. It was binded correctly, but I tightend the screw on the remote and on idle position it sent 59%. Just loosen the screw back to 50%. It‘s crazy fast now!
```

---
## \#21 Posted by: TheManShaker Posted at: 2017-05-18T20:12:04.452Z Reads: 44

```
New mode new problem... The Vesc stopped working after half a day of working. I opened it up and it was extremly hot. there is a chip which gets melting hot. Do you guys know how to fix it?
<img src="/uploads/db1493/original/3X/d/8/d812516608b1284a186229c127d8408fe3227bd8.jpg" width="375" height="500">
<img src="/uploads/db1493/original/3X/4/4/445d901047648641ea4178cbeff755d18261df20.jpg" width="375" height="500">
<img src="/uploads/db1493/original/3X/6/0/601151a00985be607d8a6b62f28289e076a479c5.jpg" width="375" height="500">
```

---
## \#22 Posted by: TheManShaker Posted at: 2018-01-07T18:46:49.824Z Reads: 26

```
I figured it out. It was my error shorting the Reciever to my badly insulateted DIY Battery.
```

---
## \#23 Posted by: FredrikHems Posted at: 2018-01-07T19:27:33.377Z Reads: 26

```
You can set your cuttof lower than that. Most people set them to about 2.7v per cell. There is still quite a bit of power left at 3.2v for Li-ions.
```

---
## \#24 Posted by: TheManShaker Posted at: 2018-01-07T21:17:42.246Z Reads: 24

```
I now have 530Wh which is enough for me to keep the cell at 3.2v. If i am not wrong this helps the lifecycles of the cell.
```

---
## \#25 Posted by: FredrikHems Posted at: 2018-01-07T21:20:37.649Z Reads: 24

```
Alright. But just FYI at 3.2v you still have 700-500 mah left in each cell :wink:
```

---
