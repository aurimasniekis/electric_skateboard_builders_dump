# First build, choose motor, pulley and wheels

### Replies: 16 Views: 2067

## \#1 Posted by: coffeliten Posted at: 2017-04-17T20:27:44.148Z Reads: 164

```
Hi, i found this on instructables! 
https://www.instructables.com/id/Powerful-2000W-Electric-Longboard/

I want to build my own esk8 but im thinking of some changes.
Which motor is the best? I want a top speed of 20-22mph and good torque. And what size of the pulleys and the wheels do i need?

https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5055-280kv-brushless-outrunner-motor.html
http://www.hellray.de/shop/#!/eSk8-de-Motor-esk8-6374-170kV-3-0KW-mit-Sensoren/p/66640990/category=15255004

To this i will use 12 single cell batteries
https://hobbyking.com/en_us/turnigy-5000mah-1s-20c-lipoly-single-cell.html

A car ESC
https://hobbyking.com/en_us/hobbykingr-x-car-120a-brushless-car-esc-sensored-sensorless.html

And this charger
https://hobbyking.com/en_us/turnigy-reaktor-250w-10a-1-6s-balance-charger.html

So will i be able to make a good esk8 with this setup (SK3 motor)
what else do i need to make the board complete, the links on instructables doesent work!

Thanx for the help
```

---
## \#2 Posted by: mmaner Posted at: 2017-04-17T20:30:41.716Z Reads: 143

```
Mostly your plan looks ok, other than the motor and battery.  A 5055 motor is really small, very little torque.  I sue 6355's and bigger.  12 individual lipos is going to be hard to fit on the deck.  Maybe x4 3s or x3 4s would be easier.
```

---
## \#3 Posted by: coffeliten Posted at: 2017-04-17T20:44:59.023Z Reads: 146

```
Thanx for input.. i still want a 6s motor, is this a better alternative? 
http://www.hellray.de/shop/#!/eSk8-de-Motor-esk8-6374-170kV-3-0KW-mit-Sensoren/p/66640990/category=15255004

Regarding the batteries, Bart on instructables fitted 12 under his board, im gonna use the same type of board.
<img src="/uploads/db1493/original/3X/3/c/3c4b3bdbd55b24ccaa2d8b62f001e4a707ffef44.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/f/8/f80c15a87c1dccc7a87a4798860bbebcdcae691a.jpg" width="666" height="500">
```

---
## \#4 Posted by: coffeliten Posted at: 2017-04-17T21:02:04.132Z Reads: 134

```
Or should i go for something like this? Will the 12 single cell batteries be enough?
http://alienpowersystem.com/shop/brushless-motors/alien-6374-hev-outrunner-brushless-motor-200kv-3300w/
```

---
## \#5 Posted by: mmaner Posted at: 2017-04-17T22:20:11.397Z Reads: 129

```
Yeah, I saw that build and was impressed, but its tight, I mean really tight.  There is barely any room for the electrics.  

I have never used a 6374, I assume there is more available torque and generates less heat.  But I've never needed it, my 6355's run great.  If you are doing a single motor build I would go ahead and get the bigger motor, it cant hurt.  

As far as the battery is concerned, the only advantage to using multiple cells is AMP delivery.  You can get A better C raiting "AMP delivery" by using x6 [Turnigy 5000mAh 2S 30C Lipo Pack](https://hobbyking.com/en_us/turnigy-5000mah-2s-30c-lipo-pack.html).  There are lots of people that say 10c & 20c lipos are pretty bland, 30c will give you some real torque.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-04-17T23:12:39.306Z Reads: 128

```
I don't fully understand how you will balance charge a 12s battery with a 6s charger.

About the C rating, @mmaner is correct, Lipos need plenty of vitamin C to keep them from getting sick.
In my opinion, 30C should be considered the minimum.
I have run 25C Lipos at 12s and it was ok but pretty saggy.
I'm currently running 60/120C Lipos at 10s and even those sag a little. But not nearly as much as the 25C.
```

---
## \#7 Posted by: IsTalo Posted at: 2017-04-17T23:52:01.751Z Reads: 119

```
Maybe he is doing like the instructables, 6s2p. 6 in Series and 2 in Parallel
```

---
## \#8 Posted by: Namasaki Posted at: 2017-04-18T00:14:17.749Z Reads: 112

```
Ok, your right, not sure how I got the idea he was trying to do 12s.
I was thinking series not parallel.
```

---
## \#9 Posted by: IsTalo Posted at: 2017-04-18T00:15:11.973Z Reads: 109

```
I was confused too, also because he is saying "12 single cells"
```

---
## \#10 Posted by: coffeliten Posted at: 2017-04-18T00:42:09.348Z Reads: 106

```
Sorry, my bad..im a complete rookie when it comes to electronics, im doing 6s2p.. A friend of mine is gonna help me put it all together.
I just need to figure out what kind of motor, batteries, wheels and pulleys im gonna use. Should i go for a 6374? 200kv or more?
No matter how much i read i just get more confused =(
```

---
## \#11 Posted by: GinoDePolo Posted at: 2017-04-18T04:58:54.746Z Reads: 98

```
I just finished a build with that EXACT motor. I mean I am only doing initial test runs with it but it definitely reaches 20mph if not higher with a 6s setup. I am also not using a VESC but rather a trackstar 150A ESC and I have to say I am very impressed. I was very worried it wasn't going to be very fast after I had such a small budget but this thing slays! I cannot really speak for how long it will last given these are not the "best" electronics on the market. But it works. And it works well.
```

---
## \#12 Posted by: coffeliten Posted at: 2017-04-20T09:15:07.444Z Reads: 84

```
So i have ordered everything i need to build my first board, what do you guys think about this setup?

Motor:
https://hobbyking.com/en_us/ntm-prop-drive-50-60-270kv-2400w-1.html

Batteries (6s3p)
https://hobbyking.com/en_us/turnigy-5000mah-3s-20c-lipo-pack.html

ESC:
https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-120a.html

Madrid weezer board, alien power trucks, alien power wheels 83mm, alien power abec9
```

---
## \#13 Posted by: Bazingazunga Posted at: 2017-04-20T10:19:59.318Z Reads: 76

```
You in the UK?
```

---
## \#15 Posted by: bartroosen12 Posted at: 2017-04-20T11:07:20.484Z Reads: 79

```
These parts looks like a very good choise
```

---
## \#16 Posted by: Jaykob Posted at: 2017-07-13T14:54:13.000Z Reads: 56

```
Hi! First build and i'm holding my index on the order button. But first I would really like your input!

This is what i already have.

Board is a Fibretec similar to this:
http://www.kahalani.se/fibretec-longboards-21
Trucks (Not sure about the length):
http://www.skatesonhaight.com/Paris-Longboard-Trucks-V2-180mm-Black-Raw-p/ptv2802.htm

This is what I think I will get
Motor:
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-245kv-brushless-outrunner-motor.html
Mount/Pulley/Belt (15 mm belt I think):
http://alienpowersystem.com/shop/cnc-kit/alien-drive-complete-kits/alien-drive-systems-electric-longboard-diy-kit-50mm-motor/
Wheels:
http://www.ebay.com/itm/Blank-Pro-83mm-Longboard-Orange-Flywheels-ABEC-7-Bearings-Spacers-/132257857467?hash=item1ecb2ebfbb:g:IqsAAOSwWdZZZSzi
ESC:
diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/
Battery 2 pcs(?):
https://hobbyking.com/en_us/zippy-flightmax-5000mah-5s1p-20c.html
Remote/Controller:
diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-nano-remote-controller/


What do you guys think? Im really unsure about the batteries and motor. 
I don't have a clue about what else to get when it comes to batteries but I'm pretty sure that Alien or Torque motor would be what i would buy instead (if I would get something else). 

I might need some new risers to prevent wheel bite as well..

Am I completely off? 

Would really appreciate any inputs! :slight_smile:

//Jaykob
```

---
## \#17 Posted by: Jaykob Posted at: 2017-07-13T15:44:24.213Z Reads: 45

```
Figured I would bump this topic instead of making a new one. Hope that's alright!
```

---
