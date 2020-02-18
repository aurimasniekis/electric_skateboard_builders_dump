# Basic specialised board

### Replies: 8 Views: 725

## \#1 Posted by: MAK Posted at: 2017-03-09T23:42:54.760Z Reads: 123

```
Hello,
I'm looking at building a board that I can use for commuting more than ludicrous speed (hence specialised). Although this is also my first build (hence basic).
So I'm wanting to build a board that can get me from A to B in reasonable time and be able to go up some reasonable hills. I'm not really looking to make something that can fling me forward at 40+ mph up vertical walls, more something that travels at say 15mph (maybe 20mph at most) and has reasonable torque to be able to push me up some hills.
I'm aware that smaller wheels, and therefore smaller wheel pulleys, will give me more torque but at the same time I also understand that having larger wheels will make bumpier terrain a bit more comfortable/ smooth.

So basically I'm asking, in order to build a board that can get me from one place to another, up some hills, across mildly bumpy terrain:
 - What size wheel should be used?
 - What motor rating to use?
 - What sort of power should I be supplying? Does a higher voltage mean higher speed or higher torque?
 
Any other advice would be greatly appreciated.
Thank you all for your time,
MAK
```

---
## \#2 Posted by: sl33py Posted at: 2017-03-10T00:05:23.734Z Reads: 118

```
Welcome MAK!

Sounds pretty reasonable - especially your target speeds of 15-20mph.

How heavy are you?

Where do you want to ride - what kind of hills are we talking about - 10%, 20%, more?

I typically gear for about 25 as max and like big wheels...  It really is all in the gearing...  

Without knowing your weight we might steer you a bit wrong, but here's my stab at your questions (i'm a big heavy guy btw).

83mm is a great start - clones for saving $, or get the softest legit Flywheels you can for more cush.  I personally like going up to 97's if the board shape will clear them (don't like risers if can avoid).

Motor and speed - linked to voltage or # Series battery you are aiming for (and what ESC you want to use).  I like VESC and 8-10s.

190kv and 10s is a sweet setup.  Newer VESC 6 is coming and might remove the 60k ERPM limit and let you run 12s with >200kv motors, but generally with 4.12 and similar (not sure about VESCX or DIYes VESC1 (or whatever @Torqueboards calls it)), will max at 10s w/ 190kv motors - pushing 200kv @10s is the limit.

Higher voltage *does* mean more speed - more voltage = more RPM's and i like to gear down to 14/40 or similar (don't go below 13t on motor gear to avoid skipping), and 36t or 40t also help keep speeds down.

For batteries - shoot for lipos that give 100A power handling capacity (5000mAh 20c minimum - c x Ah = Amps capacity to supply).

Hope that helps and makes sense.  give us some more detail and we'll get you dialed in.

GL!
```

---
## \#3 Posted by: Namasaki Posted at: 2017-03-10T00:12:58.435Z Reads: 99

```
15-20 mph is lots of fun and comfortable.
```

---
## \#4 Posted by: MAK Posted at: 2017-03-10T15:10:33.871Z Reads: 94

```
Thanks for the reply.
I weigh about 70kg, maybe 75 with a backpack.
From what Google maps and a little bit of research was able to tell me the most incline I tend to see on my route is about 10% but it definitely feels more so let's say 20%.
I'll be making the deck myself so I can alter it to suit whatever wheel size I end up choosing. 
My knowledge of ESCs is pretty minimal so I'll be getting a couple of friends studying electrical engineering/ mechatronics to help me out there. Do you recommend the VESC?
Thanks,
MAK
```

---
## \#5 Posted by: sl33py Posted at: 2017-03-13T21:01:41.328Z Reads: 67

```
I *strongly* recommend the VESC (or the new VESCX, or Chaka's Direct FET 4.12 variant).  The newer VESC 6 (vs 4.12) is very close to release - do a search and start reading to see if you want to wait or get 4.12 or VESCX variants.

I have VESC's from 2+ years ago now (v4.6/4.7 iirc) still working fine.

As a general rule (thanks to @chaka for finding and educating us on this limitation) - you don't want to exceed 60,000 ERPM's.  In practice, you should avoid more than 10s on 190kv/200kv and if you want to go to 12s you want 170 or 149kv or lower (like some hub motors).

While 75kg/165lbs is relatively light, your expectations for climbing hills may need to be adjusted.  I think 10-15% should be doable, but if you really want to do 20% and not get a good run at it...  You might eventually need to go to dual motors if you want to accelerate from a stop up a hill without a run at it, or want to go faster up the hill...
```

---
## \#6 Posted by: saul Posted at: 2017-03-14T06:12:41.370Z Reads: 53

```
whats your budget? that looks like the only limiting factor here...
```

---
## \#7 Posted by: sl33py Posted at: 2017-03-14T17:05:24.870Z Reads: 48

```
Also - if you are going with a single motor only to start - I'd suggest the bigger 6374 motor and 15mm belt.  The bigger motor for a bit extra power, and the wider belt gives you more contact area on the belt to avoid skipping when accelerating or braking.  You can run the belt a smidge looser too and it should be more forgiving to adjust.  if you can't find 15mm setup - go 12mm at the skinniest.  The 9mm belts will almost always skip especially when braking.

If you gear down (running higher voltages like 8-10-12s), I'd suggest the 40t 15mm setup from @Titoxd10001.  I got a set from him and they are really nice.  No cutting of your hanger like the injection molded 12mm setup from Enertion.  These are classic and durable aluminum w/ steel motor gears.  A nice option if you want to keep speeds down on bigger wheels and higher voltages.  

If you go bigger motors and wider belts - if you later decide you want more hill climbing power and need a second motor - you'll have to go dual diagonal.  Just FYI.  Lots of folks like that setup.  

I also saw an email from @Trampa today that the VESC 6 beta from Trampa and Ben is open and you can pay.  Not cheap, but the extra $ is going to Ben and helping fund his innovation (an important thing to support IMO).  These are early beta ESC's, but Ben has a great track record and two of the four 4.6/4.7 VESC's i bought from him directly a few years ago are still going strong (2 were on board that was stolen and likely still working well for some asshat). :rage:

Anyway - like @Saul said - what's your budget?  We can definitely help you spend your hard earned pesos...

HTH - GL!
```

---
## \#8 Posted by: trampa Posted at: 2017-03-14T18:33:55.123Z Reads: 32

```
A small number of VESC 6 Beta is still available. If you like to have one, drop me a note via PM.

Frank
```

---
