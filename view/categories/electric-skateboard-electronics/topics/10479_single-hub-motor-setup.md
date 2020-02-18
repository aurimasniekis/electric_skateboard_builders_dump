# Single hub motor setup

### Replies: 20 Views: 1750

## \#1 Posted by: pengy Posted at: 2016-10-01T21:56:48.390Z Reads: 211

```
Hey everyone, I'm looking to build my E-board and would like to put the motor in the wheel (Hub motor)
After a long research I've been thinking that around a 90kv motor would work best for my needs: I'm 200 pounds and would ride mainly on flat surfaces but would like it to be able to do some moderate hills..
I was looking at the carvon v2.5's performance and this is the kind of performance I would like to achieve. I plan to ride probably no more than 20mph top speed.

My problem is finding this kind of motor which will also fit in a 83mm wheel.. I'm thinking up to 63mm motor width should be fine. 
I found a Turnigy sk3 6374 149kv and was looking at perhaps this will be good for me to run at 10s or 12s but afraid that it won't give enough torque since it is going to be a 1:1 ratio.. (in wheel hub motor)

Does anybody know if the 149kv will be good or where I could find lower kv motors for my needs? Thank you.
```

---
## \#2 Posted by: Namasaki Posted at: 2016-10-01T22:07:45.814Z Reads: 201

```
Nice thing about the Carvon V2 and V2.5 is that you won't have to worry about the urethane coming loose from the motor.
Also they have cooling fans on the back of their motors to pull air through them.
V2's are 145kv and really fast.
V2.5's are somewhere around 80kv and more for hills and heavy loads.
For a guy who is 200lbs, you probably need 80kv dual drive especially going up hills.
```

---
## \#3 Posted by: pengy Posted at: 2016-10-01T22:18:30.492Z Reads: 183

```
You are right they are 85kv on the carvon 2.5 and someone did 28mph. They look good but I was thinking of cutting costs and make it myself
```

---
## \#4 Posted by: pengy Posted at: 2016-10-01T23:54:45.118Z Reads: 158

```
So maybe even 70kv, upto 100kv as long as it is powerful. Why are they so hard to find?
```

---
## \#5 Posted by: pengy Posted at: 2016-10-02T00:33:27.539Z Reads: 153

```
Also another thought about the wattage, I'm just wondering if that's going to be something I should consider looking into, as a 3000w 149kv motor might give more real life torque compared to a 2000w 80kv?
especially as I'm planning to run it with a 10s or more
```

---
## \#6 Posted by: evoheyax Posted at: 2016-10-02T01:06:41.631Z Reads: 144

```
What tools are you working with? Turning an outrunner into a hub means you'll need some accurate metal cutting tools which could cost you $500-$1000. I wanted to take your path, but I just found through research that it's not worth it for a few motors. If you want cheap hub motors, check out hummies hubs. He lets them do dirt cheap. Either way, with what you need, it won't be cheap. But spend the money, it'll be well worth it.
```

---
## \#7 Posted by: pengy Posted at: 2016-10-02T02:13:10.945Z Reads: 135

```
I was thinking about working with plastic actually instead of metal as I have seen it applied by some companies and different hub motor builds. So making plastic molds for covering the motor and than secure it with a cap from one side, if the chosen motor has some hatches I would make the plastic go in them to make a more firm hold to the motor and probably apply some kind of silicon or rubber between the motor and the mount. And then cut the matching radius to clear the inside of the wheel for the motor with the motor holder. I plan to concave some lines on the wheel that will match the motor cover. I was thinking to do the mold myself and with any help, use local professionals.

Of course at that point I would like to find an easy affordable solution.

I've heard about hummies hubs but have no idea of where to get them and their cost..
if you know that would be great to look into.
```

---
## \#8 Posted by: caustin Posted at: 2016-10-02T02:19:27.664Z Reads: 123

```
www.steelhubs.com
@Hummie
```

---
## \#9 Posted by: pengy Posted at: 2016-10-02T02:32:53.951Z Reads: 117

```
Thanks! Looks interesting
But two hubs means I have to have two ESCs isn't it?
```

---
## \#10 Posted by: caustin Posted at: 2016-10-02T02:36:19.110Z Reads: 113

```
Yes 1esc per motor
```

---
## \#11 Posted by: pengy Posted at: 2016-10-02T02:51:47.438Z Reads: 112

```
That's not a bad deal, need to decide between that and the carvon v2.5 which has one hub but looks like it has all the power I need, and save some weight by using only one ESC and hub.. Or to do it myself.
```

---
## \#12 Posted by: evoheyax Posted at: 2016-10-02T03:08:06.537Z Reads: 108

```
Hub motors get hot and plastic melts under heat. I don't think plastic near motors is a good idea. Not to mention the strength of plastic vs steel. Steel is just a better way to go. I have the tools to convert a motor into a hub motor, yet I still don't do it because like I said, it's not worth the effort for 1 or 2 hub motors.

But if you are insistent, knock your self out. It depends if you really really want to make your own or if you are doing it cause you just want to ride. If your just trying to save a quick penny, making your own will cost more in the long run. It's the false economy that gets you.

Carvons are great. I just don't imagine 1 getting a me up hills. I am using a dual carvon v2 right now and I have overheating issues with my vescs. The dual carvon 2.5 won't have these issues, but a single carvon 2.5 at 200 pounds (same as me) and hills (same as me) might.
```

---
## \#13 Posted by: pengy Posted at: 2016-10-02T07:05:16.743Z Reads: 97

```
Yeah the heat is an issue that is hard to expect, was wondering maybe with the highest possible volts the motor can take, it would heat up less due to less amp draw but I don't know if there's a sweet spot for that. How many volts do you use with your carvon2? Come to think about it for dual hummies motors that is a good price, it would make a it more expensive probably to build it myself. Although it means that I would need two ESCs which could be expensive. BTW would you say I should go with 2 VESCs? Or could find a more affordable solution..
```

---
## \#14 Posted by: evoheyax Posted at: 2016-10-02T07:20:51.687Z Reads: 101

```
Depends how much of a gambler you are... Heres my hierarchy of E-board Sped Controllers

Chakas vescs
         |
        \/
Other Vescs (have little no BOM changes)
        |
       \/
FVT 120 amp
        |
       \/
Other Car ESCs

Car esc's are really hit or miss. Sometimes, you really get a dude. My first car esc was a dud. Then, I blew out 3 with bad settings. They can be harder to configure as there's often spotty documentation. With the vesc, you can set numerical values based on scientific values. Thus use can use physics and math to configure it properly. The FVT 120, I've had bad experience running 1 motor with. I drew too many amps, and it blew. The vesc has amp limits, so you won't break it like this. The vesc has many other built in protections such as overheating protection, and over discharge protection to protect your batteries. The problem is that a lot of vescs seem to be hit or miss. There's various theories as to whose better than who. Chaka has been the only thus far that has modded the BOM to remove weak points, thus making it more robust. But many have had success with other vendors vesc. There's been a fair number of bad experiences too. Chaka fixes vescs that break free, while the rest do not, if they offer repair services at all. It sucks to pay $160 for a speed controller, imagine paying over $700 for a quad one like I did... The thing is, it'll last. And if it doesn't he'll fix it.
```

---
## \#15 Posted by: pengy Posted at: 2016-10-02T18:24:16.292Z Reads: 86

```
With these things, cheap ends up costing more.. and I do like the amp over draw and heat protection of the VESD, it shouldn't come to that according to careful calculations but still.. And heard it makes things go quieter which I don't know if true.. 

For now I'm still considering my options, and was looking also at the "conventional way" with a motor belt and pulleys that will host I think something like a 149-190kv motor and then just need to figure out the cogs/gears ratio.. Just to see if I understand, for a 2:1 ratio, one cog is twice the diameter of the other?
and from 149kv will drop it to 74.5kv?

Thanks for the helpful info
```

---
## \#16 Posted by: evoheyax Posted at: 2016-10-02T19:53:27.918Z Reads: 80

```
You need half the teeth. So 11 to 22 teeth would half.
```

---
## \#17 Posted by: pengy Posted at: 2016-10-02T22:15:26.251Z Reads: 81

```
Cool.
I found this:
diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/

But the amp seems a bit low (50 amp continues)
```

---
## \#18 Posted by: Jinra Posted at: 2016-10-02T22:18:22.092Z Reads: 83

```
You'll never pull 50a continuous. The VESC is arguably the most popular ESC on this forum and a recommended choice :) @RunPlayBack runs a single carvon with the VESC i believe
```

---
## \#19 Posted by: pengy Posted at: 2016-10-04T16:56:26.421Z Reads: 76

```
Great thank you guys. Just bought the Turnigy sk3 6374 149kv!

Which in this speed calculator site I got a scary top speed and the torque should be not bad either on a close to 3:1 ratio I entered. I also put 90% efficiency, have no idea what it means but i'm assuming I won't get a 100%
<img src="/uploads/db1493/original/3X/e/a/ea1167b57069851c7b9ea1c5e9a7f35fb536c742.jpg" width="690" height="387">

Is this a good ratio? 10 and 28 teeth pulleys?
Plan to ride mostly on flat surfaces I think no more than 16mph and want to put the emphasis more on the range.
```

---
## \#20 Posted by: Jinra Posted at: 2016-10-04T17:24:14.420Z Reads: 69

```
the ratio is good, but the teeth count on the motor pulley is too small. You'll probably get a lot of belt skipping. Try to stay 14+ teeth. You can go 40/14.
```

---
