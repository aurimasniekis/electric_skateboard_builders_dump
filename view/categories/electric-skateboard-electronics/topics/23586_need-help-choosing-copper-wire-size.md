# Need help choosing copper wire size

### Replies: 16 Views: 2277

## \#1 Posted by: BladeZ Posted at: 2017-05-21T02:33:10.404Z Reads: 223

```
Hi guys..

I'm planning to build my own battery pack for my board.. I've done my research on how to build them etc but one thing I still can't understand is choosing the copper wire size for soldering.. I don't have spot welder so soldering is my only option for now.. From what I understand, copper wire can deliver higher current compare to nickel strip.. Btw, My configuration is 10s3p and I will be using dual Alien 190kv 6355..

The bms I will be using is 60A for continuous discharge, 120A peak discharge..
https://de.aliexpress.com/item/36V-BMS-60A-120A-Electric-bicycle-Lithium-ion-Battery-BMS-10S-42V-2000W-Battery-Pack-BMS/32797321201.html?spm=2114.01010208.3.40.NM0t2W&ws_ab_test=searchweb0_0%2Csearchweb201602_3_10152_10065_10151_10068_436_10136_10157_10137

Now the question is, what gauge copper wire I should use in order to deliver max 60A to the VESC (30A for each VESC = 30A for each motor) without causing too much heat on the wire or worse case break the wire connection..? I read a few post saying 14 AWG is enough but I'm not really sure.. A lot people use only 2-3 layer nickel strip which can deliver less current compare to copper wire, but have no problem at all..

Anyway I arrage the battery this way so it's relatively thin, not so wide, but long configuration..
<img src="/uploads/db1493/original/3X/d/0/d0bfb8c6eb8482ad96ee1bac59e09a4036fd8dc4.jpg" width="690" height="388">
Right side are the possible battery I would use.. Most probably LG HG2 since 20Ax3p = 60A.. (Ignore the circles, it's so that i can see it clearer)

Really need your help.. Once this problem solved I can start doing the project.. Thanks in advance.. Cheers..
```

---
## \#2 Posted by: mmaner Posted at: 2017-05-21T02:43:14.071Z Reads: 207

```
You might look at sleds, does away with a lot of the issues with not welding.
```

---
## \#3 Posted by: BladeZ Posted at: 2017-05-21T03:15:40.077Z Reads: 203

```
Wow.. Never thought of that.. Good tips.. But I'm still curious about copper wire size.. Thanks anyway..
```

---
## \#4 Posted by: treenutter Posted at: 2017-05-21T03:48:26.937Z Reads: 203

```
Lots of info on wire gauge in this thread:

https://www.electric-skateboard.builders/t/wire-gauge-in-esk8/213
```

---
## \#5 Posted by: BladeZ Posted at: 2017-05-21T13:59:03.445Z Reads: 173

```
Thanks.. I think I will go for 14 AWG copper wire for the battery connection..
```

---
## \#6 Posted by: BladeZ Posted at: 2017-05-21T18:48:13.215Z Reads: 152

```
Do you guys think this copper wire good enough to wire the battery cells..? 1.7mm should be equal to 13-14 Gauge wire..

http://www.ebay.de/itm/Kupferdraht-1-7mm-blank-LANGE-WAHLBAR-Kupfer-Basteldraht-Keshe-Draht-2mm-1-00-08-/252912577653?var=&hash=item3ae2c3ac75:m:mhpgZhfFRD3tdmY7AHjVzIQ
```

---
## \#7 Posted by: nikoli280 Posted at: 2017-05-21T19:30:13.430Z Reads: 137

```
Im am building the exact same setup just with 5 pr cell, still 10S. 

And i use the 0.15mm nickel band plus 1.5mm solid copper wire. If you are only going to use copper wire and 10S. Then go with 2mm just to be sure. 

I think you can make it with all down to 1mm since the max current draw pr cell is 60/10 = 6A. which is not alot. But rather be on the safe side with a bit thicker wire.
```

---
## \#8 Posted by: BladeZ Posted at: 2017-05-21T19:46:21.524Z Reads: 132

```
> the max current draw pr cell is 60/10 = 6A.

That's where my calculation went wrong.. I thought I have to divide the max current to how many cells in parallel which in my case 3p.. So i thought each cell will have to deliver 20A..

Thanks a lot for that information..
```

---
## \#9 Posted by: jmasta Posted at: 2017-05-21T21:43:47.130Z Reads: 123

```
The post above you is incorrect

For 60A at 3p, each cell must supply 20A
```

---
## \#10 Posted by: BladeZ Posted at: 2017-05-22T00:43:12.286Z Reads: 111

```
So based on this diagram having 10-14 gauge wire for the battery connection is alright for my build right..? Since 14 gauge wire can allow up to 24A current while 10 gauge wire can go up to 52A.. I think I would use 12 gauge wire between the cells and 10 gauge for the positive and negative end..

<img src="/uploads/db1493/original/3X/c/2/c22ef42e13d9bfa9be78564fb6a4a7b04422b436.png" width="512" height="500">
```

---
## \#11 Posted by: ChrisH Posted at: 2017-07-14T18:33:20.762Z Reads: 91

```
Hey. I'm following your diagram to build the same battery since the configuration is the best for soldering solid copper. ( I know soldering isn't the best way), sorry if I'm being stupid but do you need to insulate between the two rows of 15 when pushing together or can the whole thing be pushed together then shrink wrapped. Cheers guys!!
```

---
## \#12 Posted by: BladeZ Posted at: 2017-07-14T18:55:12.308Z Reads: 86

```
You  need to insulate the gap.. The only thing connected the top pack and bottom pack is the number 5, connected with the wire.. I would suggest to insulate and get some thin foam (I use heat resistance one) in between.. There are other configuration that don't require these.. But the negative wire will be on the bottom right instead of bottom left.. Your choice..
```

---
## \#13 Posted by: treenutter Posted at: 2017-07-14T19:28:00.437Z Reads: 84

```
@BladeZ Not exactly sure what you're going to use that copper wire for, but generally we use shielded (silicone) wire unless you're making short connections and they will be wrapped in another way. I can't read the description but look around for battery builds here and you'll find lots of examples and part lists.
```

---
## \#14 Posted by: jrpwit Posted at: 2017-07-14T19:33:47.126Z Reads: 79

```
Just get some 10 guage wire like this. 14 is too small. I have bought this wire and its really good https://www.amazon.com/BNTECHGO-Silicone-Temperature-Resistant-Flexible/dp/B017TGYW3S/ref=sr_1_4?s=industrial&ie=UTF8&qid=1500060696&sr=1-4&keywords=10+gauge
```

---
## \#15 Posted by: merkyle Posted at: 2019-01-28T05:59:52.811Z Reads: 36

```
Would 12 be alright?
```

---
## \#16 Posted by: jrpwit Posted at: 2019-01-29T21:17:26.467Z Reads: 30

```
Yeah 12 is okay. Probably won't make much of a difference. 2 years later lol
```

---
