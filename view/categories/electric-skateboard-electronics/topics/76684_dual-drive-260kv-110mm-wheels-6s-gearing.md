# Dual Drive 260KV - 110mm Wheels - 6S - Gearing?

### Replies: 24 Views: 676

## \#1 Posted by: Owen Posted at: 2018-12-01T11:30:38.162Z Reads: 137

```
Hi guys. I've been hunting the forum and haven't quite found anything that answered my question so thought that I'd come here.

I have purchased 2 X Turnigy SK3 6354 260 KV Motors : 
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6354-260kv-brushless-outrunner-motor.html

And 2 -  X CAR Beast ESC's 150 A ( I would've preferred VESC's but budget yaknow ) : 
https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-150a.html

I have some 6S packs too and was thinking of running 6S to each motor ( that's the ESC's max ) and having 2 X 5Ah packs in parallel for more capacity. 

I REALLY want the 110mm wheels because the look AWESOME : 
https://www.amazon.co.uk/Slick-Revolution-Wheels-Electric-Skateboard/dp/B07417D1RC/ref=cts_sp_1_vtp?th=1

I've just been struggling to work out gear ratios. I know big wheels and high KV is already quite a lot of speed but would the other motor bring my torque up to a reasonable amount if I have a 15 to 36 tooth reduction for example?

I have had a look on Esk8 calculator and is says with this ratio, I should get a top speed of 30.99 mph. But I need to know if I'd get enough torque to have fun? ;)


And Trucks wise, I've been looking at something like this
https://www.ebay.co.uk/itm/NEW-7-STREETSURFING-LONGBOARD-BOLT-ON-or-DROPTHROUGH-TRUCKS-245-MM-OV-ALL/132873824772

With one of these decks

https://www.customskateboards.com/blank-longboards/Blank-Laying-It-Down-Longboard

Has anyone got good motor mount recommendations?

I appreciate this was a lot to ask, sorry!

Thanks for your help.

Owen.
```

---
## \#2 Posted by: moon Posted at: 2018-12-01T11:33:51.066Z Reads: 119

```
first off you  need to buy 5 decks and its from USA so shipping will be >$100

If really budget is what you want you might aswell get a meepo
```

---
## \#3 Posted by: Owen Posted at: 2018-12-01T11:47:01.848Z Reads: 113

```
Well I won't necessarily get that deck. It was just an idea. And I want my own board that I can upgrade over time, not just buying a store bought one...
```

---
## \#4 Posted by: moon Posted at: 2018-12-01T11:48:43.690Z Reads: 112

```
Then spend a little more if you can and start with a single motor

https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html

Get a VESC should be around £45

And get caliber trucks
```

---
## \#5 Posted by: Owen Posted at: 2018-12-01T11:51:29.276Z Reads: 98

```
Are two 260KV motors not ideal then?
```

---
## \#6 Posted by: moon Posted at: 2018-12-01T11:51:53.897Z Reads: 97

```
No you need like 190kv or lower

and that motor i linked is bigger and cheaper
```

---
## \#7 Posted by: Owen Posted at: 2018-12-01T11:52:26.224Z Reads: 93

```
But what about using a gear reduction? Surely this would create the torque I need?
```

---
## \#8 Posted by: Pedrodemio Posted at: 2018-12-01T12:41:30.546Z Reads: 86

```
What top speed are you after?
```

---
## \#9 Posted by: Owen Posted at: 2018-12-01T14:15:13.109Z Reads: 86

```
Hiya, Probably around 30? Seems reasonable for a good amount of torque.

Cheers.
```

---
## \#10 Posted by: Sn4pz Posted at: 2018-12-01T14:30:23.802Z Reads: 81

```
[quote="Owen, post:9, topic:76684"]
Probably around 30? Seems reasonable for a good amount of torque.
[/quote]


You trade torque for top speed and vice versa, you certainly would not have the 'gripping' torque you think you will if your top speed is 30mph with 260kv motors. Look at the motor above and take his advice, hes trying to ensure you wont spend twice. weve all done it :man_shrugging:
```

---
## \#11 Posted by: Owen Posted at: 2018-12-01T14:33:31.676Z Reads: 73

```
Thanks. I'd be spending twice if I bought another  motor after I just bought 2 ;)
```

---
## \#12 Posted by: Owen Posted at: 2018-12-01T14:37:07.569Z Reads: 70

```
Can I do Dual Drive 6364? Or not needed?
```

---
## \#13 Posted by: moon Posted at: 2018-12-01T14:44:56.515Z Reads: 70

```
Depends what trucks you use, you are kind of limited to one truck which is TB  218mm
```

---
## \#14 Posted by: Owen Posted at: 2018-12-01T14:46:56.944Z Reads: 73

```
I bought the 6364 :) Sorry to be a pain, What sort of current would I be looking at on a VESC? Like 75 continuous or is that too low?

Cheers
```

---
## \#15 Posted by: moon Posted at: 2018-12-01T14:49:10.800Z Reads: 72

```
[quote="Owen, post:14, topic:76684"]
I bought the 6364
[/quote]

They are good motors but you need to get the right trucks for them really. Or you can use diagonal drive.

You should read more

https://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980/2
```

---
## \#16 Posted by: Jmding Posted at: 2018-12-01T17:58:03.066Z Reads: 63

```
The big problem is that you are running 6s, or about 20 V. The motor can't handle much more than 60A, 20V * 60A = 1200 watts. That's a little more than the Chinese boards, but not enough to make it worth the time, effort, and expense.

In diy, the most minimal build plan that makes sense is imo 12s, LiPo, single 6355 200 kv, chain drive, geared to 25 mph. Otherwise it usually makes more sense to buy a Chinese hub motor board or a used boosted.
```

---
## \#17 Posted by: b264 Posted at: 2018-12-01T18:16:46.434Z Reads: 64

```
Don't buy motors with a kv over 190 or 200.

Use [a calculator](https://calc.3dservisas.eu).  10 N&middot;m is adequate/not much torque and 25 N&middot;m or more is a lot of torque. ("Total Max Torque" in the Overview)
```

---
## \#18 Posted by: Owen Posted at: 2018-12-01T18:17:03.452Z Reads: 62

```
I'd be using dual motors so hopefully less current would be drawn. I'd upgerade to 12s VESC's when I can afford it too. So 12s (44.4v) * 70A MAX = 3108 Watts which is kinda reasonable. Obviously, I wouldn't be running 70A continuous, more like 30? Only 70 maybe starting off.
```

---
## \#19 Posted by: Owen Posted at: 2018-12-01T18:17:50.425Z Reads: 57

```
Thanks, ill have a look.
```

---
## \#20 Posted by: Skunk Posted at: 2018-12-01T20:37:05.712Z Reads: 58

```
You're gonna want caliber trucks at the very least.
If you go with the normal calibers 6364 wont actually fix next to each other. 
But you could have one facing forward and one backwards.
Or
Buy @torqueboards 218 truck (basically a longer caliber truck) 
Then you could mount the motors next to each other.

Basically 
![blob|375x500](upload://rtuyWOsI6eiO8mQuxAC5qui4qwO.png) ![CB10632E-78F4-438F-9114-1FB173AD7E85|375x500](upload://zhchFpyIdlDh5sebyob0J9i864r.jpeg) ![image|666x500](upload://fp5LtX8u81iN0YE2XhrblSxucb.jpeg)
```

---
## \#21 Posted by: pat.speed Posted at: 2018-12-01T22:40:58.717Z Reads: 49

```
I made the same mistake, buying the hk xcar esc. Don’t get me wrong it’s a good esc, but not so much for esk8. Plus it’s actually cheaper to buy 2 vescs.

2x xcar + programming card ~$185
2x flipsky vesc + loop key ~$165

Edit: prices are in AUD
```

---
## \#22 Posted by: Owen Posted at: 2018-12-02T16:36:04.314Z Reads: 37

```
Yo, thanks a lot Kelly!

Now I've ordered the 6364 and already have 2 x 6354, I don't know which to use.. I guess I could get the 218 Truck and try dual 6354 or single 6364?

Cheers for your help!

(Sorry about the slow reply, I got blocked from replying...)
```

---
## \#23 Posted by: Owen Posted at: 2018-12-02T16:42:26.371Z Reads: 36

```
Thanks for the Help!  I bought the ESC's on a black Friday deal as well as the motors and a battery and a program card for £180 which was a bargain ;)  I am doing a Jet Surfboard project aswell  so thats the main reason for buying all that, just wanted to see if I could cross use them :) 

Cheers for your help!
```

---
## \#24 Posted by: Owen Posted at: 2018-12-02T16:49:29.000Z Reads: 33

```
What current VESC's are usually used do you know? Because surely starting off current is at least 70A?
```

---
