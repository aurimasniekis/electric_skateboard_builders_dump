# Motor detection not working all the time

### Replies: 8 Views: 272

## \#1 Posted by: Shaibazsayed66 Posted at: 2018-04-17T16:50:31.632Z Reads: 63

```
hey guys 

I'm working on a project of e-bikes 
ordered parts everything needed  for a  ebike  things like battery motors and all 

BUT'

on youtube and other places i found that focbox is the best esc in the market so i ordered just to make 1 prototype 

n OMG its not able to run the motor at all :triumph:
 
I'm not able to do a motor detection, 
In terminal no faults  
then tried foc ( r = 0 ) :disappointed:

motor run's cheap ESC but not on foc  even doe being so expensive
guys plz help invest a lot of money in this prototype
```

---
## \#2 Posted by: GrecoMan Posted at: 2018-04-17T16:55:48.526Z Reads: 60

```
lol what

what’s your setup? batt cutoffs? battery voltage? motor kv?
```

---
## \#3 Posted by: Shaibazsayed66 Posted at: 2018-04-17T18:06:33.462Z Reads: 53

```
42v battery 10s 2p panasonic 1865b 3400mAh
battery cut off @33v
motor 35kw
```

---
## \#4 Posted by: Deckoz Posted at: 2018-04-17T21:13:08.096Z Reads: 45

```
Soo

Are you running the stock vesc tool(3.***) On a focbox. Or are you running 2.*** Firmware?

If it's the first... You'll never get a detection.. you'll need ackmaniac 3.100 or go back to 2.*** Firmware.
```

---
## \#5 Posted by: Shaibazsayed66 Posted at: 2018-04-19T11:04:14.684Z Reads: 24

```
yes Mr. deckoz can u help me in doing this im stuck for a long time cause I have no idea how it done
and I never done it , this is my 1st time 
can you help me in setting it up please :bowing_man:t2:
```

---
## \#6 Posted by: telnoi Posted at: 2018-04-19T11:52:38.467Z Reads: 20

```
*Show photographs of your wiring
*Provide a proper description of what you have done, what firmware you are using, if the motor reacts at all
```

---
## \#7 Posted by: onepunchboard Posted at: 2018-04-19T18:09:43.810Z Reads: 11

```
if the motor is big or old, they have high resistance that requires more currents. I believe bike motor is 80% or less efficiency.

just up D value by 0.01 untill u find the detection.
do not just put 0.10 like that it mass up emf coupling and u will burn something. slowly up the value.
this is how I did with troublesome detection
```

---
## \#8 Posted by: Shaibazsayed66 Posted at: 2018-04-19T19:01:57.307Z Reads: 11

```
oo  yes ill try it out
```

---
