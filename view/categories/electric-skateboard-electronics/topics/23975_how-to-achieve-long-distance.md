# How to achieve long distance?

### Replies: 10 Views: 1124

## \#1 Posted by: chewydinosaurs Posted at: 2017-05-27T02:57:54.490Z Reads: 164

```
So I'm running 2 4000mah 3s batteries in series and I get around 2ish miles before my battery checker doohickey tells me I have 35% left in the batteries (it plugs into the 6s balance cable port). I'm thinking abut going up to 4s or 5s 5000mah batteries but I want to make sure I can at least get 6 miles in distance as I need to get around campus at college. Thanks.
```

---
## \#2 Posted by: JLabs Posted at: 2017-05-27T02:59:55.716Z Reads: 164

```
You only have a total of 4000mAh because the batteries are in series. If you were to put them in parallel you would double the mAh but get half the voltage.

So if you want a lot of range, you can get 2x 5000mAh 6s batteries and but them in parallel for 10,000mAh
```

---
## \#3 Posted by: mmaner Posted at: 2017-05-27T03:13:21.511Z Reads: 157

```
With x2 5000mah 3s lipos in series (6s) I get about 7 miles. You should be getting at least 4, unless you are hitting the throttle really hard.  One of my current builds uses x2 8000mah 3s lipos (6s) and I get 11 miles out of it.
```

---
## \#4 Posted by: chewydinosaurs Posted at: 2017-05-27T04:05:52.735Z Reads: 146

```
1. How important is C rating
2. I'm trying to keep this build as thin as possible so do I go with batteries in series or in parallel
3. What's the lowest voltage a vesc powered board can run on
```

---
## \#6 Posted by: NickTheDude Posted at: 2017-05-27T04:19:54.431Z Reads: 141

```
It would be pretty dumb. There wouldn't be enough power to work and the range would not increase anyways.
```

---
## \#5 Posted by: chewydinosaurs Posted at: 2017-05-27T04:53:02.434Z Reads: 132

```
Im just experimenting with range, and am curious how much power I would get with two 3s 4000mah lipos in parallel instead of series. Im mainly trying to get range here while keeping the board as thin as possible and not spending a butt load of money on big bulky batteries.
```

---
## \#7 Posted by: hornet90 Posted at: 2017-05-27T05:37:46.456Z Reads: 117

```
If your sticking with a 6s set up get 2x3s 5000mah 60-65c if you around 85kg you will get 6-7 miles
or 3 2s 6600mah 65c all hooked up in series,
Turnigy nano-tech A-SPEC 6600mah 2S 65~130C Lipo Boat Pack
ill be testing the 2s next week i hope
I had 2 Turnigy Graphene 5000mAh 3S 65C LiPo Pack w/XT90 i love them 7 miles doing 12 to 23mph
no sag felt great im 85kg 
If you dont need to do any more than 7 miles stick with 6s its 7.5 miles to work from my house i need to go wth a 10s set up 7 out and 7 back i wish i had done a 10s or 12s set up at the start.

Thats the crack ,
```

---
## \#8 Posted by: evoheyax Posted at: 2017-05-27T18:15:51.102Z Reads: 76

```
A few things to consider about range which I have learned through mine and other people on this forums experiments.

Factors that affect range:
1) Speed (wind resistance). This is the biggest factor to consider. If you really want a long range, ride between 5-10 mph only. But those speeds suck to me, so I just go for a massive battery pack so I can have range.
2) Rider Weight
3) Rider Style (slamming the throttle like I like to do does result in a higher amp draw, just like stomping the gas pedal in a car)

in addition of course to battery size. You should also remember that Wh is the real measurement of range. Switching from parallel to series or vice versa will not have very much effect on range.
```

---
## \#9 Posted by: chewydinosaurs Posted at: 2017-05-30T05:00:24.133Z Reads: 54

```
I do have a custom motor mount which isn't the most amazing and the tension on the belt might be little to much? I don't know how much that would effect it but I do slam the throttle quite a bit. I have a 280kv motor so I can get some good speed going but torque isn't there so I'm assuming that may drain my battery as well
```

---
## \#10 Posted by: evoheyax Posted at: 2017-05-30T05:31:41.764Z Reads: 52

```
The reason torque isn't there is your running a low voltage with a high kv motor. If you drun 12s instead, you'll see a night a day difference.

The only issue you'll have if your belt is too loose or tight is belts will break fairly often, because the teeth will slip.

I personally think the zippy 8000 mAh series are the best lipos. 6x 2s, 3x 4s, or 2x 6s. I've had them all and they never fail, min of 5 miles if you ride aggressive and stop every block and are heavier (I'm 6'1", 200 lb) and have a lot of step hills and don't ride below 20 except for stop signs, and gun it after the stop sign every time.

Idk what ESCs your using though. If you have a VESC, then run 12s. You'll thank me later, trust me.
```

---
