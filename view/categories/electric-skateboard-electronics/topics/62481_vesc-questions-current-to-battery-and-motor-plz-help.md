# Vesc questions (Current to battery and motor) plz help

### Replies: 10 Views: 388

## \#1 Posted by: Travo Posted at: 2018-07-21T20:59:07.077Z Reads: 104

```
Hello everyone! I am at the final stage of my board but ran into a problem. I built a 10s2p battery out of Samsung 30q batteries. (The same one Mike beard did but with 30q instead of 25r).
I’m not sure how to calculate the max amp out and max regen for the board and was wondering if someone could help me out? Side note I have the torque boards 190kv motor and I’m pretty sure I put the numbers in right but if anyone has one or knows what they put or would put in there’s please let me know. (Please don’t rip on me I’m a noob :slight_smile: )

![MSW_10_Current%20limits_set|690x370](upload://7mYpb5FccYdwpOVUnNeD501NE2l.jpg)
```

---
## \#2 Posted by: briman05 Posted at: 2018-07-21T21:15:36.016Z Reads: 96

```
You put the amps of your motor for the positive for the battery you the 30q are 15 amp discharge so a 2p would be 30 Amps which is what you would put in the battery max if you are doing a single motor.
```

---
## \#3 Posted by: Travo Posted at: 2018-07-21T21:20:16.923Z Reads: 92

```
Okay that makes sense, for the bat regen what should I do
```

---
## \#4 Posted by: briman05 Posted at: 2018-07-21T21:21:42.877Z Reads: 90

```
Bat regen I would do around -12-15
```

---
## \#5 Posted by: Travo Posted at: 2018-07-21T22:30:39.215Z Reads: 86

```
Okay thanks so much! What should I run the motor at, it's the torque boards 190kv motor 
[Link](collections/electric-skateboard-starter-collection/products/electric-skateboard-motor-6355-190kv)
```

---
## \#6 Posted by: Hummie Posted at: 2018-07-21T23:46:06.955Z Reads: 81

```
30q are shown good to 20amp discharge so can raise the bat amps.  Motor amps u can put whatever u want and its likely limited to 100.  It's unrelated to what the battery can do.
```

---
## \#7 Posted by: skatardude10 Posted at: 2018-07-22T01:12:30.163Z Reads: 70

```
For max Regen... 30Q are rated to 4A per cell max charge. With 2P you can safely set this to 8A.

If you aren't maxing out your brakes most of the time though, it shouldn't hurt to up this to 10A somewhat conservatively or 12A somewhat aggressively if you want stronger breaks in emergency situations. I am no battery expert, the logic I run with is an echo of words heard elsewhere throughout this forum: "we only max brake for a little bit at the time... Can't be too bad can it?" ... and ... "Would you rather risk your life... Or a few charge cycles on your battery when you could have saved your life instead" ... *kinda thing*

I run 25r in 4P at 20A max Regen (dual drive 10A each) and it comes in handy compared to the otherwise 16A rated max charge (8A each). I just try to be easy on the brakes as much as possible and only use full brake for a few seconds at most when I *really need it*.
```

---
## \#8 Posted by: Travo Posted at: 2018-07-22T01:18:41.341Z Reads: 66

```
That's a good point, rather live and waste some cycles then not be able to ride the board period. Thanks for the advice
```

---
## \#9 Posted by: Hummie Posted at: 2018-07-22T07:15:50.922Z Reads: 60

```
id be nice to see a thermometer on cells.  if they arent getting hot maybe theyre fine.  when they give the charge current i wonder what that really means.  continuous i imagine.  that's a hell of a long time compared to the brake time especially with the motor negative amps in there too which i imagine helps with braking without doing the battery regen.    i bet you could crank huge amps into a cell for a very short period of time.  not that i recommend it but wonder.
http://batteryuniversity.com/learn/article/ultra_fast_chargers
wow.
```

---
## \#10 Posted by: Hummie Posted at: 2018-07-22T17:44:34.932Z Reads: 49

```
totally counter intuitive results related to high pulsed current (maybe braking current):
https://www.chemistryworld.com/news/fire-starting-battery-dendrites-go-with-the-flow/3008867.article

i havent read the full study though and think you'd have to pay to get there.  maybe other similar studies could be found or someone could easily do one.
i dont know if the sulfur chemistry used in the study is similar enough to ours to make assumptions.   
https://arstechnica.com/science/2018/03/researchers-heal-destructive-dendrite-growth-in-lithium-metal-batteries/?comments=1

got the study
file:///C:/Users/me%20john%20murphy/Downloads/Self-heatinginducedhealingoflithiumdendrites.pdf
maybe it will work for you
```

---
