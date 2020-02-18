# I broke two lipo batteries and i don&rsquo;t know why

### Replies: 18 Views: 1937

## \#1 Posted by: tueboard Posted at: 2016-09-16T10:47:23.448Z Reads: 174

```
the following picture is a battery nearly to explode (used only two times) VS a brand new (Floureon 3S 35C 11.1V 5500mAh)

<img src="/uploads/db1493/original/3X/8/e/8ef4dd4ecdd901656c981e77dee04096469d92b9.jpg" width="666" height="500">

if i try to charge the first one the imax b6 (i think that is the original one, the color text b6 is yellow) shows the message "err cell connect", i've the same problem with another one less swollen.

could my vesc configuration damaged my batteries?

<img src="/uploads/db1493/original/3X/c/f/cf5afe43af46c02e6eb17768a0d7c8e2ac0f01d9.png" width="690" height="339">

i used the imax b6 with 1.0A - S3 11.1V (i tried to put it more Amps but after a while imax stops or restarts)

maybe my fault is not to calibrate the balance charger before charging the batteries...

I recently purchased HK accucell 6 but i didn't tried yet... if i break the batteries again i will purchase another batteries from turnigy or zippy..

Do you have any idea what's happened?

thanks
```

---
## \#2 Posted by: karma Posted at: 2016-09-16T11:08:21.173Z Reads: 160

```
What's the current voltage of the puffy Lipo?
```

---
## \#3 Posted by: susplus Posted at: 2016-09-16T12:04:03.263Z Reads: 156

```
well your battery cutoff start and end are to low. Are you  using a 3s setup on your board? I presume that you are using 2 batteries in series which means you have a 6s setup on your board. So what you did is that you drained the battery to such an extend that the battery charger won't charge it anymore. You must have drained one or more cells to under 1V. In this case i strongly recommend to discard that battery in a safe way. It is impossible to recharge it and if by any miracle you would succeed to charge it, it won't last you more than a charge or two extra. 

correct me if i am wrong. you have not stated anything about your current battery setup and i was just guessing. ( from my point of view a 3s setup on a board won't get you faster than pushing speed )
```

---
## \#4 Posted by: tueboard Posted at: 2016-09-16T12:10:35.579Z Reads: 151

```
sorry, do you know if there is any option to check the voltage with the balance charger if get the error when i'm trying to charge?

or the only way is to use a multimeter?
```

---
## \#5 Posted by: tueboard Posted at: 2016-09-16T12:12:06.928Z Reads: 152

```
yes, sorry i'm using 2x 3c batteries in series
```

---
## \#6 Posted by: 2-alex-2 Posted at: 2016-09-16T12:41:37.891Z Reads: 151

```
Then yes you low voltage is miles out 2x3s in series should be like 21v cut off. Or a little higher if you wan to be safer.
```

---
## \#7 Posted by: PB1 Posted at: 2016-09-16T12:52:47.185Z Reads: 147

```
next time you buy something, buy a so called lipo checker, they are not expensive! Or go to dx.com and order some now. 
This allows you to quickly check each cell using the balance port. 

If you don't have a lipo checker or volt meter, connect the battery to your charger, select low amps to charge (e.g. 0.5amps) and start charging. 
Then your charger should show you (somewhere) the voltage of every cell. If you're very lucky you might be able to bring your battery back to life. But please: WATCH IF WHILE CHARGING!

Any yes, with the above VESC settings your will successfully destroy every battery pack you have. You might even destroy your board. Battery cutoff start and end are far too low!!!!
```

---
## \#8 Posted by: susplus Posted at: 2016-09-16T13:32:32.664Z Reads: 133

```
a LiIpo Checker is about 2.5 euros. they are great and will act as a safety net if any of the cell voltages drop. The vesc works only with the whole voltage and does not keep count of cell voltage. making the Lipo Alarm a must ;) you are lucky though that the battery did not explode :) have a drink to that 
just change the cut off end to 21V as 2-alex-2 said and cut off start at 22.5v and you should be ok for the future. When the  battery voltage will drop to 22.5v you will feel it. The board will not have as much power ;)
```

---
## \#9 Posted by: karma Posted at: 2016-09-16T16:02:54.132Z Reads: 128

```
You can check voltage of individual cells on the balance charger, look it up!
```

---
## \#10 Posted by: tueboard Posted at: 2016-09-17T10:30:22.323Z Reads: 110

```
@PB1 @susplus i want to try 2 batteries in series each one with 6S, 8000mAh, 22.2V, 35c do you know if the cut off end cut off start shoud be the same? thank you
```

---
## \#11 Posted by: PB1 Posted at: 2016-09-17T10:41:28.313Z Reads: 107

```
No,  they should not be the same.  
Cut off start is the soft setting.  If your batteries are at that level,  the VESC limits the amps it draws and you can only ride slowly.  

Cut off end is the hard setting.  If your batteries drop to this level,  the VESC limits amps to 0 and you have to walk.  

It depends on how conservative you want to be with your batteries.  I've set my vescs to 3.4v and 3.1v per cell which is very conservative.
```

---
## \#12 Posted by: susplus Posted at: 2016-09-17T11:37:46.398Z Reads: 104

```
@PB1: actually 3.1 is way to low for a LiPo...you will kill their life....3.3V is the most minimum you should have....

I have set mine to 3.5v start and 3.3v end. But my lipo alarm will set off at 3.4 just to be sure. 

@miquelcamps i do not recommend having both of them at the same value although you can do it. It will simply mean that once it will hit that value you simply have to push ( just as PB1 mentioned )  i do recommend having them at least 0.2v apart. This way you will feel that the board is not pushing with the same power and that your batteries are going dry. Maybe stop before it reaches that point....( it will prolong you battery life) 
just make sure to make the calculation: 12s means= 39.6V cut off end ( for a 3.3v per cell )
```

---
## \#13 Posted by: PB1 Posted at: 2016-09-17T12:31:02.748Z Reads: 97

```
@susplus, yes you are rigth. 3.5v and 3.3v are probably better values to extend the battery life.


And definately a lot better than 10v and 8v at 6s ;-)
```

---
## \#14 Posted by: stealth71 Posted at: 2016-09-17T13:02:34.585Z Reads: 100

```
No reason to run lipos below 3.65V per cell.  Keep them between 3.65 and 4.2 and you should be fine.  People over discharge them all the time, but the data shows 3.65 is where they take a big drop.

Also make sure the charger is on constant balance if it has that mode.  My Turnigy Reaktor has constant balance mode, but you have to turn it on.
```

---
## \#15 Posted by: tueboard Posted at: 2016-09-17T13:38:55.202Z Reads: 102

```
thank you for all your comments, I hope not to break the batteries this time
```

---
## \#16 Posted by: tueboard Posted at: 2016-09-19T17:21:00.591Z Reads: 82

```
so do you recommend this config?

battery cutoff start 45,30v (3.65v*12s)+1,5v
battery cutoff end 43,8v (3.65v*12s)
```

---
## \#17 Posted by: stealth71 Posted at: 2016-09-19T17:28:54.413Z Reads: 83

```
I am still working on determining the best cutofff voltage.  I noticed riding this weekend that the voltage sag makes me hit the low cut off towards the end of my ride.  I would start there to be safe and see what your range is like.  I had mine set to start 45V and end 43.40V.
```

---
## \#18 Posted by: Okami Posted at: 2016-09-19T19:41:34.171Z Reads: 71

```
https://www.youtube.com/watch?v=pljSZcEwc8Q
```

---
