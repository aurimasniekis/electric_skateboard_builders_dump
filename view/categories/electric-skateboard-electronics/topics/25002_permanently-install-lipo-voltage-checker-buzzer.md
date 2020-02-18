# Permanently install LiPo voltage checker/buzzer?

### Replies: 24 Views: 4719

## \#1 Posted by: kidcisco Posted at: 2017-06-09T23:36:47.519Z Reads: 252

```
Is it possible to permanently mount a LiPo buzzer (like linked) to my board so that I can check the voltage and get notified while I'm riding? Not well versed with electronics so any advice is appreciated.

My setup:
2x Turnigy 5000mAh 3S 20C Lipo Pack (wired in series)

LiPo Alarm Buzzer:
https://www.amazon.com/RioRand-C23212-Voltage-Checker-Warning/dp/B003Y6E6IE/ref=pd_lpo_vtph_21_bs_tr_t_2?_encoding=UTF8&psc=1&refRID=8HJSXHSTC8XSB1BZ8EVE
```

---
## \#2 Posted by: Smorto Posted at: 2017-06-10T00:18:21.735Z Reads: 241

```
Yes it is possible, people have done it before but it is not recommended. This is because these checkers generally drain voltage from one cell which might make your pack uneven. A voltage meter like this one is much better.

https://www.amazon.com/RioRand-Waterproof-Digital-Voltmeter-Motorcycle/dp/B009XQKCQY/ref=sr_1_12?ie=UTF8&qid=1497053854&sr=8-12&keywords=voltage+meter
```

---
## \#3 Posted by: IsTalo Posted at: 2017-06-10T10:22:22.881Z Reads: 218

```
DON't USE A BUZZER

Seriously, own experience, it was 4am, and I would wake up at 5:40Am to go to school, than the buzzer started bipping inside of my enclosure, I was so sleepy and had to open all six screws and disconnect it from the battery, it was consuming one cell more than the others and now my battery is unbalanced and I need a Bms hehe
```

---
## \#4 Posted by: lowGuido Posted at: 2017-06-10T10:48:18.983Z Reads: 212

```
Yeah i use these in pretty much all my builds.
Don't leave them on all the time obviously. Just switched with the board main power. Doesn't unbalance the cells. 
https://www.instagram.com/p/BP6RyQgh318/
```

---
## \#5 Posted by: kidcisco Posted at: 2017-06-10T20:39:03.673Z Reads: 190

```
Nice. I'm wondering if there might be a slimmer version of on of those meters as I'd like to mount it to the top of my board so I can see it while riding. 

Also, would you mind linking me to that circuit breaker thing you use to turn the board on? That looks like a decent solution to powering the board on and off safely.
```

---
## \#6 Posted by: kidcisco Posted at: 2017-06-14T08:55:45.164Z Reads: 176

```
BTW it was your youtube video that made me more forward with my first build. One other question though - the ESC I plan on getting (X-Car 120A) says that it has a low-voltage cut off....is a meter/buzzer even necessary if it's got this? I'm assuming that when it gets to a point that's too low it will just shut off..or am I wrong?
```

---
## \#7 Posted by: lowGuido Posted at: 2017-06-14T09:01:03.277Z Reads: 170

```
you can just go with the low voltage cut off of the ESC but its just an over all voltage so if you have one cell that is a little weaker than the others it wont pick that up, where as a lipo alarm will check each cell.[quote="kidcisco, post:6, topic:25002"]
it was your youtube video that made me more forward with my first build
[/quote]

Im glad that im making a difference in the Esk8 world.
```

---
## \#8 Posted by: kidcisco Posted at: 2017-06-14T09:24:26.621Z Reads: 165

```
Thanks for everything you've done. So since I'm building my first board now and I want to be as careful and cautious about treating the batteries properly (while staying on budget) what's the best thing I can do to keep my batteries in good condition: relying on voltage cutoff, having a buzzer hooked up when the esc is on, having a mounted voltage meter and eyeing (similar to what was linked up top) or what?
```

---
## \#9 Posted by: pjotr47 Posted at: 2017-06-14T09:39:13.180Z Reads: 154

```
And how do you switch off the lipo teste? positve wire? negative wire from lipo tester?
```

---
## \#10 Posted by: lowGuido Posted at: 2017-06-14T09:59:02.226Z Reads: 149

```
Negative wire switched.

@kidcisco I think the best way to look after batteries is to never fully discharge them and slow charge them on low current when you charge them back up.
I got lipos that are 3 years old with daily use and no signs of puffing or cell imbalance..
```

---
## \#11 Posted by: kidcisco Posted at: 2017-07-07T08:56:54.161Z Reads: 134

```
@lowGuido Hey man, I'm following all your videos for my first build and I'm stuck on two things - this low voltage buzzer and connecting my batteries to my 6s adapter (not sure which battery goes in which side). If you ever get a few minutes could you possibly explain to me (I'm very visual and not expirienced in electronics) how to permanently mount this lipo buzzer so that it turns off when the board is off (using anti spark loop). It's either this alarm or I get a cheapo screen like your latest video and do it like that but I already bought this so I'd like to use it (I like how it has an alarm also). Thanks bro.
```

---
## \#12 Posted by: lowGuido Posted at: 2017-07-07T12:15:42.509Z Reads: 127

```
the trick is to use the anti spark loop key on the negative wire. then you can put the negative of your lipo alarm in after the loop.
understand that that's not how I did it in my video because I used a different type of voltage display on that one.


http://www.electric-skateboard.builders/uploads/db1493/original/2X/b/bab1353099cd12f59ebeab37ab3f88ac0431d5fb.PNG
there is a diagram here however be aware when I drew the diagram I put the number display facing forwards to look nice. In reality the display would be on the back because the negative is the first pin from the left.
```

---
## \#13 Posted by: kidcisco Posted at: 2017-07-10T22:10:35.473Z Reads: 114

```
@lowGuido

The diagram helps a lot. In your opinion should I use this voltage meter buzzer or just use one of those illuminated meters (like the one in the video you uploaded recently) and mount that to the front of my board? Do the meters you used in the video detect the voltage in each cell or is as a whole? My main concern is safety and battery longevity.

Also, noticed one of the balance leads has the black wire cut - is this necessary? I've read something about this - as a way to prevent a problem if you connect the batteries wrong, am I right?
```

---
## \#14 Posted by: lowGuido Posted at: 2017-07-11T00:37:47.076Z Reads: 107

```
I like the buzzer because it is cheap and loud.  So there is no mistake when you need to stop. They also watch each cell where as the illuminated meter only shows overall voltage. 

The cut wire is cut because it is not needed and there really is no point connecting it.
It just adds confusion.
```

---
## \#15 Posted by: kidcisco Posted at: 2017-10-14T00:07:06.526Z Reads: 93

```
Could you kindly look at how I wired up my lipo alarm and tell me if it looks right. It's a little messy but I want to be sure before I connect it. 

The negative wire from the alarm isn't attached but does it go BEFORE or AFTER my anti spark loop key?

Which battery connects to which balance lead? That part really confuses me...

<img src="/uploads/db1493/original/3X/7/c/7cd79fe400994b8edae0bf271214394ee01f56ab.jpg" width="281" height="500">
```

---
## \#16 Posted by: lowGuido Posted at: 2017-10-14T11:45:29.473Z Reads: 90

```
looks legit.
Just make sure you get the batteries the right way around when you plug the balance leads in.

And the negative goes on the esc side of the loop which must be on the negative battery discharge lead.
```

---
## \#17 Posted by: kidcisco Posted at: 2017-10-14T18:55:59.547Z Reads: 85

```
Sweet, thanks. Btw, for reference, 

[Just plug the batteries in this order](http://www.electric-skateboard.builders/uploads/db1493/original/2X/b/bab1353099cd12f59ebeab37ab3f88ac0431d5fb.PNG)? (Lipo alarm is actually flipped around though right?)

Also, I had a question about that diagram you made. Why does it have a charger port on there if you charge using the balance adapters? Am I missing something or is that necessary?
```

---
## \#18 Posted by: lowGuido Posted at: 2017-10-14T21:32:58.009Z Reads: 76

```
when I originally built that I was using the deans connector as a charging port, that was before I realised that I could save a bit of wiring/weight/hassle by just charging the balance leads.

and yes that diagram is correct with the exception of the lipo alarm being flipped because it made the diagram look nicer if I drew the display on it even though it is technically the BACK of the alarm.
```

---
## \#19 Posted by: kidcisco Posted at: 2017-10-31T20:21:33.744Z Reads: 69

```
Will I need to reset the alarm voltage level everytime I power down my board and want to use it? I have it permanently wired to the negative battery before the anti spark switch.
```

---
## \#20 Posted by: kidcisco Posted at: 2017-11-04T10:31:30.167Z Reads: 71

```
@lowGuido

So I've had 4 battery packs mysteriously drain themselves in the past 2 weeks and I haven't even riden my board one time. I've had the board hooked up, batteries connected to esc, balance plugs connected to the charging port with lipo alarm wired in (exactly how you do it), but I've left the loop key out, so it 'hasn't had power'. No lights, no beeps, nothing... But my batteries are dying while sitting for a few days, even though nothing has power. What could be causing this?
```

---
## \#21 Posted by: lowGuido Posted at: 2017-11-04T10:47:32.356Z Reads: 66

```
weird.
charge them up and then remove the lipo alarm completely and see if they still drain.
I can't see where the battery can be draining if you have removed the loop key?
do you have a clear photo of the wiring setup?
```

---
## \#22 Posted by: kidcisco Posted at: 2017-11-05T07:34:39.042Z Reads: 65

```
I pretty much copied your wiring videos and diagrams 100%. 

The one thing I'm not sure about is this (don't mind the messy connections. With the lipo alarm, is the 4th wire (the one i attached to the middle red wire) supposed to be on the red wire, black wire, or both, or does it matter? Could this be causing an issue?

<img src="/uploads/db1493/original/3X/7/c/7cd79fe400994b8edae0bf271214394ee01f56ab.jpg" width="281" height="500">

It could also be a power supply issue for my charger. I finally got a 12v 6a charger and and am balancing the packs now to see if I can try again. Before with my 3a charger i couldn't even charge passed 3.7 unless i dropped the amperage to 1-1.5a...
```

---
## \#24 Posted by: ricoghardforth Posted at: 2018-03-20T13:03:03.605Z Reads: 44

```
I've bought two of these, one each for my zippy 5000MAh 5S1P batteries.  Do they really take that much power from a single cell to cause problems with leaving one cell unbalanced. Shurely nobody would use them if this was the case.  I would think the size of the cells I'm using wouldn't be affected that much with the 10's of mAh the display would use for the duration of the ride.  I want to add a switch so I can power them off when I don't want them on.  Will adding a switch inline on the negative line to pin 1 do this. I was going to use a double pole double throw and switch both off from the one switch.

[1-6s lipo alarm](https://www.ebay.co.uk/itm/2x-RC-Lipo-Battery-Low-Voltage-Alarm-1S-8S-Buzzer-Indicator-Checker-Tester-LED/302607233502?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649)
```

---
## \#25 Posted by: dragopepper Posted at: 2018-03-20T14:27:49.312Z Reads: 41

```
Maybe it's better to buy one of this:
https://www.banggood.com/12V-6-63V-LCD-Acid-Lead-Lithium-Battery-Capacity-Indicator-Digital-Voltmeter-p-1233260.html?rmmds=myorder

yes this one don't show the voltage of every single cell, but it switch off automaticly after a couple of seconds.
I have additional combined it with a loop key.

![IMG_20180320_152138|690x387](upload://lZK8oDv1NeZiT5FmKmo84mvGq2g.jpg)
```

---
