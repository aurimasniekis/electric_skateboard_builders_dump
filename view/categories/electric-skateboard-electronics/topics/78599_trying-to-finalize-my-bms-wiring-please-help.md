# Trying to finalize my BMS wiring. Please help

### Replies: 8 Views: 469

## \#1 Posted by: Reelop19 Posted at: 2018-12-21T03:00:28.860Z Reads: 70

```
Please see my diagram. I’ve also included a picture of my bms. I’m not so sure about the connection for my anti spark or the best way to tap into the wiring. Also, do I just need a PPM splitter to connect the two motors together with my nano remote?  Thoughts?
![image|374x500](upload://hr4Z1rNsv4lDAfIkmMWPEhOZuV7.jpeg) 
![image|375x499](upload://uvoGSwuWWymjJcqqj4eSkVVe3Zw.jpeg)
![image|690x384](upload://4es87CcQzNKr0iTBnyvEAY10JNY.jpeg) ![image|375x500](upload://xHAS5NE8nygnXeAmQSSaQIwDh8F.jpeg)
```

---
## \#2 Posted by: Andy87 Posted at: 2018-12-21T06:14:31.464Z Reads: 55

```
I assume you want to use your bms for charge and discharge?
Does the BMS have a build in e-switch you going to use?
Can you tell us the exact model of the BSM and if you have it would be good to also post the wiring diagram which came with the bms.
Without this you can´t say if your diagramm is right or not.

The antispark in your diagramm is a xt90s ?
if yes, just swap it out to any of this two possitions
![Unbenannt|435x499](upload://tTPhTuEBzCs0LGX8vX3c2zg5650.png) 

No need to have multiple extra plugs.
The anti spark switch will only help in the moment you connect the plugs.
so if you connect your battery to the esc always use the xt90s plug (if the bms has an e-switch and the switch is off, than it doesn´t matter at all)

Edit: you can use CAN cable to connect your focboxes, or a split ppm cabel. both will work fine.
```

---
## \#3 Posted by: mynamesmatt Posted at: 2018-12-21T06:21:39.113Z Reads: 51

```
that anti spark will work, but will be a pain in the ass bc you connect the circuit to the focboxs rather than using a key which you can just plug in a loop key
![Screenshot_20181221-171934_Samsung%20Notes|262x500](upload://9BdfIxEirO6NFAz49dpMcvf8Pm4.jpeg)
that's the easiest way to implement a loop key. 
also make sure all your voltages are correct for the bms' balance leads
```

---
## \#4 Posted by: Reelop19 Posted at: 2018-12-21T19:52:12.809Z Reads: 32

```
Updated with diagram and on/off switch
```

---
## \#5 Posted by: Andy87 Posted at: 2018-12-21T20:09:02.340Z Reads: 32

```
Where is the first pack in your drawing and where is the first and the last balance wire?

If you use the e-switch on your bms you don’t need an separate anti spart.
I non the less would change one of your xt60 plugs to a xt90s (how I was drawing it before)

For how much amps your bms is rated?
If you use a bms as discharge too you also don’t need a second fuse.
The fuse on the charge port is fine thou 👌
```

---
## \#6 Posted by: Reelop19 Posted at: 2018-12-21T20:31:35.151Z Reads: 30

```
1st pack is bottom left along with 1st balance wire. Last balance wire bottom right. So the switch I have then is an e switch (pictured with 4 wires coming out) not an anti spark?  Not quite sure where I wire those 4
```

---
## \#7 Posted by: Andy87 Posted at: 2018-12-21T20:46:37.224Z Reads: 27

```
We need to know which bms exactly you have and if it is a charge only bms or a charge and discharge bms.
If it’s a charge only than you need a separate anti spark switch or a loop key how @mynamesmatt suggested.
If it’s a charge/discharge bms you can use the build in e switch and don’t need an anti spark switch
```

---
## \#8 Posted by: Reelop19 Posted at: 2018-12-21T21:16:50.665Z Reads: 20

```
My bad. Forgot to include it. I bought this one

https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F322370780260
```

---
