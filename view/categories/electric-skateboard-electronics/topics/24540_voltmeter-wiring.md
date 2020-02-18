# Voltmeter wiring

### Replies: 20 Views: 1592

## \#1 Posted by: Youssless Posted at: 2017-06-04T12:43:45.879Z Reads: 210

```
Hey guys, back today with yet another question for you helpful folk. 

So I made a connection from an anti-spark xt90 to 5.5mm bullet connectors and soldered in my voltmeter. Mainly for practice soldering (I'm horrible I've discovered) but the connections are really strong and I think it'll work so I'd love for an expert pair of eyes to have a look.

My questions:

1) Am I fine to use the anti-spark connector here as my on/off switch?
2) why is my voltmeter reading at 0.0V? does it have something to do with that yellow wire and the balance leads on my battery?

<img src="/uploads/db1493/original/3X/0/4/043f861f5a155eba0f1a34446bd8a6c4f60b6bd1.jpeg" width="281" height="500">

<img src="/uploads/db1493/original/3X/a/6/a6511e20ffb7b44661f1c1d9c85bb8604faf36de.jpeg" width="281" height="500">
```

---
## \#2 Posted by: Randyc1 Posted at: 2017-06-04T14:09:05.343Z Reads: 194

```
What do instructions say?,

Red and Black are maybe just to power Voltmeter and yellow reads the Voltage ,..  if thats the case Yellow would go on Posotive (red)Also.
```

---
## \#3 Posted by: Youssless Posted at: 2017-06-04T14:31:16.045Z Reads: 191

```
Thanks for your response. Unfortunately this didn't come with instructions. Just a plastic bag from China. 

I'll try connect the yellow to the positive wire and see what that does...

Yup, it gives me a reading but it jumps all over the place so let me try solder it on...

It works but the reading is very jumpy and varies greatly, I have a 9s LiPo setup on storage voltage (3.8V each cell) so I'm hoping to see 34V ish but it dances around the 40.0-45.7V mark...
```

---
## \#5 Posted by: Randyc1 Posted at: 2017-06-04T18:41:11.779Z Reads: 175

```
That is a fucked up wiring color scheme ?

...My Drok Voltmeter needs a 5-30v power source (red&black),...then white wire goes to eskate battery Pos.
```

---
## \#6 Posted by: Youssless Posted at: 2017-06-04T18:47:34.928Z Reads: 171

```
The meter can take readings of up to 100V I think it claimed and leaving it bouncing between figures for about 2 hours didn't do anything to it. 

Why would a 12V power source be needed?
```

---
## \#7 Posted by: Youssless Posted at: 2017-06-04T18:48:23.370Z Reads: 170

```
So I need a battery for my voltmeter? 

I think I should just grab a different voltmeter altogether, no?
```

---
## \#9 Posted by: Youssless Posted at: 2017-06-04T19:04:07.234Z Reads: 165

```
Thank you for the explanation, I've looked at and bought the [more recommended voltmeter](http://www.ebay.co.uk/itm/172143986261?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT) that has the positive and ground wires only.  

Hopefully this will be a more convenient solution.
```

---
## \#10 Posted by: Randyc1 Posted at: 2017-06-04T20:45:51.158Z Reads: 155

```
I just get the Voltmeter's power by tapping into Recievers power source ,  then other wire goes to battery Positive.
```

---
## \#11 Posted by: Aggdaddy Posted at: 2017-06-04T21:33:19.919Z Reads: 148

```
I'm using one of those, but I decided to use a 2s battery from my quadcopter collection to power it and I'll also use it to power my lights.  There is a YouTube video on how to do the wiring.
```

---
## \#12 Posted by: jmasta Posted at: 2017-06-04T23:27:00.460Z Reads: 140

```
Why not just get a 12V BEC?  Then you wouldn't have to worry about charging another battery
```

---
## \#13 Posted by: Aggdaddy Posted at: 2017-06-05T00:07:59.678Z Reads: 134

```
receiver and bec is on the other end of the board near the motors    voltmeter is in the center.    I don't mind charging batteries.   They do not get much use anyway
```

---
## \#14 Posted by: Namasaki Posted at: 2017-06-05T00:35:48.477Z Reads: 129

```
[quote="Youssless, post:7, topic:24540"]
So I need a battery for my voltmeter?
[/quote]
No, you just need to toss that meter and buy the right type of meter.
There are plenty available that do not require additional voltage. To operate
https://www.amazon.com/gp/product/B00IG1AYEW/ref=oh_aui_detailpage_o06_s00?ie=UTF8&th=1
```

---
## \#15 Posted by: thisguyhere Posted at: 2017-06-05T06:23:50.646Z Reads: 121

```
i have one of these three wire led volt meters.

[on mine](https://www.amazon.com/gp/product/B00C58JGE6/), two of the wires is for + / - of your pack, and one a 5v power source for the meter itself.

for the third 5v wire, i tapped into the 5v pin on the remote control port:

<img src="/uploads/db1493/original/3X/f/5/f5ffd8fa7a40eb4adc21b2c2116d5936a578a3b9.png" width="429" height="500">
```

---
## \#16 Posted by: smurf Posted at: 2017-06-05T06:51:29.506Z Reads: 114

```
Cheap and easy
https://www.instagram.com/p/BLl0RpuD_Rr/
```

---
## \#17 Posted by: Youssless Posted at: 2017-06-05T08:17:00.257Z Reads: 109

```
Thanks Namasaki, I ordered [this one](http://www.ebay.co.uk/itm/172143986261?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT) and will solder it in for peace of mind. I'm looking to work on my enclosure next and really tempted to just use a Tupperware box (but out of respect for the field I'll actually be making a vaccuum formed enclosure).

My next issue is with my VESC, I'm being told the one I bought is messed up...
```

---
## \#18 Posted by: Norco Posted at: 2017-06-05T08:46:27.498Z Reads: 109

```
That meter would be fine but it just needs wiring up correctly.

I would recommend doing what @Randyc1 said and take the 5v and common ground from the receiver supply and then wire just the measuring yellow wire to the pos from the battery.

Using an external battery wont work as you need to have a common ground.
```

---
## \#19 Posted by: Youssless Posted at: 2017-06-05T09:31:33.656Z Reads: 103

```
Thanks, so another option I have is to solder the leads into the base of the pins or wires for the molex connector for my receiver?
```

---
## \#20 Posted by: Norco Posted at: 2017-06-05T12:48:00.043Z Reads: 101

```
Yes - although I'm not familier with that receiver would you would just need to know which is the +5v and GND. 

On a benchwheel receiver there is a second set of pins that are redundant - I suspect for a dual set up but they are not connected to anything. All I did was put a solder bridge across the 2 rows of pins then use a servo cable I had laying around. That way your receiver remains removable (if you need it to be - I do as readout will be deck mounted)
```

---
## \#21 Posted by: mschil2440 Posted at: 2017-07-10T13:11:55.906Z Reads: 88

```
How did this voltmeter work out?
```

---
## \#22 Posted by: Youssless Posted at: 2017-07-10T13:40:55.572Z Reads: 84

```
Not the best, though I didn't give it enough of a try since they're cheap and I ordered a different one. The other one I got from eBay works well and generally does a good job but I still stopped to recharge when it said 25% left (about 10 miles on my 9S lipos).

I currently use @Ackmaniac's BLDC tool and android app as it gives me very easy to read, real-time readings for everything with the board and would recommend that since the bluetooth HM10 module is just slightly more expensive than the voltmeters (£3 vs £5).

Feel free to PM me any questions.
```

---
