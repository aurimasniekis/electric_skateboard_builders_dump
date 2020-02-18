# Is it dangerous to use Lipo on E board?

### Replies: 21 Views: 1543

## \#1 Posted by: Ron189 Posted at: 2018-05-12T12:10:41.436Z Reads: 280

```
I want to use for my 12s electric skateboard project Lipo batteries, is it dangerous? Is it ok?
```

---
## \#2 Posted by: light-v Posted at: 2018-05-12T12:15:38.806Z Reads: 280

```
You have to be careful when charging (where 90% of lipo issues happen) and secure them from impacts. Avoid puncture damage at all cost. Other than that it's not as bad as some people say.
```

---
## \#3 Posted by: Orin635 Posted at: 2018-05-12T12:16:14.107Z Reads: 276

```
I use lipos and a imax b6 charger
```

---
## \#4 Posted by: Quezacotl Posted at: 2018-05-12T12:22:56.354Z Reads: 268

```
Not much dangerous than Li-Ion when considering the building of the pack. Actually in my opinion, easier to build, all you need is some soldering and being careful not to short them.
```

---
## \#5 Posted by: MysticalDork Posted at: 2018-05-12T12:36:31.965Z Reads: 257

```
Using lipos for esk8 is no more dangerous than using them for anything else. 

Be careful, don't do stupid shit and take reasonable precautions, and you'll be ok.

I recommend a BMS.
```

---
## \#6 Posted by: TehAtheist Posted at: 2018-05-12T13:30:47.815Z Reads: 233

```
If you take care of your board no issues should happen.
The risk of  using an E-board in general is much higher than the risk of damage by your lipos.
```

---
## \#7 Posted by: michichopf Posted at: 2018-05-12T14:34:49.398Z Reads: 212

```
Got lipos set up trough a bms. I am chargin also trough the bms with a regular 2a charger. Is that stupid?
```

---
## \#8 Posted by: Acido Posted at: 2018-05-12T16:10:28.867Z Reads: 192

```
As long they are in an enclosure its okay
IMO going liion i the long term is better
```

---
## \#9 Posted by: Acido Posted at: 2018-05-12T16:10:52.318Z Reads: 187

```
Its smarter than thru balance charger :D
```

---
## \#10 Posted by: MysticalDork Posted at: 2018-05-12T19:04:21.692Z Reads: 160

```
Erring on the side of safety is never stupid.
```

---
## \#11 Posted by: Brontech Posted at: 2018-05-12T19:31:55.809Z Reads: 152

```
I have two 6s lipos is series that have caused zero issues over a year and counting. Just buy a high quality lipo with a good charge/discharge and don't do any stupid stuff with the batteries and you should be fine.
```

---
## \#12 Posted by: b264 Posted at: 2018-05-12T20:02:27.988Z Reads: 147

```
Running at 12S on vesc-style hardware is more dangerous than running lipo instead of li-ion.  10S is a much more sensible choice if you don't like streetface.
```

---
## \#13 Posted by: Blitz Posted at: 2018-05-12T20:06:04.981Z Reads: 145

```
10s fanatic  :arrow_up:

[quote="b264, post:12, topic:55200"]
10S is a much more sensible
[/quote]
```

---
## \#14 Posted by: Mikaelj Posted at: 2018-05-12T21:12:08.475Z Reads: 139

```
Make sure they are identical, preferably the same batch, and that they are balanced equally (same voltage on all cells) between the connected batteries.
```

---
## \#15 Posted by: pixelsilva Posted at: 2018-05-13T15:53:37.890Z Reads: 112

```
We are literally....

![kicking-a-bomb|375x500](upload://alZH3kU9VM6Gd1TOKS2b77WyfmX.jpg)

...every day. But don't worry, 'as long as you don't do smthng stupid' you will be fineeeee. 😶
```

---
## \#16 Posted by: Ixf Posted at: 2018-05-13T16:18:30.212Z Reads: 106

```
I run Lipos on one of my DIY.
Figuring out charging is the only tricky part.
Otherwise I actually prefer lipo.
I can balance each individually cell not just group of cell.
I can muck with the battery configuration easily since its all plugs.

There are pros and cons to lipo and the danger is there but is easily mitigated by being careful and just generally knowing what you are doing
```

---
## \#17 Posted by: louwii Posted at: 2018-05-13T17:59:34.157Z Reads: 100

```
I use 2 5S lipos on my build. No problem at all. It's easy to assemble and cheaper to buy.
```

---
## \#18 Posted by: lrdesigns Posted at: 2018-05-14T01:57:09.460Z Reads: 89

```
Its not anymore dangerous than Lion if you treat them right. Actually most of the fires on this forum have been Lion. Physical damage or overcharge are the only time a fire is possible. 

The main downside is they are not as durable as lion, and very easy to over discharge which will bring them to an early grave. So you need to run individual cell alarm on lipo's in my opinion to guard against this. 

Good example of 12s lipo setup. 

https://www.electric-skateboard.builders/t/ceramic-surfer-arbor-highground-modular-flight-ready-12s-lipo-220wh-dual-5065-140kv-torque-218s-97mm-gt2b-commuter/30020/4?u=lrdesigns 

A bms is a good idea, but most charge to 4.2 and I like to charge mine to 4.1 to extend life cycles. Using a balance changer is just like having an external BMS with LCD readout, but its not as convenient as a BMS.
```

---
## \#19 Posted by: Ron189 Posted at: 2018-05-14T10:41:42.195Z Reads: 72

```
I have programmed the Esc to shut down the motor at 30%
So I dont worry about that, is an overheating possible?
```

---
## \#20 Posted by: lrdesigns Posted at: 2018-05-15T00:48:23.113Z Reads: 53

```
Over heating is very unlikely unless the battery is way way to small for a skateboard. You would have such little range on a battery that size it would be obviously bad.

I have seen many lipos pull over current in RC models, they will puff up if that happens. Its quite rare to pull enough current from them that they catch fire. As they are designed for high amp draw first, they actually heat up less under load than Lion. 

Even with an esc low voltage cut off its still a good idea to run individual cell alarm. As the discharge curve on lipo is quite flat, then after 3.6v it quickly drops off a cliff. The esc will monitor total pack voltage but its quite likely one or two cells will perform worse than the rest and they can drop down to 2.0v before the esc will go into low voltage mode. Or run a more conservative low voltage setting of 3.6x12 = 43.2v but it still does not totally eliminate the risk of one cell going low without you knowing it. 

I like these [alarms](https://www.aliexpress.com/item/3-7-30V-1-8S-LiPo-Li-po-ion-Fe-Battery-Voltage-Tester-Low-Voltage-Buzzer/32688047450.html?spm=2114.search0104.3.32.17b723b6pkza5t&ws_ab_test=searchweb0_0,searchweb201602_4_10152_10151_10065_10344_10068_5722815_10342_10343_10340_5722915_10341_5722615_10696_10084_10083_10618_10307_5722715_5711215_10059_308_100031_10103_10624_10623_10622_5711315_5722515_10621_10620,searchweb201603_25,ppcSwitch_5&algo_expid=4b180e2b-55eb-47c3-9f5b-b11ac25c1d80-4&algo_pvid=4b180e2b-55eb-47c3-9f5b-b11ac25c1d80&priceBeautifyAB=0) 
![image|466x380](upload://1DDcIz4ud2gCAZfGknECm8WZFoU.jpg)

Or if you want to get really fancy [these](https://www.aliexpress.com/item/ISDT-BC-8S-Battery-Checker-with-Two-85dB-Buzzer-OLED-Screen-for-LiPo-LiHv-LiFe-LiIon/32811429468.html?spm=a2g0s.8937460.0.0.67132e0ehSg07V) alarms will tell you the minimum voltage under load of each cell.  
![image|603x438](upload://s0fSPWsg50tTExhoh6FN93T63oG.jpg)
```

---
## \#21 Posted by: b264 Posted at: 2018-05-15T05:17:01.298Z Reads: 45

```
Use a BMS just like you would with li-ion and it will be fine.  Make sure you use the correct voltage cutoffs, which will be different than li-ion.

When you don't use a BMS is when things can get flaky.
```

---
