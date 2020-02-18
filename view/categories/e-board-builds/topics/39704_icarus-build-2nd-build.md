# Icarus build (2nd build)

### Replies: 11 Views: 753

## \#1 Posted by: Enrico Posted at: 2017-11-29T22:56:57.153Z Reads: 141

```
Deck: Flex 2 Icarus
Trucks: Caliber 50 
Wheels: Orangatang Kegel
Belt & Pulley: Torque boards kegel set 14T motor pulley 36T wheel pulley
Mount: Torqueboards V4
Motor: Torqueboards 6355 190kv
Battery: Torqueboards 12s2p with enclosure
Focbox
Enertion nano controller
Single drive

I really want to try mount it on a drop but am worried about ground clearance with the drive system, what do you guys think?

Also for mounting the battery & enclosure, is it a good idea to use ordinary wood screws (x6)? I don't want to have holes going all the way through the deck. Thinking of mounting the battery to the board with velcro some something to reduce the weight on the enclosure
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-11-29T23:25:58.558Z Reads: 120

```
Wood screws are a good solution if you don't intend to be taking the enclosure off many times. The wood will wear out in the screw holes. I'd recommend getting some insert nuts. They thread into the wood, and give you some nice, long lasting and strong threads for you to abuse.

Also, 260kv with 12s is WAY over the focbox's erpm limit. You'll either be limited to the maximum erpm setting even though your battery/wheels/motor setup can go faster, or you risk frying your DRV and eating pavement.
```

---
## \#3 Posted by: BoostedBuilder Posted at: 2017-11-29T23:27:58.365Z Reads: 108

```
[quote="Enrico, post:1, topic:39704"]
I really want to try mount it on a drop but am worried about ground clearance with the drive system, what do you guys think?
[/quote]


You can buy some sidewinders (if you are not planning to go very fast) and back mount the motor. Or just back mount the motor on the Caliber)
```

---
## \#4 Posted by: Enrico Posted at: 2017-11-29T23:54:05.534Z Reads: 92

```
What's the focbox erpm limit? 
To be honest, I only chose the 260kv motor so I can run a 50mm motor, I don't mind setting my speed limit to something like 40kmh

https://scottkellum.github.io/Esk8-RPM-finder/
according to scott's erpm calculator, 40kmh speed limit will set my erpm at 47.7k erpm which is lower than the 60k erpm limit for a vesc.
```

---
## \#5 Posted by: MysticalDork Posted at: 2017-11-30T00:11:50.382Z Reads: 84

```
The focbox (and all controllers based on vesc 4.xx hardware) have a limit of 60k erpm. 260kv with 12s would give a maximum of ~91k erpm. Banggood has some <200kv 50xx motors.
```

---
## \#6 Posted by: MysticalDork Posted at: 2017-11-30T00:14:34.126Z Reads: 86

```
It is worth mentioning that if your desired speed is that far below what your board would be capable of, you should adjust your gearing. You'll get much better startup torque, acceleration and hill climb if you gear your motor for the speed you want, rather than setting limits, essentially running it at 50% throttle the whole time.
```

---
## \#7 Posted by: Colson003 Posted at: 2017-11-30T00:15:45.736Z Reads: 85

```
@chaka also sells 5065 motors. 170 and 200kv http://www.ollinboardcompany.com/products?page=2
```

---
## \#8 Posted by: Enrico Posted at: 2017-11-30T04:12:24.242Z Reads: 72

```
Ok, I managed to change my motor to a 63mm 190kv. This new motor combined with the 12s battery puts me at 57456 ERPM, just under 60k. 

How does this sound?

Also, about your insert nuts; I have never used these before (first time i've heard of them) so i'm not sure how strong they are. I looked at somebody's post with the 12s2p battery from torqueboards and the casing had velcro on it which I'm supposed to mount the battery to. Because of this, the six insert nuts will be holding all the weight of the 12s2p battery + focbox. You reckon it's still safe or should I just hold my breath and use countersink screws + nut?
```

---
## \#9 Posted by: MysticalDork Posted at: 2017-11-30T06:07:53.259Z Reads: 70

```
With a fully charged battery (4.2v/cell) you'll actually hit 67K erpm, but the soft limit in the controller will handle that no problem, and it's only like 10% rather than 50%, which is good. 
(Whatever you do, DO NOT check the box in BLDC tool that says "limit erpm with negative torque", it will cause the board to stop out from under you at maximum speed, and you will eat pavement.)

I did my board with insert nuts (like, 20 of them or so) and the battery (and vescs, and everything else) is supported by them no problem. I'd worry about the plastic of the enclosure giving before the insert nuts, they're really quite ferocious. I used cheap shitty ones because I was using so many. If you're only going to use 6, I'd recommend getting some nice ones from McMaster or something.
```

---
## \#10 Posted by: Enrico Posted at: 2017-11-30T06:09:06.519Z Reads: 68

```
I'm more worried about the nuts stripping the precious wood of the icarus deck
```

---
## \#11 Posted by: MysticalDork Posted at: 2017-11-30T06:17:11.505Z Reads: 68

```
They'll be less likely to do so than wood screws will. They're larger in diameter, which means they have more meat to bite into. If you generate enough force to strip the nuts, you'll have already destroyed the enclosure.

Here are some nice ones on McMaster, designed for hardwood. https://www.mcmaster.com/#threaded-inserts/=1ah4xb1
```

---
