# VESC Configuration 12s problem

### Replies: 9 Views: 1535

## \#1 Posted by: OleksiiF Posted at: 2017-02-11T16:11:51.434Z Reads: 131

```
I bought a VESC 4.12 and faced a problem with running it on 12s batteries

my set up is:

190kv sk3 motor;
4 * 3s 5.8a batteries in series
bt2b
vesc

i made an configuration for my remote, but when im starting my board with 12s batteries, and slightly touch the trigger (10%) motor becomes insane and goes to 100% of max rotational speed on about 3 seconds. the rest 11-100% of trigger are doing nothing. No change of rotation speed. BUT! If i use 9s, 6s, 3s batteries, motor controls by the trigger very accurately -  i give 10% throttle - motor spins at 10% of max speed and so on i give 50% throttle, motor gives 50% power

Here is my motor config
<img src="/uploads/db1493/original/3X/4/3/438347aa244893985eff3dc282f88e2cb281fd47.JPG" width="690" height="328">

Here is my ppm config for gt2b
<img src="/uploads/db1493/original/3X/a/6/a6a5a7603770f38cc819734e412a264752325b49.JPG" width="690" height="332">


Interesting part with ppm config that, 
max pulsw. shows with 100% trigger: 1.85 pulsw.
0% trigger: 1.37 pulsw.
min. pulsw. shows with -100% trigger: 0.49 pulsw.
Deadband: 0.15
But if i use this values, than with 0% trigger (doing nothing) it shows 63% on display scale. and board going somewhere  even if i turn off remote

So, to make display scale show around 50%, i used this walues:
max pulsw.  1.93 pulsw. now with 100% trigger scale shows 93%
0% trigger: 1.38 pulsw.
min. pulsw. : 0.78 pulsw.
Deadband: 0.15

Now, if not touch trigger, motor is not rotating, BUT! if turn remote off(scale moves from 52% to 62%), motor still starts to rotate,
so i changed Deadband: 0.25
and it solved the problem.

But how can i change configuration to use 12s batteries with full control motor rotational speed by my remote? am i missing something?
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-02-11T16:22:31.259Z Reads: 111

```
You need to get your settings for the PPM right. Have a look here.

http://www.electric-skateboard.builders/t/vesc-faq-setting-up-receiver-and-brakes/244
```

---
## \#3 Posted by: OleksiiF Posted at: 2017-02-11T16:28:23.160Z Reads: 110

```
I already watched this video, i did everything according to what Marcin sad in this video, but i still have my problem unsolved
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-02-11T16:30:59.673Z Reads: 106

```
I recommend you to use my firmeware mod. There you can adjust min, center and max pulsewidth. And you can use a setup wizard that makes is easy to get the settings right. And in current control it is normal that when you give only 10 % throttle that the wheels will spin up fast. When you stand on the board it is a completely different story. But in the bench you need only very very little power to spin the wheels fast.
```

---
## \#5 Posted by: OleksiiF Posted at: 2017-02-11T16:32:52.416Z Reads: 104

```
Can you give me a link?
```

---
## \#6 Posted by: Tonto2k Posted at: 2017-02-12T05:56:56.175Z Reads: 95

```
Search @Ackmaniac extended watt mode. I run 12s & 6374 and think It's awesome !
```

---
## \#7 Posted by: OleksiiF Posted at: 2017-02-12T14:40:14.309Z Reads: 86

```
I did use your firmware today (thanks a lot, its really good ill definitely will use it), but
i still have same problem: 

motor is not controlled be remote properly: i give 20% throttle, and motror in couple of seconds starts to spin at 100%
here is my configuration:<img src="/uploads/db1493/original/3X/0/6/0674fabf9f16b8da2b241375d5f6d2e17336e603.JPG" width="690" height="303"><img src="/uploads/db1493/original/3X/6/1/61efea0ab3152009ad925eac368f20bb0aae3179.JPG" width="690" height="417"><img src="/uploads/db1493/original/3X/9/7/973f96436c12a1a78211723c63fa41ff1bc581d4.JPG" width="671" height="499">

am i missing something?
```

---
## \#8 Posted by: Ackmaniac Posted at: 2017-02-12T16:01:03.870Z Reads: 72

```
That's absolutely normal. On the bench only a little bbit of power is needed to spin the wheels at full speed. Try it when you ride it. then it works. You don't control the speed of the wheels with the remote, you control the power output.

What you mean is duty cycle or PID control. But don't even try it. The board isn't usable with these control modes.
```

---
## \#9 Posted by: Titoxd10001 Posted at: 2017-02-12T19:15:24.401Z Reads: 63

```
If you did a mod to the gt2b controller like badwolf/madmunkey you need to limit up travel on the the trigger to set up failsafe properly. The pulsewidth need to be close to 1 and 2 to be able to set failsafe at exactly 50%
```

---
