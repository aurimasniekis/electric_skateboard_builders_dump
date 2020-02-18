# Maytech VESC in FOC

### Replies: 15 Views: 1941

## \#1 Posted by: Sarky1 Posted at: 2017-01-03T20:20:00.991Z Reads: 334

```
Hey Guys,

I'm wondering if anyone is running Maytech VESC in foc mode. Have you had any issues?
```

---
## \#2 Posted by: wmj259 Posted at: 2017-01-03T20:21:09.988Z Reads: 334

```
@Baz_L might know.
```

---
## \#3 Posted by: Baz_L Posted at: 2017-01-03T20:34:51.430Z Reads: 330

```
Nope haven't tried in FOC mode before. Everything's smooth in BLDC mode for me anyway
```

---
## \#4 Posted by: Sarky1 Posted at: 2017-01-03T21:24:41.796Z Reads: 308

```
Yeah smooth for me just wondering if its worth the switch.
```

---
## \#5 Posted by: Eboosted Posted at: 2017-01-04T00:26:48.462Z Reads: 288

```
I'll try FOC mode after one month runing BLDC, I've seen too many DRV errors and fried VESC to be 100% comfortable!
```

---
## \#6 Posted by: lrdesigns Posted at: 2017-01-04T10:18:11.458Z Reads: 266

```
When I ordered mine they said don't use VOC. So I would take that as a no or quite risky.
```

---
## \#7 Posted by: Sarky1 Posted at: 2017-01-04T16:52:55.732Z Reads: 248

```
Yeah I was also warned but I'm wondering if this is simply because of people blowing up the chips with the incorrect settings. I will talk to my contact at Maytech and see if I can get some more info.
```

---
## \#8 Posted by: themegak Posted at: 2017-01-04T17:04:35.190Z Reads: 239

```
It must be people blowing their drv's from not setting up properly.  I've been riding only in FOC mode for some time on my builds with sensored motors.  Got to tell you it is silky smooth and quiet.  Won't go back to BLDC.  If you try FOC mode, make sure you watch "realtime data" while you are testing on the bench.  If the vesc throws errors then stop immediately and adjust your settings.  Honestly, if more folks watched "realtime data" on the bench it would result in way less issues.
```

---
## \#9 Posted by: Sarky1 Posted at: 2017-01-04T19:46:00.399Z Reads: 222

```
[quote="themegak, post:8, topic:15603"]
you are testing on the bench.  If the vesc throws errors then stop immediately and adjust your settings.  Honestly,
[/quote]

Thanks, is this on Maytech VESC's ?
```

---
## \#10 Posted by: fraannk Posted at: 2018-04-26T08:17:07.730Z Reads: 132

```
I would like to know as well! 

Anyone knows which components to upgrade to get the Maytechs FOC compatible? :) 

(sorry for bumping)
```

---
## \#11 Posted by: themegak Posted at: 2018-04-26T14:05:54.508Z Reads: 109

```
I don't think it is worth it to try and upgrade a maytech vesc.  You are better off buying a better vesc (focbox, ollin, vesc 6).   That being said you can try foc with Maytech vescs but watch realtime data like i said when you are testing on the bench and start with very conservitive batt / motor amp settings.  You can always ramp up while testing and see what happens.  But do not try to ride it unless you have verified no errors on the bench.  It is very easy to blow the DRV's on Maytech Vescs.  I think you might be better off just going BLDC on the Maytechs you have and upgrade to an FOCBox later and try FOC then.
```

---
## \#12 Posted by: themegak Posted at: 2018-04-26T14:10:06.420Z Reads: 103

```
Yes this would especially be true for Maytech vescs which i believe are the lowest quality vescs available.  Always watch realtime data on the bench it will save you a lot of time and heartache when you are testing your setup on the bench.
```

---
## \#13 Posted by: evoheyax Posted at: 2018-04-26T14:16:59.763Z Reads: 100

```
Well the reason it’s not recommended is the default 4.12 BOM doesn’t include upgrades that make it more stable in foc. Chaka experimented for a fee years to get the 4.12 super stable and was successful. Even posted his upgrades here on the forum. But no one is making them with those upgrades right now. Which is why it’s more risky.
```

---
## \#14 Posted by: fraannk Posted at: 2018-04-26T14:19:21.394Z Reads: 98

```
Yeah, it’s because I just tried FOC on my FOCBOX’es on my main build, and it’s so smoooooth, and the budget is not there right now to upgrade those Maytech’s to two FOCBOX’es..
```

---
## \#15 Posted by: jordan314 Posted at: 2019-01-15T18:15:55.227Z Reads: 40

```
Hi,
I'm wondering if I broke my maytech VESC by trying FOC mode first.
I bought two maytech FOCs from ebay. The hardware was just a decimal point version off so I updated the firmware. I'm trying 90mm maytech hub motors that are rated at 25A, so I put my motor current control at 20A and -20A. My battery is rated at 30A, so I tried a 25A limit and -10A for recharging, and tried FOC mode.
The VESC utility can spin up the motors during test mode in both FOC mode and BLDC mode. But when I tried the arrow keys to spin the motor the VESC blinks red three times and the wheel tries to move but doesn't. When I try it in BLDC mode it also doesn't move, but doesn't blink red. I tried the other VESC in BLDC first, and I can spin it with the arrow keys. But the first one doesn't work with the arrow keys. However it can still spin the motor during test mode. Does that mean I blew the VESC somehow?
```

---
