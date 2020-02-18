# New builder drivetrain validation please?

### Replies: 9 Views: 860

## \#1 Posted by: Ragnar Posted at: 2016-09-04T13:55:45.484Z Reads: 111

```
Hi all,

I'm just starting my first build. So far I have a deck (Vanguard), Trucks (Caliber 2 50) & Wheels (Kegel).

I'm looking to create a dual motor setup, and now I need to start piecing together my drivetrain.

I'm thinking of this [Alien Drive Systems kit](http://alienpowersystem.com/shop/cnc-kit/alien-drive-complete-kits/alien-drive-systems-electric-longboard-diy-kit-63mm-motor/?attribute_truck-ring-adapter=caliber%2Fcaliber+II&attribute_wheel-hub-drive-adapter=Orangatang+kegel+and+similar), which should get me clamps, motor mounts, pulleys and belts. The motor pulley is a 10mm shaft size, which might not work for my motor, but I can find a replacement if needed.

I'm finding it quite hard (as I'm sure most do) to find suitable motors - Options for me right now seem to be either 2x eSk8.de's 6354, 200kV 2.1kW or 2x Enertion's 6355 R-SPEC, 190kV 2.4kW.

eSk8 has a 10mm shaft which looks like it should go well with the Alien pulley (though I'm not sure if it has a keyway, some pictures seem to show one and others don't). Enertion's is 8mm, so I'd need to get new motor pulleys, but I don't think that adds too much to the cost cost.

In terms of gearing the Alien kit comes with a 15T/32T setup. Not sure what battery I'll go for right now... with a 10S I think that would give me more than enough weighted speed at 190 or 200 kV. With an 8S I think it's should still be acceptable?

What do you more experienced guys think?
```

---
## \#2 Posted by: michaeld33 Posted at: 2016-09-04T14:45:38.657Z Reads: 98

```
That motor pulley is designed especially for a specific 10mm shaft motor with 3mm keyway. Hard to find right now. I'm getting some in stock probably in 2 weeks. ADS has some on the way too. There are many 8mm bore pulleys, though, so you should be fine no matter what motor you get. Just out of curiosity, why not the SK3?
```

---
## \#3 Posted by: Ragnar Posted at: 2016-09-04T16:45:40.070Z Reads: 82

```
Yeah, the Alien kit comes with a 10mm pulley which doesn't seem to be that common a shaft size. The eSk8 seems to match though? If I go for the R-Spec then I'll get their motor pulleys to match for a small extra cost.

Reason for not the SK3 is simply that I can't find them for love nor money anywhere :(
```

---
## \#4 Posted by: torqueboards Posted at: 2016-09-04T16:47:30.709Z Reads: 80

```
@Ragnar If you haven't checked us out yet. www.. Free shipping over $300+ for international included.
```

---
## \#5 Posted by: Ragnar Posted at: 2016-09-04T22:16:11.202Z Reads: 60

```
@torqueboards To be honest I had checked out DIY but was worried about import tax to the UK and was trying to source stuff here or at least in Europe. Been taking a second look this evening and I am tempted.
```

---
## \#6 Posted by: Ragnar Posted at: 2016-09-05T21:12:30.801Z Reads: 52

```
@torqueboards thanks for making me look again...

I'm liking the look of those V4 mounts and also the great reviews people give your motors.

So my shopping list now looks like:
* 2x 6355 190KV
* 2x Motor Keyway <- Do I need these or do they ship with the motors?
* 2x Single Bolt On Motor Mount w/Drive Wheel Kit - configured as:
  Motor Mount Size: 63mm
  Truck Type: Caliber
  Motor Mount Color: Black
  Gearing: 16T/36T 9mm Kegel

Can I ask, does that look like a good dual-motor set-up to you (thinking of running it on 4s2p or 5s2p but I haven't figured that part out fully yet)?
Clamps and motors should fit between my 184mm Caliber II 50s?
Would you recommend 12T or 14T instead of 16T on the motor pulley?
What length belts come with that kit? I'd like to pick up a couple of spares.

I'll get 2x VESC while I'm buying stuff and I'll probably add a controller and some wiring bits too

Thanks!
```

---
## \#7 Posted by: michaeld33 Posted at: 2016-09-05T22:03:12.355Z Reads: 44

```
Keyway comes with the keyway pulley, not the motor.
```

---
## \#8 Posted by: torqueboards Posted at: 2016-09-05T22:06:09.645Z Reads: 42

```
You don't need the keyway as they come with the motor. It's just additional as some people just want a keyway. We don't include a keyway with our motor pulleys just our motors.

Instead of the Kegel. I'd recommend the ABEC wheels since the pulley is 12mm.

Personally, I'd recommend just 10S. I wouldn't bother running only 4S or 5S.

You can fit a dual rear setup on 184mm Caliber Trucks but the motors have to be a 55mm length.

For 12mm, we only have 13T and 16T options.
For 9mm, we have 12T, 14T, 16T options.

Lower the teeth, the higher your gearing.

Typically, 16T/36T is ideal.

The belt size for mounting inside is 255mm. For mounting outward, it's 265mm.

As for the VESCs, you'd want the XT90 Parallel Connector, CanBus Connector, Male to Male Servo Connector.
```

---
## \#9 Posted by: Ragnar Posted at: 2016-09-05T22:16:32.996Z Reads: 42

```
Thanks man,

I already have Kegel's on the way, so I'll stick with them for now - 2x 9mm drive should be fine from what I've read here so far.

Sorry - I'm still getting used to the battery terminology - I meant 2x4S or 2x5S wired up in series to get me 8S or 10S :blush:

Yeah, figured out the 55mm requirement, so the 6355s should fit on OK I believe.

I'll go 16T/36T but might add a couple of different sizes motor pulleys so I can experiment - I'll check one of the online calculators to see what speed difference it makes. I'm going for inside mounting, so I'll pick up some extra 255mm belts.

Thanks again - Expect an order soon! :slight_smile:
```

---
