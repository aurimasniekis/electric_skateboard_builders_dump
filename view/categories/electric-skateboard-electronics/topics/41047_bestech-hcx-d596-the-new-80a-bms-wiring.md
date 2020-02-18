# Bestech HCX-D596 - The new 80A BMS - wiring

### Replies: 47 Views: 4516

## \#1 Posted by: DavidBanner Posted at: 2017-12-14T21:29:49.034Z Reads: 575

```
*** solved - see [here](http://www.electric-skateboard.builders/t/bestech-hcx-d596-the-new-80a-bms-wiring/41047/14?u=davidbanner) for wiring diagram and connection procedure ***


I've had some of the new HCX-D596 BMS modules arrive but there are no wiring diagrams 

This is how I think they are likely to be wired:
<img src="/uploads/db1493/original/3X/a/8/a8618febc777d362f4c727040aa5c03bfdaa308a.jpg" width="645" height="484">

<img src="/uploads/db1493/original/3X/9/a/9ab1343d47fcd072719871590744c778117d3a9a.jpg" width="690" height="367">


What does everyone else think?

My biggest worry is the balance leads as the pin order could be the reverse to what I have in the diagram
```

---
## \#2 Posted by: HighMasterGogo Posted at: 2017-12-14T21:36:38.497Z Reads: 514

```
Sorry, can't help with wiring but wondering if you'll be selling these on street wing?
```

---
## \#3 Posted by: DavidBanner Posted at: 2017-12-14T21:40:17.659Z Reads: 508

```
@HighMasterGogo  yes I will be adding them to the site in the coming days .

drop me a PM if you need one quickly
```

---
## \#4 Posted by: psychotiller Posted at: 2017-12-14T23:36:27.018Z Reads: 474

```
Are these 10s or 12s? Edit- I see it's 10s. B1 is usually far left, then 1-10
```

---
## \#5 Posted by: DavidBanner Posted at: 2017-12-14T23:46:28.419Z Reads: 464

```
thanks @psychotiller :) 

[quote="psychotiller, post:4, topic:41047"]
B1 is usually far left
[/quote]

80A packs and "usually" are not my favourite combination :grin:
```

---
## \#6 Posted by: DavidBanner Posted at: 2017-12-15T10:57:29.158Z Reads: 448

```
I've done some more digging, thinking and tracing the PCBs

There is a place for another balance connector to the left of the balance connector, this has a silkscreen label of 11 - 1. It is impossible to check the silkscreen of the balance connector (without desoldering) in use as it is under the connector

Stuff in Green is confirmed by the PCB silkscreen
Stuff in Red is up for debate

The balance connector is 11 PIN just to really fuck with my head, as all of the other Bestech 10S BMS I have seen use 10 PIN connectors...
<img src="/uploads/db1493/original/3X/b/8/b84d3ea0823740341d3eed39c4410d3181af8b17.jpg" width="690" height="367">

<img src="/uploads/db1493/original/3X/8/8/887ee648a061bdbe2be1ff6e9150c43d101a6222.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/0/1/01661364aecea9f4fd03ab570234f41c536c1abb.jpg" width="690" height="457">
```

---
## \#7 Posted by: scepterr Posted at: 2017-12-15T11:02:24.831Z Reads: 407

```
That looks correct, first pin would be B0 I assume

Also possible it has P+ and P- 

I would grab a drained low discharge cell if you have one and hook it up to b-, b0,1 and test the pads, though I'm not sure it would function properly without the full series...so maybe a test 10s1p pack
Put a 1a fuse on it or something if you have
```

---
## \#8 Posted by: DavidBanner Posted at: 2017-12-15T11:18:15.224Z Reads: 406

```
I think I am going to have to wait for the wiring diagram. 

I am not one to shy away from a good session of hunt the trace, but when it comes to high amp packs there is no room for error and I am already short of BMSes to fill backs orders that have come in so I really don't want to bork the BMS
```

---
## \#9 Posted by: scepterr Posted at: 2017-12-15T11:20:33.678Z Reads: 373

```
Did you check for writing on the backside of the top PCB?
```

---
## \#10 Posted by: DavidBanner Posted at: 2017-12-15T11:22:50.227Z Reads: 368

```

no, it would require desoldering a 7 pin sil which is connecting the two PCBs. I really, really hate desoldering those things
```

---
## \#11 Posted by: PXSS Posted at: 2017-12-15T12:42:23.243Z Reads: 363

```
B0-B10 right to left. 
Grab your multimeter and set it to check continuity. Check between pins b0 and b-
```

---
## \#12 Posted by: ducktaperules Posted at: 2017-12-15T12:51:45.380Z Reads: 363

```
it should be easy to check if the first and last balance pins are connected to positive and negative using continuity check on a multi-meter. if so the other 9 pins will be the intermediate balance points and it will also tell you which direction they go in.
```

---
## \#13 Posted by: DavidBanner Posted at: 2017-12-15T13:07:13.089Z Reads: 394

```
@ducktaperules - nice thinking there mister!  I deserve a slap for not thinking of that myself

we have continuity between B- and the far right pin, which must therefore be Battery 0 / -
```

---
## \#14 Posted by: DavidBanner Posted at: 2017-12-15T13:15:52.554Z Reads: 394

```
and of course, having worked it out independently I just got an email from BesTech.

Lucy all is forgiven :)

<img src="/uploads/db1493/original/3X/7/f/7fc83e1a704c86b660b9f0947a444e3b898e8c85.jpg" width="690" height="478">

Steps for how to connect the PCM with cells in order.
1. Connect Pack’s negative with B-;
2. Connect cell 1 with B1;
3. Connect cell 2 with B2; 
4. ....
11.Connect cell 10 with B10;
Then measure the cell’s voltage in order to see if the voltage is progressive increase.If yes,you can plug the connector to the PCM in order. Also if the connector and wires is not matched,please don’t plug,or the PCM will be damaged.
12.Connect Pack’s positive with B10;
13.Connect Load’s negative with P-; Connect Charger’s negative with C-;
14.Connect Load’s positive with B10; Connect Charger’s positivewith B10;

*************************************
```

---
## \#17 Posted by: ervinelin Posted at: 2018-06-12T17:03:41.404Z Reads: 293

```
Sorry for digging up an old thread, but I just wired this BMS together and thankfully no magic smoke...

But I have 2 questions I wanted to ask:
1. When the E-switch is disconnected, the voltage across the load output is an odd 27 volts as opposed to what I thought would be 0.
2. Do I need to turn on the E-switch to charge the BMS?

Thanks!
Erv.
```

---
## \#18 Posted by: DavidBanner Posted at: 2018-06-12T17:12:10.059Z Reads: 282

```
1. is normal
2. yes
```

---
## \#19 Posted by: ervinelin Posted at: 2018-06-12T17:13:30.104Z Reads: 281

```
Thanks but wont this mean there would be 27V going into my VESC even though the E-switch is turned off?
```

---
## \#20 Posted by: DavidBanner Posted at: 2018-06-12T17:55:27.840Z Reads: 283

```
[quote="ervinelin, post:19, topic:41047, full:true"]
Thanks but wont this mean there would be 27V going into my VESC even though the E-switch is turned off?
[/quote]

no, it wont do it under load.

it's something to do with caps, blue smoke and voodoo ;) there more technical descriptions of why to be found using the search
```

---
## \#21 Posted by: ervinelin Posted at: 2018-06-12T18:19:03.629Z Reads: 273

```
Great... thanks a lot for the assurance! Was getting a bit worried I messed up!!
```

---
## \#22 Posted by: oripaamoni Posted at: 2018-07-09T00:47:12.734Z Reads: 271

```
can somebody point me to where to buy this BMS?
```

---
## \#23 Posted by: rickyd Posted at: 2018-07-09T06:36:38.633Z Reads: 269

```
You can order directly from Bestech: http://bestechpower.com/

I also have one of them for sale (EU), because you have to order two at a time unfortunately:
https://www.electric-skateboard.builders/t/eu-germany-new-for-sale-bestech-bms-hcx-d596-12s-80a/60985
```

---
## \#24 Posted by: GunnarK Posted at: 2018-07-28T18:08:07.950Z Reads: 254

```
Just to help some people out since I had some trouble with this (I got the answers from @pjotr47)
Here is a screenshot of how you should connect your wires

![IMG-20180728-WA0039|250x500](upload://hvjjrAs4bcurNTV1AT2NXOLNp0g.jpg)
Solder your wires on those squares the arrows are pointing at.

The **11** (!) balances wires need to be wired as follows:
Left to right when viewing the BMS as in my photo
10, 9, ..., 3, 2, 1, B-
```

---
## \#26 Posted by: dg798 Posted at: 2018-08-03T01:02:18.232Z Reads: 230

```
does this diagram seem right for wiring the balance leads on a 12s?
https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/8/3/839c1e65e39ce3fb4349d203ad20d3e611fb4519_1_375x500.jpg
```

---
## \#27 Posted by: GunnarK Posted at: 2018-08-03T11:24:19.695Z Reads: 213

```
Please complete the wiring. There are some leads missing. It looks like you wired the cells in a random order
```

---
## \#28 Posted by: rickyd Posted at: 2018-08-03T11:35:07.156Z Reads: 211

```
Also, the first pin (from the bottom) is supposed to be connected to ground, if I'm not mistaken.
```

---
## \#29 Posted by: yazuna Posted at: 2018-11-19T17:46:33.943Z Reads: 186

```
Quite a noob question: trying to understand where the e-switch is as it's not marked clearly anywhere..
Could anybody help with this (while waiting for bestech response)..
Thanks
```

---
## \#30 Posted by: DavidBanner Posted at: 2018-11-25T12:30:22.022Z Reads: 181

```
the e-switch is the two white wires that are attached to the BMS, you will need to attach a latching switching/button to those wires
```

---
## \#31 Posted by: yazuna Posted at: 2018-11-25T13:05:35.847Z Reads: 177

```
Thanks for the answer. It turned out Bestech sold me the non e-switch version in the end so will have to think about the alternative (the two white wires I have are for the temperature sensor apparently).
```

---
## \#32 Posted by: UKRider Posted at: 2018-12-01T10:35:06.575Z Reads: 162

```
Talking about the e-switch, what voltage does it need to be able to handle? Is it dependent on the pack, so for 10S pack must it handle 42v? What about amps?
```

---
## \#33 Posted by: GunnarK Posted at: 2018-12-03T10:00:37.490Z Reads: 155

```
The e switch does not handle any outside current. The two wires just need to be connected to create a positive signal which will boot the BMS.

Use a switch of some sort that holds it's state
How come you think you need to wire your battery to the eswtich?
```

---
## \#34 Posted by: UKRider Posted at: 2018-12-03T10:42:05.058Z Reads: 163

```
No I will not wire it to the battery, it will be wired to the BMS of course. I was thinking would 12v suffice or would it need to go up to 42v rating. I know there isn't much current, that not the concern.
```

---
## \#35 Posted by: Eboosted Posted at: 2018-12-31T20:04:33.283Z Reads: 158

```
I have this same bms but it's a 12s version, I'm not 100% sure if the first pin of the balance connector goes to negative b0 or to B1 (positive of first pack), hope to get input from you guys. 

![20181231_143844|690x388](upload://fAuAPuveODkn7D7BlN4QjFBolWC.jpeg)

It seems I need to plug both connectors the one with 11 pins and the one with 2 pins, that gives me a total of 13 pins.
```

---
## \#36 Posted by: sayekim Posted at: 2019-01-01T00:51:11.102Z Reads: 152

```
b0 goes to negative of p1. b1 to positive of p1 and so on. Yes you need to use both the two pin and 11 pin for the balance wires. 
I have the same 12s bms. Unfortunately I shorted it accidentally.
```

---
## \#37 Posted by: JFK Posted at: 2019-01-23T18:51:36.636Z Reads: 133

```
Hi all,

I have bought the 14S version (HCX-D596) with E-Switch.
To understand well, this switch need to be open or closed to boot up the BMS ?
Finally, it work out of the box without switch ?
Thanks.
```

---
## \#38 Posted by: UKRider Posted at: 2019-01-29T18:41:51.582Z Reads: 126

```
@jfk The switch must be ON for it to be powered to charge or discharge.

Does the D596 allow for regenerate current coming from the VESC to pass into the BMS and then go and charge the battery pack?? @sayekim @Eboosted @DavidBanner
```

---
## \#39 Posted by: sayekim Posted at: 2019-01-29T20:03:16.094Z Reads: 125

```
Yes. Even if it doesn’t the esc allows it if you let it. Which everyone does. 

You don’t need a bms for regenerative braking.
```

---
## \#40 Posted by: DavidBanner Posted at: 2019-01-29T20:07:38.766Z Reads: 121

```
[quote="UKRider, post:38, topic:41047"]
Does the D596 allow for regenerate current coming from the VESC to pass into the BMS and then go and charge the battery pack??
[/quote]

yes, I agree with @sayekim  it does
```

---
## \#41 Posted by: UKRider Posted at: 2019-01-29T20:08:18.139Z Reads: 116

```
So does that also.mean that the regen current is nicely balanced back to the pack as it should be??
```

---
## \#42 Posted by: DavidBanner Posted at: 2019-01-29T20:09:15.425Z Reads: 120

```
the BMS will balance the cells
```

---
## \#43 Posted by: UKRider Posted at: 2019-01-29T20:11:20.396Z Reads: 121

```
That's good to know. :grin: At first I thought that on the Bestech the charge is different to discharge wires therefore it would only balance through the charge wires.
```

---
## \#44 Posted by: sayekim Posted at: 2019-01-29T20:26:17.627Z Reads: 116

```
A bms only balance charges when it is charging. There is no other balancing. 
Most seem to start balance charging at around 4.18 volts. 

Mind you not all bms apparently balance charge either. Be sure to check that yours does if it is what you want.
```

---
## \#45 Posted by: UKRider Posted at: 2019-01-29T21:21:24.216Z Reads: 117

```
Just to clear things.

So talking about the Bestech D596 it will only balance when a charger is connected. Not when regen current is passed back through it. This means the regen current will go back into the batteries with no balance just as a standard charge.
```

---
## \#46 Posted by: sayekim Posted at: 2019-01-29T21:53:50.151Z Reads: 117

```
Yeah that’s right.
```

---
## \#47 Posted by: DavidBanner Posted at: 2019-01-29T23:33:58.102Z Reads: 118

```
afiak this explaination (which i was too lazy to write myself so cut and pasted) is correct: 
balancing usually  *starts* when the charger stops. For a pack with a BMS, balancing is handled by the BMS, not the charger. So when the first cell group reaches full, the BMS cuts off the charger and drains the highest cell group(s) slowly using its onboard resistors. Once its lower, it allows the charger to turn back on. It repeats until all cell groups are full.
```

---
## \#50 Posted by: Mich21050 Posted at: 2019-04-17T21:56:01.895Z Reads: 89

```
Please don't post the question everywhere. I'm sure someone with experience regarding that bms will help you on your other thread. :slight_smile:
```

---
## \#51 Posted by: Silverline Posted at: 2019-04-18T22:44:00.595Z Reads: 86

```
As seeing here om my bestech BMS / charge
https://youtu.be/XwDFkwLSguU
```

---
## \#52 Posted by: Dunmer Posted at: 2019-10-31T12:00:33.872Z Reads: 23

```
Sorry to dig this thread up. I have the 12s 80amp version. Somebody here in the thread got 27v on the load output. I got 6,7v on my xt90 plug when they bms is turned of. How, why? 😁 Can't wrap my head around it. Thx!
```

---
