# BMS help needed *magic smoke escaped*

### Replies: 25 Views: 1651

## \#1 Posted by: Bataleon Posted at: 2017-11-04T17:48:28.050Z Reads: 148

```
A friend and I connected up a BMS like in the diagram below and things began to smoke after the balance leads were plugged-in.

Where did we go wrong?

<img src="/uploads/db1493/original/3X/8/0/80138f33efeb41d0816c8ed31b665255cc78c2f8.jpg" width="351" height="500">
```

---
## \#2 Posted by: lowGuido Posted at: 2017-11-04T19:43:53.088Z Reads: 130

```
your diagram looks correct. but there is a fairly good chance that what you did didn't match your diagram.
I reckon you got one of the balance leads out of sequence, and that would have burnt out a row of resistors on the BMS board.
```

---
## \#3 Posted by: chuttney1 Posted at: 2017-11-05T08:17:13.408Z Reads: 107

```
Something about the wiring portion of the balance wires to the BMS seems off.
```

---
## \#4 Posted by: hornet90 Posted at: 2017-11-05T08:43:18.914Z Reads: 101

```
its the last 3 wires on each pack last wire is red so pack 2 and 3 are wrong 
dont use wire 1 on any pack im not great on this but thats what i think
<img src="/uploads/db1493/original/3X/b/1/b1edfd053cf06b8187a1a0a5b505f207ee0439e1.png" width="592" height="500">
```

---
## \#5 Posted by: cryo Posted at: 2017-11-05T09:21:13.781Z Reads: 88

```
I agree with Hornet, while the way you wired the balance leads seems correct, doing it hornets way is just much cleaner as its 3 balance wires per 3s battery which just clicks. The way you wired it in the original can give way to more confusion which is what i think may have happened.
```

---
## \#6 Posted by: ducktaperules Posted at: 2017-11-05T09:24:19.135Z Reads: 87

```
is this a 9s bms or a 10 s bms?
```

---
## \#7 Posted by: hornet90 Posted at: 2017-11-05T09:26:04.859Z Reads: 85

```
well spoted should  be 9s he used a 10s
```

---
## \#8 Posted by: ducktaperules Posted at: 2017-11-05T09:45:08.659Z Reads: 84

```
balance connector usually has (NoOfCells + 1) wires. Assuming this is a 9s BMS that has 10 ports then you have to also wire ground.

**EDIT : "Assuming this is a 9s BMS" this assumption was wrong therefore this diagram is wrong. DO NOT USE THIS DIAGRAM.**

Im guessing it should be like this: 
<img src="/uploads/db1493/original/3X/c/4/c4f5c3300e20545f53bc28e8bc23d7f1ba85b61e.jpg" width="351" height="500">

The port 4 and 7 could be connected with either of the 2 wires i have shown, they should do the same things because they are connected, i have just shown both for clarity.

This means in your diagram you have connected  3.7v of cell 1 to ground inside the BMS. If you were lucky you just dumped current through a ground trace and there may be no long term damage. If you left it to long you may have just a burned trace that you could replace, this would be fairly obvious on the PCB. If not there may have been some resistors between between the plug and ground that may have cooked. If this is the case you would see them when you look at the PCB in the BMS.

To confirm that this is what happened i would expect to see the voltage of cell 1 pack 1 slightley lower than the others if you check with a multi meter.
```

---
## \#9 Posted by: hornet90 Posted at: 2017-11-05T10:35:21.022Z Reads: 73

```
As far as I know all the bestech bms would be 9 wires for 9s 10 wires for 10s
```

---
## \#10 Posted by: cryo Posted at: 2017-11-05T11:03:02.646Z Reads: 75

```
Yea I have no clue about bestech bms'. 

I had a look at the product page and they don't even have any wiring diagrams. Can't tell if OP bought the wrong board or what, seems weird that a 9s bms would have 10 balance leads.
http://bestechpower.com/333v9spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
```

---
## \#11 Posted by: Bataleon Posted at: 2017-11-05T11:47:43.860Z Reads: 72

```
Thanks for all of the replies. Sorry, I forgot to mention the BMS is 10S but we're only using a 9S pack, hence pin B10 being disconnected.

@ducktaperules, the first pin of the BMS balance connector is marked as B1, so we decided not to connect the balance lead which read 0v to the first pin.

When measuring the individual cell voltages, we kept the black multimeter probe attached to B-, and then measured each cell, making sure the voltage increased by the correct amount (i.e. 3.7v, 7.4v, 11.1v etc).  Is this correct?

<img src="/uploads/db1493/original/3X/c/0/c0e219dedfb71d3e77869efde816dec9a929dd01.jpg" width="690" height="462">
```

---
## \#12 Posted by: hornet90 Posted at: 2017-11-05T12:07:30.871Z Reads: 67

```
Ok the pic I put up is right Its wired  wrong and you need a 9s bms 
I've wired 10s bestech be for and that's the way I done it
```

---
## \#13 Posted by: hornet90 Posted at: 2017-11-05T12:12:27.847Z Reads: 70

```
http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014/72?u=hornet90
```

---
## \#14 Posted by: cryo Posted at: 2017-11-05T12:24:52.974Z Reads: 70

```
Yea im fairly certain you cant use a 10s bms for a 9s battery. Dont quote me on that though
```

---
## \#15 Posted by: Namasaki Posted at: 2017-11-05T17:38:13.811Z Reads: 65

```
[quote="cryo, post:14, topic:37348, full:true"]
Yea im fairly certain you cant use a 10s bms for a 9s battery. Dont quote me on that though
[/quote]

You are correct. 
A Bestech 10s bms will not work with a 9s battery.
```

---
## \#16 Posted by: Namasaki Posted at: 2017-11-05T17:41:11.234Z Reads: 62

```
Your balance wiring is not correct. 
You should omit the ground balance wire of each pack and use the 3 positive wires.
```

---
## \#17 Posted by: Namasaki Posted at: 2017-11-05T17:43:57.209Z Reads: 60

```
This diagram is totally wrong. 
<img src="/uploads/db1493/original/3X/e/4/e41f67b091fe8dfd5b9a69f73f16bfa43839cf3d.jpg" width="281" height="499">
```

---
## \#18 Posted by: ducktaperules Posted at: 2017-11-05T17:52:17.573Z Reads: 54

```
thanks for clarifying, i have put a note in my post so that no one uses that diagram
```

---
## \#19 Posted by: hornet90 Posted at: 2017-11-05T20:35:47.735Z Reads: 55

```
Did u get 2 10s bms
```

---
## \#20 Posted by: icon Posted at: 2017-11-05T20:49:53.317Z Reads: 55

```
http://www.electric-skateboard.builders/t/balance-wiring-problem-9s/5974
You might get some nice info from here ;)
```

---
## \#21 Posted by: Bataleon Posted at: 2017-11-19T14:14:23.447Z Reads: 42

```
Sorry for the radio silence all, things have been crazy at work.

I received confirmation from Bestech that their 10S BMS will work fine with a 9S lipo config.

So far @hornet90's [suggestion](http://www.electric-skateboard.builders/t/bms-help-needed-magic-smoke-escaped/37348/4) seems to make the most sense: leave off the negative balance wire from each 3S pack, then connect the remaining wires in order of increasing voltage.

Can anybody confirm this? Really don’t want to toast a third BMS. The image below has been updated to reflect the suggested changes.

Thanks

<img src="/uploads/db1493/original/3X/5/1/51f6eeef1af0025f82ff5e6167ec12a45a6b60b8.jpg" width="351" height="500">
```

---
## \#22 Posted by: hornet90 Posted at: 2017-11-19T15:41:05.136Z Reads: 31

```
Still not looking right to me........
```

---
## \#23 Posted by: hornet90 Posted at: 2017-11-19T15:54:28.783Z Reads: 31

```
<img src="/uploads/db1493/original/3X/c/8/c81aa991b3a7fef422c19f0bf9e3c2a63f72c883.jpg" width="281" height="499">


Its the only way it looks right to me still not sure
```

---
## \#24 Posted by: hornet90 Posted at: 2017-11-19T15:56:37.116Z Reads: 31

```
when thinking about it if u order a 9s there would be 1 wire less.......dont forget to cap that last wire
```

---
## \#25 Posted by: hornet90 Posted at: 2017-11-19T15:59:00.312Z Reads: 29

```
sorry your 1 is the same didnt look at it right
```

---
