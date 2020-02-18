# BMS Wiring &amp; Loop Key Polarity

### Replies: 7 Views: 1057

## \#1 Posted by: Marty Posted at: 2017-01-04T19:39:05.078Z Reads: 132

```
Hi
just want to upgrade my board with a BMS and a XT90 Anti Spark as a Loop Key
my questions are:

#1 for this BMS
<img src="/uploads/db1493/original/3X/c/a/ca604f021c7ee9eb784ec42ffa0d34092ef8ef0e.JPG" width="666" height="500">
How do I properly wire this thing up - bought it in China with no manual etc.
Am I right with my guessing - but guessing is not the best ;-)
B+ Battery positive
B- Battery negative
P+ ESC positive
P- ESC negative
ok thats pretty straight forward, but like to add a Charge Plug - but as there is no "CH" as on many others.
So should it be:
B+ Charge positive
P- Charge negative
And what is the one pin labeled with "D-"
Balance Leads are pretty clear to me

#2 Loop Key with a XT90 Anti Spark
I read a bit in here about that but still dont have a clear solution.
Should it be in the positive (common ground would stay untouched) or in the negative (as the BMS works via the negative) ? Well "normally" it shouldnt matter where a switch is placed ;-)

Thanks and Cheers
Marty
```

---
## \#2 Posted by: IDVert3X Posted at: 2017-01-04T20:05:50.470Z Reads: 122

```
XT90 antispark is just a switch with resistor and resistor has no polarity, neither switch does.
It doesn't matter really matter where you put it. 
I personally prefer to cut common ground so I know for sure nothing is powered.

E: of course you want to put in between BMS and load, as @PXSS pointed.
```

---
## \#3 Posted by: PXSS Posted at: 2017-01-04T20:34:58.944Z Reads: 114

```
Loop switch needs to go between BMS and ESC on either lead. I personally put it on +
You do not want it between BMS and battery as you would not be able to charge without the board being powered. (Could be dangerous)
```

---
## \#4 Posted by: Marty Posted at: 2017-01-04T20:57:45.902Z Reads: 108

```
yeah where it belongs is clear - between ESC and BMS, but as you see in the first two answeres - 2 answeres - 2 opinions whether in + or in -
I know as in a house installation you put the switch in the "live" wire - whereas it phsyically wouldn matter ;-)

thanks anyway - any suggestions about the BMS wiriging and the confusing "D-" pin ?
```

---
## \#5 Posted by: IDVert3X Posted at: 2017-01-04T21:27:55.564Z Reads: 99

```
Take a look at it's datasheet ( if 
Or try to find something using google images...
You can search using an image :)
In the worst case, you can always ask seller for help :D
```

---
## \#6 Posted by: 2-alex-2 Posted at: 2017-01-04T23:07:13.534Z Reads: 90

```
<img src="/uploads/db1493/original/3X/b/d/bd09a68d88cbd61b2637b8a8a77d5735535e56ba.PNG" width="281" height="499">

Hope that helps.
```

---
## \#7 Posted by: Marty Posted at: 2017-01-05T14:33:41.689Z Reads: 61

```
yeah thanks - I searched google & pictures in advance a lot, but just also came acrros these simmilar ones.
Datasheet - yes nice - but only values and specs
ask seller - yeah if someone of you understands chinese ;-))
anyway - thanks for all your help - Ill figure it out - hopefully
```

---
