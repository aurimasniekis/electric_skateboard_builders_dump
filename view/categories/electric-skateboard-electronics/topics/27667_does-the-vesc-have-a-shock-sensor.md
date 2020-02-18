# Does the VESC have a shock sensor?

### Replies: 7 Views: 427

## \#1 Posted by: mattdig Posted at: 2017-07-15T03:43:05.134Z Reads: 113

```
If I drop off a high curb or run over a sizeable rut, the board sometimes cuts out for a few seconds. 

So, dumb question: before I go hunting for loose connections on my board, does the VESC have a sensor that detects drops and turns off automatically? Or do I just have a loose connection somewhere? My board never did this before I installed the VESC, which is why I'm curious.
```

---
## \#2 Posted by: JdogAwesome Posted at: 2017-07-15T05:10:27.735Z Reads: 103

```
It would need to have an accelerometer to be able to sense this and the VESC does not have one. Though occasionally after going over a large crack or a bump my board will cut out. Not sure why this happens but it's not the VESC purposely doing so.
```

---
## \#3 Posted by: rich Posted at: 2017-07-15T05:56:11.462Z Reads: 90

```
[quote="mattdig, post:1, topic:27667"]
If I drop off a high curb or run over a sizeable rut, the board sometimes cuts out for a few seconds. [/quote]

My vesc had exactly the same behavior, even small cracks and the vesc was down for seconds, that's very dangerous.
I put a bit of foam under the vesc (+receiver) and i've never had problems again, not the biggest bump was a problem.

Try this, in my case it was the solution.
```

---
## \#4 Posted by: mattdig Posted at: 2017-07-15T19:19:57.516Z Reads: 58

```
I do have a bit of foam, but I had to remove a bunch of it to let the MOSFETs breathe. It was overheating way too often.
```

---
## \#5 Posted by: wafflejock Posted at: 2017-07-15T19:27:03.525Z Reads: 54

```
Don't have this behavior with my VESC but it's a 4.12 one so a bit older and from DIY.  I do have an occasional drop out but I think it's settings related for me since it only seems to start happening when I'm around 37V and my battery cut offs are set pretty high for a 10S so it might just be getting voltage dips into below the low voltage cut off in my case or something else (it's pretty intermittent waiting on a metr.at telemetry module to see if it gives me any more info about what's going on when that happens).

Not much help I guess but just saying I ride over lots of beat up road and don't have drop outs from the VESC itself (when I had a crappier connection for my receiver to the VESC that was a problem, make sure your connection there is good and ideally solder it or hot glue the JST plug into the PPM port on the VESC).
```

---
## \#6 Posted by: rich Posted at: 2017-07-16T22:36:31.960Z Reads: 32

```
[quote="wafflejock, post:5, topic:27667"]
I had a crappier connection for my receiver to the VESC that was a problem
[/quote]

That makes sense to me, too.
I also had evil faults due to snapped off wire on the receiver (wire was hard bend after the JST plug). All 2-3 minutes there was suddenly FULL THROTTLE until i was braking, when i released the brake full throttle again. It only stopped when i unplugged de JST plug on the receiver. After replugging there was 2-3 minutes time to have the next full throttle experience. It took some time until i realized it's the wire. Fortunately i had no accident due to this.

This was the scariest esk8 experience which i ever had!
```

---
## \#7 Posted by: wafflejock Posted at: 2017-07-16T22:50:10.077Z Reads: 27

```
Ugh yeah have had things go full throttle when the radio on my custom made receiver disconnected from the board connecting it to the micro-controller.  The controllers and VESC should all fail-safe to IDLE throttle when anything comes disconnected but I broke the front off my first board because of something like this in my own receiver (I fixed my code but shocked how many "real" consumer controllers seem to not fail safe to idle by default).

After I had that problem I bench tested pulling all the pins one by one to see what happened and make sure if any other pin got disconnected it would still go idle.

Yesterday had a really rough crash but wasn't really control related was just cruising too fast and got some speed wobble tried slowing down a bit but sometimes braking can make it worse and ended up spilling pretty hard on my side (think I may have busted a rib but it didn't kill me or break any limbs, and don't think there's much that can be done about it except ice and taking it easy until it heals up).  Getting some bigger wheels and tightening up the trucks both might have helped but also just shouldn't have been cruising at that speed (got too confident things have been going too well, reality had to knock me back into place).
```

---
