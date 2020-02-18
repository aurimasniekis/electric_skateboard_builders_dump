# Full brakes when board is turned on without touching throttle, now getting big sparks from my anti spark. Not sure what to do to salvage this. Help?

### Replies: 25 Views: 977

## \#1 Posted by: LaCha Posted at: 2017-03-01T21:56:03.114Z Reads: 143

```
Hi guys, need a little help here. My board automatically applies full brakes when the board is turned on, The default neutral throttle is brake. Any idea what could be going on? I have no idea if it's the remote or my settings. I'm using 10S8P Samsung 25R, dual diagonal sk3 6374 192kv, Maytech VESCs, and a mini remote and receiver. here are the settings from my VESC. 
<img src="/uploads/db1493/original/3X/7/1/713f030987f7fe1e379d25e8637b7bcad7bc3222.png" width="690" height="387"><img src="/uploads/db1493/original/3X/1/1/11ea54f233ae453a0dc7562ea985052114d3179e.png" width="690" height="387"><img src="/uploads/db1493/original/3X/f/5/f500963738da094e3199f6a68261a26959a09b3f.png" width="690" height="387"><img src="/uploads/db1493/original/3X/1/3/131d992ac6e7bb0732ec1c5e82cd5a2a0ca76745.png" width="690" height="387"><img src="/uploads/db1493/original/3X/9/7/974125c13dcd4d5bb774bf619518280fb0096de3.png" width="690" height="387">
```

---
## \#2 Posted by: Namasaki Posted at: 2017-03-01T21:59:47.753Z Reads: 117

```
in what position do you have the trim knobs on the mini remote?
If they are at 12:00, you will need to turn the one on the right clockwise until the motor starts spinning then back it off till the motor stops spinning. Usually about 2:00.
Then test the trigger for throttle letting it off slowly to neutral. If the motor doesn't stop, turn the knob back counterclockwise until the motor stops. Then test throttle and brakes .
```

---
## \#3 Posted by: LaCha Posted at: 2017-03-01T22:06:27.492Z Reads: 116

```
<img src="/uploads/db1493/original/3X/2/d/2d1030f4e908af144b4af2de623581a542acbf76.jpg" width="281" height="500">
```

---
## \#4 Posted by: jaykup Posted at: 2017-03-01T22:07:27.006Z Reads: 113

```
Run the auto detection wizard under the PPM section to setup the controller

<img src="/uploads/db1493/original/3X/5/e/5e9ab64a4f2f73667900c286a720c37d08915fd9.png" width="690" height="308">

You should have values in most of those fields (my settings are 0 because I don't have the vesc hooked up.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-03-01T22:08:00.879Z Reads: 108

```
the one on the left is for channel 1 steering wheel
the one on the right is for channel 2 trigger
Be sure your vesc is plugged into channel 2 on the receiver
```

---
## \#6 Posted by: LaCha Posted at: 2017-03-01T22:08:57.312Z Reads: 110

```
it's plugged into channel 2, would turning the knob around help? I'll give it a shot.
```

---
## \#7 Posted by: LaCha Posted at: 2017-03-01T22:10:58.199Z Reads: 111

```
i don't have the auto wizard option. =/
```

---
## \#8 Posted by: Namasaki Posted at: 2017-03-01T22:14:05.812Z Reads: 110

```
this video will tell you how to set up your controller on standard bldc tool
https://youtu.be/OtuofrQr3F8
```

---
## \#9 Posted by: LaCha Posted at: 2017-03-01T22:23:56.185Z Reads: 103

```
OMG, that solved it. I am so in love with you right now. Thank you very much good sir!
```

---
## \#10 Posted by: Namasaki Posted at: 2017-03-01T22:31:43.040Z Reads: 97

```
What fixed it, the bldc settings?
```

---
## \#11 Posted by: LaCha Posted at: 2017-03-01T22:33:59.246Z Reads: 95

```
Yeah, that video about setting up the remote. Thanks! I guess I was reading so much about vesc settings and motors and things that I somehow didn't see that you needed to program the remote as well.
```

---
## \#12 Posted by: Namasaki Posted at: 2017-03-01T22:42:51.667Z Reads: 96

```
Ya, there is kinda a lot to setting up your vesc for the first time. It's well worth it though.
No other Esc even comes close. And the mini remote which is what I use, works really well with the vesc.
One other think to check is that you have fail safe enabled on your controller.
You should be able to turn the remote off while the board is still on without the motor taking off on its own. It should just stay in neutral.
If it doesn't stay in neutral then you will need to re-bind the remote to the receiver.
The mini remote usually has a solid connection but just in case it does loose connection with the receiver, it is very important to have the fail safe activated.
It's also nice to be able to turn the remote off and on when ever without having to turn the board off.
```

---
## \#13 Posted by: LaCha Posted at: 2017-03-01T22:48:16.832Z Reads: 91

```
Ah crap. I must have missed out on doing that too. Gonna research it. Luckily I hadn't taken it out for a proper ride yet and was just playing around with it in my room. Thanks bro! You're the best!
```

---
## \#14 Posted by: LaCha Posted at: 2017-03-02T22:35:33.762Z Reads: 80

```
I rode my board for about 15km today, I felt my board getting rather sluggish along the way. Stopped riding, removed my loop key, and carried it home since I was already nearby. When I got home, wanted to power on and check my vesc settings. So plugged my loop key back in, and big spark from my anti-sparks. Immediately cut off the wires and started feeling around my other components to see if anything else was heating up. Nothing. Any thoughts guys? I tried making a second loop key and plugging it in, but same big spark, managed to salvage it because I was prepared this time, and pulled it quick enough. Then proceeded to redo all my soldering across the entire board. Still no luck. <img src="/uploads/db1493/original/3X/a/c/ace1c3548232036eb3a7b460f223a8378a009296.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/8/9/890a2ed02687115c8bf9e5bc924ed6d2f8e544cf.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/b/9/b9e6de357ba24e06b458fd7713572143599293ee.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/2/5/25c0b835c3b6ba6963438a07519a9fb2be79b76a.jpg" width="281" height="500">
```

---
## \#15 Posted by: mmaner Posted at: 2017-03-02T23:06:02.265Z Reads: 66

```
I've only bought XT-90S 's a couple of times, but they alleys had green on 1 edge.  Are you sure they are XT-90 Anti Sparks?
```

---
## \#16 Posted by: LaCha Posted at: 2017-03-02T23:13:02.774Z Reads: 65

```
Yeah definitely. They only have that green line on the female side. You can see it in some of my pics. Like the pic where I'm holding the burned out ones, you can somewhat see the side of the connector above my thumb.
```

---
## \#17 Posted by: mmaner Posted at: 2017-03-02T23:16:38.872Z Reads: 67

```
Ahhh, I can't see it in my phone.  Busted screen and out of town, so bloody fingers until Monday 😀.  I would suggest using a multimeter to make sure you don't have a shorted or crossed NEG somewhere, maybe between the battery and the Anti-Spark.
```

---
## \#18 Posted by: LaCha Posted at: 2017-03-02T23:23:04.935Z Reads: 63

```
Oh damn. I hope it's not my battery. It was the single most expensive thing in my build. everything was working fine on my test rides before I added that extra anti spark though. Shall go and look at multimeters on my next off day. Hope they're cheap. :frowning:
```

---
## \#19 Posted by: mmaner Posted at: 2017-03-02T23:54:51.541Z Reads: 60

```
You can get one at a Lowe's or home depot for 20 bucks or less, if there's one around. 

I'd start by removing the Anti-Spark.  Leave only the battery connected to the VESC, the VESC connected to the motor and receiver and see if you have any problems.  If not, then it's just a wiring issue.  That should be easy to solve if that's the case.

Be ready to pull the VESC in a hurry if it looks hinky or you see sparks.  If you do it's prolly a battery issue. 

Let me know if I can help any more.
```

---
## \#20 Posted by: LaCha Posted at: 2017-03-03T06:11:49.127Z Reads: 58

```
Are my vescs dead?<img src="/uploads/db1493/original/3X/1/9/194c95d1ca25b1f52cc6dfc10e31d8cee40131da.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/d/0/d0432a9ecb688567280dbdc65f2999da2a8bc99a.jpg" width="281" height="500">
```

---
## \#21 Posted by: LaCha Posted at: 2017-03-03T06:12:43.196Z Reads: 52

```
It sparks when it's just the vescs as well.
```

---
## \#22 Posted by: jaykup Posted at: 2017-03-03T15:38:17.066Z Reads: 49

```
Some things I would check - 

**Battery** - Is the total battery voltage measured at the main power plug within normal range?  Also check each series voltage on the BMS plug to see if they are roughly the same.

**Vesc** - Check the resistance between the positive and negative battery terminals on the VESC.  Is it shorted?  Check the DRV chip (the big long microchip closest to the motor connection).  Does it have a small hole anywhere in it?

You can power up the VESC with your charger and plug it into a PC by USB to see if it's still working while by-passing the battery altogether. Then if it connects and powers up, with no DRV error your vesc is probably fine.

**Anti-spark key** - these things have a resistor or something in them to prevent them from sparking.  They can fail and not work right or at all.  Maybe try with a regular XT90 key.  A spark is OK AFAIK, just bad for the contacts over time.

**Opinion** Those VESCs are cheap Chinese versions.  Built with lower quality components usually and are suspect.
```

---
## \#23 Posted by: boards Posted at: 2017-03-03T15:47:28.797Z Reads: 46

```
Your spark key got unplugged half way, causing all the current to go through the resistor (also causing the black marks). Since the resister got eaten up it sparks.
```

---
## \#24 Posted by: LaCha Posted at: 2017-03-03T16:24:28.671Z Reads: 43

```
Thanks for the help! I'll try it once I get back from work if I can muster the energy. It wasn't a normal spark, it was way too big for that. I actually have some nice blisters on my fingers now from the burn.
```

---
## \#25 Posted by: LaCha Posted at: 2017-03-03T16:25:43.056Z Reads: 43

```
That was the second one I tried to solder on. The one I managed to pull out because I was expecting the spark. The first one is completely fused together. Can't pull it apart, that's y I cut it off instead. no gaps as far as I can see though.
```

---
