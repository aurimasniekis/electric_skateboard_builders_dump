# Hobbyking VESC + FOC

### Replies: 28 Views: 2114

## \#1 Posted by: Kookaburra Posted at: 2018-04-06T11:37:11.807Z Reads: 345

```
In the forum, there are a bunch of posts about people frying there VESCs with FOC. 
I recently received my Hobbyking VESC (HW 4.10) and I want to know if it is safe to operate in FOC mode?
```

---
## \#2 Posted by: Tuomalar Posted at: 2018-04-06T11:44:12.463Z Reads: 343

```
[quote="Kookaburra, post:1, topic:51387"]
a bunch of posts
[/quote]

Answer is simple AF: Don't do it.
```

---
## \#3 Posted by: Jakebarnhill1 Posted at: 2018-04-06T12:29:36.062Z Reads: 340

```
don't do it! I've tried it with hobbyking VESCS and they fry within a few minutes, although it depends on the motor, it would be more likely to work on a hub motor with high inductance, over a regular outrunner.

when I tried FOC with hobbyking VESC on my hub motors it didn't fry the vesc but the motors didn't run well at high RPM. I would stick to BLDC. When I tried FOC on a 190kv SK3 6363 the vesc fried within a few minutes!
```

---
## \#4 Posted by: squishy654 Posted at: 2018-04-06T13:05:19.655Z Reads: 325

```
I ride all my hobbyking vesc's in foc mode without any issues at all..never fried one using the motor made for it..
```

---
## \#5 Posted by: Acido Posted at: 2018-04-06T13:14:22.496Z Reads: 309

```
Unless you have focbox its a  total 100% sure NO lol
```

---
## \#6 Posted by: squishy654 Posted at: 2018-04-06T13:29:28.937Z Reads: 296

```
My experience doesn't seem to jive with what people are saying and that reputation was formed before the hk vesc was even released..I think it's from torque vesc..
```

---
## \#7 Posted by: Tuomalar Posted at: 2018-04-06T13:54:21.124Z Reads: 283

```
Well HK vesc’s reputation might be worse than it truly is, but 4.12 vesc’s reputation with FOC is something to bear in mind. 

In the other words: if u have extra money and you don’t know what to do with it give HK vescs a change. If u are on budget use BLDC.
```

---
## \#8 Posted by: squishy654 Posted at: 2018-04-06T14:18:31.163Z Reads: 277

```
Maybe you guys didn't hear me, but I run foc on 5 different hk vesc without any issues over thousands of miles on both 10 and 12 cell...all my rides use it..and it's never failed or fried once...
```

---
## \#9 Posted by: squishy654 Posted at: 2018-04-06T14:20:14.095Z Reads: 269

```
I'm not as dishonest as an outdated reputation, obviously lol..seems TB vesc is the cause of the reputation which was established before anyone gave hk a chance..
```

---
## \#10 Posted by: TarzanHBK Posted at: 2018-04-06T14:43:01.265Z Reads: 262

```
but your running them all with the low kv HK motor?
Have you tried it with a 190 kV on 12s?
```

---
## \#11 Posted by: squishy654 Posted at: 2018-04-06T14:54:42.305Z Reads: 254

```
Sure have..
```

---
## \#12 Posted by: Blitz Posted at: 2018-04-06T14:56:50.435Z Reads: 250

```
I Heard someones HK vesc died 6 months later and HK refunded and let him keep the corps.
I got the feeling that Hk was shady but I've gotten refunds received orders that had no tracking on them (to save monies) Its all good. for me <--
```

---
## \#13 Posted by: squishy654 Posted at: 2018-04-06T14:57:49.309Z Reads: 251

```
I shorted the phase wires on one once while riding it got caught on the motor and shorted out and fried obviously that is a mechanical failure and shorted phase wires that's the only time I've ever had a problem with 1
```

---
## \#14 Posted by: bigben Posted at: 2018-04-06T15:05:16.065Z Reads: 245

```
There have been a lot of problems with original form factor vesc 4. Here is someone, @squishy654 who is stating as fact that he has no problems with them. Is there anyone who can offer up as fact to the contrary that they don’t work? Rumour is not accepted.
```

---
## \#15 Posted by: squishy654 Posted at: 2018-04-06T16:09:20.684Z Reads: 238

```
This might come down to manufacture QC...also it might come down to people not setting them up correctly or trying to power too powerful of a motor, when they should have two or something...granted most of my boards use the HK 125kv motor, that motor is 2000W and pulls like a truck, so I don't see the issue...I use it mostly because it's smooth in FOC sensored mode and it's sealed so it is robust and lasts a long time, the 125kv is simply it's gearing, not a representation of it's overall power, it has very good torque with a 15/36 gearing on 97mm and 90mm, which is delivered smoothly up to into the 20's (mph)..which is fast enough to kill anyone without a helmet...right?

I have used the 170kv and 190kv SK3 motors in BLDC and FOC mode but they were not as smooth, due to not having sensors so I got some Ollin and LHB sensored motors for my dual setups...but as for a single motor setup, 125kv at 2000w is just about right, and I weigh over 200lbs..so give it a try..before you knock it..and realize kv is nothing more than "RPM per volt" it is not an indicator of power at all, only how that power is applied...
```

---
## \#16 Posted by: rojitor Posted at: 2018-04-08T00:48:08.221Z Reads: 213

```
![meme3367932059|340x333](upload://acjVH0L3SJay9Q3qsyk3SmmDkfu.jpg)
```

---
## \#17 Posted by: ervinelin Posted at: 2018-04-08T00:56:42.845Z Reads: 209

```
I run FOC on HK ESCs since day 1. One single, one dual drive... Only time they died on me was when they got wet in the rain...
```

---
## \#18 Posted by: Kookaburra Posted at: 2018-04-08T04:44:42.772Z Reads: 204

```
Thanks, which motor and battery configuration are you running?
```

---
## \#19 Posted by: ervinelin Posted at: 2018-04-08T05:55:35.926Z Reads: 201

```
Racerstar 5065, 10S2P and 10S3P
```

---
## \#20 Posted by: rey8801 Posted at: 2018-04-08T10:05:19.155Z Reads: 198

```
Thanks for sharing this information. Could you tell me which HK vesc you have been using? Good alternative if I need more vesc in future. Would you consider the ride with them as smooth as with other VESCs (TB, Maytech, Focbox ecc...)? Thx
```

---
## \#21 Posted by: squishy654 Posted at: 2018-04-08T16:31:21.423Z Reads: 180

```
There's only one vesc in the hobbyking store, just different listings for different warehouses
```

---
## \#22 Posted by: rey8801 Posted at: 2018-04-08T17:21:13.076Z Reads: 182

```
Found it https://hobbyking.com/it_it/turnigy-sk8-esc-for-electric-skateboard-conversion.html. Unfortunately out of stock. Althought the kit is available for a bit more and with other parts included. Not bad.
```

---
## \#23 Posted by: Kookaburra Posted at: 2018-04-11T18:06:07.971Z Reads: 173

```
Just to inform you:
-flashed ackmanias firmware to the VESC
-set up FOC
-ran it for roughly 20 km till now

Configuration:
Sk3 192kv + 6s LiPo
```

---
## \#24 Posted by: slick Posted at: 2018-06-08T21:22:17.776Z Reads: 154

```
...how is your Hobbyking-VESC running on FOC? any news? I was just wondering cause I have one too...
```

---
## \#25 Posted by: Kookaburra Posted at: 2018-07-16T06:07:29.988Z Reads: 128

```
It is still working like a charm
```

---
## \#26 Posted by: slick Posted at: 2018-07-28T07:10:22.956Z Reads: 108

```
excellent...I have mine running on FOC since day 1 and so far so good.
```

---
## \#27 Posted by: squishy654 Posted at: 2018-07-29T22:10:31.082Z Reads: 98

```
I told you guys lol, it works great on sensored foc, always has..
```

---
## \#28 Posted by: slick Posted at: 2018-07-31T06:33:46.695Z Reads: 67

```
works great with my sk3 5065 236kv motor running on 8S1P 5000mah LiPo. Been running since summer started and still going. I have to mention that I have been riding short distances...3 km to work and back home (total 6km per day)...so i havent experienced overheating yet. I've not done a range test yet since I dont  have full confidence in my belt drive -but- i am switching to chain drive as soon as my steel sprocket arrives.
```

---
