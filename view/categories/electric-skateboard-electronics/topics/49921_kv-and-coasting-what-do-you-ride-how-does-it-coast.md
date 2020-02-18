# Kv and coasting - What do you ride, how does it coast-

### Replies: 29 Views: 1256

## \#1 Posted by: 666 Posted at: 2018-03-23T14:58:26.693Z Reads: 228

```
Wussup $katerzz
 
So I read somewhere (kaly on this forum) that the higher the kv the lower resistance the motor has. Since I love the feeling of flow I want the build to have "maximum coasting abilities". With this I mean longest distance ride after releasing the trothle. Like that brand new high speed bearings feeling.

So what would be the perfect kv for optimum coastability? And what battery pack would match with this? 

I was thinking 239 to 245 kv, would this be safe for the vesc rpm limit with a 10s li ion? I'm assuming it would be a bit overkill and I'd have to go more like 8 - 9 s.

I don't know what motor and wheel pulley I would need with this.

I weigh about 70-75 kg, wheels between 73 - 83 (don't know what I'm gonna settle for, used to pool and street setup, never had longboard). I want maximum speed of about 47 kph without frying my electronics. Don't care to much for torque, but don't wanna be defeated by a bit of a hill either.

I'm assuming dual motor  = dual resistance, so I'm gonna start single and work my way up to double to see what I like most. I think double would be better for more straight acceleration ( if the power is only coming from one side I think you'd ride a bit crooked no?)

Thanks fo reading, have a good day 😎
```

---
## \#2 Posted by: Hummie Posted at: 2018-03-23T15:04:07.153Z Reads: 216

```
I don’t think kv necessarily relates to cogging while unpowered.  Less cogging from more poles.  Less resistance from a hub motor with many poles.
```

---
## \#3 Posted by: professor_shartsis Posted at: 2018-03-23T15:07:24.898Z Reads: 207

```
Subtracting "turns" from the motor's winding decreases the **electrical resistance** of the motor in ohms & increases the kv a proportional amount.

New KV * New Turns = Original KV * Original Turns

New KV = (Original KV * Original Turns) / New Turns

I am not aware that changing the KV in any way improves "coasting ability."
```

---
## \#4 Posted by: Der6FingerJo Posted at: 2018-03-23T15:19:13.729Z Reads: 183

```
Kaly probably meant the electrical resistance.
Higher kv motors use more copper, so they can handle higher currents.

In the end, different KV motors of the same type still use the same magnets on the same bearings so the coasting resistance should be the same really.
```

---
## \#5 Posted by: professor_shartsis Posted at: 2018-03-23T15:21:40.470Z Reads: 175

```
[quote="Der6FingerJo, post:4, topic:49921"]
Kaly probably meant the electrical resistance.

Higher kv motors use more copper, so they can handle higher currents.
[/quote]


Assuming the original motor has maximum copper fill, decreasing the number of turns to increase kv will result in either A) less copper or B) equal copper if you increase the wire cross section proportionally to the number of "turns" which were removed to increase the kv-- and decreasing the number of turns (shortening the winding) or increasing the wire's cross section each have the effect of lowering the motor's electrical resisitance. interestingly, changing the wire's cross section without changing the number of turns affects the electrical resistance but not the KV. increasing the max rpm per volt (KV) by decreasing turns and resistance also lowers the torque per motor amp (KT) by a proportional amount.
```

---
## \#6 Posted by: Deckoz Posted at: 2018-03-23T15:44:11.951Z Reads: 152

```
Loose 20mm belts.

On abec 107 on flat ground, 1 push 32ft
With belts on 27ft.

Every other board I've built with smaller width tighter belts has had a rolling distance of half or less with belts on, especially if idlers are involved

Don't so much think kv matters...as much as drivetrain resistance (belt system) unless you are talking about hubs.. ...
```

---
## \#7 Posted by: onepunchboard Posted at: 2018-03-23T15:46:04.904Z Reads: 152

```
u need loose belt and idler. kv doesnt effect too much. i went from 260 to 190. 190 is more resistant but almost no difference with coasting with loose belt.
```

---
## \#8 Posted by: squishy654 Posted at: 2018-03-23T15:58:57.673Z Reads: 149

```
I think it's unrelated to KV, although it might be apart of the equation. It has more to do with the poles and even the strength of the magnets chosen...some argue that a motor with more resistance has more torque under power for its size as well, so something to think about...it sort of makes sense, the stronger the magnets the harder it cogs, the more "strength" it will have as well...so a good motor that can coast well, may be weak and inefficient...there's most likely a balance for every use model of a brushless motor..This industry uses large scale 3D RC airplane motors, designed to hover a 10k$ plywood aircraft about 1.5 the size of a full scale...these motors are beefy..and strong...not really made for efficiency or coasting at all..dudes who are making electric skateboard specific motors might be doing things differently, like the sealed stuff...I know the HK skate motor coasts really nice, mostly because it's rolling mass and it's designed for skateboards..since we do not require the motor to change RPM quickly there's lots of headroom to configure motors more for the purpose of coasting..we don't require stiff cogging motors like a multirotor may enjoy, they are changing RPM's hundreds of times a second with dynamic breaking and such..our purpose is like a soft start rc helicopter, smooth and accurate and free running is better, but we may end up carrying more mass for the same overall wattage, which is no big deal, because we ain't flying in the air worried about overall weight..I imagine you can build a sensored sealed 200kv motor with large weak magnets in an oversized can, same wattage and coast for days..
```

---
## \#9 Posted by: professor_shartsis Posted at: 2018-03-23T16:02:30.954Z Reads: 136

```
Lower KV could result in more mechanical resistance at the same RPM if one attempts to coast downhill faster than the no load rpm of the motor (considering the battery pack voltage.) Above no load rpm, the back emf-voltage produced by the motor would be greater than the battery pack voltage and would lead to reverse-current charging the battery above this speed. The mechanical "braking" one would experience above no load rpm would result from charging the battery and the electrical resistance of the circuit. A lower KV motor would experience this drag or braking-sensation-above-no-load-rpm at a lower RPM than a higher KV motor, because a higher KV motor produces lower back emf voltage per rpm than a lower kv motor. I do not recommend coasting faster than the no load speed of the motor due to the possibility of uncontrolled current damaging a battery or ESC.
```

---
## \#10 Posted by: Deckoz Posted at: 2018-03-23T16:16:14.714Z Reads: 124

```
^^^ this


You'll find with quads, multistrad motors aren't as powerful but make the smoothest freestyle quads. While solid core motors have alot more power and hard harder to tune to be smooth. While possible to get close, multistrad motors are smooth as butter. Talking about windings not the stators btw... So no one gets confused.

But also multistrand motors are more efficient... Then solid core if you talk about watts wasted... Overall. Ie you'll get longer flight times out of multistrand then solid strand. Things like this matter when you talk about flying.. not many consider it as our boards aren't reliant on weight so much like quads..
```

---
## \#11 Posted by: trampa Posted at: 2018-03-23T16:26:56.824Z Reads: 114

```
Coasting is relative to the torque setup. A high torque setup, usually doesn't coast as nice as a low torque setup. Everyone said they experience the best coasting on hub motors, since they lack gearing and in consequence torque. First thing I realized riding the Raptor 2, was lack of coasting, since the hubs of this board are designed to output a lot of torque (a lot of poles and low KV). Costing wasn't a lot better than on regular geared setups. 

What I learned:  You can't have the best of both worlds. Either your board has good torque, or good coasting. KV doesn't matter, as long as you compensate the higher KV with more gearing. Weather you go for high KV and high gear ratio, or low KV and longer gearing, the coasting is the same. The only way to have good coasting is on a setup for speed, which lacks low end torque and hill climb.
```

---
## \#12 Posted by: Deckoz Posted at: 2018-03-23T16:29:32.238Z Reads: 111

```
Raptor 2 only coasts like 16ft off of one push...


I run 15/36 or a 2.4:1 reduction...

I've also run a 14/34 2.43:1, 16/40 2.5:1, 12/32 2.67, 15/50 3.33:1 all on 107abecs..

I think friction from teeth in mesh plays a bigger part then the reduction does..just based on my feetometers. The 2.43 and 2.67 are setup for more torque then the 2.4, and roll better or the same as there's less teeth in mesh...
```

---
## \#13 Posted by: mixedcreation Posted at: 2018-03-23T17:13:59.519Z Reads: 105

```
So you want like a Jed board type of coasting?  In all honesty I would like to build a small lightweight cruiser with the abilities of the jed board "coasting" and the programming of mellow's endless ride.
```

---
## \#14 Posted by: Hummie Posted at: 2018-03-23T17:40:40.537Z Reads: 99

```
Mellow motors which I think ae still standard 12 tooth coast really well. Don't know if its from software.
There's no benefit of using multistand wire unless the motor is gong so fast the Eddy currents are a lot there. And then litz wire is a benefit. We aren't at that erpm. Thick solid wire is better than because it has more copper n less enamel. If u get more copper then less resistance. Whether ur flying r riding efficiency is eff 
More teeth is Les cogging. 
Anyone smell devin5
```

---
## \#15 Posted by: aigenic Posted at: 2018-03-23T19:00:46.577Z Reads: 88

```
What about jed boards? According to the videos I have seen their gear system is the best for coasting...even outperforming hub motors :O Is it because of the no belt, just gears system, or is there a different reason?
```

---
## \#16 Posted by: Okami Posted at: 2018-03-23T22:20:10.606Z Reads: 85

```
I think gears are the answer, check what @Nowind has said recently concerning riding with direct drive (dd) versus belt drive.. different feel to it
```

---
## \#17 Posted by: professor_shartsis Posted at: 2018-03-23T22:30:09.645Z Reads: 82

```
same size stator... higher kv vs lower kv... same # of motor amps... gearing of each adjusted to equalize final torque at the wheel edge between both KVs @ same motor amps... the higher kv motor must spin at more rpm at the same motor amps limit to deliver the same mechanical power at the same ground speed. more motor rpm at the same wheel rpm equals more motor bearing drag while coasting at the same ground speed with higher kv for the same performance with the same motor amp setting.
```

---
## \#18 Posted by: b264 Posted at: 2018-03-23T22:37:56.505Z Reads: 79

```
Gears are NOT direct drive.  Gears are gears.

Direct drive would be something like a hub motor or a Carvon system.
```

---
## \#19 Posted by: Okami Posted at: 2018-03-23T23:13:03.794Z Reads: 78

```
yep, good call.. just heard the rumor about direct gear driven drivetrain benefits.. forgot to mention / include hub motor 'direct drives'.. havent looked much into jed boards, honestly

I know carvon has familiarized us with direct drive with directly mounting original wheels.. I suppose im spending more time / attention on mountainboards, sorry if i confused anyone
```

---
## \#20 Posted by: 666 Posted at: 2018-03-24T00:33:22.209Z Reads: 79

```
So I go for a motor with a lot of poles, loose wide belt and optimize gears for speed over torque. If I overstand correctly?

I still want to go as fast as possible so I don't really want a weak motor. I will check out the hk -oh just figured out hk is hobbyking lol, so you mean the sk3 right- and the multistrad. What are quads? Drones or something?
There are a lot of new abbreviations and jargon to learn damn.

@professor_shartsis I'm not talking about going downhill there are no hills here and if there where i'd go without motor. But if I where to go down a hill it'd be safer for the battery and vesc to do it with a higher kv motor right?

So professor, are you implying that theorethically a higher kv motor creates more drag for the same speed.Because of the way the gearing is optimized to have the same torque? And thus is worse at coasting? Or am I interpreting completely wrong? 

Everybody else is saying kv probably doesn't matter for coastin. 

@Der6FingerJo Kaly literally said this

"The coasting is the reason for the 239 Kv.
At higher kv the drag is minimum and if you take advantage of coasting properly the battery range can be increase and I willl take that every day.

I am one of the guys that really prefer carving and coasting so the motor with lower Kv motors just kill the fun for me."
```

---
## \#21 Posted by: E1Allen Posted at: 2018-03-24T00:39:44.376Z Reads: 69

```
Mine coasts 278.3ft after I let off the throttle going 37mph...
```

---
## \#22 Posted by: 666 Posted at: 2018-03-24T00:42:01.995Z Reads: 72

```
What's your setup?
```

---
## \#23 Posted by: professor_shartsis Posted at: 2018-03-24T00:42:11.734Z Reads: 72

```
[quote="666, post:20, topic:49921"]
So professor, are you implying that theorethically a higher kv motor creates more drag for the same speed.Because of the way the gearing is optimized to have the same torque? And thus is worse at coasting? Or am I interpreting completely wrong?
[/quote]


**If** you adjust your gear ratio between motor pulley & wheel cog such that the torque is the same at the wheel between lower and higher kv at the same number of motor amps, the higher kv motor will need to turn more rpm at the same ground speed, and thus in theory, the higher kv motor will create more drag from a coasting perspective for the same performance while powered.
```

---
## \#24 Posted by: E1Allen Posted at: 2018-03-24T00:46:25.804Z Reads: 70

```
Just the normal dual 6374 setup on 15/36 gears.   I never find myself coasting..
```

---
## \#25 Posted by: 666 Posted at: 2018-03-24T00:51:19.748Z Reads: 72

```
Okay thanks that makes sense, and if they would both be 15/36? I'm assuming the higher kv would have less drag??
```

---
## \#26 Posted by: professor_shartsis Posted at: 2018-03-24T00:52:30.995Z Reads: 70

```
With the same gear ratio & same stator, higher vs lower kv, drag should be the same in theory-- unless you pass the no load rpm downhill, which is slower with lower kv.
```

---
## \#27 Posted by: Hummie Posted at: 2018-12-01T17:57:32.774Z Reads: 39

```
The resistance is caused by eddy currents and hysteresis and the winding doesn’t matter. Super thin laminations (or powder core) or another stator design could reduce these losses and improve coasting
```

---
## \#28 Posted by: mikenyc Posted at: 2018-12-01T19:12:26.552Z Reads: 34

```
I don’t think he’s going to reply to you until at least May 1, 2019, 8AM EST.
```

---
## \#29 Posted by: Hummie Posted at: 2018-12-01T19:54:40.630Z Reads: 34

```
Yea I know been a while but I was just posting about this yesterday.  But confused “cogging” which you feel in ur hands spinning the motor which is not a true loss.   https://www.electric-skateboard.builders/t/4x-times-less-magnetic-resistance-easier-coasting/76644/5
```

---
