# No load no belt Watts vs no load belt, wheel, idlers

### Replies: 5 Views: 278

## \#1 Posted by: Sebike Posted at: 2018-12-04T10:54:37.160Z Reads: 123

```
So for the 100th time I wanted to try and figure out the real kv of my motors. Since the kv command still gives me a "0 kv" read, I had to check all the values via the @Ackmaniac app and do the maths myself.

This made me realize that a full throttle gives significantly different W values on the two motors (with no load).

The darkmatter/flipsky/whatever motor (#1) read 17 watts with belt /dual idlers/ abec 97s. Motor curr was 0,5 A and batt curr was 0,4 A.
At the same time, the sealed Maytech (#2) read 38 W, mot curr 1,2 and batt curr 1,0. For both, number of vescs was set to "1".

Without belts the #1 read  - 4W - 0,1 motor amps  and - 0,1 batt amps.
#2 read 10 W, 0,3 A and 0,2 A.

First of all I was a bit surprised that the app showed twice the power/amps for one motor than that of the other motor. 
Why would one motor consume twice as many amps as the other one? They're not the same motors, but both are 6374. Is it normal that difference is this huge, or is this maybe only a difference with no load? 

I was also a bit surprised that the difference in watts between belts+wheels vs no belts was this big.

Any thoughts or experiences?

![Screenshot_20181204-112718|281x500](upload://wuwOrElt76OpR45pTnHwYrwG9WK.png) ![Screenshot_20181204-112743|281x500](upload://bOEti36pjRKgHY4LT4rYl5EmMNN.png)
```

---
## \#2 Posted by: Deckoz Posted at: 2018-12-04T12:43:45.942Z Reads: 91

```
not all motors are created equal.


a motor with thicker windings, thinner laminations and higher power arc magnets, will run lower watts and generate more torque per watt, than another motor of the same kV with thinner windings, thicker laminations or lower power magnets

Ive been saying for people to run thick ass windings, with 0.15 laminations (vs the standard 0.20 or 0.25), and n52SH instead n48H for a long time. its because  no load wattage is lower, and the output torque per watt is higher. meaning more efficient. 

Better design means less heat, more acceleration, longer battery life, and longer service life.

But hey what do I know... lol
```

---
## \#3 Posted by: Grozniy Posted at: 2018-12-04T20:16:34.659Z Reads: 64

```
Esk8 jesus @Deckoz , what motor that has these specs?
```

---
## \#4 Posted by: Sebike Posted at: 2018-12-04T23:57:32.151Z Reads: 50

```
So this would suggest that the maytech motors are less efficient and less torquey as compared to the flipsky-/dark matter-/januxflux-like motors. 

The Maytech motor actually feels a bit weaker and gets slightly warmer compared to the other motor (running it as a single drive). 

However, there are apparently different aspects of "better design", as these more efficient motors have several design /manufacturing flaws causing them to fail more frequently than the Maytechs, which on the other hand are less efficient, heat up a bit more, BUT don't fall apart.
```

---
## \#5 Posted by: Pedrodemio Posted at: 2018-12-05T17:34:00.379Z Reads: 32

```
Just a note, changing the grade of the magnet without re evaluating a design is really bad, magnet maximum operation temperature is not defined only by grade, but by geometry, and comparing N52 and N48 for the same geometry you get way lower max operating point without permanent strenght loss for the N52
```

---
