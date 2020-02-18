# Looking for well reviewed BMS for a home made 10S4P made with Samsung 25R

### Replies: 24 Views: 2209

## \#1 Posted by: marc2912 Posted at: 2016-11-21T16:40:08.890Z Reads: 187

```
Title says it all.  Planning on making my own pack.  Sourced a spot welder and 40 Samsung 25R.  I'm looking to tie all this to a good BMS (also would love pointers on a good charger).

Thanks.
```

---
## \#2 Posted by: flatsp0t Posted at: 2016-11-21T16:46:03.607Z Reads: 192

```
The ones from http://www.batterysupports.com/lion-lipo-nbsp-36v-nbsp-10s-c-32_41.html are widely used and approved.
Another good source is BestechPower.
```

---
## \#3 Posted by: Jinra Posted at: 2016-11-21T16:46:11.471Z Reads: 190

```
Supower (batterysupports.com) has good BMS's and they're @longhairedboy's BMS of choice I believe. BMS's are fairly simple devices so you can't go wrong with most choices. Just make sure to check the datasheet to make sure specs fall in line with what you're looking for.

I use a cheap $20 BMS from aliexpress myself since I don't rely on it for discharging. I only use it to balance charge. The reason I got this one was due to the small size of it.

https://www.aliexpress.com/item/Free-Shipping-36V-10ah-battery-BMS-3-7V-18650-li-ion-cell-10S-BMS-PCB-PCM/32283661813.html?spm=2114.13010608.0.0.aRgJil
```

---
## \#4 Posted by: marc2912 Posted at: 2016-11-21T17:17:57.762Z Reads: 173

```
[quote="flatsp0t, post:2, topic:13414, full:true"]
The ones from http://www.batterysupports.com/lion-lipo-nbsp-36v-nbsp-10s-c-32_41.html are widely used and approved.Another good source is BestechPower.
[/quote]

Thanks, looking there now.

[quote="Jinra, post:3, topic:13414"]
I use a cheap $20 BMS from aliexpress myself since I don't rely on it for discharging. I only use it to balance charge. The reason I got this one was due to the small size of it.
[/quote]

What are you using for discharging?
```

---
## \#5 Posted by: Jinra Posted at: 2016-11-21T17:19:51.646Z Reads: 164

```
Nothing, I just hook up the batteries direct to VESC.
```

---
## \#6 Posted by: marc2912 Posted at: 2016-11-21T17:25:47.747Z Reads: 160

```
[quote="Jinra, post:5, topic:13414, full:true"]
Nothing, I just hook up the batteries direct to VESC.
[/quote]


Any downside to doing it this way that I'm not grasping? 

I'm making 10S4P with some 25Rs and I've got the Ollin Board Company VESC 4.12 - Vedder's Speed Controller on order (2 since I'm running dual).
```

---
## \#7 Posted by: Jinra Posted at: 2016-11-21T17:27:25.930Z Reads: 157

```
You don't get the over-discharge protection on the BMS, but you can set this up in the VESC anyway. You also aren't protected in case of a short, but you can fix this by adding a fuse as well. I personally don't use a fuse since there isn't room in my builds.
```

---
## \#8 Posted by: marc2912 Posted at: 2016-11-21T17:41:23.465Z Reads: 159

```
[quote="Jinra, post:7, topic:13414, full:true"]
You don't get the over-discharge protection on the BMS, but you can set this up in the VESC anyway. You also aren't protected in case of a short, but you can fix this by adding a fuse as well. I personally don't use a fuse since there isn't room in my builds.
[/quote]

Thanks, guessing this is it?

http://www.electric-skateboard.builders/t/carbonated-enertion-vescs-hi5ber-overtaker-custom-10s4p-25r-pack-with-cell-level-fusing-abec-flywheels/10879
```

---
## \#9 Posted by: Jinra Posted at: 2016-11-21T17:45:48.273Z Reads: 143

```
I have two builds, but yea that's one of them.
```

---
## \#10 Posted by: longhairedboy Posted at: 2016-11-21T19:30:37.355Z Reads: 136

```
also going direct from battery you don't get auto shut off protection for accessories like BECs and UBECs but if you're not using those its irrelevant. If all you have is the pack and two vescs its fine to use the VESC as the safety cut off.

i use BMSs for discharge in my builds because i want the whole damn thing to die immediately upon 0%, regardless of what else is happening in there.
```

---
## \#11 Posted by: marc2912 Posted at: 2016-11-21T19:46:45.654Z Reads: 133

```
[quote="longhairedboy, post:10, topic:13414, full:true"]
i use BMSs for discharge in my builds because i want the whole damn thing to die immediately upon 0%, regardless of what else is happening in there.
[/quote]

Not sure I get what you mean here.
```

---
## \#12 Posted by: Jinra Posted at: 2016-11-21T19:50:25.371Z Reads: 127

```
He doesn't want cells to overdischarge, meaning once it hits the BMS cutoff voltage, it just shuts down. If you're using the VESC you can program this. If your using a hobby ESC, not so much.
```

---
## \#13 Posted by: Namasaki Posted at: 2016-11-21T19:52:26.856Z Reads: 132

```
The best setup is a BMS for discharge as well as charge. 
The over discharge protection that the Vesc offers is by monitoring total pack voltage. 
So theoretically, you could have one or more cells fall below safe voltage without triggering the protection. 
A BMS will monitor each cell group giving a higher level of protection. 
It also protects against over charging by regen brakes. 
And, the BMS also has external short protection that will save every part of your build in the event of a wiring short. 
I tested that myself on Saturday when I was checking pack voltage at the charging socket with s multi meter and accidentally shorted the pos and beg pins.
Everything was on including 2 Vescs and receiver.  
There was a big spark and the BMS instantly shut down opening the circuit. My meter probs where melted as where the charge socket pins. 
When I removed the enclosure, I found that nothing inside was affected. The wires coming from the charge socket showed no signs of heat. 
The total voltage from my fully charged 10s pack only dropped 1/10 of a volt.
```

---
## \#14 Posted by: longhairedboy Posted at: 2016-11-21T20:39:43.782Z Reads: 128

```
All of those are excellent points as well.  BMSs will prevent fires. Unattended and balanced charging is only one small part of it. 

I'm building for customers so while i may be cool with some DIY tricks in my own builds, i always do what's safe in my customer's builds. That means protecting the pack on both charge and discharge. 

And for those of you wondering, when the BMS shuts down while you're riding the only thing that happens is you loose thrust and coast. 

And if you're on a slope that allows it you can reach down and turn the board back on after a few seconds and let the coasting recharge your board a little and also give you your brakes back so you can come to a full stop without tearing a hole in your shoe. 

Once my son towed me for a quarter mile after we ran a customer's pack dead during a full discharge test and i got about 3% of my pack back, which was enough to get me back to my vehicle. Fun times. 

I also have a set of scorched volt meter leads that are missing chunks of copper lol
```

---
## \#15 Posted by: marc2912 Posted at: 2016-11-21T20:58:46.740Z Reads: 125

```
[quote="longhairedboy, post:14, topic:13414, full:true"]
All of those are excellent points as well.  BMSs will prevent fires. Unattended and balanced charging is only one small part of it. 

I'm building for customers so while i may be cool with some DIY tricks in my own builds, i always do what's safe in my customer's builds. That means protecting the pack on both charge and discharge. 

And for those of you wondering, when the BMS shuts down while you're riding the only thing that happens is you loose thrust and coast. 

And if you're on a slope that allows it you can reach down and turn the board back on after a few seconds and let the coasting recharge your board a little and also give you your brakes back so you can come to a full stop without tearing a hole in your shoe. 

Once my son towed me for a quarter mile after we ran a customer's pack dead during a full discharge test and i got about 3% of my pack back, which was enough to get me back to my vehicle. Fun times. 

I also have a set of scorched volt meter leads that are missing chunks of copper lol
[/quote]

Thanks for the detailed reply.  Just want to check to make sure I'm not losing my marbles.  Since the 25R is 20A continuous and I'm doing 10S4P I should get at least 80A continuous BMS?
```

---
## \#16 Posted by: marc2912 Posted at: 2016-11-21T21:11:05.996Z Reads: 122

```
[quote="flatsp0t, post:2, topic:13414, full:true"]
The ones from http://www.batterysupports.com/lion-lipo-nbsp-36v-nbsp-10s-c-32_41.html are widely used and approved.Another good source is BestechPower.
[/quote]

Quick question on BestechPower.  I (in my very limited knowledge) think this would be a great BMS with a lot of options I might use in the future ...
http://bestechpower.com/communicationbms/BMSD338.html

How would I go about ordering this? Do they sell single boards?
```

---
## \#17 Posted by: flatsp0t Posted at: 2016-11-21T21:14:06.443Z Reads: 119

```
Send them a mail and request one, they will handle it as "sample".
```

---
## \#18 Posted by: willpark16 Posted at: 2016-11-21T22:52:02.964Z Reads: 116

```
@cmatson has one
```

---
## \#19 Posted by: cmatson Posted at: 2016-11-22T01:30:13.393Z Reads: 111

```
ya, my BMS failed on me after less than a month of use, so I wouldn't pick it- 

check with @longhairedboy he probably knows best along with @barajabali
```

---
## \#20 Posted by: longhairedboy Posted at: 2016-11-22T13:11:43.615Z Reads: 106

```
i build 4P packs on those which do allow a continuous draw of 80 amps, yes. However I use 60 amp BMSs. In the past I've used 80 amp BMSs and that's fine too. I use 60 amp ones because they're smaller and easier to fit in there and also because 60 amps is plenty, more than you'll probably ever use at 10S or 12S.
```

---
## \#21 Posted by: longhairedboy Posted at: 2016-11-22T13:13:36.468Z Reads: 98

```
I'm still working on a 4 month old RMA for three 10S BMSs i got from Bestech which failed on arrival. 

BTW their minimum sample size is two units, so when you order them you have to get at least two of them. 

I've never had any issue at all with the Battery Supports BMSs.
```

---
## \#22 Posted by: marc2912 Posted at: 2016-11-22T14:06:08.421Z Reads: 96

```
The fact that they're so unresponsive to your RMA's is not a good sign...  I sent them an email and asked for a price on 2 of a specific unit.  Instead they replied with asking more on my application and saying they don't do this or that which makes me not even want to work with them...
```

---
## \#23 Posted by: longhairedboy Posted at: 2016-11-22T15:39:21.343Z Reads: 94

```
They've been responsive, but they are taking full advantage of the fact that i returned the units using USPS First Class International which aparently loses the ability to track the package once it leaves Miami. So they told me to send them back, and i did, and now they're in the wind and i have no obvious course of resolution. China Post has no desire to help either of us and USPS is helpless. Its just a bad situation all around. The three units were essentially DOA. Bad e-switches. They would have been perfect for my builds, too. 

I'm so sick of bad e-switches that i had my own modified vedder switches made at macrofab.
```

---
## \#24 Posted by: Eboosted Posted at: 2017-01-23T06:08:33.087Z Reads: 75

```
Hey @longhairedboy I also bought a 60A BMS from Battery Supports but my battery pack is also a 10S4P with Samsung 25R, so 20A continuos with 4 paraller means 80A.

Should I limit "battery amp" in the VESC settings at 30A for each VESC (dual setup) in order to protect the BMS and be withing it's max current limits?

@Ackmaniac would you suggest this?
```

---
