# Dual motor build with high KV motors

### Replies: 12 Views: 435

## \#1 Posted by: gliz5714 Posted at: 2018-05-21T13:03:45.096Z Reads: 106

```
Odd question - I am currently running a 6s1p on 295kv (Very flat where I live).  Can this be upgraded to a 6s2p with dual 295kvs?  Usually I see dual builds on 10s or higher, but curious if it is possible on a dual 295kv.  Would it be crazy?
```

---
## \#2 Posted by: Michaelj1 Posted at: 2018-05-21T13:13:41.416Z Reads: 101

```
Jeez bro you gonna be flying😂 highest I went with my 6s setup was dual 270kvs. I would assume you could go dual, but from my understanding they’d get kinda hot. I guess it would probably be better to run 2, takes the load off of using just 1 motor
```

---
## \#3 Posted by: gliz5714 Posted at: 2018-05-21T13:15:26.556Z Reads: 99

```
Ha yea, I know.. I am just looking at a less expensive way to upgrade the board!  already have over half the set up!  Figure if I need to, I can limit the motors as well.

Thanks for your response!  I am going to look a bit more into it then.
```

---
## \#4 Posted by: professor_shartsis Posted at: 2018-05-21T13:16:16.129Z Reads: 96

```
if you have a vesc you are already close to the 60,000 erpm limit w/ 6S

6S * 3.8v per cell * 295kv * 7 electrical rotations per physical revolution = 47,082 erpm max
```

---
## \#5 Posted by: gliz5714 Posted at: 2018-05-21T13:17:33.092Z Reads: 88

```
Yea, have a FocBox on the single.  I assumed that if you are rolling duals you would need to double up the VESCs so I would have an 'extra' 60,000erpm to play with no?
```

---
## \#6 Posted by: TowerCrisis Posted at: 2018-05-21T13:40:25.200Z Reads: 78

```
No, each vesc will still be limited to 60,000
```

---
## \#7 Posted by: gliz5714 Posted at: 2018-05-21T13:45:49.283Z Reads: 74

```
Correct, so dual VESC for dual 295kv would be ample no?  As the Prof said - 295kv on a 6s is only running at 75% of the suggested max so it wouldn't change right?  The only 'scary' part would be the speed?
```

---
## \#8 Posted by: professor_shartsis Posted at: 2018-05-21T13:47:18.329Z Reads: 71

```
the problem comes if you switch to 10S on certain versions of vesc... switching to 2 motors without changing to 10S should be fine.

6S * 3.8v per cell * 295kv * 7 electrical rotations per physical revolution = 47,082 erpm max

10S * 3.8v per cell * 295kv * 7 electrical rotations per physical revolution = 78,470 erpm max

^this one puts you above 60,000erpm
```

---
## \#9 Posted by: gliz5714 Posted at: 2018-05-21T13:50:49.492Z Reads: 66

```
Oh sorry for the confusion!  No, I was going to stick with a 6s build.  I was just referencing that I had only really seen dual builds that are 10s or greater and rarely see any 6s dual builds!

Current set up: 6s1p with vesc with one 295kv

Upgrade: I would look at a 6s2p set up with dual 295kv motors (with the dual VESCs).
```

---
## \#10 Posted by: TowerCrisis Posted at: 2018-05-21T13:56:05.050Z Reads: 64

```
That will be fine so long as you keep using the 60,000 erpm limit on each vesc.
```

---
## \#11 Posted by: professor_shartsis Posted at: 2018-05-21T14:06:22.315Z Reads: 56

```
here’s a prediction for (2) 295kv, 22.8v bat, 0.05ohm winding, 90mm tire, 2.62:1 gearing, 80a motor limit setting, 30a battery current limit setting

https://image.ibb.co/kBvcRT/BC16_A85_F_9_FD7_47_DA_9_ECF_80_D1_DA9_A89_FE.jpg

this arrangement gives roughly ~25mph top speed and about 67lbs peak thrust (bottom left chart). if you lower the gear ratio below 2.62:1, you have enough peak power for about 35mph (top middle chart), or if you increase the gear reduction ratio, it will lower the top speed below 25mph but you will get more peak thrust/acceleration (bottom left chart) & higher electrical to mechanical conversion efficiency (top left chart). battery current limit is set to 30a since you have a focbox.
```

---
## \#12 Posted by: gliz5714 Posted at: 2018-05-21T15:36:46.573Z Reads: 42

```
Wow thanks for that information!  Looks like it is going to have some nice acceleration - something that is definitely lacking in my current build.
```

---
