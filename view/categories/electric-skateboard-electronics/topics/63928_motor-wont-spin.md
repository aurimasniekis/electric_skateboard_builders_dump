# Motor won&rsquo;t spin

### Replies: 9 Views: 483

## \#1 Posted by: drassak Posted at: 2018-08-05T18:05:14.696Z Reads: 96

```
hello guys,

I have been using my setup for a couple of month and it suddenly stopped working while riding:
I made a check on the component and everything looks fine except the VESC wont spin the motor:

Motor : OK, will spin if driven with another vesc
battery : OK
Remote/ reciver : OK the signal is passing thru

VESC : Something is wrong but cannot tell what:
the blue led turns on, the green led too when i pull the throttle. No blinking red. 
I get no fault code when logging in the BLDC tool.
The motor won't spin, and the motor detection does not works either.

any idea what could be wrong?

thank you

Paul
```

---
## \#2 Posted by: strattos Posted at: 2018-08-05T18:21:45.358Z Reads: 82

```
Pictures would help potentially. And have you attempted to redo motor detection. Checked all your solder joints for the connectors?
```

---
## \#3 Posted by: sayekim Posted at: 2018-08-05T21:42:40.582Z Reads: 72

```
Weird. I had the exact same problem with a meepo esc first gen. Leds worked and turned green from remote input. Kieran laughed at me (chinese smiley face their way of communicating) and said my esc needs to be replaced. 
I purchased a wowgo esc to replace it and was riding again after. 

I always wondered what was wrong with it. Hope you find out. It might shed some light as to why mine doesn’t work either.
```

---
## \#4 Posted by: drassak Posted at: 2018-08-06T07:11:09.706Z Reads: 60

```
I'll maybe upload some close ups from the vesc but apart from that there is nothing visual, Solder on the connectors are Ok.

The motor detection is failing, the motor doesn't spin.
```

---
## \#5 Posted by: EvanWhy Posted at: 2019-01-04T06:04:04.949Z Reads: 34

```
I'm having the same issue, has anyone figured it out?
```

---
## \#6 Posted by: Andy87 Posted at: 2019-01-04T08:28:39.514Z Reads: 32

```
Did you do all the trouble shooting like @drassak?
No faults no red lights on the vesc?
```

---
## \#7 Posted by: drassak Posted at: 2019-01-04T08:55:58.298Z Reads: 30

```
Hey, unfortunately there was no miracle, i made sure the motor was ok and changer the VESC
```

---
## \#8 Posted by: EvanWhy Posted at: 2019-01-04T20:39:54.490Z Reads: 28

```
yeah it seems like there's no faults on the vesc. I checked to see if the drv was fried and it looked fine. the weird thing is, is that sometimes when I try to detect the hall sensors the motor drives but then it says motor detection failed. and then when I try to do it again, the motor doesn't spin.
```

---
## \#9 Posted by: kuphjr Posted at: 2019-01-16T15:25:39.224Z Reads: 22

```
has anyone made any progress on a solution to this issue?? It just started happening for me too!
```

---
