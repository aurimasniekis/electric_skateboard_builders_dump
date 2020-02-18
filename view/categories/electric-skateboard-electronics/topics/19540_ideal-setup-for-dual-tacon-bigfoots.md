# Ideal setup for dual Tacon BigFoots?

### Replies: 23 Views: 1696

## \#1 Posted by: oneafrikan Posted at: 2017-03-23T08:44:31.919Z Reads: 121

```
Morning dudes and dudettes,

What would you think is the best electrics setup for a daily driver with dual Tacon BigFoot motors, which needs to do the following:
- carry me and backpack - 110kgs / 240 pounds
- minimum 8 miles, ideally minimum 15 mile range on single charge; hopefully a lot more!
- belt driven drivetrain, not hub motors
- probably dual diagonal (got to have that snowboard feel)
- 90 or 97mm wheels
- assuming vesc's will be used

My focus is stability, reliability, ease of use - not trying to shoot the lights out or do anything sexy, so want to minimise components so there are as few points of failure as possible. 

Also not trying to go tooooo fast - a steady 20mph odd is fast enough on the roads I use, so that plus some room for acceleration if needs be is fine.

Any thoughts? Suggestions? Things to avoid?

Thx!!
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2017-03-23T09:51:22.756Z Reads: 112

```
@oneafrikan looks like a pretty standard build, not sure if you are thinking dual diagonal...Run at 10s, Lipos if you wanna carry extra or get an 18650 pack of some sort, like 10s4p...run 15t/36t on 12 or 15mm belts using your 90 or 97 wheels .....if you want lights, get some shred lights.....put them on as you need them...and just get a mini remote....of course what even mounting kit you make or buy.... boom ur done lol
```

---
## \#3 Posted by: saul Posted at: 2017-03-23T10:24:02.315Z Reads: 99

```
I have single tacon on 8s and 80mm wheels. 25mph. 16 miles on 8s 10ah lipo. 

I am also about 80lb lighter, but dual 245kv you have a pretty fast setup.
I think lower kv would be good for 90/97s. i'm already running 14/16 on 80mm and
the motor lacks torque on the low end and require more amps than a smaller 190kv 6355 on the same setup.
the 0-10 is a bit slow. then 10-20 is:boom: :joy:

plus since the tacon is a 6364 you need super wide trucks or you can only go diagonal.

10s 190kv is also more common, so you can probably find more deals. 10s3p or more should give you the range you want.
```

---
## \#4 Posted by: oneafrikan Posted at: 2017-03-23T18:01:30.002Z Reads: 82

```
Yup that's pretty much it. DD for sure. 

Ok so 10s4p gonna be ok for those motors? I was reading on the forum elsewhere that 8s is better?
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2017-03-23T20:30:58.368Z Reads: 71

```
Yeah 8s will be fine.  I wouldn't over think the build.. you want it simple with the least failure points...a reliable ride
```

---
## \#6 Posted by: oneafrikan Posted at: 2017-03-23T22:20:21.525Z Reads: 66

```
Cool thx dude
```

---
## \#7 Posted by: Michaelinvegas Posted at: 2017-03-23T22:36:15.921Z Reads: 64

```
what deck are you thinking?
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2017-03-23T22:37:36.855Z Reads: 63

```
@Mark posted up this cool looking freeboard deck on chat  

https://store.freebord.com/blank-canvas-maple-deck/
```

---
## \#9 Posted by: oneafrikan Posted at: 2017-03-23T22:55:03.147Z Reads: 62

```
I've got a landyachtz bamboo which I want to do CF treatment on, ala @whitepony, and then my Kebbek Max Irwin which I push on is an awesome deck which I think would work nice too.

Gonna check out the one you linked to, thx!
```

---
## \#10 Posted by: oneafrikan Posted at: 2017-03-23T23:01:47.671Z Reads: 61

```
That does look sweet! And would be even more like a snowboard! Thanks dude!! Could do CF on that too to stiffen up...
```

---
## \#11 Posted by: Michaelinvegas Posted at: 2017-03-23T23:02:53.999Z Reads: 60

```
And let's not forget...it's cheap! Me likely cheap!
```

---
## \#12 Posted by: oneafrikan Posted at: 2017-03-23T23:05:48.417Z Reads: 60

```
Yea, good one! Crap that is cheap!

This hobby is definitely not a cheap one, like say gardening ;-)
```

---
## \#13 Posted by: Michaelinvegas Posted at: 2017-03-23T23:09:34.675Z Reads: 56

```
Hahah ... first time I've heard anyone compare this to gardening...but hey who cares? Lol

Yeah, I love finding cool decks cheap....I like finding expensive decks cheap too! Like on eBay sometimes
```

---
## \#14 Posted by: sl33py Posted at: 2017-03-23T23:56:49.232Z Reads: 56

```
[quote="oneafrikan, post:1, topic:19540"]
assuming vesc's will be used
[/quote]


Hey man - quick concern on your proposed setup.  Speed and ERPM / Dead DRV (if VESC 4.12).

97mm - 245kv - 10s - 15/40 (i'd gear down as far as possible and use the 15mm wide [kit from @Titoxd10001](http://www.electric-skateboard.builders/t/15mm-steel-motor-pulley-11-40t-abec-flywheel-mbs-all-terrain-pulley/16586)) 

Besides the ERPM being too high (about 62k), you would also have a top speed of 36mph/60kph!

I'd suggest first a lower KV motor like 190/168/149 - and definitely the 40t w/ those bigger wheels (i *love* the 97mm flywheels - super butter!!).

Alternatively you could decrease voltage to 8 or 9s - possibly with the above lower kv motor.  Personally i like lower gearing like 14/40 or 15/40 and 10s w/ lower kv motor.

VESC-X might not have the 60k ERPM limitation.  I know the VESC 6 should remove this limit - but you'll still have a speed board capable of 30+ i'd guess.

Look forward to seeing the build - GL and HTH!
```

---
## \#15 Posted by: Michaelinvegas Posted at: 2017-03-24T00:12:25.426Z Reads: 50

```
He did want 8s .... he should be be good... Right?
```

---
## \#16 Posted by: sl33py Posted at: 2017-03-24T00:46:56.842Z Reads: 46

```
Yes - about 50k ERPM and 30mph/48kph.  Still bloody fast...  

Should be less likely to kill the DRV (not guaranteed - maybe look at VESCX, Chaka's Direct FET, or VESC 6).
```

---
## \#17 Posted by: Michaelinvegas Posted at: 2017-03-24T02:19:34.722Z Reads: 43

```
Lol he has the option to go slower lol
```

---
## \#18 Posted by: oneafrikan Posted at: 2017-03-24T09:39:47.622Z Reads: 40

```
That's really helpful! I think I should be going slower... I've got a kid and a wife and a mortgage and an income to protect so can't afford to be in hospital for much at all! Damn I wish I was 25 now! 

And because I'm a big dude I'm thinking torque more important anyways.

So slower would be:
Same wheels (97)
Lower KV motors
Gearing down

Could I accomplish the speed reduction with the same Tacon motors & 10s battery just by gearing down??

I'm gonna check the esk8 calculator as well to answer my own questions - but I guess mechanically how easy is it to find 40T pulleys for Abecs? And/or how easy is it to find 8s 18650 batteries off the shelf?
```

---
## \#19 Posted by: saul Posted at: 2017-03-24T10:07:07.028Z Reads: 41

```
[quote="oneafrikan, post:18, topic:19540"]
Damn I wish I was 25 now!
[/quote]

no, you really don't! :sob:

gearing has its limits. 15/40 is a good place for 97s.

and you can limit erpm to keep the board under 25mph.
but i still say use some 200kv or lower motors. the tacon i'm using needs at least 40amp to get enough torque for hills. 
with dual this is less but you'll still need a battery that can do 60A+ cont. for bigger hills. thats like an 8s5p or 6p with hg2 or 30q cells. lots of cells...
```

---
## \#20 Posted by: oneafrikan Posted at: 2017-03-24T12:35:17.025Z Reads: 42

```
What kind of continuous Amps would a 10s4p put out?
```

---
## \#21 Posted by: treenutter Posted at: 2017-03-24T13:14:37.868Z Reads: 43

```
[quote="oneafrikan, post:20, topic:19540, full:true"]
What kind of continuous Amps would a 10s4p put out?
[/quote]

assuming it's made with Samsung 25R's, 80A continuous and bursts that are much higher.

[quote="oneafrikan, post:18, topic:19540"]
Could I accomplish the speed reduction with the same Tacon motors & 10s battery just by gearing down??
[/quote]

Yes but gearing ratio is limited by a few things' mainly the size of the wheel. You're limited to 44T on a 97mm wheel I think, although 40T is the more commonly used size. Speed reduction can always be achieved using limits in VESC.
```

---
## \#22 Posted by: sl33py Posted at: 2017-03-24T17:18:20.779Z Reads: 38

```
[quote="oneafrikan, post:18, topic:19540"]
Could I accomplish the speed reduction with the same Tacon motors & 10s battery just by gearing down??
[/quote]

As other mentioned - you can limit ERPM to 60K or less (Again - confirm you are on VESC 4.12?).  This will limit speed a bit.

You might want to go w/ high C Lipos vs 18650 cells, or you will need 4 or more in parallel to avoid major sag.  Lipos are higher discharge and if you get a 45C or 60C pack it will sag less when you have huge amp draw w/ the Tacon.  A suggestion.

Gearing will only do so much.  If you go 15mm which i suggest, i might try to find a 14t motor gear, and definitely get the "kit" from @Titoxd10001 - great price and the only 15mm wide 40t i've found.  DIYes may have one and you can always 3d print one, but it won't be as durable as the aluminum.  Realistically it looks like you can slow down about 2mph going from 15t to 14t on the motor gear everything else staying the same. Still 62k ERPM for 10s Tacon 245kv.

If you get the largest wheel gear (likely need to 3d print) like the 44t mentioned - 15/44 = 32/33mph and 14/44 = 30mph.

I'd suggest going down in motor kv to 190/168/149.  I'm a big guy too, so can sympathize...

Best of luck!
```

---
## \#23 Posted by: oneafrikan Posted at: 2017-03-25T13:17:13.942Z Reads: 30

```
Sounds like simplest approach is to just use a lower KV motor - more wheel & gearing options down the track...

So what to do with the Tacons!!??
```

---
