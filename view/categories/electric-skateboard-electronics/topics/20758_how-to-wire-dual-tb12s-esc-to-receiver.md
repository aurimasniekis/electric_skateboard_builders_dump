# How to wire dual TB12s esc to receiver

### Replies: 12 Views: 1288

## \#1 Posted by: cj1556 Posted at: 2017-04-10T22:52:41.889Z Reads: 114

```
I'm having trouble figuring out how to wire  my two TB 12s esc's to my gt2b receiver. can someone tell me or show me how they wire two esc's to one receiver
```

---
## \#2 Posted by: Namasaki Posted at: 2017-04-10T23:22:48.285Z Reads: 110

```
You need a signal Y harness . 
You connect both Esc's to the dual input of the harness  and the single output of the the harness  to your reciever. 
If the Esc's have 5v output to power the receiver, you'll need to cut the red wire on one of the connectors to the Esc's. So that only one of them supplies voltage to the reciever.

http://m.ebay.com/itm/381084976067?_mwBanner=1
```

---
## \#3 Posted by: t0m_r1dd1e Posted at: 2017-04-10T23:26:15.454Z Reads: 107

```
So first you have a servo connector that goes from the throttle channel of the receiver (channel 2 IIRC) to the first VESC. Then you have a CAN BUS cable going from that VESC to the other one. Then you have to configure it in BLDC. Plug in the first VESC first and check the box for "Enable multiple esc over CAN" under App Settings/PPM. Then you have to hook the second VESC up to BLDC and give it an ID of something higher than 0 under App Settings/General and then it should be good to go. Assuming you've already done motor detection/config on both VESCs, that should be it. 


Or you can get a servo cable splitter and just plug one end into each VESC.
```

---
## \#4 Posted by: Namasaki Posted at: 2017-04-10T23:28:28.910Z Reads: 91

```
He's not using Vescs
```

---
## \#5 Posted by: i2oadsweepei2 Posted at: 2017-04-10T23:32:18.217Z Reads: 87

```
X2 for the servo y-harness that namasaki linked. I have four of TB12s esc's and that's what I use too. They aren't perfectly synced when on the bench, but it's not noticeable to me while riding. Just confirm the polarities before turning the power on.
```

---
## \#6 Posted by: cj1556 Posted at: 2017-04-11T00:22:14.504Z Reads: 82

```
Thanks for the info guys! I currently have it wired like this picture, and it's working!

<img src="/uploads/db1493/original/3X/e/f/ef3213bcb1fae46dd6722ac159bc8d63b276e4e4.JPG" width="316" height="500">

My problem now is that yes, both motors run at the same time like I want,  but....

A: one throttles up slowly while the other one goes to max rpm instantly 

B: with my wiiceiver remote, if I hold the motors at full throttle for a few seconds they slow down to zero, and when I press on the throttle again they work fine. It's almost as if I'm tripping some sort of voltage limit

C: Upon seeing problem B, I figured I'd try my gt2b remote and receiver. With that one, it works totally fine but if I push the brake too hard on the controller, one of my escs/motors William completely shut off.  (The same one that throttled too slowly) 

I have an esc programming card on order. Do you guys think that these problems can be fixed with just that? or do I have a bum esc? Any more help would be greatly appreciated!
```

---
## \#7 Posted by: i2oadsweepei2 Posted at: 2017-04-11T00:38:02.015Z Reads: 74

```
Just to confiirn Is the receiver only being powered from one esc or bec? It's hard to answer without more info. Did you try each esc and motor one at a time? See if the problems happens separately too.
```

---
## \#8 Posted by: cj1556 Posted at: 2017-04-11T00:44:55.557Z Reads: 73

```
Yes the receiver is only powered by one esc, I've tried the possibly faulty esc alone and problem C still happens. Also again one of the escs has no problem while the other is problematic
```

---
## \#9 Posted by: i2oadsweepei2 Posted at: 2017-04-11T00:50:31.836Z Reads: 70

```
Yup sounds like there could be a problem. Maybe @torqueboards has seen this problem or knows why it happens. You can catch him on live chat on his website too sometimes.
```

---
## \#10 Posted by: cj1556 Posted at: 2017-04-11T00:53:58.990Z Reads: 67

```
Okay thanks!
```

---
## \#11 Posted by: Namasaki Posted at: 2017-04-11T02:26:57.242Z Reads: 62

```
Do you have the program box ?
You need to make sure both Esc's have same firm ware and settings.
```

---
## \#12 Posted by: cj1556 Posted at: 2017-04-11T12:02:43.000Z Reads: 57

```
Not yet, but I will sometime this week
```

---
