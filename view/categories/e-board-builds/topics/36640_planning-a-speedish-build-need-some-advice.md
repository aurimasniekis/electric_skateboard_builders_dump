# Planning a speedish build, need some advice

### Replies: 11 Views: 575

## \#1 Posted by: 12meterkuk Posted at: 2017-10-27T16:05:11.252Z Reads: 123

```
Hey everyone, I am thinking of making a fairly quick board, using a downhill deck.

So far in my esk8 adventure I have built a 10s4p 18650 battery, rebuilt a friend's board, and assembled a chinese kit.

I think its time for me to move up to the next level

Would like to have some feedback on the parts i will be using.

Torqueboards 12s4p battery with enclosure 

Torqueboards single motor mount

Caliber 2 trucks

Torqueboards 6374 190 kv

90mm abecs

16/36 gearing

Single vesc

Estimated with a calculator that it should be able to go over 50kmph (pretty fast for me)

My concern is with the battery pack and the erpm limit

I contacted torqueboards live chat and asked for dimensions or some pictures of the enclosure or battery and they didn't have it. So I am working of an estimated 20 inch length enclosure which means i need a 25 inch + wheelbase. If anyone has a bought this battery from them and have pictures or measurements of it it would be greatly appreciated

And with this 12s setup, I will be nearing the erpm limit at 57000+ Should i limit this?

Thanks in advance.
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2017-10-27T19:02:48.731Z Reads: 96

```
If your running 12s and a 190kv you should be fine your close to the rpm limit but you will never exceed it, maybe if you go super fast. For torque boards enclosure picture I have the old one(not sure if they updated it don't think they have changed it just yet they are tho) that they provide when you buy a 12s4p<img src="/uploads/db1493/original/3X/1/b/1b083ecbc8d9da9928fe11c4b4b39908031ee892.jpg" width="690" height="381">
```

---
## \#3 Posted by: 12meterkuk Posted at: 2017-10-27T23:38:52.635Z Reads: 75

```
You're da man!
```

---
## \#4 Posted by: pat.speed Posted at: 2017-10-27T23:48:07.030Z Reads: 72

```
Actually he will exceed it. I'm guessing you were working off the nominal voltage but when his battery is fully charged the max erpm is around 67,000. This will possibly fry your Vesc. I would recommend a 10s battery instead and at full charge it will be around 55,000 erpm so you will have some extra room. Also there is no point getting the 12s over the 10s because the extra speed you would get will be limited by the Vesc so the erpm doesn't go over 60,000. Although 12s will get you a bit more range and less sag
```

---
## \#5 Posted by: 12meterkuk Posted at: 2017-10-27T23:54:59.320Z Reads: 69

```
[quote="pat.speed, post:4, topic:36640"]
Also there is no point getting the 12s over the 10s because the extra speed you would get will be limited by the Vesc so the erpm doesn't go over 60,000
[/quote]

I'm getting the 12s pack as its double layered so I can fit it in a 26 inch wheelbase deck. with 10s i think the pack alone is 20 inches as it's a single layer. If i limit the erpm will the board brake or jerk when i reach 60k erpm?
```

---
## \#6 Posted by: pat.speed Posted at: 2017-10-28T06:07:36.030Z Reads: 54

```
Oh ok. I don't have experience with this but from my understanding there is a box that you tick to stop it from braking. It is called something like apply negative torque? I've heard @Namasaki say it before so maybe he could help
```

---
## \#7 Posted by: Jinra Posted at: 2017-10-28T06:31:40.524Z Reads: 51

```
He won't exceed it. Voltage sag, inefficiencies, and other factors will prevent the motor from approaching, let alone exceeding 60k

[quote="pat.speed, post:6, topic:36640"]
It is called something like apply negative torque? I've heard @Namasaki say it before so maybe he could help
[/quote]

Turning this on is how you street your face, since it'll apply sudden braking force at max speed.
```

---
## \#8 Posted by: pat.speed Posted at: 2017-10-28T06:35:27.200Z Reads: 44

```
What about if you goes down a hill? I meant untick that box so that doesn't happen
```

---
## \#9 Posted by: 12meterkuk Posted at: 2017-10-28T06:41:03.268Z Reads: 45

```
don't worry, no hills where i live. Thats why i went with single drive. And cost savings too :joy:
```

---
## \#10 Posted by: Jinra Posted at: 2017-10-28T06:44:52.735Z Reads: 49

```
Gotcha, yea you want that off in pretty much all situations. People tend to not accelerate downhill, and it's a bad idea in general. I go 35mph comfortably nearly anywhere, but I'm scared going even past 20mph downhill. Going full speed down a hill is just asking for injury, unless of course your an experienced downhill boarder.
```

---
## \#11 Posted by: Namasaki Posted at: 2017-10-28T18:03:34.287Z Reads: 33

```
The "limit erpm with negative torque" box is usually checked by default. 
And as @Jinra stated, if you somehow did manage to exceed 60k, the Brakes would come on.
I always recommend turning that function off.
```

---
