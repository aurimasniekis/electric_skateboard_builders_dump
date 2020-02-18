# All electronics hooked up and motor not spinning?! HELP

### Replies: 29 Views: 2223

## \#1 Posted by: Zorb Posted at: 2016-07-04T21:51:50.859Z Reads: 151

```
Hey Everyone!

Well for quite some time now I've been trying to get my board up and running. When I started the build process it all started quite well in that when I hooked up all of the electronics everything was working. I could control the motor forwards and use cruise control but I couldn't reverse. This was because the programming card for the ESC was broken, after some time torqueboards gave me the PC firmware for the ESC. I was able to then get the programming card to work and then I connected it to the ESC and programmed the commands. After I did this I could not control the motor. I've messed around with all parts but cannot find a solution. 

The parts which I am using:
-TorqueBoards 120A 6S ESC 
-Wiiceiver
-Wireless Nyko nunchuck
-Turnigy Aerodrive SK3 - 5055-280kv Brushless Outrunner Motor
-2 Zippy 3S 5000mah batteries in series

What happens when I turn it on is that the motor does the beep sequence. Then when I pair the nyko remote nothing happens there is no motor movement whatsoever. The nyko is transmitting the signal because the light on the receiver does flash when I press the button. 

In order to test if the motor was the problem I connected another brushless motor from a drone and it reacted the same way with the beeping sequence. Then I tried a wired wii nunchuck and the result was the same. I also tested the nyko on a wii and it worked properly. I took apart the ESC to see if there were any problems on the inside and there seemed to be none. Needless to say when I put it back together the same problem still continued. I tried to reflash the ESC with the programming board and directly with a PC. Note when I turn on the ESC with the motor connected and the wiiceiver disconnected the motor makes no beeps, so the wiiceiver is sending some sort of signal. After trying all of this the same problem continued. I also tried to calibrate the throttle of the wiiceiver controller but it did not work as I could not even complete the calibration process.

Overall I believe that the problem is most likely the ESC but could also be the wiiceiver. I tried everything which I could and now I have no idea on how to get this up and running. I am willing to try anything but do not want to spend more money on this project until I can see that it is actually running. Any help is greatly appreciated.If you have any suggestions or questions in further diagnosis the problem please feel free to mention below as I am trying to build this ASAP and will try to answer immediately. 

https://youtu.be/_piZ08YXxyo

Thanks in advance :D
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-07-04T22:25:51.126Z Reads: 124

```
Well #1 you shouldn't  try to test the motor unmounted ....that's asking for trouble

Is prob the wiiceiver....imo they suck....and you should solder the connection to the wiiceiver..........

If you have a different tx/rx you can check....but 99% it's the wiiceiver...they can be touchy
```

---
## \#3 Posted by: Zorb Posted at: 2016-07-04T23:10:56.935Z Reads: 115

```
Unfortunately I don't have another tx/rx to test it. Any way I can test if the wiiceiver is working, or if I can use an arduino uni and test it like that. 

I don't wanna spend more money on this if I don't know it's gonna work.
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2016-07-04T23:18:59.940Z Reads: 109

```
Well let's see .... If ur wiiceiver is jacked...you need to buy another...of ur esc is jacked ....u need to buy another .....

Like I said 99% it's that dumb wiiceiver lol
```

---
## \#5 Posted by: treenutter Posted at: 2016-07-04T23:39:23.210Z Reads: 98

```
[quote="Zorb, post:1, topic:5569"]
that the motor does the beep sequence
[/quote]

I think it's your ESC that beeps, right? How are you connecting the motor wires to the ESC? Are they bullet connectors? They are taped up so we can't tell. 

I don't have a wiiciever so I don't know what the light sequences mean, but it seems to be connecting to the nunchuck. Are you sure you're plugged into the right port on the esc, and in the correct position?
```

---
## \#6 Posted by: Zorb Posted at: 2016-07-04T23:57:10.317Z Reads: 92

```
Yeah I think the beep comes from the ESC, might be the motor but I don't think that's even possible. Also when the beeps happen the motor moves a little bit.

They are bullet connectors but the ESC and motor ones are different so they are connected with some wire inside. I'm 99% sure that they are connected.

I tired connecting the wires to the wiiceiver in all the possible ways and nothing changes. That's how they are connected on the  site.
```

---
## \#7 Posted by: Zorb Posted at: 2016-07-04T23:57:38.873Z Reads: 87

```
Any way to know if the ESC is the problem?
```

---
## \#8 Posted by: Stevemk14ebr Posted at: 2016-07-05T00:10:54.975Z Reads: 90

```
Those esc's beep when either the signal wire is not working or the batteries are jacked up. It's probably the remote. Get an arduino and read the values coming from the receiver using the pulseIn command on arduino. If they vary when you push the trigger forward and backward then your receiver is working, if they don't then it is broken. You can also wire an arduino to your esc and control it as a servo to see if it is broken.
```

---
## \#9 Posted by: treenutter Posted at: 2016-07-05T00:14:55.910Z Reads: 86

```
[quote="Zorb, post:6, topic:5569"]
They are bullet connectors but the ESC and motor ones are different so they are connected with some wire inside. I'm 99% sure that they are connected.
[/quote]

Can you please explain this further? Maybe a pic of the connections? Did you solder the wires together by removing the bullet connectors? This sounds like a problem.
```

---
## \#10 Posted by: Zorb Posted at: 2016-07-05T00:40:15.657Z Reads: 82

```
Do you know where I need to plug in the wires on the arduino and wiiceiver?
```

---
## \#11 Posted by: Michaelinvegas Posted at: 2016-07-05T00:42:00.064Z Reads: 80

```
Honestly it would be the 1% chance that the esc is the problem.....

If you don't have another rx/tx to use I place of the wiiceiver (which would help figure out where the issue is) then I would follow the others steps
```

---
## \#12 Posted by: Michaelinvegas Posted at: 2016-07-05T00:44:26.698Z Reads: 76

```
Did you try the second set of pins? I had one that was able to control two ESCs ... But only one set of pins worked...weird
```

---
## \#13 Posted by: Stevemk14ebr Posted at: 2016-07-05T01:00:14.249Z Reads: 76

```
It's super easy just plug the sensor pin into a pwm capable pin on the arudiuno then do pulsein() on that pin. http://www.instructables.com/id/Using-FM-RC-Controllers-with-Arduino/step2/Connecting-it-all/

Rough guess (yours may be different):
black wire = ground
red = 5v power
yellow = sensor pin *this goes to the arduino*
```

---
## \#14 Posted by: psychotiller Posted at: 2016-07-05T01:11:21.574Z Reads: 73

```
You need to properly connect your motor wires. Solder the right male/famale connectors in place. Loose connections cause all kinds of problems. Most of which you are listing here.
```

---
## \#15 Posted by: Michaelinvegas Posted at: 2016-07-05T02:56:56.837Z Reads: 68

```
Where's @lowGuido when you need him.....
```

---
## \#16 Posted by: JLabs Posted at: 2016-07-05T03:15:29.756Z Reads: 67

```
Ok so you purchased the wiiceiver so I don't think it's the problem. I have had a problem with the FVT esc's. My $100 bet is that the wire is shorted or cracked' inside the esc. I have had this problem before. I had to take the esc apart, snap off the bottom plate, and desolder the wiiceiver/switch wires, then resolder some new thickes wires back on. Before putting it back together I made the hole a bit bigger with a 3d print modifier, but you could use a dremel.  Hope this helps, it worked for me, I can post some pics tomorrow if u need.
```

---
## \#17 Posted by: lowGuido Posted at: 2016-07-05T05:31:06.968Z Reads: 64

```
It looks like a problem with the wiiceiver.  You move the camera around too much in the video so I any see what the lighrs are doing.  But it looks like they go out at one stage. That shouldn't happen.
```

---
## \#18 Posted by: Zorb Posted at: 2016-07-05T17:46:58.378Z Reads: 55

```
Is it these cables, on my board they seem to be soldered.

 <img src="/uploads/db1493/original/2X/5/5fc6cbb0421e8bbcb91d06bd4770b7d644d4ef43.jpg" width="655" height="500">
```

---
## \#19 Posted by: Stevemk14ebr Posted at: 2016-07-05T18:02:52.504Z Reads: 52

```
No. You want the cable that plugs into the prongs on the rc receiver that go to the esc, might be different on the nunchuck thing you have. If you dont know electronics just buy a new receiver and test it out on your board, they are really cheap.
```

---
## \#20 Posted by: JLabs Posted at: 2016-07-05T18:09:44.461Z Reads: 49

```
There is a puncture in the black cable. Desolder the wires and just replace them. They are junk and just hardware then to Wii board with no connector.
<img src="/uploads/db1493/original/2X/1/1aedbb2c50c0daf809541fad7fa5ef8e6bdab49d.jpg" width="282" height="500">
<img src="/uploads/db1493/original/2X/0/080726b4cb6749e15bb41bc9b3242fb8f430a43d.jpg" width="282" height="500">
```

---
## \#21 Posted by: JLabs Posted at: 2016-07-05T18:22:05.814Z Reads: 47

```
If you replace the wires and cut a bigger hole like I did I can almost guarantee that it will work. I hope this helps
```

---
## \#23 Posted by: Zorb Posted at: 2016-07-05T18:34:50.462Z Reads: 44

```
So just to make sure it is the cables that are in the pic above that go to the wiiceiver?
```

---
## \#24 Posted by: JLabs Posted at: 2016-07-05T20:12:52.124Z Reads: 45

```
Yes the 3 cables that u took a picture of (not the switch wires). They go to the wiiceiver. Just replace them with some small wire, thicker than what is there now
```

---
## \#25 Posted by: Zorb Posted at: 2016-07-05T23:07:22.629Z Reads: 44

```
Soldered the new cables and  nothing has changed. Any other ideas?

<img src="/uploads/db1493/original/2X/d/d499502638d9845b9ff46ae67f493d767e710faf.jpg" width="626" height="500">
```

---
## \#26 Posted by: Zorb Posted at: 2016-07-05T23:17:34.779Z Reads: 43

```
Here's a better video with the lights. Any new insight?

https://youtu.be/DMQmGII6zVo
```

---
## \#27 Posted by: JLabs Posted at: 2016-07-06T00:58:25.822Z Reads: 39

```
Yeah, something is wrong with the wiiceiver, the lights should not do that.. I would take the heat shrink off and check the solder joints, it's possible someone made a mistake
```

---
## \#28 Posted by: laurnts Posted at: 2016-07-06T01:49:03.745Z Reads: 38

```
From the video, it looks like your ESC is the problem. I have similar ESC it should be very noisy especially from the fan. I didn't hear that, so you might wanna check and or replace the ESC.
```

---
## \#29 Posted by: lowGuido Posted at: 2016-07-06T02:05:23.199Z Reads: 37

```
Yeah something isnt right with the wiiceiver.  The green light should flash with acceleration and the red with braking.
```

---
## \#30 Posted by: Cptanpanic Posted at: 2016-08-19T16:04:55.902Z Reads: 28

```
What did you end up doing?
```

---
