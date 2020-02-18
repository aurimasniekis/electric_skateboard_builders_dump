# 12s and FOC - is it safe or not?

### Replies: 22 Views: 888

## \#1 Posted by: accrobrandon Posted at: 2018-08-24T14:40:20.062Z Reads: 230

```
Most posts are older and still are about 50/50 on whether running foc on 12s is safe or not and looking for a more current answer or opinions? to foc or bldc...

Im building a 12s 30q at some point this week w/ an 80a bms. On focboxes dual 6355 190kv motors..

where do we all stand now a days on it or any particular settings limits if going FOC?

thanks!
```

---
## \#2 Posted by: Blitz Posted at: 2018-08-24T14:41:51.241Z Reads: 230

```
FOCbox
I've heard that can run Foc safely. and I believe 12s should be fine (but maybe i'm mistaken) 

And here you can see a small debate from @b264 for team 10s.
https://www.electric-skateboard.builders/t/advantages-of-10s/65801/15
```

---
## \#3 Posted by: longhairedboy Posted at: 2018-08-24T14:57:20.184Z Reads: 217

```
Yes. 12S on FocBoxes in FOC mode is perfectly fine. This is a 12S5P 30Q on FOC with FocBoxes:

https://longhairedboy.com/collections/all/products/witchblade-gt-candy-crusher-edition

All I do now is 12S FOC on FocBoxes for customer boards.
```

---
## \#4 Posted by: Blitz Posted at: 2018-08-24T15:02:40.140Z Reads: 195

```
Man, every-time i see that board I get butterflies.
```

---
## \#5 Posted by: Kug3lis Posted at: 2018-08-24T15:05:14.975Z Reads: 194

```
So far I run without issues regarding 12s FOC, but many things depend how you build, your battery pack, wiring and all other variables, because there are so many variables which can influence it..
```

---
## \#6 Posted by: ARetardedPillow Posted at: 2018-08-24T15:06:28.559Z Reads: 190

```
Is there a difference between voltage spikes and running FOC and BLDC? Just curious
```

---
## \#7 Posted by: Kug3lis Posted at: 2018-08-24T15:09:02.677Z Reads: 189

```
FOC runs a lot of calculation to produce sine looking control waves, and that means more mosfet switching much more stress and etc compared to bldc, which just runs :)

https://i.stack.imgur.com/ccHs1.jpg

EDIT:

FOC = sinusoidal control
BLDC = trapezoidal control
```

---
## \#8 Posted by: ARetardedPillow Posted at: 2018-08-24T15:10:28.418Z Reads: 178

```
Whelp, BLDC it is, I like the noise of BLDC anyways
```

---
## \#9 Posted by: Saturn_Corp Posted at: 2018-08-24T16:41:15.059Z Reads: 155

```
Since it looks like FOC with 12s should be fine, what should be avoided in settings wise or other, when running FOC?
```

---
## \#10 Posted by: Hummie Posted at: 2018-08-24T16:51:19.140Z Reads: 152

```
i thought foc was more a hair more efficient in the esc..or is it the motor?
```

---
## \#11 Posted by: Kug3lis Posted at: 2018-08-24T17:05:31.265Z Reads: 150

```
About efficiency I can't tell much, but FOC makes sound better by simulating perfect sinusoidal, more switching more losses at mosfets and etc, so I don't know if FOC is more efficient...
```

---
## \#12 Posted by: Battosaii Posted at: 2018-08-24T17:05:35.695Z Reads: 148

```
I do notice my motors get noticble more warm on FOC than BLDC but I love the smoothness and I do miss the noise.

I've been running FOC on 12s on VescX and Focbox with great success.
```

---
## \#13 Posted by: Hummie Posted at: 2018-08-24T17:12:25.903Z Reads: 151

```
it makes sense the motor would run a bit cooler on foc as the current it receives would be sine not trap waves but the esc would get hotter as it has to do more switching.  ive never compared and am always in foc though
```

---
## \#14 Posted by: longhairedboy Posted at: 2018-08-24T17:46:31.976Z Reads: 146

```
Some people are wondering about battery types and wiring and all the variables. 

I use 12AWG wire throughout my builds. From the pack mains through the deck and all the way to the stator windings is 12awg with the exception of the focbox phase tails which are 14 awg i think. I think that probably makes some difference. I've never had very good luck with those shitty phase leads that usually comes on motors. A good hard regen down a fast hill will melt those things. 

I also try to keep the distance between the battery and focboxes at a minimum.  The way i build my decks means i have long sensor and phase leads, however.  I'm not sure how that affects things, but it doesn't seem to have a negative effect if it does.

BLDC v FOC is kind of a personal choice. BLDC will give you a higher top end speed than FOC, but FOC gives you a level of polish you can't get with BLDC. And when all the extra top end is over 35mph anyway.... i mean most people really don't care to go that fast.
```

---
## \#15 Posted by: Deakbannok Posted at: 2018-08-24T19:39:56.403Z Reads: 128

```
I ran 12s6p 30Q FOC VESC 4.10 from ﹰChiang ﹰMai to ﹰPai in 2 days without issue. It was one hella ride through the passea. Because the first day storm showed up.
```

---
## \#16 Posted by: Toughook Posted at: 2018-08-24T22:09:18.339Z Reads: 117

```
Ok, I'm running dual 6374 with focbox. Unsensored BLDC 10s5p. 

What exactly am i missing out on? My board runs just fine. It's fast, the brakes work, and as far as I can tell, it's quiet. 

Are we talking big % increases over my current set-up, or marginal gains?
```

---
## \#17 Posted by: Eboosted Posted at: 2018-08-25T05:11:13.120Z Reads: 98

```
All my fast builds are 12s, my favorite lightest board is 10s3p and it's not slow but I love when I need to grab mall it
```

---
## \#18 Posted by: Highwon Posted at: 2018-08-25T05:36:55.736Z Reads: 94

```
I’m foccing with 12S to and no problems!
```

---
## \#19 Posted by: Skunk Posted at: 2018-08-25T05:58:33.043Z Reads: 92

```
[quote="longhairedboy, post:14, topic:65948"]
I also try to keep the distance between the battery and focboxes at a minimum
[/quote]

I plan on filling the cutout of my @Hummie deck with all battery.(12s5) so I had planed on mounting my focboxes in the cnc heatsink case @Kug3lis makes. I'm guessing around 10 inches between battery and controller.  Do you think that's okay.  Or should I shot for getting them a bit closer?
```

---
## \#20 Posted by: Hummie Posted at: 2018-08-25T06:44:36.341Z Reads: 81

```
there's math calculation based on the diameter and length and the inductance produced in the wire but then it seems to go out the window according to people who do the math and some people are using wires longer than they should be able and not breaking.   better to go the shortest fattest battery wires to reduce the inductance.  10 inches is generally thought of as fine if 10 awg
```

---
## \#21 Posted by: 370HSSV Posted at: 2018-08-25T07:24:29.709Z Reads: 77

```
been running 12S4P FOC mode on VESCX for couple month now, no problem at all. Motors are 170kv 6374s
```

---
## \#22 Posted by: Andy87 Posted at: 2018-08-25T08:26:27.317Z Reads: 70

```
I see a lot of guys with a mtb built, battery in the middle of the deck and the vescs on the tail.
The wires surely about 40-50cm there.
Would like to know if there any complications appear?
```

---
