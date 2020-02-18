# Has there been a serious attempt at a DIY Onewheel?

### Replies: 18 Views: 5575

## \#1 Posted by: Anubis Posted at: 2019-01-22T13:17:01.427Z Reads: 279

```
The only complication I can think of would be the motor controller. It would be super cheap too, those phat hubs/tires aren't actually greatly expensive, and I'd suspect you could match the OW XR+'s specs/performance with a 12S3P 30Q battery. Has someone actually tried this out? It would be awesome to see
```

---
## \#2 Posted by: ryansinatra Posted at: 2019-01-22T13:20:33.038Z Reads: 277

```
https://www.electric-skateboard.builders/t/onewheel-build-guide/80129?u=ryansinatra
```

---
## \#3 Posted by: Anubis Posted at: 2019-01-22T13:25:06.914Z Reads: 269

```
Yep, looks like the ESC is the main issue I suppose :( I'll follow this thread
```

---
## \#4 Posted by: Slak Posted at: 2019-01-22T15:17:57.409Z Reads: 253

```
I saw a video on Youtube of a guy (from Poland iirc) who did a Onewheel-like using Hoverboard parts (wheels, controllers, gyro, batteries, etc...). Should be easy to find on YT (sorry, I'm at work and can't connect to YT from here)
```

---
## \#5 Posted by: Anubis Posted at: 2019-01-22T15:28:31.508Z Reads: 240

```
Yea i saw that, but he used like a really small battery and I was hoping to find a built using a proper vesc and stuff
```

---
## \#6 Posted by: Lionpuncher Posted at: 2019-01-22T15:58:01.161Z Reads: 227

```
Onewheel’s use a 16s1p LifePo battery. Not sure their range with those.  Would be cool to see a diy Onewheel in the wild with a long range.
```

---
## \#7 Posted by: Lunasi Posted at: 2019-01-22T16:18:47.347Z Reads: 214

```
A one wheel motor controller would not be a cheap thing to make, in fact that's one of the hardest parts of recreating it, not for the normal esc use, but for the balance software. You would need a few people to redesign the ESC from bottom up, also one wheel has a lot of patents on their products and some people who have tried to do that in the past have been given cease-and-desist orders. The one other company who has made something close to a one wheel is Trotter. They've already had numerous run ins with one wheel and are still on the map only cuz they're Chinese and China doesn't give a crap about one wheels patent cries. That said I would love to see somebody make some custom ESC s for it, the original beta one wheel went up to 40 miles per hour and they only changed it because 10 of their pro riders injured themselves on it.
```

---
## \#8 Posted by: Anubis Posted at: 2019-01-22T16:30:26.055Z Reads: 196

```
I think XR+ Uses 18650 but im not 100% sure. its very hard to find a source where it shows the actual internals
```

---
## \#9 Posted by: olestra Posted at: 2019-01-22T16:46:15.584Z Reads: 203

```
one wheel pisses me off, locking that up with patents -- there was a working example of one about 4 years before they started, posted on hack-a-day. Some dude at MIT's project. flipping patent office has always interpreted prior art as already patented, which precludes the open sharing of ideas

//rant over
```

---
## \#10 Posted by: barajabali Posted at: 2019-01-22T16:55:38.414Z Reads: 196

```
The OW XR uses 15s2p VTC6 cells.

Source: I have one lol

I love the OW to be honest. Electric skateboarders usually hate on them but for me, its all about having fun and its a fun little board. Thing is.. it's pretty sketchy. So a DIY version will never be in the works from me since DIY is almost always more sketch then a refined production version.
```

---
## \#11 Posted by: Bor.inc Posted at: 2019-01-22T17:02:34.888Z Reads: 185

```
http://transistor-man.com/Index.html
this man has made a splendid looking onewheel

http://transistor-man.com/flying_nimbus.html
```

---
## \#12 Posted by: Anubis Posted at: 2019-01-22T17:21:16.212Z Reads: 175

```
I knew it was 18650 ;;;))))

Why would anyone hate on a OW? Its not even an esk8, and if you get on one offroad you realise its fun as fuck. Anyone who hates is just jealous on their shitty evolve or someshit <3
```

---
## \#13 Posted by: olestra Posted at: 2019-01-23T16:53:59.516Z Reads: 144

```
love the device, dislike the business practice of patenting ideas derived from open sharing.
```

---
## \#14 Posted by: dareno Posted at: 2019-01-23T18:49:37.947Z Reads: 128

```
[quote="barajabali, post:10, topic:81704"]
DIY is almost always more sketch then a refined production version.
[/quote]

Wait what?  :face_with_raised_eyebrow:
```

---
## \#15 Posted by: moon Posted at: 2019-01-23T18:51:09.424Z Reads: 129

```
https://media.tenor.com/images/dbed891c264c9fc5ff3eebc8cc7ac206/tenor.gif
```

---
## \#16 Posted by: BooYA Posted at: 2019-01-23T20:49:19.501Z Reads: 117

```
The esc is no problem, could use a vesc in duty cycle mode. As for the balancing, a simple FPV/racing drone flight controller would do the job! Set it up in self level mode, with a custom layout, single pwm motor output slaved to the pitch axis. Then you would need some PID tuning and an arming switch ( some kind of large flat momentary push button under the foot)
```

---
## \#17 Posted by: BooYA Posted at: 2019-01-23T20:52:21.427Z Reads: 113

```
All these functions are basic on any FPV race drone Flight controller. I think the electronic part is actually quite easily doable!
```

---
## \#18 Posted by: webst Posted at: 2019-11-28T19:01:15.310Z Reads: 26

```
Although there is difference between duty cycle and current control the real problem is lower max speed on 10-12S. 

Available chinese wheel has KV around 12 which gives at max 50,4V*12 = 604,8 RPM which gives 604,8*0,79m = 477 meters per minute * 0.06 = 28kmh (17mph). 

This is unloaded, considering resistance, motor efficiency and safety margin for breaking (controlling the motor at high downhill speeds) it's 20kmh maximum which is around 12mph and this is the main problem with lower voltage.
```

---
