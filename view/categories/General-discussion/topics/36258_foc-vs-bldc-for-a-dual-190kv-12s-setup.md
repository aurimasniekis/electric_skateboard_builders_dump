# FOC vs BLDC for a Dual 190kv 12s setup

### Replies: 23 Views: 2002

## \#1 Posted by: Mattmccrary8 Posted at: 2017-10-23T14:03:30.029Z Reads: 291

```
Ok I have done my fair share of reading. I just blew out my first vesc by burning the DRV. 

My setup - All TB products VESC’s, dual 6374 190kv motor, 12s4p battery, 100mbs wheels, 16/36 gearing but soon to be 16/40 with either 97 or 107abecs. 

I was being dumb trying to shave down my MBS wheels like kaly and one vesc blew out. I was in FOC mode.

My question is. To avoid burning another VESC, is FOC to strenuous for my setup because I’m already pushing the erpm limit? Should I just stay in bldc mode? I want my board to go consistent 30-35mph without blowing out anything
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2017-10-23T15:02:09.692Z Reads: 282

```
First foc to from what I have read only supports 10s or is very not stable at 12s , second you can't just throw any vesc into foc most vesc on the market will get the DRV blown because the components quality is not good enough, if you want to run foc the only good vesc to do that are , Ollin vesc , Enertion and vesc 6.0 someone correct me if am wrong here
```

---
## \#3 Posted by: Mattmccrary8 Posted at: 2017-10-23T15:07:32.334Z Reads: 280

```
That’s exactly why I blew one. So my new question would be, can I get a smooth start with no cog in bldc mode. 

Is there such thing as running bldc mode sensored or is that pointless?
```

---
## \#4 Posted by: Jinra Posted at: 2017-10-23T15:07:36.829Z Reads: 267

```
Don't use a TB vesc for foc, they're known to fail on that mode
```

---
## \#5 Posted by: Exiledd_Top Posted at: 2017-10-23T15:10:02.149Z Reads: 266

```
I've don't know , I assume there is a sensored bldc , I've never done it , but yes sensored has a gradual acceleration on start up smooth , I've seen a sensored board before
```

---
## \#6 Posted by: b264 Posted at: 2017-10-23T15:19:22.860Z Reads: 269

```
[quote="Jinra, post:4, topic:36258, full:true"]
Don't use a TB vesc for foc, they're known to fail on that mode
[/quote]

What's the best esc/vesc for foc?
```

---
## \#7 Posted by: MontPierre Posted at: 2017-10-23T15:22:17.113Z Reads: 259

```
Focbox!  Obviously there have been cases of DRV’s blown on FOCBOXes but very rear. I’m not aware of any totally bullet proof vesc but focbox seems to be a winner lately. vesc 6 could be game changer as well ;)
```

---
## \#8 Posted by: evoheyax Posted at: 2017-10-23T15:25:09.942Z Reads: 259

```
[quote="Exiledd_Top, post:2, topic:36258"]
First foc to from what I have read only supports 10s or is very not stable at 12s
[/quote]

Not true. I run 12s FOC (or should I say, ran :( ) with hummies v4 motors, never had an issue with 12s and FOC.

But again, this is with hub motors. The reason your hearing this is likely the erpm limit. Because belt drive motors spin at higher erpm's, they can get closer to the limit and in a lot of case, go above the limit and thus blow their DRV chip. If running hub motors, since its a 1:1 gear ratio, you can't get close to the erpm limit unless your going like, 60 mph, maybe then. So 12s FOC with hubs is safe.

You are right though that not every vesc is equal. I use chaka vescs and now, I'm messing with FOCBOX's. They seem to support FOC fine. Again, don't go over the erpm limit though. That is why the DRV blows more often than not on the FOCBOX or a chaka vesc.
```

---
## \#9 Posted by: willpark16 Posted at: 2017-10-23T15:29:53.486Z Reads: 243

```
ive seenvery few focbox errors a decent majority due to user error, the ones that were manufacturing error you were able to send back to enertion
```

---
## \#10 Posted by: Jinra Posted at: 2017-10-23T15:38:52.138Z Reads: 240

```
The only one I can say is Ollin Vesc. I'm sure FOCboxes are great and have 2 of them myself, but I haven't used them yet. Those and the VESC6 for obvious reasons.
```

---
## \#11 Posted by: GrecoMan Posted at: 2017-10-23T15:43:02.907Z Reads: 244

```
definetly @chaka vescs. period.
```

---
## \#12 Posted by: ShutterShock Posted at: 2017-10-24T06:49:25.222Z Reads: 234

```
I run BLDC sensored and I think it is way better than just the standard VESC sensorless.  To be more specific I run it in hybrid mode so that at higher speeds it switches to sensorless. Perfect smooth startup every time.
```

---
## \#13 Posted by: Mattmccrary8 Posted at: 2017-10-24T13:11:50.651Z Reads: 224

```
How do you set this up. It sounds amazing. Do I just click the hybrid button on the top. I don’t want to blow another vesc
```

---
## \#14 Posted by: guyguy Posted at: 2017-10-24T13:36:05.050Z Reads: 216

```
Been running FOC with ollin vescs for about 900 miles with no issues
```

---
## \#15 Posted by: GrecoMan Posted at: 2017-10-25T00:42:33.504Z Reads: 199

```
OLLIN FTW!

10chars
```

---
## \#16 Posted by: thisguyhere Posted at: 2017-10-25T00:43:58.769Z Reads: 200

```
12s FOC? ...
```

---
## \#17 Posted by: guyguy Posted at: 2017-10-25T01:00:52.133Z Reads: 196

```
10s

10 chars
```

---
## \#18 Posted by: jmasta Posted at: 2017-10-25T01:08:57.621Z Reads: 192

```
190kv is too high for 12s on v4 VESC hardware, FOCbox included.  Did you have a 60k ERPM limit programmed?  You probably wouldn't reach this limit while actually riding it, but were trying to shave down the wheels with the board unweighted. Sounds like the source of your DRV failure...
```

---
## \#19 Posted by: ShutterShock Posted at: 2017-10-25T04:55:12.456Z Reads: 190

```
Yep just click hybrid, and do motor detection with the hall sensors and fill it into the table. Obviously you have to have your motor sensors connected to the VESC
```

---
## \#20 Posted by: SORRENTINO Posted at: 2017-10-25T05:00:36.400Z Reads: 191

```
Enertion focbox is horrible also and this was in bldc mode. :sob: <img src="/uploads/db1493/original/3X/4/e/4e76432a53db327a60938a2cd39dc43c7f24e8c7.jpg" width="666" height="500">
```

---
## \#21 Posted by: Colson003 Posted at: 2017-10-25T05:23:05.132Z Reads: 186

```
I'm currently running TB vesc FOC sensored with hubth 6s, so yeah that points more toward erpm. haven't had an issue other than heat.
```

---
## \#22 Posted by: jmasta Posted at: 2017-10-25T06:00:01.867Z Reads: 181

```
I mean essentially FOCbox is just the VESC 4.12 repackaged with better thermal management.  They put direct FETs on the same side and added a heatsink to handle higher current loads.  But at the heart of it, it's still VESC v4, and thus still plagued with the same problems.  The key is just convincing everyone it's better :smirk:
```

---
## \#23 Posted by: Achmed20 Posted at: 2018-01-15T23:30:11.096Z Reads: 146

```
meh ...
got a new trampa board here and now i cant decide if i try FOC on 12S with 2 190KV motors and 2 focboxes or not. 

as far as i understood it only becomes a problem at +60k erpm, so would it help if i just set the erpm limit to 55k just to be safe? i usualy dont drive faster then 35kmh so the 12S setup is mainly for gaining watt hours.
```

---
