# Too many amps using my 6S with a VESC? Or do I have the wrong settings?

### Replies: 16 Views: 1252

## \#1 Posted by: UniqueSnowflakeN27 Posted at: 2017-03-14T15:32:11.185Z Reads: 124

```
Today was the first time I rode my board with a VESC and my homemade Samsung 25R 6S4P battery. 

Last summer I used a 120A hobbyking ESC with 4x 3S 5000mah 25c lipos (6S2P) which worked great. I could climb any hill basically and I never ran into any problems. 

But after riding today I could barely climb any hills, nor accelerate very fast. If I did the VESC would just shut down for a few seconds and then be good to go again. I didn't even need to reconnect the remote.

I believe that the VESC in combination with the 6S battery requires more amps than the VESC can handle. It's the same Motor - SK3 6364 245KV with a 16teeth and 36teeth pulley system. 83mm wheels.

I'm thinking, maybe I get away with just changing the gearing to give more torque and lower top speed. Or should I just bite the bullet and upgrade to something like 8S/10S? 

If anyone can spot an error in my BLDC TOOL settings that'd be great though. 

<img src="/uploads/db1493/original/3X/8/f/8f5a381adb46a5b9d8a930d5f4f88b8c11b67720.png" width="690" height="388">

<img src="/uploads/db1493/original/3X/6/b/6b2a28a658ec81d8a5af7c285d28df760f3f0830.png" width="690" height="388">


<img src="/uploads/db1493/original/3X/5/f/5fa2370ce118fcb90a4095ed6389a91cc7f4d4ae.png" width="690" height="388">

<img src="/uploads/db1493/original/3X/c/8/c8f8241646f78c4e5279342787371f0279a002bc.png" width="690" height="388">
```

---
## \#2 Posted by: Maxid Posted at: 2017-03-14T15:42:41.543Z Reads: 103

```
Probably voltage sag - the 25Rs are known to sag quite a lot. 20V as cutoff values is too high.
You should go to 3V per cell for start and 2.8V for end values.
```

---
## \#3 Posted by: Blasto Posted at: 2017-03-14T15:44:56.470Z Reads: 102

```
leave your minimum input voltage at 8V and your maximum input voltage at 57V
```

---
## \#4 Posted by: UniqueSnowflakeN27 Posted at: 2017-03-14T15:50:50.992Z Reads: 101

```
Just changed it to what you guys said - giving it a try! Will report as soon as I get back. 

@Maxid Isn't 2.8V way to low though? I though 18650s didn't like going below 3.3V. I also thought that havin 4P would prevent voltage sag?
```

---
## \#5 Posted by: Maxid Posted at: 2017-03-14T15:52:01.117Z Reads: 104

```
the 25r are rated for 2.5V - 2.8V will give you some healthy margin. Also this is for cutoff end - which you should only rarely reach.
3.3V is for Lipos - they have a totally different discharge characteristic than 18650 cells.

[quote="UniqueSnowflakeN27, post:4, topic:19060, full:true"]
I also thought that havin 4P would prevent voltage sag?
[/quote]

it does - but if you are going to drain the battery at 60A then you will still get the sag in one cell as if you drain 15A in a 1P.
```

---
## \#6 Posted by: UniqueSnowflakeN27 Posted at: 2017-03-14T16:38:32.499Z Reads: 94

```
Just came back. 

Sadly it didn't make much of a difference, though I did notice a small improvement. But it is not really as it is at the moment. It's far too weak. 

Makes sense @Maxid ! Thanks for trying anyways :slight_smile: I think I'll wait and see if someone else knows what might be wrong, if not I will probably just rebuild the pack to a 8S3P.
```

---
## \#7 Posted by: Maxid Posted at: 2017-03-14T16:57:12.818Z Reads: 88

```
why did you choose the "slow absolute max"?
Your battery can also be used with an 80A battery current.
```

---
## \#8 Posted by: UniqueSnowflakeN27 Posted at: 2017-03-14T16:58:00.475Z Reads: 83

```
I thought the VESC was maxed at 60amps anyways?
```

---
## \#9 Posted by: Maxid Posted at: 2017-03-14T16:58:43.362Z Reads: 81

```
For continuous use yes - but you are not going to use that. For short periods uphill it could help though. The temperature cut-offs will make sure you don't use too much.
```

---
## \#10 Posted by: UniqueSnowflakeN27 Posted at: 2017-03-14T16:59:39.741Z Reads: 79

```
Huh. Would you suggest setting the "Absolute max" to 80amps and uncheck "slow absolute max"?
```

---
## \#11 Posted by: Maxid Posted at: 2017-03-14T17:00:13.002Z Reads: 80

```
I think I have like 130A in there. Just use the default value.
```

---
## \#12 Posted by: UniqueSnowflakeN27 Posted at: 2017-03-14T17:00:49.850Z Reads: 80

```
I'll try it! Be right back
```

---
## \#13 Posted by: Maxid Posted at: 2017-03-14T17:04:13.093Z Reads: 80

```
That's what Vedder says:
“Absolute max” is checked in every PWM switching cycle and used in case the soft back-off strategy for the other limits doesn’t work. I usually set it way higher than the other limits because soft back-off is preferred rather than switching off the motor with a fault code, but it should never be higher than 150A.
The “Slow absolute max” box will make sure that a filtered version of the maximum current limit is used. This is useful if there is much noise and that fault code kicks in all the time. I usually have it ticked.

So i guess it will not make a difference in your case
```

---
## \#14 Posted by: UniqueSnowflakeN27 Posted at: 2017-03-14T17:13:55.111Z Reads: 83

```
WORKED GREAT, THANK YOU!!!

Shit did wonders. Works great now, had one small hiccup where it glitched a little but that seemed to work itself out. 

I still need to adjust my acceleration but that will take some tweaking. 

Thank you again!

PS: I also adjusted my "Bat max" to 80amps.
```

---
## \#15 Posted by: Maxid Posted at: 2017-03-14T17:24:12.560Z Reads: 80

```
for the acceleration I can only recommend @Ackmaniac's firmware with throttle curves!
```

---
## \#17 Posted by: Hummie Posted at: 2017-03-15T06:31:41.141Z Reads: 55

```
you don't need firmware to get consistent power output you just need the right ratio of batt to motor amp settings.   batt amps allowing more power at high speed and motor at slow speed.   Motor amps aren't true amps but just the amperage that would be on for a fraction of a second and when put in the full context of the second it's much lower..depending on the duty cycle.  so setting to 150 motor amps you still won't go above 80 real amps if you set the bat amps to 80 and you can have extreme acceleration if you want it.  INfact it's the only way you can get to 80 amps on the lower duty cycle lower speeds....doing much higher motor amps
```

---
