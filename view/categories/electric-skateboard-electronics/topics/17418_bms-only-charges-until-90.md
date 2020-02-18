# BMS only charges until 90%

### Replies: 34 Views: 2941

## \#1 Posted by: Eboosted Posted at: 2017-02-09T01:06:41.425Z Reads: 207

```
I'm not sure if my BMS is ok but, If I plug my 42V 2A charger the battery metter quickly raises to 100% if I unplug it, it goes down to 90%

The max voltage I can charge the pack is 40V instead of 42V
.
Any ideas?
```

---
## \#2 Posted by: smurf Posted at: 2017-02-09T01:20:47.018Z Reads: 204

```
Have you double checked with a volt meter?
```

---
## \#3 Posted by: Eboosted Posted at: 2017-02-09T01:39:43.445Z Reads: 199

```
Yes the 10S battery pack has only 40.5V at the end of the charge. Maybe I need to use a charger with more than 42V 2A
```

---
## \#4 Posted by: PXSS Posted at: 2017-02-09T02:09:21.144Z Reads: 192

```
Is it going up to 42v while charging and then coming down or just stopping at 40.5?
```

---
## \#5 Posted by: smurf Posted at: 2017-02-09T02:14:17.282Z Reads: 189

```
It's not necessarily a bad thing as stopping at 41V is good for battery health in exchange for a small loss in capacity.
```

---
## \#6 Posted by: Pantologist Posted at: 2017-02-09T02:35:40.271Z Reads: 188

```
Did you check the voltage of each parallel pack? Make sure there isn't a dud or disconnected balancing connector.

If it's just a simple voltmeter, then it will be skewed by the current from the charger.
```

---
## \#7 Posted by: michaelcpg Posted at: 2017-02-09T02:47:47.380Z Reads: 185

```
The charger may still actually be charging when the battery meter hits 100% while plugged in. Mine does this. 

Essentially, when you're plugged in charging, your battery meter will show that the level of charge is higher than it actually is. My battery meter usually shows its at 100% when the charge gets up to around 90% but the charger will keep charging until the BMS cuts off the circuit when the battery is actually fully charged.

I agree with @smurf though, charging your board closer to 90% or less each time rather than fully charging it every time is a good idea as long as you don't need the full range of your battery as it'll help increase the life of the battery.
```

---
## \#8 Posted by: Eboosted Posted at: 2017-02-09T03:13:09.378Z Reads: 180

```
@Pantologist yes I check the charge if each pack.

There is a difference in one pack that holds a lower voltage than the other 9, for instance while all the packs have 3.794V the bad one only sees 3.685, there is a difference 0.11V, not sure if this has something to do with the fact it doesn't reach 42V
```

---
## \#9 Posted by: Pantologist Posted at: 2017-02-09T03:33:13.655Z Reads: 174

```
Wel, it probably does not start balancing until it reaches 42v... How long did you leave it charging? Is it actually stopping the charge current at ~40V?
```

---
## \#10 Posted by: Eboosted Posted at: 2017-02-09T05:36:37.632Z Reads: 176

```
The charger I'm using is the Evolve one with 42V 2A, it has a led that turns green once it reaches 42V.

I'm not sure what the oroblem is buy the BMS might stop charging/balancing when it detects  an unbalanced pack, maybe, maybe not.
```

---
## \#11 Posted by: Pantologist Posted at: 2017-02-09T05:48:57.240Z Reads: 170

```
I am pretty sure Evolve charger's cut off at a lower voltage to improve battery charge cycles. 

http://www.electric-skateboard.builders/t/cheap-chargers-with-customizeable-end-of-charge-voltage/6902/14?

@whitepony might know.
```

---
## \#12 Posted by: Eboosted Posted at: 2017-02-09T05:53:03.342Z Reads: 166

```
I also have @barajbali charger it also goes up to 42V @ 2A, samething happens, stops charging at 40.5V
```

---
## \#13 Posted by: Alextech Posted at: 2017-02-09T06:01:47.558Z Reads: 166

```
What BMS do you have? Some BMS cut off voltage at 4.25v and do not allow the other packs to reach full voltage.
```

---
## \#14 Posted by: Eboosted Posted at: 2017-02-09T06:18:53.967Z Reads: 160

```
I have the battery supports 10S 60A BMS, I couldn't find the charging strategy of this particular BMS.

Tmorrow I'll messure the voltage of each cable of the BMS disconnected from the battery to see if any wires are not giving me the correct voltage
```

---
## \#15 Posted by: Namasaki Posted at: 2017-02-18T04:52:10.733Z Reads: 143

```
I had a similar problem with my setup when I replaced one of my 5 Lipo packs. It had a storage charge and the rest of the packs where higher. My bms and charger would not fully charge the system but would stop short of a full charge. So I got my hobby charger out and balance charged each of the five packs separately matching them in voltage and then reconnected them to the bms. It worked fine after that.
```

---
## \#16 Posted by: Eboosted Posted at: 2017-02-18T06:05:18.088Z Reads: 138

```
I've been battling with this problem for weeks, but everyday it was charging more and more until 3 days it reached 100%.

I opened the battery cover and measured the voltage of each pack:

1. 3.74
2. 3.74
3. 3.74
4. 3.76
5. 3.77
6. 3.78
7. 3.66
8. 3.77
9. 3.67
10. 3.79

Cell 7 is always below average by 0.12V, it'd say that's acceptable.

I wonder what'd happen if I discharge each pack, but the lowest one, individually until I get the same voltage, in other words, balance all packs?, I may have to do that sometime.
```

---
## \#17 Posted by: Namasaki Posted at: 2017-02-18T13:30:40.931Z Reads: 137

```
Try charging them indavidually to 100% to balance them and then reconnect the BMS.
```

---
## \#18 Posted by: JohnnyMeduse Posted at: 2017-02-18T18:53:49.834Z Reads: 138

```
do you have a little indicator light on your charger.... if so follow it (wait until it is green, and then wait to see if it flashes in the balancing phase), but don't believe you lcd.

edit: sorry just read the entire thread... try a other charger...
```

---
## \#19 Posted by: Eboosted Posted at: 2017-02-19T04:01:47.735Z Reads: 134

```
I have 3 chargers, it was doing it on all three of them
```

---
## \#20 Posted by: michaelcpg Posted at: 2017-03-05T21:48:03.289Z Reads: 135

```
Did you get this sorted in the end? Think I'm starting to get a similar issue as my board is only charging to around 93% atm. Probably because I haven't bothered to fully charge the battery and let the BMS balance the cells for several months...
```

---
## \#21 Posted by: Namasaki Posted at: 2017-03-05T22:14:02.489Z Reads: 128

```
I have been having a similar issue with my setup using brick chargers. My 10s pack would only get up to 41.8 or 41.9 and the charger would switch off and the green light would come on. At first I wasn't sure if it was the BMS limiting the charge or the chargers.
So I got a Lab power supply with CC and CV variable output up to 60v and 5a, connected that to the charge port and set it at 42v and 5a and with that I was able to charge my pack to a full 42v. So I have concluded that the brick chargers just can't do the job completely.
Since I am using five 2s Lipos in series and they are easily replaced, I am more concerned about getting maximum performance and range than longevity of the batteries.
<img src="/uploads/db1493/original/3X/7/9/791cdee632cad64b2e152de0ce22a56a33c032b1.jpeg" width="666" height="500">
```

---
## \#22 Posted by: michaelcpg Posted at: 2017-03-05T22:46:47.207Z Reads: 121

```
Hmm ok interesting to know. I just find ita bit strange in my case because I've never had issues in the past with this charger when charging to 100%
```

---
## \#23 Posted by: Eboosted Posted at: 2017-03-05T22:54:32.936Z Reads: 121

```
You need to measure the voltage of each individual pack, if one of them has a lower or higher charge than the others then the pack is unbalanced and a regular charger would have a hard time keeping charging constant, you would need a better (more capacity) charger as stated by @Namasaki 

The other option would be to manually balance each individual pack, after you do that, you will be able to charge fully 100% 42v with just a regular brick charger
```

---
## \#24 Posted by: michaelcpg Posted at: 2017-03-05T22:59:36.200Z Reads: 121

```
Thanks for the input. I'll pull the battery apart tonight and test the voltage on each pack. Fingers crossed I'll just need to manually charge each pack to balance them out again.
```

---
## \#25 Posted by: Skitzor Posted at: 2017-03-08T19:05:22.059Z Reads: 115

```
Facing the same issues. Charging only to 90%. Which would be an alternative charger, but not ridiculously expensive as a lab power supply :smiley:.

Background info. Enertion Space cell 3 and as well the slow as fast charger do this ...  Other space cell 3 is still charging fine with the same chargers
```

---
## \#26 Posted by: Eboosted Posted at: 2017-03-08T20:59:49.648Z Reads: 108

```
If you guys take appart your batteries you will see there's one invidividual pack with more voltage than the others, this was my battery a couple of nights before on my 10S4P with Samsunh 25R and Battery Supports 37V 60A BMS.

Pack 1: 40.1
Pack 2: 40.0
Pack 3: 40.1
Pack 4: 40.1
Pack 5: 39.9
Pack 6: 40.2
Pack 7: 40.0
Pack 8: 41.9

As you can see the last pack has way more charge than the others, I have no idea why this happens, but BMS sees the voltage on everypack and if some of those reach 42V it stops charging, even though the 42V as a full pack hasn't been reached, in order to protect the higher cells from overcharging.

I left the board on overnight with the charger plugged in and at the next day the board had 100% charge again, when it reached 100% the charger still had the red led indicating it was still working/charging/balancing. This time BMS did it's job, but I still need to check the voltage of each pack again.
```

---
## \#27 Posted by: Namasaki Posted at: 2017-03-08T21:07:26.611Z Reads: 106

```
Note that the battery supports BMS has a very low balancing current (less than 100ma) so the balancing process is bound to be very slow.
```

---
## \#28 Posted by: Namasaki Posted at: 2017-03-08T21:14:48.179Z Reads: 102

```
Some BMS modules like the one from Bestech will keep your cells close to balanced during discharge. 
I don't know if the battery supports does but if so, it would be a good reason to not bypass during discharge.
```

---
## \#29 Posted by: Eboosted Posted at: 2017-03-08T23:13:28.543Z Reads: 99

```
If balancing during charging is good enough, I don't see a point to balance them during discharge, at least not as importantant as charging
```

---
## \#30 Posted by: Namasaki Posted at: 2017-03-08T23:40:55.847Z Reads: 98

```
Maybe not as important, and definitely not when using a hobby charger because of their excellent balancing ability. But as we are finding out, onboard BMS circuits do not seem to have as good of a balancing circuit as hobby chargers. At least that has been my experience even when using a quality BMS. 
IMO, that makes keeping our cells in balance all the time more important.
```

---
## \#31 Posted by: Namasaki Posted at: 2017-03-08T23:48:48.117Z Reads: 96

```
Then again, when I think about it, how do I know my BMS is keeping my cells balanced during discharge and it's not just that they're depleting evenly because they are well matched?
```

---
## \#32 Posted by: PXSS Posted at: 2017-03-09T00:00:08.719Z Reads: 93

```
What BMS do you have @Namasaki? BMSs with discharge balancing are extremely complex as they need a processor to read in all the voltages and open and close switches in order to keep cells balanced. How much did you pay for it?
```

---
## \#33 Posted by: Eboosted Posted at: 2017-03-09T00:19:03.587Z Reads: 90

```
I think he has the Bestech BMS, pretty good one but not available in USA just China, so shipping/waiting is always a PIA, it's kinda pricy but a good buy IMHO
```

---
## \#34 Posted by: Namasaki Posted at: 2017-03-09T01:19:30.288Z Reads: 89

```
This is the one I use. The sales Rep told me that they keep the batteries balanced continually when it's turned on. 
I have noticed that when braking down a steep hill on a full battery and watching my voltage meter that the voltage would climb but not go over 42.3 and when I let off the brakes and coast the battery would step back down until it got to 41.9 where it would stay. 

http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
```

---
