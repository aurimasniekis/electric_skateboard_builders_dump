# First E-Board Build Questions

### Replies: 19 Views: 3236

## \#1 Posted by: hanthony96 Posted at: 2015-12-09T00:05:16.738Z Reads: 146

```
Hey guys,

So im looking into starting my first build and i have read a lot of stuff online but was wondering what everyone thinks will be best for my build.

So my budget is set at under $700 hopefully. And im thinking im going to need a dual diagonal motor setup because my city has lots and lots of big hills, but i do only weigh 145 ibs.

I already have a sector 9 cruiser longboard which i hope wont be a problem using due to its smaller width.
Im thinking this is what i might need but not sure?

2-Tacon 245KV motors
2- ESC/Vesc (could you use 1 for both motors?)
-a set of paris 180mm trucks
2-zippy 5000mah 20C lipos
-not sure the best way to go with the mounts

how reliable can the cheaper chinese made parts be? What are the best "bang for your buck" parts/batteries/etc.?

Thanks and hoping to learn a lot from this community.
-Hudson
```

---
## \#2 Posted by: sl33py Posted at: 2015-12-09T00:31:43.613Z Reads: 144

```
Hey Hudson!  Welcome to the madness.  Looks like a good start for your build.  

I'm not familiar with the S9 Cruiser so not sure how much room you will have.

You need one ESC per motor.  VESC or otherwise.  I'd definitely recommend the VESC over a RC Car ESC, but there are some decent ones (XERUN, FVT, etc.).  For the flexibility and voltage range (up to 12s) i still would recommend the VESC as the best option.  You will have some steps to configure, but if you are able to follow instructions, and copy and paste, it shouldn't be a problem.

Trucks are personal preference, but the keyed hanger (not round can't rotate) on the Caliber trucks i think helps lock in the mount.  I've used Paris w/ some ADS mounts, but most seem to be setup for Caliber trucks (Enertion, DIYes (also has paris mount), and ADS (also has paris mounts)).  

Batteries - which 5000mAh Zippy's?  3s, 4s, 5s, 6s?  I like two slimmer 3/4s batteries in series for 6/8s to the ESC's.  Again personal preference.

Some chinese parts are great quality, others junk.  I'd stick to the well known and recommended components, or the cheap ones you don't mind swapping if/when they die.  Like lipo alarms...

HTH - GL!
```

---
## \#3 Posted by: Sharkface Posted at: 2015-12-09T01:23:57.770Z Reads: 131

```
The only thing left out here was that at 12s that 245kv motor would fry the VESV (90% sure on that so feel free to correct me.

A combination of turnigy sk3 6374 190kv motor with a 12 tooth pulley on it, and 83mm abec 11 flywheels with a 36 tooth pulley on it powered by a vesc at 12s will put you rreeaalllyyy close to a 20mph top speed and have more torque than you can shake a stick at. My 149kv sk3 motor with 12s tackles every hill except one that i have tried so far here in san francisco bay area, and thats with just a single motor setup... bbbuuuutttt i have def not tried going up a 25% or more incline at this time.
```

---
## \#4 Posted by: cmatson Posted at: 2015-12-09T03:42:14.468Z Reads: 119

```
if you wanted to keep costs down (and especially with your weight) I think a single motor 6374 setup would be totally doable. Like @Sharkface said, 190kv motor pared with either 10s or 12s would have you rocketing up hills.

I also agree with @sl33py's point about the trucks: paris are fine, but caliber's are common because they don't have tapering hanger, and mounts can clamp onto their shape really well. Enertion and DiyElectricSkateboard both have mounts for calibers, and DIY has one for paris trucks too. You can't really go wrong either way, but I think calibers are just slightly better for an eboard application.  

Right now my setup is a 6355 190kv motor on 10s, and I'm around your weight- there aren't many hills here, but the setup still gets me up to speed very quickly, and is a beast for being a small single motor build.
```

---
## \#5 Posted by: locktight Posted at: 2015-12-09T04:29:16.132Z Reads: 108

```
I agree with @cmatson i think a single motor build is your best bet. Get a decent sized motor 6355 or 6374 i would recomend the later. This should get you enough power but if it is still an issue you can gear the motor down. USE THE SEARCH TOOL it is your best freind and will help answer your questions.
```

---
## \#6 Posted by: longhairedboy Posted at: 2015-12-09T15:11:37.563Z Reads: 103

```
These mounts are the sickest. Get these and a set of 180mm caliber IIs and call it a day. 
http://longhairedboy.com/shop/drive-system/adjustable-modular-motor-mount-for-caliber-ii-trucks/

also don't forget to check out the boxes and and box mounting kits I have on there. 
http://longhairedboy.com/product-category/component-enclosures/

What cell count/voltage are those zippys? You going twin 3S for 6S? or twin 4S for 8S? or are you doing a 10Ah 6S or 8S?
```

---
## \#7 Posted by: hanthony96 Posted at: 2015-12-09T17:53:06.153Z Reads: 103

```
@longhairedboy @cmatson What battery setup would yall suggest? and I'm wanting to use a wiiceiver or comparable remote so what VESC would yall suggest/is a good value? How does it work pairing your batteries->motors-> and VESCs ? I know you need different things for each but i dont want to buy anything that wont work with another product because it doesnt match. 
Thanks guys!
```

---
## \#8 Posted by: locktight Posted at: 2015-12-09T19:12:07.573Z Reads: 100

```
I would start choosing a motor. Find what kv it is and make sure it has enough watts. Then calculate the battery voltadge needed to make this motor spin to your disired speed. Then choose an esc that can handle this voltadge.

In general a good motor kv range is 190-245
To power this i would recomend anywhere from 10s to 6s battery.(36-22volts)
Then an esc that can handle the voltadge your looking for the vesc can handle up to 63.
```

---
## \#9 Posted by: cmatson Posted at: 2015-12-09T21:48:16.219Z Reads: 102

```
VESC: $110
Wheels: $30 (abec 83mm flywheel clones)
Trucks: $50 (I recommend calibers, but Paris will work)
Mount/pulley system: $130 (either from enertion, or diyelectricskateboard. Longhairedboy's recommended mount would work well too, but you'd have to buy the belts and pulleys seperate)
Remote: $35 (go with the good old reliable gtb2.. you can get them cheap on amazon, and they never cut out signal like the wii reciever does) 
Deck: anything, but generally less flex is better for mounting components

Here is where you divert off though in terms of batteries:
cheaper, 6s setup (less powerful, with more heat)
Better, 10s or 12s setup (more powerful, with less heat/more efficiency) 

I'd highly recommend going with the higher voltage of either 10s or 12s- it will be so worth it in the long run. 

For 10s/12s go around 149-190kv (higher = faster)
For 6s 245kv is really common
```

---
## \#10 Posted by: torqueboards Posted at: 2015-12-10T04:03:51.393Z Reads: 99

```
6S 230KV works well.. Would get you to 20mph if that's as fast as you want.

12S 230KV works too. KV can be similar around that range.

There's also the 2.4ghz Mini Remote too. product/torqueboards-2-4ghz-mini-remote-controller/

If you use VESC, use the custom Wii Nunchuck.
```

---
## \#11 Posted by: longhairedboy Posted at: 2015-12-10T20:07:56.014Z Reads: 97

```
@hanthony96 I've also got enertion compatible 53tooth 9mm belts, so if you're using any of his performance pulleys you can get the belts from me too at a later date when you run out. onloop is pretty good about piling in the belts with your order though. I got like six belts with my last drive system from him. 

 I'm not selling motors... yet... but i think that when i finally do the pulleys and belts may be irrelevant... that's not a hint or anything... please ignore the ellipses after every phrase... they aren't indicative of anything... yet... ...
```

---
## \#12 Posted by: cmatson Posted at: 2015-12-10T20:59:21.857Z Reads: 90

```
@longhairedboy I'm waiting for you to sell everything, so that I can get eboard parts in like 3 days, lol. 

Side note, have you talked to jason about possibly being a US retailer? It would be pretty sweet if he sent you wheel pulleys, motors, etc in bulk so that us here in the states don't have to pay $40+ for shipping.

 it would also take some stress of jason's workload because you'd be filling orders too;)
```

---
## \#13 Posted by: longhairedboy Posted at: 2015-12-10T22:17:02.651Z Reads: 89

```
i have some things in the works. Lets just say i'm attempting to seize an opportunity that i let slip by me a few times before.  :smile:
```

---
## \#14 Posted by: psychotiller Posted at: 2015-12-11T02:09:16.961Z Reads: 88

```
Fast shipping too! Thanks for the belts brotha!
```

---
## \#15 Posted by: WrinklyWink Posted at: 2016-05-11T10:52:11.450Z Reads: 55

```
at 12s with 230kv torqueboard motors what are the configs for the vesc?
```

---
## \#16 Posted by: torqueboards Posted at: 2016-05-11T16:38:42.761Z Reads: 54

```
@WrinklyWink You'd only want to use 10S for my  230KV motor on VESC. You can't use 12S with VESC.
```

---
## \#18 Posted by: WrinklyWink Posted at: 2016-05-11T17:51:57.550Z Reads: 50

```
i heard something about new 200kv motors.. that you'd be offering, and with configs. could we return your 230kvs with these?
```

---
## \#19 Posted by: torqueboards Posted at: 2016-05-12T03:38:55.530Z Reads: 48

```
@WrinklyWink - I was originally thinking of moving down in KV due to the VESC but I might just keep it at 230KV for now. Perhaps in the future I may make it 200kv.
```

---
## \#20 Posted by: axelleboss Posted at: 2016-10-13T17:41:00.275Z Reads: 21

```
Hi I just bought this motor from alien power systems:http://alienpowersystem.com/shop/brushless-motors/alien-5070-hev-sensored-outrunner-brushless-motor-270kv-2200w/
The thing it unlike sk3 motors which have a flat spot, this motor has a keyway.
Do you think it will still work with this sprocket:http://www.ebay.com/itm/1-4-12T-Rotary-Chain-Drive-Sprocket-12-Tooth-Pitch-6-35mm-Bore-5-6-8-10mm-/161940970678?var=&hash=item25b46f1cb6:m:m3rf6KeBnmJqoJmGjfqRq2g
Basically I m trying to figure out if set screws work with keyways.
```

---
