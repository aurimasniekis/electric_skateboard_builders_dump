# Impact of Switching from 270KV 5055 to 190KV 6364 Motors?

### Replies: 13 Views: 535

## \#1 Posted by: humanisticnick Posted at: 2018-10-24T14:51:07.409Z Reads: 128

```
Thinking about switching my 10s setup from dual 270KV 5055 motors to dual 6364-190kv (can't go bigger because of the layout), cost would be ~$200. My goal would be to reduce top speed and noticeably increase my hill climbing abilities on my ATS board. Given I'm on 10s and not 12s do you think this would provide a noticeable difference? Don't want to spend money for the sake of it.

Any advice would be appreciated.
```

---
## \#2 Posted by: mmaner Posted at: 2018-10-24T14:51:50.106Z Reads: 126

```
this will get you the loss of higher speed, increase of torque.  190kv is pretty sweet on 10s.
```

---
## \#3 Posted by: Sn4pz Posted at: 2018-10-24T15:17:55.605Z Reads: 118

```
its probably going to jerk you around for the first few tries. 80kv jump and such an increase in size.... :crazy_face: tons of power
```

---
## \#4 Posted by: amazingdave Posted at: 2018-10-24T15:21:04.204Z Reads: 113

```
Great for hills and putting you flat on your ass! It’ll do what you’re after.
```

---
## \#5 Posted by: Sender Posted at: 2018-10-24T15:23:04.845Z Reads: 108

```
200kv 6369s from psychotiller would be a good inbetween.  Not as much of a top end loss, still tons of torque
```

---
## \#6 Posted by: Eboostin Posted at: 2018-10-24T16:21:49.377Z Reads: 99

```
![image|260x195](upload://do7FG1foNbJNdaTBnJ4ZsmOnMoC.gif)
```

---
## \#7 Posted by: Jmding Posted at: 2018-10-24T16:49:33.849Z Reads: 86

```
No way to adjust your gear ratio?
```

---
## \#8 Posted by: humanisticnick Posted at: 2018-10-24T16:59:26.246Z Reads: 88

```
there might be, but my hope is to mount the 6364 in the same spot as the 5055 and change as little as possible. I think I already have the smallest gear on my 8mm shaft and the largest gear on my ATS wheels.
```

---
## \#9 Posted by: Darklinks Posted at: 2018-10-24T18:03:09.812Z Reads: 76

```
I am doing the same on my build just waiting on the sk3 6364... motor mount are made by @Idea ![image|690x459](upload://yZ3gjGVZQ7t9z5hEo5kZfUxZtuS.jpeg) ![image|666x500](upload://vk2zgaVGXPDnGLdWA5lUyISYu3I.jpeg) ![image|666x500](upload://xYXdfUeHLmWJWwQDiOSTNpGaeuK.jpeg)
```

---
## \#10 Posted by: Jmding Posted at: 2018-10-24T18:36:37.853Z Reads: 70

```
Oh, I see... You're using DIYEBoard trucks, where its kind of tricky to adjust gearing...

Looking at your setup, the biggest limiter to torque is actually your ESC, which is limited to roughly 24A combined  (12A each motor).

If you want to stick to those ESCs, you might as well use Racerstar 5045 or 5065, 200 Kv motors.  Those are more likely to fit your motor mount, are smaller, lighter, and cheaper as well.  Torque = current / Kv, so the smaller 200 Kv motors will give you just as much torque as the 6364's, up until you put too much current through them and cause them to overheat.  But the 50xx 200 Kv motors should be good up to about 30A each (that's what Boosted puts through them), which is well over what your ESC is capable of pushing out.
```

---
## \#11 Posted by: dareno Posted at: 2018-10-24T22:38:53.658Z Reads: 62

```
Yeah @Jmding is on the money there.  Without changing the esc theres no point in running 63mm motors  if you can even get them on the mounts. (they are 50mm pattern I believe)  You need to be able to pull more current from the battery to get a significant torque increase so new vesc would be the best bet and some 200 kv 50mm motors.  Best scenario if you have a limited budget.
```

---
## \#12 Posted by: humanisticnick Posted at: 2018-10-25T04:07:37.542Z Reads: 50

```
I bought a dual flipsky 4.20 and remote recently that I was planning on subbing in when I did the motor swap. Are you saying that hypothetically even if I kept the exact same motors I have now i would see a power increase just by switching to the dual vecs? Do you think the dual 4.2 could put out enough power for 6364s?
```

---
## \#13 Posted by: Jmding Posted at: 2018-10-25T05:29:12.641Z Reads: 42

```
Your motors are probably good to about 40 amps each, and are being driven at 12 amps each. So when you swap your esc and configure to higher motor amps, you can expect a roughly 3x increase in torque (at least at lower speeds, at high speeds it may be limited by your battery limits).

That esc is suspected to have issues above 30-40 amps anyway (I don't know the exact figure, you'll have to ask the dual FSESC 4.20 guys) so there's really no point in going to 63xx without upgrading escs again.
```

---
