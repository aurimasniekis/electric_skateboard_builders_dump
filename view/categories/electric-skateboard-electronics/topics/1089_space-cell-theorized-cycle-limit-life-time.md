# SPACE cell, theorized cycle limit/life time

### Replies: 17 Views: 2345

## \#1 Posted by: Sharkface Posted at: 2016-01-24T03:08:50.125Z Reads: 105

```
Continuing the discussion from [Who is stoked for the end of 2015 wave of VESC from enertion?](http://www.electric-skateboard.builders/t/who-is-stoked-for-the-end-of-2015-wave-of-vesc-from-enertion/521/53):

[quote="disastorm, post:53, topic:521, full:true"]
I ordered mine in October (Order #1182) and didn't get an email yet, so I wouldn't rely on emails to determine who hes sending until he actually sends it. Did he send the email to you guys randomly or did you ask him when he was shipping it and he just replied to you? 

He said in a previous post that he ordered enough Vescs for everyone + extra although that was a few weeks ago so I'm not sure if hes surpassed the limit by now.
[/quote]

Continuing the discussion from [Behind the Scenes | Raptor Electric Skateboard Production Process](http://www.electric-skateboard.builders/t/behind-the-scenes-raptor-electric-skateboard-production-process/619/120):

[quote="Dedbny, post:120, topic:619, full:true"]
So you have had it a year and a half. When you say you can tell its definatley getting old what do you mean? That its taking longer to charge or its not lasting as loing in a session and your not getting the same range. How much time were you getting out of it initially and now?
[/quote]
So the example I gave was specifically with the 26650 batteries that I am using for my ecig. I do not currently own or operate a space cell. Just use the same batteries that the space cell is using (18650s in the space cell, and my brand new ecig. have 26650s in the old ecig)

So again, I am talking about a year and a half of using my ecig with the same two batteries. This is charging them to 100% then draining them till my ecig barely works. which is about less than 10%.

I can tell the battery is getting old because it will charge slower, and deplete faster. It has yet to fluff up any. So in theory that SPACE cell has the possibility of making it a year with being 100% drained every 2-3 days. 

Anybody have a space cell that is older than 6 months that could weigh in here?

[quote="Dedbny, post:120, topic:619, full:true"]
Sorry to highjack thread, but good to know. Probably should be in the space cell thread.
[/quote]
My reply created a new thread, so we are golden buddy
```

---
## \#2 Posted by: Dedbny Posted at: 2016-01-24T05:44:45.064Z Reads: 98

```
Onloop -Stopping charge before the battery is 100% charged is perfectly fine. In fact only charging to 80 or 90% capacity increases life span of the battery.
```

---
## \#3 Posted by: Dedbny Posted at: 2016-01-24T05:47:13.334Z Reads: 98

```
cmatson -  the % display always shows a couple percent higher than what is actually in the battery while charging. If it said 90 while charging and you unplugged it, it'd probably drop to around 87 or even lower.
So if you want a full charge, wait for the green light :wink:

Both taken from space cell charger thread.
```

---
## \#4 Posted by: Sharkface Posted at: 2016-01-24T07:06:30.550Z Reads: 96

```
Does anybody know if the latge amount of voltage going through the 18650s decreases the life span of them?
```

---
## \#5 Posted by: TF22 Posted at: 2016-01-24T08:33:42.149Z Reads: 90

```
I know its not my place to comment on what other people do to their bodies, but ecigs aren't much better than regular tar cigarettes. As a toxicologist for my day job, (ik not super glorious) The regulation on Ecigs is shit and practically nonexistent. just my two cents. The shit I found in them is scary: numerous cancerous agents.
```

---
## \#6 Posted by: Sharkface Posted at: 2016-01-24T08:59:21.956Z Reads: 90

```
No they are not much better, no i shouldnt be smoking, yes its wasted money, yes its unregulated, and yes i am an addicted slave.

That being said, having an ecig is the only thing thats kept me away from the pack or more a day habbit.... so yes im fucked, but im slowly, ver very slowly improving. If scare tactics worked i wouldnt have started in the first place
```

---
## \#7 Posted by: cmatson Posted at: 2016-01-24T13:51:34.630Z Reads: 89

```
just to add, here is what @onloop said about the voltages equalling percents:
The Low Voltage Cut off (LVC) of S.P.A.C.E Cell is 27.5v
This is how the LCD is programmed.
42v = 100%
40v = 80%
37v = 50%
35v = 30%
33v = 10%
32v = 0%

Once the battery reaches 0% under load you will probably be hitting the LVC

So in theory you can ride it until the readout reaches 0%
```

---
## \#8 Posted by: Sharkface Posted at: 2016-01-24T17:26:45.629Z Reads: 86

```
How does the voltage sag from drawing current get factored into this? if at all?
```

---
## \#9 Posted by: chaka Posted at: 2016-01-24T19:56:34.613Z Reads: 83

```
It is all about voltage sag. The more current you draw from your cells the more the voltage will sag. As the voltage sags lower and lower towards a 3v cutoff the amperage will climb by as much as 20 percent.

If you make sure you never get your pack hot due to excessive voltage sag it will have a much longer life. Likewise never let get hot from excessive charge currents.
```

---
## \#10 Posted by: Sharkface Posted at: 2016-01-25T04:30:29.045Z Reads: 79

```
So in theory would a really high level BMS have temp gauges being monitored on the cells?
```

---
## \#11 Posted by: chaka Posted at: 2016-01-25T04:59:54.032Z Reads: 78

```
The bms units I use have a temp sensor. I think the space cell has one too. Somewhat standard. They are always set to a very high value though. Just enough to keep the pack from going into thermal runaway.
```

---
## \#12 Posted by: KMeyerson Posted at: 2016-01-28T01:10:16.857Z Reads: 72

```
The expected life cycle for these Li(NCM) batteries as they are is more of less 500 cycles before degradation.
I'm working with the same battery chemistry and have consulted several companies on this subject.

Li(NCM) cells might last longer with more parallel set, but the Space Cell is much less than 5P (which should have a cycle count closer to 1000 cycles).

For the batteries size, weight, and capacity - the Space Cell is still the best for boards.
```

---
## \#13 Posted by: Sharkface Posted at: 2016-01-28T21:40:46.383Z Reads: 70

```
[quote="KMeyerson, post:12, topic:1089"]
The expected life cycle for these Li(NCM) batteries as they are is more of less 500 cycles before degradation.I'm working with the same battery chemistry and have consulted several companies on this subject.

Li(NCM) cells might last longer with more parallel set, but the Space Cell is much less than 5P (which should have a cycle count closer to 1000 cycles).
[/quote]

The Space Cell is made up of 18650s which run off of [LiFePO4][1] technology. This Li(NCM) you mentioned seems to be different unless I am mistaken? However a quick search and I found this: http://www.batteryspace.com/Custom-LiNiMnCo-Battery-Packs.aspx

Even though we are talking about different chemical makeups, the cycle counts would be about the same correct?


  [1]: https://en.wikipedia.org/wiki/Lithium_iron_phosphate_battery
```

---
## \#14 Posted by: onloop Posted at: 2016-01-28T23:39:32.353Z Reads: 64

```
The S.P.A.C.E. Cell Is not Lifepo4, 18650 is a form factor and it can have various chemistries. Some 18650 are LiFePO4 but the space cell isn't. It uses LG HE2 batteries. Lifepo4 is lower voltage per cell and in most cases outdated when it comes to high discharge batteries

The chemistry of the LG Chem HE2 battery is:  Li[NiMnCo]O (H-NMC) / Graphite + SiO. So The HE2 is basically an NMC (nickel-manganese-cobalt) battery
```

---
## \#15 Posted by: mostwanted Posted at: 2016-01-29T00:14:08.963Z Reads: 67

```
now there's 18650 HE4 !
i dont know whats the difference between HE2 & HE4 . but it sounds better . got my info through my local sg supplier friend .
```

---
## \#16 Posted by: cmatson Posted at: 2016-01-29T01:34:38.877Z Reads: 68

```
[quote="mostwanted, post:15, topic:1089"]
i dont know whats the difference between HE2 & HE4 . but it sounds better .
[/quote]

haha they are almost identical :wink:

To be honest, from the testing I've seen the he4 are just newer (as in the he2 came out first), but have nearly the capacity, discharge rate, etc. 

Maybe @chaka can chime in, but I'm pretty sure these two different cells are as similar as 18650 cells can be.
```

---
## \#17 Posted by: chaka Posted at: 2016-01-29T02:16:32.377Z Reads: 65

```
They are nearly identical. Testing shows the he4 to have around 100 mAh more capacity in real world testing and a slightly longer cycle life under high discharge. The he2 is rated at 200 cycles at 15 amps and the he4 is rated at 200 cycles at 20 amp. 

It is worth considering that the capacity ratings on both cells is 2500 mAh at 0.5 amp discharge. Higher discharge rates will show lower capacity. At higher discharge rates they both will show lower capacity than the rated spec.
```

---
