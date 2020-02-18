# Electric Longboards for Larger Riders

### Replies: 16 Views: 4132

## \#1 Posted by: claudiofiore88 Posted at: 2015-09-04T18:36:38.200Z Reads: 184

```
So my current setup is a single drive with an sk3 213 kv running at 8s. I weigh 265 lbs+ (120 kg+). Although the board gets going, I've found that the motor likes to "fart" from a stand still, when accelerating too quickly, or stopping and slowing down. My question is should I swap for a lower kv motor like a 149 kv for the added torque, or should I invest in a dual drive setup?
```

---
## \#2 Posted by: treenutter Posted at: 2015-09-04T20:47:58.740Z Reads: 186

```
I think your options are (in the order I would attempt them, based on cost and complexity):

1) Try different settings on your current ESC, there may be parameters that can assist with cogging at "takeoff"
2) Modify your gearing to a different ratio to favor torque (larger drive wheel or smaller motor pulley) 
3) Try an ESC that is optimized for esk8... so VESC
4) Add hall sensors to your SK3 or move to a sensored motor\esc
5) If none of these work, move to dual motor setup
```

---
## \#3 Posted by: claudiofiore88 Posted at: 2015-09-04T21:30:10.730Z Reads: 183

```
I've tried or considered most of those you listed. I've tried playing around with the esc settings. Seems to make little difference. I've been looking around around for pulleys. I've got a 36:14 or about a 2.5:1 ratio. I've been trying to find a smaller, with no luck since my motor had an 8 mm shaft and the ones with less teeth are meant for a 6 mm shaft.
```

---
## \#4 Posted by: joren Posted at: 2015-09-04T21:54:05.944Z Reads: 174

```
I'm in your same boat!  In mountain biking terms, we're clydesdales!  

I'm setting up a board now and I'm gonna try a 50:12 ratio with 90mm wheels, 280kv motor. Dual motors.  I live on a hill too. When it gets up, I'll let you know if I get cogging.

Do you have the means to drill out the 12T gear to fit your 8mm shaft? If you don't want to buy a 8mm bit, 5/16" is only 0.025" smaller.  Easy to elongate with aluminum.  I'm sure this is silly, but is your belt tight enough?
```

---
## \#5 Posted by: claudiofiore88 Posted at: 2015-09-04T22:29:00.949Z Reads: 170

```
Wow!  A 50:12 is more than a 4:1.  I should be able to drill out the bore to make it fit.  What I realized the other day was that my small pulley was set backwards, so the 2 pulleys were not aligned with each other correctly ultimately ruining my belts teeth.  I'm sure that and the a possibly loose belt could have contributed to the excessive cogging, right?
```

---
## \#6 Posted by: sl33py Posted at: 2015-09-04T23:18:02.101Z Reads: 204

```
I'm about 265 out of the shower - so understand where you are coming from (6'8" / 2m).

Where are you in the states - i'm in seattle and you could try one of mine to compare!

I know that when the belt is loose and i brake too hard it starts skipping teeth - what you are hearing it seems like.  I'd first tighten your belt.

If besides that you are happy with the acceleration and top speed, you could look at a 15mm belt instead of a 9mm belt.  About the only one i know of who has these readily in stock is Torque/DIYes.  

I have a 200kv 63mm on my GF's board and it does pretty well getting me going, but hard brakes i still hear the teeth skip.

I'm setting up a guest board with 149kv SK3 6374 motor now and will see how it does in comparison.  I'm also in a slow build for my dual rear R-spec motors on a drop deck which is going to be awesome!  More is always better, but i really think the 200kv and 149kv on 12s is going to be plenty 90% of the time.  Still testing and will definitely chime in with my fellow Clydesdale brethren here!
```

---
## \#7 Posted by: onloop Posted at: 2015-09-05T01:28:56.870Z Reads: 203

```
One of the first boards I custom made was for a mate of mine who would be about 120kg.

At the time I didn't think those extra 30kg (I'm 90kg) would be a problem. So i built him this.

Dual 270kv 50mm Ntm propdrives 
14t motor : 36t wheel gearing
6S battery
83mm wheels.

For flat ground it was fine. Except his battery would last only 15 mins. Mine would last 25mins.

So it became obvious that the motors can drive the bigger load but they need more amps. Which equals heat...

Also the 6S 8000mah hobbyking zippy flight max batteries didn't like being discharged at such a high constant current. He went through three of these $120 batteries because they kept puffing up.

The motors and esc managed to hold up well.

Apart from battery going flat very quickly. The biggest problem was the system couldn't get him up the hills the rest of us where going up.

So we started trying different things.

1st I went smaller motor pulley 13:36 this was helpful, but still not enough to get him up the hill.

The hill I'm talking about is in this video, it's long & just keeps getting steeper.
https://www.youtube.com/watch?v=ioFqJPht2kM&feature=youtu.be

2nd we went for larger motors. The SK3 6354 at 245kv. Better but still could not get up the hill. The amps got too much and the Flier 120amp Dual ESC would just shutdown. 

It became my mission to build a rig that could do it. I figured we needed higher voltage but the problem was there where no ESC that could handle the high voltage.

Anyway I started designing better batteries that had much more Wh and higher voltage... Fortunately during this time the VESC started to be talked about.

I figured with the high voltage battery & vesc it would be the answer.

However I moved away and never got to try it.

This is what I would build now for my friend if money was no option.
4WD 6355 190kv motors.
10S & vesc. (People have been having issue with 12S  & vesc)
15:36 (15T has 6 teeth in mesh meaning it can transfer max torque)
83mm wheels. (Smaller wheels put less load on motors)
9mm wide belt is fine.

If money was an issue (it always is)
DD 6374 190kv (Diagonal Drive allows wide belts)
10s & Vesc
15:36 
15mm wide 5mm HTD belts.
83mm wheels.

If this didn't work. Try this
DD 6374 245kv (because it is in more efficient rpm range 8800rpm)
10s & Vesc
17:60 (3.5:1) 
3mm htd 15mm wide or wider. (With 3mm the belt needs to be as wide as possible)

39km/h top speed.

If that didn't work, keep increasing the reduction ratio. However you will eventually get to a point where the wheel pulley diameter cannot increase as it eventually hits the ground. Also you can't go below 17t on motor as there would be less teeth in mesh and more chance of belt slipping. Also as the diameter of the wheel pulley increase it also means less teeth in mesh on motor pulley!. So then you need to increase center distance to ensure belt angle does no become too obtuse. (The longer the center distance the more the belt wraps around the drive pulley putting more teeth in mesh)

If this all fails we need to invent a motor mount with dual stage reduction then we can stick with 5mm HTD 9mm wide which are common and cheap, now we may try to achieve 6:1 reduction. You won't have a very high top speed but you will go up any hill. 15:36 / 15:36 is 4.8 
14:42 / 14:42 is 6

That would be really awesome!
```

---
## \#8 Posted by: joren Posted at: 2015-09-05T01:56:42.161Z Reads: 181

```
Thanks for the great info. May I ask, has anyone ever used an idler pulley on the back side of the belt (cheap skate bearings) to properly tension the belt and provide more teeth in contact on the drive pulley? That may (hopefully) will be a way to use a smaller drive pulley at larger loads.
```

---
## \#9 Posted by: onloop Posted at: 2015-09-05T02:24:38.674Z Reads: 181

```
More reduction can never hurt.... I think it would be a nice option...

The team at leif did it. Looks like they are using 3mm pitch.

<img src='/uploads/db1493/original/1X/c6e6c3396b5ff78500e752928465e41e0b7e24e5.jpg'>
```

---
## \#10 Posted by: torqueboards Posted at: 2015-09-05T06:45:32.037Z Reads: 172

```
DUAL DRIVE --- > The single most best investment.

I've been riding a single 50mm on my normal commute which I normally use a 12S Dual Diagonal 50mm Build which is capable of climbing about 25-30% inclines at 190lbs.

The dual is much better.


Why don't you use 12T/36T? I use it and it works great.

As sl33py, the belts work a lot better when they are tighter and no chance of cogging even under pressure.

Although this does add to drag.

You can also go 15mm.

I'd go Dual Diagonal with 6374 w/ 15mm wide belts. 16/36T.
That setup would be perfectly fine.

I had my friend who's almost at that weight 240lbs. Climb up 15-20% inclines with dual diagonal 5055 280KV SK3 with 6S.

Put Dual 6374 on 12S 16/36T would be a beast of a board.
```

---
## \#11 Posted by: jasonyng Posted at: 2015-09-17T01:26:51.793Z Reads: 166

```
I am right at that 120kg weight, do you think the complete ready to ride enertion board would be appropriate for me or would I need something more?

Thanks
```

---
## \#12 Posted by: cmatson Posted at: 2015-09-17T01:39:03.740Z Reads: 165

```
his new board's have much bigger 63mm dual motors, running on a 10s battery. That is more than enough power for your weight- the original board he made used small 50mm motors on lower voltage, so naturally it was weaker. 

I have one of his new 63mm motors on my single drive board, and it's a beast.
```

---
## \#13 Posted by: deadlyrobot310 Posted at: 2016-03-29T05:58:57.483Z Reads: 147

```
Hello,
I stand right at around 220 lbs (about 100 kg). I am looking to build a single drive board (because I am a poor college student and don't have enough money to go dual). My current setup is using a 6354 260 kv motor with a VESC running on a 8s 10000 mAh battery. Will this give me enough power to get past my weight. Or should I go for a different motor or perhaps a 10s system?
```

---
## \#14 Posted by: NNGG Posted at: 2016-03-29T06:03:52.829Z Reads: 141

```
big SK3 6374 motor on 10-14S with a vesc, 

unfortunately they are out of stock unless you can wrangle a 6364 190kv+ on 12S max

Your setup is more than adequate on flat ground even accounting for weight is you start by kicking off. However anything larger than 10% hills will *probably* fry your shit. I havent had smaller SK3s
```

---
## \#15 Posted by: NNGG Posted at: 2016-03-29T06:07:09.219Z Reads: 137

```
You dont need to go dual even if you have the money unless you want some style and bling to the way you ride
```

---
## \#16 Posted by: deadlyrobot310 Posted at: 2016-03-29T06:36:14.665Z Reads: 133

```
Ok so it sounds like I need to rethink my battery setup... maybe go for a 10 or 12s (although I have heard that the vesc doesn't play well with 12s batteries). And I will keep on the lookout for a tougher motor. I do live in Illinois, which is pretty flat though so I may be fine with this setup.
```

---
