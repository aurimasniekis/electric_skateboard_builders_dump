# What is the problem of passing the ERPM limit?

### Replies: 26 Views: 3171

## \#1 Posted by: IsTalo Posted at: 2017-04-10T00:21:55.990Z Reads: 407

```
Hi, this month I discovered that vesc have a Erpm limit because the DRV chip don't supports more than 60K (Correct me), but this week I finally configured my board (And It works, it works :smiley:) and I saw that you can limit the ERPM-Don't remember where. 

So here is the question, where is the problem of passing the Erpm limit when I can limit it? Would it still be bad for the DRV chip?
```

---
## \#2 Posted by: Namasaki Posted at: 2017-04-10T00:43:28.603Z Reads: 404

```
What are the specs of your build?
```

---
## \#3 Posted by: treenutter Posted at: 2017-04-10T00:45:49.652Z Reads: 403

```
@IsTalo 

 https://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#4 Posted by: IsTalo Posted at: 2017-04-10T00:51:57.796Z Reads: 397

```
6s 6.3A/4260 300kv APS/Vesc/ 71mm wheels/ 36/16 037Xl pulleys/ Paris Trucks and some other stuff like Switch and Buzzer
```

---
## \#5 Posted by: IsTalo Posted at: 2017-04-10T00:57:23.454Z Reads: 374

```
Man, I know that is a Erpm limit, but I wanna know if there is any problem limiting it
```

---
## \#6 Posted by: treenutter Posted at: 2017-04-10T00:59:52.942Z Reads: 364

```
There is no problem limiting it. It is advised that you limit it. Perhaps I don't understand the question?
```

---
## \#7 Posted by: Namasaki Posted at: 2017-04-10T01:01:47.269Z Reads: 356

```
6s and 300kv is already below the erpm limit
25.2 x 300 = 7560rpm x 7 = 52900 erpm
The safe limit is 60000 erpm
```

---
## \#8 Posted by: IsTalo Posted at: 2017-04-10T01:26:35.386Z Reads: 344

```
The question is if that would wear out the Vesc and maybe break it, but I think It wouldn't
```

---
## \#9 Posted by: IsTalo Posted at: 2017-04-10T01:27:17.386Z Reads: 340

```
I know that it is safe, but everybode said thay the motor would blow, get too hot or don't have power to run, but it works great
```

---
## \#10 Posted by: Namasaki Posted at: 2017-04-10T01:31:50.875Z Reads: 327

```
Then its up to you to spread the word and put the myths to rest.
Make a video showing your setup and demonstrating its performance.
I for one would love to see it.
```

---
## \#11 Posted by: IsTalo Posted at: 2017-04-10T01:36:49.449Z Reads: 318

```
Sure, but I realized that I bought a belt bigger than the mount :smiley: and after 5 mins the belt was too loose and now I need to wait for the new belt, but I will make videos for sure
```

---
## \#12 Posted by: Namasaki Posted at: 2017-04-10T01:41:59.720Z Reads: 304

```
what size belt do you need?
```

---
## \#13 Posted by: IsTalo Posted at: 2017-04-10T01:50:46.300Z Reads: 302

```
It's a 114XL belt, I already ordered on the local shop, but will be ready in a few weeks
```

---
## \#14 Posted by: lowGuido Posted at: 2017-04-10T01:55:59.313Z Reads: 298

```
6s with 300kv on a 16/36 gearing should work. it will be a bit of a rocket though.
I have built loads of 6S 280kv 12/30 boards and they go quite well.

if all else fails you could gear it down a touch.

and definitely keep your long belt and add an idler. you will thank me later.
https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/e/0/e0c4b1fabf67523b0758897f9623cf9c3446c3ed_1_499x500.jpg
```

---
## \#15 Posted by: IsTalo Posted at: 2017-04-10T01:57:10.661Z Reads: 284

```
Sorry, but why? What is the difference between a longer belt and a smaller one?
```

---
## \#16 Posted by: lowGuido Posted at: 2017-04-10T01:57:14.907Z Reads: 278

```
114XL thats a huge belt
```

---
## \#17 Posted by: IsTalo Posted at: 2017-04-10T01:57:59.514Z Reads: 271

```
I bought 120Xl but it was big
```

---
## \#18 Posted by: lowGuido Posted at: 2017-04-10T02:02:44.571Z Reads: 268

```
yeah 120 is huge.. I would have thought a 102 or 104 would be a good size.
```

---
## \#19 Posted by: lowGuido Posted at: 2017-04-10T02:06:17.026Z Reads: 266

```
unless your mount is really long.
```

---
## \#20 Posted by: IsTalo Posted at: 2017-04-10T02:09:46.913Z Reads: 262

```
Noo, it is not long, but I calculated and the 114 will work perfectly
```

---
## \#21 Posted by: lowGuido Posted at: 2017-04-10T02:25:43.169Z Reads: 243

```
I usually get a small piece of wire and wrap it around the pulleys and then measure the wire. the length in inches is the part number of the belt. eg: 120 = 12.0 inches

also worth noting that the metric belts like 256 are in mm.
```

---
## \#22 Posted by: IsTalo Posted at: 2017-04-10T02:38:12.696Z Reads: 239

```
I calculated with a excel program, I'll try the wire tactic
```

---
## \#23 Posted by: jmasta Posted at: 2017-04-10T03:04:00.934Z Reads: 242

```
https://sdp-si.com/eStore/CenterDistanceDesigner

SDP/SI's center distance calculator is spot on. It tells you center-to-center distance and also number of teeth in mesh
```

---
## \#24 Posted by: Maxid Posted at: 2017-04-10T07:59:04.512Z Reads: 229

```
I have always used this one:
http://www.bbman.com/belt-length-calculator/
```

---
## \#25 Posted by: TarzanHBK Posted at: 2017-04-10T08:03:57.347Z Reads: 230

```
To answer your question about the ERPM Limit:
Vesc is capable of 100.000, but with some setups it gets jerky, so the opinion is 60.000 to be absolutly safe.
If you exceed that limit, vesc eventually loses connection to the motor and could start to stutter.
And worst case is a fried DRV chip due to that. (And maybe some broken bones due to high-speed-motor-stuttering).

So be safe and stay in the limit ;)
```

---
## \#26 Posted by: Kaly Posted at: 2017-04-11T09:57:09.018Z Reads: 202

```
@IsTalo

The 60K erpm  is a recommendation base on efficiency due to the accumulative effect of losses in a BLDC motor. 

You can read vedder explanations of the thinking behind this limit on this link. 
http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/
```

---
