# Custom battery advice for dual setups

### Replies: 10 Views: 998

## \#1 Posted by: oneafrikan Posted at: 2016-08-20T13:24:07.718Z Reads: 111

```
Hello all,

Over the last few weeks I've been putting plans together for a build.

I've already got a Bustin EQ with the following specs:
- APS ESC 120A
- APS power switch
- 7S 6300mah Lipo
- 5065 2200w motor
- Caliber trucks
- 80mm Orangutang Kegal
- 15mm wide belt system with new UST mount
- Easy Charge BMS system

And then I have managed to acquire the following parts:
2x [Tacon Bigfoot 160 245Kv](http://www.electric-skateboard.builders/t/sold-2-new-tacon-bigfoot-245kv-motors/7378) 
2x [TB welded mounts & pulleys & trucks](http://www.electric-skateboard.builders/t/used-board-parts-for-sale-10s-dual-motor-setup-sold/7280).
Not sure if I'm gonna use the Nunchuk yet, but will trial it.
I'm on the group buy for the Winning controller.

It seems like the TB mounts (50mm) won't fit the Tacons (63mm), so that means two builds should emerge from this ;-)

I have also found a custom battery builder in the EU, which means I can go for a custom / 18650 build, just like all the cool kids, without having to learn battery welding just yet!  The reason I want to do a custom build is because one of the builds will be a 46" pintail, so means more of a Boosted type design.  For the other one, I'll compare the quotes for custom vs the enertion / TB ready-made batteries, then decide from there.  Custom also means choosing battery chemistry, so that might be a factor too!

These are my goals:
1) daily commuter with dual motors & the best torque I can get from battery / motor / gearing combination
2) a weekend pintail for carving - think here range is the most important since I want to be able to ride for as long as possible around London (flat) and not have to worry about charging...

I'm more than likely gonna go VESC.

For the commuter wheels, would ideally be 97mm flywheels or the 100mm MBS All Terrains (LHB has come back and said they are good, so why not?).  For the weekend pintail, think the 80mm Kegels are fine.


So, I guess the first part is I'm going to have to get another 50mm motor for the 2nd truck, and then I can get another Alien UST mount to match the one I already have - so that takes care of the motors & drivetrain.

But I'm unsure of the right batteries, and this is where I'd appreciate some input if possible!

The calc over here: http://calc.esk8.it/ -> doesn't handle dual setups, so not sure how you work things out from there...

I read somewhere that the Tacons should be 6s - correct, or what is the ideal setup for dual tacons?

For dual 50mm - OK to go with 2x 5065 2200w (so I just get another one to match)? 
If so, what battery setup would work best? 
Can I use the 7s I already have, but just get less range & power, or would 10s make more sense?

Lastly, I'm 110kg / 240lbs ;-)  The Bustin moves me fine, and I already go fast enough to shit myself at top speed, but for the commuter I want to be able to do more of the commute by board (which means 2 hills), and for the carver, want to go more like a snowboard...

OK - whatcha think?
```

---
## \#2 Posted by: onloop Posted at: 2016-08-20T13:46:11.610Z Reads: 95

```
Depending what 5065 motors you have dual rear drive might not be possible. Motors Too wide.

245kv motors will probably need to be paired with a battery at 6s to 8s to ensure the reduction ratio & top speed is practical. This will mean more current draw, hotter.

If you are going to build a battery I suggest higher voltage to minimise current draw. 10s is stable. 12s is pushing the limits of vesc and I don't recommend it.

If you go 10s you probably need 190kv motors. This is well suited to wheels 83-90mm.

10s4p is a huge pack, should expect around 36km range. Of course this all depends on your drive train setup. If you have minimal reduction ratio you will pull too many amps and reduce your range.

If you want to keep the total weight down go a 10s3p. Good for approx 27km range.

Use high discharge cells (8c). Samsung 25r.

Because your a bigger guy you should go with two bigger motors with maximum reduction ratio to meet your desired speed and then will have ample torque.
```

---
## \#3 Posted by: oneafrikan Posted at: 2016-08-20T14:07:35.162Z Reads: 86

```
Sorry, should have been clearer.  Want to go with Dual Diagonal (probably for both).

In one of the posts here, there was someone saying that if you want to replicate the snowboard feel (which I do), then you need to have the motors at the same place as your rear heel, and front toe.  This puts the riding center of gravity in the same place as with a snowboard (I'm not an expert - the guy writing says he's an instructor, so I'll take his word for it), which makes sense to me.

I'm goofy, so that means front left, and rear right motors.  The welded trucks & mounts were exactly that, so sounded like it was too good an opportunity pass up!  So means shouldn't be an issue with motor spacing...

Gonna read the rest of your reply @onloop and come back with kvestions...
```

---
## \#4 Posted by: oneafrikan Posted at: 2016-08-20T14:39:33.650Z Reads: 78

```
OK got to this so far, thoughts?

daily commuter:
https://www.dropbox.com/s/yz6tk85ar2p1kao/Screenshot%202016-08-20%2015.35.07.png?dl=0

weekend carver:
https://www.dropbox.com/s/9g1eql1un4d3ud2/Screenshot%202016-08-20%2015.34.20.png?dl=0

@makevoid - should you calculate anything different for a dual setup, or does dual just reduce range with everything else being equal? (sorry for newb question - sill reading up as much as I can)

thanks!
```

---
## \#5 Posted by: makevoid Posted at: 2016-08-20T14:42:29.404Z Reads: 70

```
Y, range reduced a bit, more torque/acceleration but same max speed on flat usually.
```

---
## \#6 Posted by: oneafrikan Posted at: 2016-08-20T14:43:24.554Z Reads: 67

```
cool thanks.

so how do you extend range for a 6s setup? or can't you?
```

---
## \#7 Posted by: makevoid Posted at: 2016-08-20T14:59:39.876Z Reads: 63

```
With lipos, add another battery in parallel, with li-ion add 6-12-18-24-etc... more cells to your pack (in parallel of course). All of that assuming you want to stay at 6S which with li-ion I don't think it's worth it, around 10S maybe it's better if you can.
```

---
## \#8 Posted by: oneafrikan Posted at: 2016-08-20T15:03:43.627Z Reads: 60

```
thanks man.

10s with 245 Tacons feels like suicide?
http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":10,"motor-kv":245,"system-efficiency":80,"motor-pulley-teeth":16,"wheel-pulley-teeth":36,"wheel-size":100}|
;-)
```

---
## \#9 Posted by: oneafrikan Posted at: 2016-08-20T15:04:11.072Z Reads: 55

```
Or just ditch the idea of using a dual diagonal with two Tacons and use them individually on single builds?
```

---
## \#10 Posted by: makevoid Posted at: 2016-08-20T15:05:37.139Z Reads: 53

```
Y 16/36T with 100mm wheels yes, better 6S or 8S if you can't change gearings / reduce wheel size.
```

---
