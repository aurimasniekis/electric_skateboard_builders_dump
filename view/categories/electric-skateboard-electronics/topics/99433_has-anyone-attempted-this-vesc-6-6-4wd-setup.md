# Has anyone attempted this VESC 6.6 4wd setup&hellip;?

### Replies: 8 Views: 288

## \#1 Posted by: kchxaz Posted at: 2019-07-30T23:57:18.658Z Reads: 94

```
Wondering if anyone has attempted to convert their build into a 4wd setup by soldering the two wires from the CANBUS on one Flipsky 6.6 Dual VESC to a second one as seen in the pic below? Did it work? 

The CANBUS on the 6.6 Plus version of the 6.6 Dual has a port for the wires but there are only two wires yet four pins on the PCB board. Anyone know what gives? (I am speaking about *Flipsky* Dual 6.6 VESC only)

![46444573_2048271948563802_4675679029683027968_n|690x321](upload://qm0SAYRmZZTkFMi1SGsgjMWNQCB.jpeg)
```

---
## \#2 Posted by: Soflo Posted at: 2019-07-31T01:53:20.990Z Reads: 81

```
This is from the 6.6 dual mini. 4wd is has it's own position on the switch....  looks like the CAN bus is used for 4wd and its 4 pin. 
 ![Screenshot_20190730-215105_Samsung%20Internet|243x500](upload://xqgSoevuNRJr5zl5U2scfkhdJrZ.jpeg)
```

---
## \#3 Posted by: Dirt_Bag Posted at: 2019-07-31T02:16:45.569Z Reads: 77

```
I did for a a few days just for fun.

It was 4wd 6374 with a 1:5 gearing on 8 inch tires

The front couldn't get enough traction due to the slight wheelies it did from the back motors.

I instead went with bigger dual motors and cut the price substantially
```

---
## \#4 Posted by: kchxaz Posted at: 2019-07-31T02:40:23.400Z Reads: 76

```
SOflo - Yes, it *is* from the mini. It was the best image of the canbus switch that looks identical to mine on the 6.6 standard (not 'plus'). I was using it to illustrate my question if anyone was able to connect the points specified and how were the 4wd results...

Still looking for input/results if anyone has any. Thanks!

Dirtbag - so it worked? You soldered the connections exactly as shown and the VESC did indeed drive the four motors no problem? No sparking ESC or anything, lol? I'm using 6354 motors. I have soldered wires to the points identified but I am nervous to apply power. It's $600 worth of VESC that's on the line here so I am hoping to get positive feedback before I take the leap...Was there any negative results from doing this? You just didn't want 4wd?
```

---
## \#5 Posted by: Andy87 Posted at: 2019-07-31T06:21:49.257Z Reads: 66

```
@kchxaz you need to tag @Dirt_Bag to make sure he get a notification and can answer if soldering the CAN did work.

I run quad on other vescs and i don´t use CAN to connect the vesc.
I just bind a receiver to the front vesc and one receiver to the back vescs (each side is connected via CAN than).
That will work with every vesc, also with your.
you just don´t have traction controll between 4 wheels, only between two wheels, but that is no big issue in my humble opinion.
```

---
## \#6 Posted by: Dirt_Bag Posted at: 2019-07-31T06:30:49.124Z Reads: 59

```

I didnt even bother with that layout. I just used a ppm splitter cable and copied the settings on all 4 vescs. For perfect throttle matching, make sure you map the throttle identically on both.
```

---
## \#7 Posted by: kchxaz Posted at: 2019-09-03T12:54:47.485Z Reads: 42

```
DB - I'm probably over thinking this but what do you mean exactly to map the throttle identically? You mean the min/neutral/max wheel throttle position sensor? But you've only got one receiver (since you have a cable splitter coming off your single receiver - one for each Dual VESC, correct?), so you wouldn't have to perform the app wizard setup for throttle matching, right? Am I thinking about this the wrong way?
```

---
## \#8 Posted by: Dirt_Bag Posted at: 2019-09-03T22:11:46.534Z Reads: 36

```
Program dual vescs as normal. Just match the ppm values on each vesc and your good. 


Theres really nothing difficult about it, set up your first vesc and then do the second to match all the settings.
```

---
