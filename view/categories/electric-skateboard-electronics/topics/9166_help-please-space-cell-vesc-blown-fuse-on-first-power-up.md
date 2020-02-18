# Help Please! Space Cell, VESC, blown fuse on first power-up

### Replies: 19 Views: 1349

## \#1 Posted by: dual Posted at: 2016-09-07T20:32:13.389Z Reads: 158

```
Hi All,
I just got all the parts and I'm starting on the electronics, trying to configure the VESCs with the BLDC_Tool.  I don't have a bench power supply so I put a smaller fuse in the Space Cell (10s3p), plugged in the VESC, hit the switch, and the fuse blew immediately.  Any ideas?  Is there a chance the RC receiver, if connected or not connected would somehow request full power without trigger input?  Are there any common short locations I can check for on the VESC?  I've tried it with and without the motor attached.  Looking around for tips, most of the VESC troubleshooting begins once the BLDC_Tool is working so I'm not sure where to begin with this challenge.  Any thoughts or suggestions would be appreciated!  Thanks!
```

---
## \#2 Posted by: JTAG Posted at: 2016-09-07T21:05:34.465Z Reads: 153

```
[quote="dual, post:1, topic:9166"]
would be appreciated!  Thanks!
[/quote]

Fuse only blows in extreme situations. First thing I think about: You put + and - the wrong way around.
```

---
## \#3 Posted by: dual Posted at: 2016-09-08T05:06:38.753Z Reads: 132

```
Thanks. I soldered the bullet connectors on the motor wires, but otherwise I haven't done anything. Black and red wires line up as they should at the xt60 connectors, and the vscs look like the others I've seen online.
```

---
## \#4 Posted by: Jinra Posted at: 2016-09-08T05:36:06.457Z Reads: 128

```
what fuse did you put in the space cell?
```

---
## \#5 Posted by: dual Posted at: 2016-09-08T06:58:50.589Z Reads: 119

```
5A fuse.  I have two VESCs and I have tried them both. Once, I saw a very brief blue light from the VESC before the fuse went. Blue, like an LED, not like arcing. Thanks for your time!
```

---
## \#6 Posted by: Jinra Posted at: 2016-09-08T08:22:34.693Z Reads: 110

```
Is this a VESC you built yourself? It sounds like there might be a short if the fuse is blowing immediately. 

If this is a commercial VESC just use the stock 40a fuse as they've already been preprogrammed and are safe to use with proper batteries.
```

---
## \#7 Posted by: chuttney1 Posted at: 2016-09-08T08:25:33.545Z Reads: 108

```
Why are you using a 5 amp fuse? You'll be blowing so many. What Jinra said to use a 40 amp fuse is fine.
```

---
## \#8 Posted by: dual Posted at: 2016-09-08T08:56:13.816Z Reads: 108

```
I put in a 5A fuse so if something goes wrong when I first plug it in and start configuring, it goes wrong at lower amps. I'll put the 40A back in when it's time to ride. I hope there is logic in that. I bought the battery and VESC and the only thing I have changed is adding the bullet connectors for the motors - I haven't modified or made any other connections.
```

---
## \#9 Posted by: Jinra Posted at: 2016-09-08T08:59:13.280Z Reads: 104

```
just use the 40 fuse. The VESC can take a burst current of 240A which should trip a 40a fuse anyway. No reason to configure on small fuses. Your 5a fuses will probably trip during detection as well.
```

---
## \#10 Posted by: dual Posted at: 2016-09-08T09:30:01.529Z Reads: 98

```
I've blown two of those too. Same circumstances, two VESCs, tried separately (each attached alone directly to the battery) on 5A and 40A fuses.
```

---
## \#11 Posted by: Jinra Posted at: 2016-09-08T09:59:11.471Z Reads: 97

```
definitely sounds like a short. Have you tried turning it on without the VESC attached? Can you measure the current and voltage with a multimeter?
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2016-09-08T13:03:57.691Z Reads: 84

```
Do you have any picture of your connection?
```

---
## \#13 Posted by: dual Posted at: 2016-09-08T13:32:09.707Z Reads: 81

```
Thank you all! I'll get a multimeter on it in 7 hours, and take a picture as well.
```

---
## \#14 Posted by: dual Posted at: 2016-09-08T19:06:28.749Z Reads: 83

```
<img src="/uploads/db1493/original/3X/f/b/fbd2cbc69caf4ad0d6ab3369a782990c545b011a.jpg" width="375" height="500">

The yellow and green is just so I don't confuse the two. VESC 1 has blown a 5, 10, and 40A fuse. VESC 2 has blown a 5A fuse, but just worked with a 10A. That is vesc- battery only, no RX or motor. I'm glad that VESC 2 seems to be working. DMM says 36v from the battery. What else can I check on the VESC? Thanks!
```

---
## \#15 Posted by: JohnnyMeduse Posted at: 2016-09-08T19:13:06.387Z Reads: 80

```
Seen like you have a short, can tou put a picture of the other one... @Blasto 

Also, where did tou buy these VESC
```

---
## \#16 Posted by: Blasto Posted at: 2016-09-08T19:57:12.942Z Reads: 75

```
There's your short. The red wire is touching the fet pad that is directly to gnd (through the shunt).
<img src="/uploads/db1493/original/3X/1/b/1ba4d4db682ed5763430d0101eaab9d0e8c79b40.jpg" width="646" height="500">

Resolder that red wire, nothing should be damaged on the VESC
```

---
## \#17 Posted by: dual Posted at: 2016-09-08T20:09:36.454Z Reads: 72

```
Nice!  Thanks for picking that out!  I'll be able to make the repairs next week.
```

---
## \#18 Posted by: dual Posted at: 2016-09-11T19:04:54.093Z Reads: 65

```
It works!  Problem solved.  Thanks!  Electrical system is mostly complete, but having problems identifying the hall sensors with the BLDC tool so I'll try without sensors for now.  The hardware will come together this week, and there will be no more kicking.
```

---
## \#19 Posted by: Blasto Posted at: 2016-09-11T19:17:37.390Z Reads: 63

```
Good stuff man! Glad it worked out.

You know the procedure now if you want help w your setup, pics of the setup ;)
```

---
