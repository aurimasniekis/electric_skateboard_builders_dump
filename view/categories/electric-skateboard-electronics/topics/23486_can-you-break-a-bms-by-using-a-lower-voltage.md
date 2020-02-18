# Can you break a BMS by using a lower voltage?

### Replies: 32 Views: 1381

## \#1 Posted by: Jinra Posted at: 2017-05-19T17:55:03.934Z Reads: 92

```
The reason I ask is because i adjusted my charger to output 41.2v (10s) and charged my board a couple of times. However now when i charge with my 42v charger the bms only outputs 40.8v. I tested the charger and it outputs 42.3v
```

---
## \#2 Posted by: longhairedboy Posted at: 2017-05-19T18:01:49.751Z Reads: 90

```
oh that's interesting... 

Which BMS is it? one of the Battery Supports ones?
```

---
## \#3 Posted by: Jinra Posted at: 2017-05-19T18:07:50.062Z Reads: 90

```
This cheapo one. I broke one before, but that was totally my fault.

https://www.aliexpress.com/item/Free-Shipping-36V-10ah-battery-BMS-3-7V-18650-li-ion-cell-10S-BMS-PCB-PCM/32283661813.html?spm=2114.13010608.0.0.q9tQGW
```

---
## \#4 Posted by: Namasaki Posted at: 2017-05-20T01:12:08.926Z Reads: 73

```
My guess is that it's more likely that your battery just got out of balance because of undercharging and now can't charge fully because its too far out of balance.
Happened to me once when I replace 2 cells that where out of balance with the rest.
```

---
## \#5 Posted by: saul Posted at: 2017-05-20T01:17:48.284Z Reads: 70

```
could be a few things, but really 1.2v/10 is only .12V per cell. you won't be losing any real capacity.
the cells are probably just wearing down a bit, so the bms is doing its job! 

I'd be more worried if it were just spiting out the same voltage you put in.
```

---
## \#6 Posted by: Jinra Posted at: 2017-05-20T01:30:21.561Z Reads: 69

```
I'm 100% sure this isn't normal. These cells are nearly brand new. 9 of the cell groups are at 4.08v and the other one (#7) is at 4.17.

@Namasaki I guess I'll try discharging the higher voltage cell group (above). It's not that far off so I don't think that'd be causing the problem. I don't have anything to discharge it with so I'll maybe ride and charge to see if it rebalances.
```

---
## \#7 Posted by: Jinra Posted at: 2017-05-20T01:32:46.757Z Reads: 65

```
Oh one more thing guys. My BMS has P-/B-/C-, along with 11 balance wires (1 negative 10 positive). I got the balance leads hooked up correctly and I removed P- (bypassing BMS) and have C- to my charger, but I'm wondering if I even need B- hooked up (currently is) to battery negative since I'm bypassing. Wouldn't it just charge through the balance leads since there's a negative there as well?
```

---
## \#8 Posted by: Namasaki Posted at: 2017-05-20T01:33:07.899Z Reads: 59

```
It's not that far off but it could be enough to keep you from going full charge.
```

---
## \#9 Posted by: Namasaki Posted at: 2017-05-20T01:36:03.043Z Reads: 57

```
sounds feasible since there is a ground wire on the balance port.
You could try disconnecting it and charging it stopping when the pack hits 42v  and then check for balance.
I think if you manually balance down your high cells, you will be able to do a full charge with the bms.

I gotta go take my grandson to Gamestop.  Be back in a bit.
```

---
## \#10 Posted by: Jinra Posted at: 2017-05-23T04:34:20.863Z Reads: 50

```
@Namasaki @longhairedboy @saul

To loop back on this and for anyone curious, it seems like yes.. you can break (some) BMS's by using lower voltage.

<img src="/uploads/db1493/original/3X/6/1/610221f8d403f4b662c71babbb4a6c6ac793cf65.png" width="469" height="177">
```

---
## \#11 Posted by: saul Posted at: 2017-05-23T04:51:51.263Z Reads: 48

```
well I think thats more because you could not get a full charge with lower voltage.

from what i'm seeing with these cheap bms', they can work on various size batteries, they're all 12s, but you can just leave others unconnected because all the cell circuits are running in _parallel_.
```

---
## \#12 Posted by: Jinra Posted at: 2017-05-23T04:53:21.568Z Reads: 47

```
Sure, but I used a 42.2v charger afterwords and the charger thought it was full at 40.8v, can't get any higher.
```

---
## \#13 Posted by: Namasaki Posted at: 2017-05-23T05:12:12.838Z Reads: 43

```
[quote="Jinra, post:12, topic:23486, full:true"]
Sure, but I used a 42.2v charger afterwords and the charger thought it was full at 40.8v, can't get any higher.
[/quote]

Thats most likely because your cells are out of balance from undercharging.
I have experienced the same thing when one of my packs where out of balance.
In this situation, you'll have to go in and balance cells manually to get it back on track.
I don't know if undercharging can break a bms, it seems highly unlikely, however it's pretty evident that a bms can't really do it's job without a full charge.
```

---
## \#14 Posted by: Jinra Posted at: 2017-05-23T05:14:45.790Z Reads: 35

```
Isn't that the point of the BMS though? To bring your cells back to balance? My understanding is that while it's charging and a module hits the cell voltage threshold (4.2v) it'll charge the module with a trickle current while the other packs catch up. Right now one module is at 4.2v, one is at 4.17v and the others are at 4.1v. 

I get what you're saying about needing to manually balance, but i only charged it with 41.2v like 3 times, it's weird to see it this out of balance and I feel like the BMS should be the one balancing the pack for me.
```

---
## \#15 Posted by: Namasaki Posted at: 2017-05-23T05:15:19.643Z Reads: 35

```
[quote="saul, post:11, topic:23486"]
from what i'm seeing with these cheap bms', they can work on various size batteries, they're all 12s, but you can just leave others unconnected because all the cell circuits are running in parallel.
[/quote]

The balancing circuit has to be in series to work and to balance each cell or cell group.
What would happen if you took cells that are connected in series and then connected them to the balance circuit  in parallel.
I don't think that would work. I think it would cause a short circuit.
```

---
## \#16 Posted by: Namasaki Posted at: 2017-05-23T05:26:18.798Z Reads: 33

```
[quote="Jinra, post:14, topic:23486"]
Isn't that the point of the BMS though? To bring your cells back to balance?
[/quote]


Yes it most certainly is but I think you need to do a full charge for it to work properly.
```

---
## \#17 Posted by: Jinra Posted at: 2017-05-23T05:45:47.684Z Reads: 37

```
Right and that's what I'm saying, I'm plugging in 42.2v now, and it stops at about 41v. Currently, all modules are at 4.1v besides 1 which is at 4.2v. I would've assumed it would slow charge that higher pack while charging the rest. It's not really **that** out of balance.
```

---
## \#18 Posted by: Namasaki Posted at: 2017-05-23T06:12:20.474Z Reads: 36

```
I've tried several different chargers and found that the best charger to use with a bms is a lab power supply with CC/CV output. The way it works is amazing. 
It starts in CC mode with what ever amps I set the max to be and slowly brings up the voltage so that it stays just above the pack's voltage until it reaches the max voltage that I set, in my case 42v. At that point it automatically switches to CV and starts reducing charge current as the battery approaches 42v. 
So once the charge current falls below the bms balance current, (126ma for Bestech) and the battery shows 42v, the power supply will continue to provide low  current charge to to bring up the low cells while the bms continues to trim the high cells. Now it's working similar to the way a hobby charger works.
```

---
## \#19 Posted by: Jinra Posted at: 2017-05-23T06:39:07.932Z Reads: 33

```
That does sound nice, but I like the sleek & simple solution that a laptop style charger gives you. I guess I've just yet to find a high quality, reliable, BMS in a tiny form factor.
```

---
## \#20 Posted by: Namasaki Posted at: 2017-05-23T07:04:54.886Z Reads: 33

```
Well, good luck with that search 😁
```

---
## \#21 Posted by: Jinra Posted at: 2017-05-25T02:24:51.072Z Reads: 25

```
Small update:

I came back from a ride and bizarrely, the group that was .1v higher than the rest is now .1v **lower** than the rest; 3.6v on 9 packs and 3.5v on the outlier. I wonder what may cause this kind of behavior..?

The only thing I can think of is that 1 of the cells in the 4p group is not connected and therefore charges faster than the rest and depletes more than the rest. However, I checked the connections on all cells in the group and it's all reporting 3.5v.
```

---
## \#22 Posted by: Namasaki Posted at: 2017-05-25T04:19:22.834Z Reads: 25

```
Could be a variance in the internal resistance of the cells.

Still, I would not loose any sleep over 1/10 of a volt per cell group.

Sounds to me like your pack is discharging very evenly.

Are you discharging through the bms or bypassing?
```

---
## \#23 Posted by: Jinra Posted at: 2017-05-25T04:22:35.026Z Reads: 25

```
Yea I wouldn't either, but my pack never charges to 42v anymore. Always tops out at 40.8v which is about 94%.

I'm bypassing the bms for discharge. I think I'm just gonna chalk this up as busted BMS.

I just finished doing a full charge and now two OTHER modules are at 4.17 and the rest are 4.07-08.
```

---
## \#24 Posted by: Namasaki Posted at: 2017-05-25T04:26:04.275Z Reads: 26

```
Still only off by 1/10 of a volt.

I suspect this has more to do with the charger than the bms.

I think your charger is just shutting off prematurely
Especially if your using one of those 2a  $12 chargers
```

---
## \#25 Posted by: Jinra Posted at: 2017-05-25T04:26:42.574Z Reads: 26

```
Nah I've tried three chargers, which are all set to 42.2v.

2 are 2A generic, and 1 is a seemingly high quality fast charger
```

---
## \#26 Posted by: Namasaki Posted at: 2017-05-25T04:35:59.207Z Reads: 27

```
I had 2 $12 chargers and 1 5a charger from battery supports.  They all stop short. 
Now I 'm using my Lab power supply and I never have a problem getting a full charge.
My 5a BS charger is in the closet. I keep it around in case I travel. It would be a good travel charger.
```

---
## \#27 Posted by: Jinra Posted at: 2017-05-25T04:37:59.301Z Reads: 29

```
The only reason it'd stop short is if the BMS is reporting back that the voltage is matching the charger output (42.2v). I confirmed this by measuring the leads where it connects to the BMS and sure enough i got 42.2v. When I probe the side where the BMS goes to the battery I get 40.8v.

BMS's are confusing, haha. I'm ordering some BMS's from Bestech to replace this $15 thing.
```

---
## \#28 Posted by: Namasaki Posted at: 2017-05-25T04:39:52.532Z Reads: 29

```
Ok, sounds like you do have some issue with that cheap bms.
I bet you'll do better with the Bestech.  Mine have been rock solid.
And even though my chargers where stopping short, I was still getting 41.9 on the pack.
```

---
## \#29 Posted by: Jinra Posted at: 2017-05-25T06:07:01.941Z Reads: 27

```
Finally figured out the issue. I'm so dumb, just realized the BMS doesn't have a balance current, which means all it's doing is detecting a module is getting overcharged and shuts off charging. Ordering a couple BMS's from bestech with balance currents
```

---
## \#30 Posted by: Namasaki Posted at: 2017-05-25T15:33:47.338Z Reads: 24

```
LoL...
No wonder. 
Well there's another strike against those cheapo bms's
Your gonna love the Bestech with its 126ma balance current. Twice what batt sup offers. 
Did you order the 80a model with built in E-switch
Or which model did you order?
```

---
## \#31 Posted by: Jinra Posted at: 2017-05-25T15:38:55.990Z Reads: 24

```
Since I need a small one, my balance current is only 42ma, which I think I prefer since it gives the other modules time to catchup. I don't like the idea of turning on my board to charge so I'm bypassing the BMS. It's nearly impossible to find a high discharge BMS in a small form factor anyway. These are the two I picked up.

[one](http://batterybms.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D239.html)
[two](http://batterybms.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/BMS-D250.html)
```

---
## \#32 Posted by: Namasaki Posted at: 2017-05-25T17:39:02.198Z Reads: 21

```
Nice thing about Bestech besides their quality is that they offer such a wide variety of solutions.
```

---
