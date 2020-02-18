# VESC-X: Less range and a different voltage than battery

### Replies: 25 Views: 2234

## \#1 Posted by: lox897 Posted at: 2017-01-21T08:20:32.736Z Reads: 194

```
So here's the story, I'll try and explain everything in a list order so it might be easier to identify the problem:

1. VESC X ARRIVED
2. Soldered to 4x 3S lipo in series, and 5.5mm bullet connectors
3. Setup in BLDC Tool
Settings for step 3 setup:
BLDC (no sensors
Motor max 60
Motor min regen -40
Battery amp max 60
Overall max amps 130
Battery cutoff start: 44.4
Battery cutoff: 43.2

4. Ride, board works flawlessly and goes 45kmh

5. One phase wire comes loose, resolder.

6. Configure in BLDC with sensors 
Speed goes down to around 25-30kmh

7. Remove sensors leave on BLDC: speed still the same

Firmware reflash: default settings, enable FOC, now speed is 10kmh.

Any ideas what the problem could be? I will send screenshots later tonight and I will measure battery output voltage. Cells are at 3.91 each

Thanks guys, hope I can get this resolved quickly so I can start riding. I'm thinking it could be my battery voltage cutoffs? Should I try charging?
```

---
## \#2 Posted by: Maxid Posted at: 2017-01-21T08:31:23.522Z Reads: 184

```
Whats the total voltage after your antispark switch?
```

---
## \#3 Posted by: lox897 Posted at: 2017-01-21T08:32:35.046Z Reads: 180

```
Not using antispark switch. Just plugging straight into vesc. Waiting for some xt90s to come
```

---
## \#4 Posted by: DeathCookies Posted at: 2017-01-21T09:16:57.637Z Reads: 168

```
Maybe because the Esc capacitors dont like The spark by connecting a 12s battery?
```

---
## \#5 Posted by: Maxid Posted at: 2017-01-21T09:21:28.498Z Reads: 164

```
I'd still like to know to the actual voltage the VESC "sees".
```

---
## \#6 Posted by: lox897 Posted at: 2017-01-21T09:51:10.231Z Reads: 159

```
Once I have access to my laptop I'll check it
```

---
## \#7 Posted by: IDVert3X Posted at: 2017-01-21T09:53:03.729Z Reads: 155

```
Dont you have a multimeter at home?
Its the most basic and cheapest debugging tool, lol.
```

---
## \#8 Posted by: Okami Posted at: 2017-01-21T10:01:39.484Z Reads: 153

```
IS it still possible for him to add bluetooth module? :D Might as well just get better logging data.. or course, multi meter also does not come pricy.. mostly 5usd and you got yourself a voltmeter :D
```

---
## \#9 Posted by: IDVert3X Posted at: 2017-01-21T10:19:32.538Z Reads: 152

```
Sure, he can. But why BT when he can just connect the USB cable into the computer?

Also, multimeter is the most basic must-have thingie when working with electronics. They range from $10 to few hundred. I personally use mainstream $30 one.
```

---
## \#10 Posted by: lox897 Posted at: 2017-01-21T10:42:52.089Z Reads: 149

```
@IDVert3X Of course I have a multi meter! I'm not at home right now, or at the workshop. So I don't have access to any tools.
```

---
## \#11 Posted by: lox897 Posted at: 2017-01-21T12:14:08.168Z Reads: 140

```
Any ideas? @ackmaniac @chaka ?
```

---
## \#12 Posted by: lox897 Posted at: 2017-01-21T12:41:57.150Z Reads: 132

```
So I think I found the problem... the vesc is reading 43.2v into the vesc, which is where my cutoff is at. But all my lipo cells are at 3.95v per cell which is 47.4v. So why is there a difference of 4.2v?
```

---
## \#13 Posted by: Maxid Posted at: 2017-01-21T12:47:07.411Z Reads: 128

```
Because your soldering is probably not good and you have some unwanted resistance somewhere. You mentioned you had to resolder your phase wire - that might be your starting point to redo.
```

---
## \#14 Posted by: lox897 Posted at: 2017-01-21T12:53:31.232Z Reads: 127

```
Thanks @Maxid. I'll recheck the soldering connections. I do have lots of plugs to wire the 4 batteries in series. Could I lower my cutoff rate to work with the battery voltages?
```

---
## \#15 Posted by: Maxid Posted at: 2017-01-21T12:57:11.447Z Reads: 125

```
There is something wrong with your batteries - fix it first before you start using it again. The "missing" voltage is being used up somewhere and transformed to heat - you don't want to ride like this.
```

---
## \#16 Posted by: lox897 Posted at: 2017-01-21T13:03:56.570Z Reads: 124

```
Thanks so much man! I'll resolder all connections that don't look good tomorrow. Hopefully then the board will be working.
```

---
## \#17 Posted by: IDVert3X Posted at: 2017-01-21T13:35:59.756Z Reads: 122

```
Better advice: take your multimeter, switch on the board, measure voltages across connections.
They should be very close to zero. If there is a voltage, it means there is a voltage drop because of resistance, then you know you need to resolder it. And remember, the higher the current, the higher the voltage drop will be.

Another way is to keep the board shutted down and measure the resistance using the multimeter. It should be close to zero as well. This is the safer way, but will drain your multimeter battery more quickly.

If neither of these shows any signs of error, come back and we can discuss it further.
```

---
## \#18 Posted by: lox897 Posted at: 2017-01-22T00:38:10.836Z Reads: 100

```
So the issues could be one of two things:
A wrong resistor on the vesc (I am speaking to Charles from Enertion and @JohnnyMeduse about the issue

Or bad soldering

I will be able to confirm the final issue today. I would also highly recommend that anyone else who feels like their cutoff is getting activated sooner than usual to check the voltage from battery directly (with multimeter) and check the voltage on your BLDC tool. If there is a difference, there could be a wrong resistor on your vesc x.
```

---
## \#19 Posted by: Pathaim Posted at: 2017-01-22T00:48:05.475Z Reads: 100

```
Have you tried reading the voltage with all 4 lipos in series but without the vesc? to see if the vesc is reading wrong or if the cells are really trhat low
```

---
## \#20 Posted by: lox897 Posted at: 2017-01-22T00:48:41.221Z Reads: 101

```
Haven't got my good multimeter. The one at home is my grandpa's one. It's super crap
```

---
## \#21 Posted by: lox897 Posted at: 2017-01-22T00:51:27.611Z Reads: 96

```
Issue resolved: One of the resistors inside the vesc is wrong. Enertion is sending a new VESC. Awesome service @onloop @EnertionSupport
```

---
## \#22 Posted by: Pathaim Posted at: 2017-01-22T00:53:28.110Z Reads: 95

```
hope its only your vesc and isn't an issue on others
```

---
## \#23 Posted by: zmoney Posted at: 2017-01-22T00:56:43.981Z Reads: 96

```
Do you know which resistor? :thinking:
```

---
## \#24 Posted by: lox897 Posted at: 2017-01-22T00:57:09.621Z Reads: 97

```
R4 is the resistor I think
```

---
## \#25 Posted by: zmoney Posted at: 2017-01-22T02:13:08.206Z Reads: 92

```
<img src="/uploads/db1493/original/3X/a/4/a4455516ce1bd687d0180a709a5d8ed05c4f288b.JPG" width="581" height="500">

Makes sense! Glad they were able to help you out. :slight_smile:
```

---
