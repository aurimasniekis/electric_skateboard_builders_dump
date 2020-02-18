# Flipsky FSESC 6.6 over voltage during braking

### Replies: 19 Views: 410

## \#1 Posted by: ElectricCoast Posted at: 2018-12-13T03:25:47.109Z Reads: 131

```
Hey guys  having a problem when I have my battery freshly charged.  With the known issue of the voltage reading fluctuations with the Flipsky 6.6 singles and duals has anyone else experienced braking loss basically no brakes due to an over-voltage error. This is happening to me on one of my builds but only when the battery is fresh. Once the battery has drained down some of its voltage or capacity the braking issue goes away.  My question for you more experienced individuals is, is there a workaround for this issue?
```

---
## \#2 Posted by: deltazeta Posted at: 2018-12-13T03:56:45.152Z Reads: 125

```
@Winfly <del></del>
```

---
## \#3 Posted by: Winfly Posted at: 2018-12-13T04:23:46.765Z Reads: 123

```
This literally happened to me today. Are you running 12s or 13s, bypass bms? I'm on 13s charge only bypass bms with 2x 6.6 singles. I was going down a 14% grade hill and I suddenly remembered that I was on a full charge battery so I foot brake down the hill instead. Didn't get any cutout tho. maybe cus I caught it early. It can also be your bms that's cutting out the power.



![image|233x500](upload://jUulSDFol0EEiVogsPbRrzKUNCv.jpeg)
```

---
## \#4 Posted by: lrdesigns Posted at: 2018-12-13T04:28:50.898Z Reads: 111

```
What is your battery voltage and your max voltage set in vesc tool?

If you run the "no hardware limits" firmware you can turn up max voltage to 59v but that might be a bad idea if the vesc does not have accurate readings. Could result in more than 60v in use. :boom: :ambulance:
```

---
## \#5 Posted by: ElectricCoast Posted at: 2018-12-13T05:10:35.193Z Reads: 100

```
 Running 12s FOC.  Charge only BMS.
```

---
## \#6 Posted by: lrdesigns Posted at: 2018-12-13T05:16:32.181Z Reads: 99

```
Is max voltage set at 57?
```

---
## \#7 Posted by: Winfly Posted at: 2018-12-13T05:18:11.768Z Reads: 97

```
I'm using no_hardware_limit and default max_voltage at 57. And I didn't experience any cutout before I switched to footbrake.
```

---
## \#8 Posted by: ElectricCoast Posted at: 2018-12-14T03:34:12.982Z Reads: 78

```
Max voltage is set at 57.  Where do I confirm that no hardware limits setting?  Can I find that using METR pro or do I need to crack open the enclosure and plug in via USB?
```

---
## \#9 Posted by: ElectricCoast Posted at: 2018-12-14T03:40:55.821Z Reads: 79

```
BTW I'm running sensored TB 6380's 170 kv if you need to know that.
```

---
## \#10 Posted by: lrdesigns Posted at: 2018-12-14T03:42:01.319Z Reads: 77

```
Its not a setting, its a version of the firmware that does not have software limits. Its a use at own risk type deal.  You have to re-load the firmware to take advantage of it.  

![image|690x463](upload://yWw5YovVuxGdahBozhYVLKyMnfO.png)
```

---
## \#11 Posted by: ElectricCoast Posted at: 2018-12-14T03:43:38.269Z Reads: 69

```
Ahh ok..  Sorry I wouldn't consider myself an expert at Vesc related items.
```

---
## \#12 Posted by: lrdesigns Posted at: 2018-12-14T03:44:46.135Z Reads: 68

```
No need for sorry, hope I didn't sound rude, just trying to help. Yeah it can be confusing. Cheers. 

If you do load it, just be carefull.
```

---
## \#13 Posted by: ElectricCoast Posted at: 2018-12-14T03:45:54.598Z Reads: 67

```
Oh no you did come across as rude.  I would consider myself a noob when it comes to the software.
```

---
## \#14 Posted by: ElectricCoast Posted at: 2018-12-14T03:50:26.094Z Reads: 65

```
Going to install one of my unites in this board.  Move these 6.6's to my sons board.  I'm still trying to figure out and I think I do need to remove my antispark switch and come directly off my battery for my unity and utilize the smart switch in it.  Sorry I just ventured off subject.
```

---
## \#15 Posted by: Deodand Posted at: 2018-12-14T03:52:00.847Z Reads: 66

```
yeah remove the anti-spark for sure. 2 switches is just more wasted energy and failure points. Keep me posted if the unity shows any over-voltage issues like the 6.6 is showing.
```

---
## \#16 Posted by: lrdesigns Posted at: 2018-12-14T04:03:45.280Z Reads: 64

```
57v/12 cells = 4.75v average, that is quite high and not normal. 

Is that just from a short brake or like a really big hill? Or at like max speed down hill then brake?

I think it probably has to do with funky voltage reading of the fesc 6.6 and is not the actual real battery voltage.

But it could also be a bad battery. Probably not in this case. 

I think the work around would be 11s or 10s or only charge to 4.1 or no big hills on a full charge.
```

---
## \#17 Posted by: ElectricCoast Posted at: 2018-12-14T04:17:00.914Z Reads: 61

```
I do not suspect that it is a bad battery.  It's brand new build from Ernesto aka Kaly.  12s4p 20700b.  This problem only occurs when the battery is fully charged.  I can only be going 5-10-15 miles per hour it doesn't matter the speed.  I could have only traveled a matter of feet and the problem occurs.  as for the length of the braking it the problem pops up a fraction of a second after I hit the brakes. 

 I am fully confident that the battery is not experiencing the perceived over voltage.  I feel it has to do with the voltage fluctuation readings from the 6.6's.  Hopefully tomorrow morning I can get the 6.6's out of the board and remove the antispark switch and hook up my unity and give it a go.  We're expecting rain for all if not most of the day tomorrow so it may be Saturday before I can get back with you guys to inform you if the 6.6's are the cause.   My gut tells me that, this may be the cause. 

I'll be putting the 6.6's in my other MBS AT board and install the no hardware limits version of the software.  Going to 11s or 12s would be point less for me since i do not have 11s or 10s battery and i would prefer not to touch the battery I had Kaly build for me. :)
```

---
## \#18 Posted by: lrdesigns Posted at: 2018-12-14T04:24:41.448Z Reads: 55

```
If its not from large breaking events and happens from a small brake then its is from voltage spikes seen in the fsesc. More capacitors / better quality ones could help reduce the spikes. That and shorter wire length between the battery and esc. 

Im sure the unity will work flawless.
```

---
## \#19 Posted by: ElectricCoast Posted at: 2018-12-14T04:28:54.948Z Reads: 52

```
Cant get much shorter on the wire lengths.  The length is less than 6 inches.  Yeah I guess if the no limits hardware firmware doesn't fix the issue I'll build a cap bank but I really don't think the voltage spikes are real rather poor design by flipsky.  I can be sitting still and my Metr Pro will show my full battery bouncing between 95% and 100% with no input at all or load.  The board and all items are sitting static and it bounces all over the place.
```

---
