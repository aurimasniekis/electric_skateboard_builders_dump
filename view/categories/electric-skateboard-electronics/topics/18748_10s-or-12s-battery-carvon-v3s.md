# 10s or 12s battery? Carvon v3&rsquo;s

### Replies: 12 Views: 1773

## \#1 Posted by: Wolfcola Posted at: 2017-03-08T12:32:34.637Z Reads: 262

```
I am going to get carvon v3s. I am a ~200lb dude. Was thinking 10s4p to get a bit more range on it but do you think that I would need 12s? I don't care about going too fast on it as it's more for just cruising around town. 

What do you think the specs would be on this for mostly flat ground with 10s or 12s? Speed and distance approx is sorta my deciding factor. 

My build list so far:

Carvon v3's
Abec 11 90mm flywheels
2 x Vesc-x 
10sp4 battery (360wh)
Enertion Remote controller
No deck picked out yet

Also hoping to run FOC with v3's and vescx. Would running 10s or 12s be any different in that regard?
```

---
## \#3 Posted by: olgamedt Posted at: 2017-03-08T18:39:30.284Z Reads: 235

```
Have a similar idea.
```

---
## \#4 Posted by: Namasaki Posted at: 2017-03-08T19:06:13.769Z Reads: 234

```
12s is a good match for the 100kv V3's
Not sure about how the Vesc deals with 12s
```

---
## \#5 Posted by: caustin Posted at: 2017-03-09T05:59:54.080Z Reads: 204

```
I am using 12s on dual v2.5.  They work well on VESC except for FOC, which works better on V2 supposedly a quirk of the lower kv v2.5 motor. Regardless, my understanding from Jerry is the EVO and REVO will be running 14s on VESC and have the kinks worked out on that (as I also understood 12s to be an effective limit on existing VESC, but that is well above my pay grade to understand lol).
```

---
## \#6 Posted by: saul Posted at: 2017-03-11T12:20:10.816Z Reads: 182

```
on flat theres not much difference. 12s would give a bit more hill climb power and a higher top speed. but even on 10s you can go 30mph+ if you hold on long enough...and have a bit of a hill to push off...
```

---
## \#7 Posted by: BigBoyToys Posted at: 2017-06-22T08:59:34.964Z Reads: 146

```
The Evo will be running 14s LiFePO4 batteries. LiFeP04 cells are 3.2v vs 3.7 for LiOn cells so 14s LiFeP04 voltage is equal to 12S Lion voltage.
```

---
## \#8 Posted by: BigBoyToys Posted at: 2017-06-22T09:02:14.145Z Reads: 142

```
Higher voltage means less amps, less amps means less heat. As a heavy guy you cant afford to have any extra heat in your motors. I definitely recommend 12S.
```

---
## \#9 Posted by: NAF Posted at: 2017-06-22T11:52:11.459Z Reads: 135

```
If you are a heavy dude I'd go for 12s. I have a 10s4p battery with CARVON SINGLE v2.5 and I havn't been even able to completely empty the battery even after super long day of riding. You have VESC-x so you shouldn't have problems with killing DRV on your vesc in FOC mode...and you'll heave more startup torque with 12s.
```

---
## \#10 Posted by: NAF Posted at: 2017-06-22T11:56:49.747Z Reads: 127

```
[quote="caustin, post:5, topic:18748"]
I am using 12s on dual v2.5.  They work well on VESC except for FOC
[/quote]

How is that ?? what's going wrong with it ? I have v.2.5 single in FOC mode and works smooth, no problems at all.
```

---
## \#11 Posted by: caustin Posted at: 2017-06-23T02:44:59.022Z Reads: 117

```
Got that guidance from Jerry directly. Experience has been that FOC on v2 works fine but sometimes on v2.5 it doesn't work well enough to favor it over BLDC. He was not able to determine why that was the case other than perhaps the windings.  I am ok with Bldc for dual v2.5 right now and moving to next build with FOC on dual v3 on Vesc6
```

---
## \#12 Posted by: caustin Posted at: 2017-06-23T02:46:10.697Z Reads: 111

```
All on 12s btw
```

---
## \#13 Posted by: Michaelinvegas Posted at: 2017-06-23T04:22:59.265Z Reads: 106

```
I run 12s foc on a 2.5v carvon ... like butta
```

---
