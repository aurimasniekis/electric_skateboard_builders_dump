# Help needed for failing batteries

### Replies: 24 Views: 3180

## \#1 Posted by: erikkondo Posted at: 2016-03-16T00:53:14.489Z Reads: 133

```
Hi Everyone,

I have a functioning DIY electric skateboard, but I am over my head electronically.
The problem I am having is that my batteries keep getting bloated and I need to replace them.
So far four batteries have failed at $50 per battery.

This is my setup:

1. Two parallel sets of two batteries in series  - ZIPPY Flightmax 4200mAh 4S2P 30C LiFePo4 Pack for a total of four batteries.<img src="/uploads/db1493/original/2X/5/5f1e95c19f1ce5859593ccd0e3abe35da0559330.jpg" width="666" height="500"> 
2. Motor - Turnigy Aerodrive SK3 - 6374-149kv Brushless Outrunner Motor
3. Transmitter = HobbyKing® GT-2 2.4Ghz 2Ch Tx & Rx 
4. Charger = iCharger 208B 350W 8s Balance/Charger
5. HobbyWing 1/8 Scale C-Xerun 150A Brushless ESC

I would appreciate any help I can get on resolving this problem.

Thank you.

Erik

Here is my Facebook Page
https://www.facebook.com/Wheelchairboarding/?fref=ts
```

---
## \#2 Posted by: claudiofiore88 Posted at: 2016-03-16T01:05:52.281Z Reads: 124

```
How many amps are you charging with? They're rated to be able to charge up to 2c, but I wouldn't personally charge more than 1c, so I'd charge at low amps like 4.2 amps or less (although I don't have experience with LiFePo4 batteries, only LiPos).  Maybe the LVC is set too low. Maybe you have an inefficient drive train, and you're drawing too many amps.  Do you have a watt meter to test it?
```

---
## \#3 Posted by: psychotiller Posted at: 2016-03-16T01:13:10.220Z Reads: 122

```
Usually, this happens from running your batteries to below their safe minimum voltage. I would change the low voltage cutoff on your esc. Then, don't ever run your board after the cut off has happened 

Charging too many amps can do it too. 

If you don't think it's either of these things, make sure you are unplugging your batteries after you ride
```

---
## \#4 Posted by: claudiofiore88 Posted at: 2016-03-16T01:18:33.834Z Reads: 122

```
[quote="psychotiller, post:3, topic:1838"]
make sure you are unplugging your batteries after you ride
[/quote]

Damn, that's the one I forgot to mention. lol
```

---
## \#5 Posted by: willpark16 Posted at: 2016-03-16T01:51:06.761Z Reads: 117

```
Go lipo, I know you're probably worried about catching fire or burning down ur lovely house but my friend has tried the lifepo4 from zippy and honestly i think that their specs are bullshit. Hes running it in a 6s setup but its riding like on a 4s(trust me we've tested it).
```

---
## \#6 Posted by: torqueboards Posted at: 2016-03-16T01:52:43.979Z Reads: 114

```
As @psychotiller mentioned usually this is running your batteries lower than expected. For example... LiPo's are 3v-3.2v low cut off. I cut them off at 3.6v and swap packs. I've found the packs last much much longer versus trying to stop them at 3.2-3v.
```

---
## \#7 Posted by: psychotiller Posted at: 2016-03-16T01:55:46.232Z Reads: 113

```
Yeah the only other thing I could suggest would be change lipo brands. I've had a couple of cheap packs puff up. ( not saying yours were cheap, but it could be a batch/type specific problem)
```

---
## \#8 Posted by: Sebastiaan Posted at: 2016-03-16T08:09:03.828Z Reads: 105

```
Gonna hijack this thread, Say if i put my cutoff at 36 volt. Does that mean when it's voltage under load?
I have an alien twin esc, just wondering about this. I always stop skating at around 37v
I have a 2 x 5s serie setup.
```

---
## \#9 Posted by: erikkondo Posted at: 2016-03-16T13:11:55.907Z Reads: 103

```

Thank you for your thoughts.
I have NOT been unplugging my batteries.
I will start doing so. Why does that matter?
```

---
## \#10 Posted by: erikkondo Posted at: 2016-03-16T13:14:43.801Z Reads: 101

```
Thanks. I will check the low cut off value.
```

---
## \#11 Posted by: claudiofiore88 Posted at: 2016-03-16T17:36:34.473Z Reads: 93

```
Because even if your esc is off it will continue to drain your batteries.
```

---
## \#12 Posted by: ex-Gooserider Posted at: 2016-03-16T21:34:21.993Z Reads: 96

```
Hi, 
First post, Erik pointed me at this forum, as I'm the guy that built the original board that he is using...  My personal suspicion about the reason for the battery problem (and I have told him this) is that he is exceeding the current draw rating for the batteries. 

The design for this board is a bit non-standard, as Erik is using the board while in a wheelchair.  Among other things this means that ALL the propulsion has to come from the motor, he can't help things along with a kick like a walking person can...  (Google for his videos, they are impressive!)

The Zippy batteries that he is using were picked to match a different setup that we changed mid build to solve some issues with the original design plan.  They are theoretically spec'd at 30C discharge, but that is ONLY a peak rating, the steady discharge should ideally be kept under 10C.

My original build used 3 batteries in parallel, (thus 1S12P)  to give a theoretical 90C peak discharge, or 30C sustained.  Multiplying this by the 4.2Ah rating on the batteries is about 360A peak,  120A sustained, which is close to the rated output of the ESC, and even at peak load doesn't over strain the batteries.

After he had mastered the board at the (estimated) 8- 10mph that the original setup gave him, Erik decided he wanted more speed, and modified the box and wiring to the 2S8P configuration shown....  This means he only has 240A peak, and 80A sustained, which is running much closer to the ESC rated draw, and is also probably drawing a higher sustained current due to the higher speed...

I had suggested when Erik said that he wanted more speed, that the proper approach would have been to keep the 3P wiring and add two more batteries to the 4 he already had so as to get a 2S12P pack which would have kept the current draw on the batteries within a more reasonable range.

Incidentally, I was the person that suggested using the LiFePO4 batteries instead of LiPos, for safety reasons - While LiPo fires are fairly rare, when they happen they are bad news indeed, and being in a wheelchair limits the 'RUN AWAY' options...  OTOH, the LiFePO4 batteries are much safer, they are less prone to failures and when they do fail it is less catastrophic...

ex-Gooserider
```

---
## \#13 Posted by: erikkondo Posted at: 2016-03-16T23:18:21.904Z Reads: 86

```
So, you want me to order 2 more batteries for a total of six.
Then make 3 parallel sets of 2 in series, correct?
```

---
## \#14 Posted by: ex-Gooserider Posted at: 2016-03-16T23:54:32.279Z Reads: 85

```
In essence yes...  Hopefully you haven't done enough damage to the ones you have now to be an issue.

Also look at some of the other suggestions about low voltage cut off values, I seem to remember we had set them on the low side initially because the ESC seemed to be tripping out earlier than it ought to.  Might be worth bumping them back up a bit.  

ex-Gooserider
```

---
## \#15 Posted by: torqueboards Posted at: 2016-03-17T01:47:12.534Z Reads: 84

```
Go for higher voltage. Your packs and setup will run better with higher voltage initially then increasing amps for more power. 8S5ah, 10S5ah, etc..

LifePo4 aren't worth it IMO. Top cell voltage is 3.7v is less so you'll have to run a bigger pack.

LiPo's are perfectly fine just don't abuse them and make sure the cell voltages are in the same range. Charge to 4.15-4.18v and discharge up to 3.7-3.6v for longer living. Get at least a 20C or 30C cell.
```

---
## \#16 Posted by: RogerD Posted at: 2016-03-17T08:40:32.181Z Reads: 78

```
It's easy to diagnose.

If you are drawing too much current the batteries will get hot to the touch. Under normal use they should stay cool, and get mildly like warm when nearing empty. If they do not get hot you are not over drawing them.

Meter the resting voltage to see if you are running them too low. That will tell you straight away.

Those are the two main causes of puffing.

Overcharging is the last,  but uncommon.
```

---
## \#17 Posted by: erikkondo Posted at: 2016-03-18T23:24:09.421Z Reads: 68

```
I checked the value on the ESC is was Custom 10.7 volts.

There are 4 cells per battery, so does that make 10.7/4 = 2.675 per cell?
There are options to select:

3v/cell
3.2v/cell
3.4/cell

What do you suggest?
```

---
## \#18 Posted by: torqueboards Posted at: 2016-03-19T02:38:11.938Z Reads: 65

```
Those packs also looked squeezed in there. The packs need a bit of room even very small to expand a bit when discharged.

What are the voltages of each of your packs or a few of your packs? Voltage of each cell.
```

---
## \#19 Posted by: ex-Gooserider Posted at: 2016-03-19T03:09:20.042Z Reads: 64

```
I'd look at what the voltage is when you are stopping riding.  It is far less of a concern with a lithium pack, but there is still SOME voltage drop under a heavy load...  The ESC is sort of 'stupid' and cuts out as soon as it sees a voltage below the shutoff value, even for a fraction of a second.

My recollection is that when we were doing testing with the original setup of three batteries in parallel,  we were getting problems after a very short time of the ESC shutting off with a low voltage error when trying to start off.  If we then put the batteries on the charger, they would only take a small charge.  Alternatively if we just power-cycled the ESC, it would work again for a while.  

Lowering the cutoff voltage seemed to reduce the problem, and I cautioned you about not running the batteries to low, particularly that you needed to stop as soon as the board seemed to lose power...

I'd try bumping it back up to 3.2V cell and see if that early cutoff problem returns.  If it does, cut back to 3.0V.  It may also be worth getting one of the battery voltage monitors that you can find for a few bucks on e-Bay and making it alarm at 3.2V and see what happens...

ex-Gooserider
```

---
## \#20 Posted by: trbt555 Posted at: 2016-03-19T08:21:30.351Z Reads: 60

```
In my experience for high current draw applications, you need to cut off above 3.2V per cell if you don't want to damage them.
The discharge curve at that voltage is so steep you will most likely end up over-discharging one or more cells due to slight unbalances if you don't.
Check out the graphs I made to determine my cutoff voltage [here][1].
If voltage sag under load is giving you premature cutoff issues you need more capacity.


  [1]: http://www.electric-skateboard.builders/t/loaded-dervish-dual-r-spec-6355-dual-vesc-nunchuck-paris-195-90mm-flywheels/524/62?u=trbt555
```

---
## \#21 Posted by: erikkondo Posted at: 2016-03-19T09:59:37.062Z Reads: 59

```
I need to make a new battery carrier.
Any suggestions? I can put it on top of the board so I have lots of room.
BTW. I just ordered a motor mount from you.
```

---
## \#22 Posted by: erikkondo Posted at: 2016-03-19T10:00:54.712Z Reads: 59

```
I will try changing the cut off as suggested.
```

---
## \#23 Posted by: torqueboards Posted at: 2016-03-19T20:00:39.705Z Reads: 55

```
@Erikkondo - You can use one of those waterproof enclosures on the top of your deck similar to the ones that you say EMTB's using. Some of them are bigger and you can have a higher increase in height.
```

---
## \#24 Posted by: jesser722 Posted at: 2016-09-03T16:38:14.049Z Reads: 38

```
Sorry to bring this up again, but I am having a similar problem with 2 5000 mah 20c lipo batteries and it is driving me crazy. I have them wired up in series and had a charging cord also connected to them. The first set i had puffed up and then this set puffed up too. I saw that you are supposed to disconnet the cords after riding? So I am supposed to take apart the board every-time i want to charge? Thanks,
 Jesser722
```

---
