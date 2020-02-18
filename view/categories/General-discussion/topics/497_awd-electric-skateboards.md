# AWD Electric Skateboards?

### Replies: 28 Views: 4744

## \#1 Posted by: claudiofiore88 Posted at: 2015-11-16T20:33:23.984Z Reads: 210

```
Has anyone here done an AWD (All Wheel Drive) setup?  An AWD setup is pretty intriguing to me being a 265 lbs+ (120 kg+) rider.  Although a setup like that would be awesome and probably allow me to go up any hill, it would most likely be a very expensive build and be quite heavy.  I'm guessing more than 20 lbs (9 kg) depending on wether you're using 50 or 63 mm motors.  There is a DR Kit with motors from a company in China called Benchwheel selling for $300 on Amazon as mentioned by @peejeixx.  I found the same ones straight from China where I could buy 2 with shipping for around $500.  The motors they come with are 5065 270 kv motors so they wouldn't have the torque of 63mm motors, so an AWD setup would be needed (I would think anyway).

http://world.taobao.com/item/45114305342.htm
```

---
## \#2 Posted by: lowGuido Posted at: 2015-11-16T20:47:28.405Z Reads: 207

```
the thought has crossed my mind a few times. but the thing that always holds me back is cost effectiveness.
4 times as much as a single motor board, or twice as much as a dual. I don't think that the gain is worth the cost.
(unless you REALLY need that extra torque)
```

---
## \#3 Posted by: monkey32 Posted at: 2015-11-16T21:01:08.480Z Reads: 200

```
Even for a bigger dude 2x 63 or even 2x 50's is enough. Maybe sl33py can weigh in here but i'm pretty sure with the right gearing, power source and (V)ESC there really isnt a need if you want a board that can get you up to speed. Thats not to say we all wouldnt love to see new crazy frankenstein-esque monster with 4 motors :smiley: .....i think someone is doing this currently with hub motors
```

---
## \#4 Posted by: claudiofiore88 Posted at: 2015-11-16T21:58:25.686Z Reads: 193

```
@lowGuido With the said kits, it would cost a little more than $1000 with 4 VESC's from @chaka or even less with rc car escs i think.  I guess it'd be more bragging rights than practicality.  The said kits run a 4 to 1 ratio, so that's quite a reduction at least compared to @onloop's kits which have about a 2.5 to 1 reduction.  I'm mainly worried about startup torque and the ability to stop quickly.  I know the VESC shouldn't have a problem with the startup torque from what I've read here, but I worry about stopping.  I've only had experience with with a single 213kv motor 8s setup with a HK 150a esc.
```

---
## \#5 Posted by: lowGuido Posted at: 2015-11-16T23:18:29.043Z Reads: 186

```
@claudiofiore88 by all means, do it. 
if for no other reason, do it for science. (I mean that's the only reason I would do it because I certainly don't need extra torque)
also don't forget to at least double your batteries so you can get some range out of it too.
```

---
## \#6 Posted by: claudiofiore88 Posted at: 2015-11-16T23:45:38.533Z Reads: 178

```
I have two 4s 10000 mah batteries, so I'm not too worried about distance, but I'm not sure what the average draw would be using 4 motors.  They're 1800 watts motors.  It there a way to calculate the potential range with multiple motors?  I know @torqueboards has a formula, but I'm not sure how to apply that to this situation.
```

---
## \#7 Posted by: cmatson Posted at: 2015-11-16T23:56:19.967Z Reads: 170

```
I say go for it! roughly speaking, it seems to be around 1,000mah on 6s gives you one mile for a dual setup...

so I'd guess around 1,750mah per mile for your setup: it's higher voltage, so you can have less mah's and go the same distance as a 6s equivalent battery, with the downside being the drain of 4 motors. The bigger thing in my opinion would be whether or not your 4s batteries an handle the type of discharge needed for 4 motors... I don't think 30c would cut it.
```

---
## \#8 Posted by: claudiofiore88 Posted at: 2015-11-17T00:25:17.875Z Reads: 169

```
That is a good point.  I hadn't even considered that.  I have the 4s 10000 mah Multistar 10c lipos.  At 100 amps continuous and 200 amps peak, they're probably more suited for a single or double motor setup.
```

---
## \#9 Posted by: lowGuido Posted at: 2015-11-17T00:28:30.278Z Reads: 167

```
or add more caps to it.
```

---
## \#10 Posted by: claudiofiore88 Posted at: 2015-11-17T00:39:40.703Z Reads: 171

```
What is the advantage of adding more caps or larger caps?
```

---
## \#11 Posted by: cmatson Posted at: 2015-11-17T00:53:38.979Z Reads: 176

```
ya, at 10c I bet they woud puff on the first ride... I would bet you'd need a minimum of 40c constant to keep the Lipo's from puffing.
```

---
## \#12 Posted by: onloop Posted at: 2015-11-17T01:16:25.372Z Reads: 182

```
Eventually, I will make one, it will have hub motors and 4 vesc, however, the cost of VESC needs to come down to make it feasible. I think 4WD hubs can equal the performance of a Dual satellite configuration.

There are a few ways to make the vesc cheaper, but the best way is through economy of scale. When I can order in 1000's qty I think it will be much cheaper. other things such as minimizing the assembly time can also help.

also, your 10C battery is probably ok, 100AMP is plenty. I really think that people over-estimate the amount of current required to get a board to perform well.

the beauty of the vesc is it can intelligently control the current to ensure it is always working within the limitations of the battery.

Do I think anyone needs a 4wd eboard? NO, with current hub motor tech it will be heavy and won't really achieve much more than a good DR satellite system. If it does happen the idea would be to use 4 smaller motors - 50mm or maybe 42mm equivalent 

I think you can design a 2wd system that can easily handle your size.
I would suggest a Dual Diagonal setup running the new 6374 R-SPEC motors - combined with the new 12mm wide belts that are soon to be available.

the torque transfer capabilities of a drive train using 12mm belt are 33% greater than the equivalent 9mm belt system.

this means your brake force is dramatically improved, combined that with the ridiculously oversized motors and you will have a true tank of an eboard!

if you go to 3mm pitch pulley at 15mm wide (or use an idler pulley on 5mm pitch to engage more teeth around a small motor pulley.) you could also get much more reduction, maybe reduce it down to have a 30km/h top speed. you can probably pull some cars with it.
```

---
## \#13 Posted by: claudiofiore88 Posted at: 2015-11-17T05:00:37.632Z Reads: 165

```
A DD setup would be really cool with the 6374 R-Spec motors, but you mentioned they'd be quite expensive.  I believe you stated somewhere on here that they're 1.5 times as expensive as the current R-Spec motors which would be around 170 US Dollars, or have you set a price yet?  Either way, I'm gonna have to wait 'til funds become available.
```

---
## \#14 Posted by: onloop Posted at: 2015-11-17T07:07:20.230Z Reads: 156

```
yeah, it would be ridiculously expensive...

the performance to cost ratio? what are you willing to sacrifice? save some coin or haul some ass? ;)

Actually, those 6374 motors are intended to be for people who just want to build single drive boards.
```

---
## \#15 Posted by: chaka Posted at: 2015-11-17T14:45:34.855Z Reads: 147

```
Theoretically speaking we could run 4 motors at 3s and have the same current draw per motor as a single motor on 12s. It would be interesting to test this in the real world with some 800kv motors and see how it performs. I might give it a try, the motors are cheap enough, under $25 each.
```

---
## \#16 Posted by: jeroenimo Posted at: 2015-11-17T15:19:48.482Z Reads: 140

```
Hmmm, well I am about to fit 2 of these 6374 bad boys on my board.. what does that make me?
```

---
## \#17 Posted by: torqueboards Posted at: 2015-11-17T16:15:50.547Z Reads: 152

```
You don't need a 4WD, IMHO. Dual motor with a higher KV will give you more power then you need. 4WD is really just overkill and bragging rights. Not that you can't make one.. The board will be way over 20 lbs. IMO not worth the cost.

The lower KV IMO is not worth it.. 230-265KV is perfect and gives you the most amount of power.

I had a friend ride my old dual motor 280KV on 6S with 1:3 gearing. He's about 230lbs which is only about 35 lbs away from 265 lbs. He was climbing up 18%-20% inclines with no issues. He was actually surprised.

I think everyone has this idea that low KV is more torque.. If you simply swapped your motor from your 213KV to a 260KV and kept your 2.5 to 1 reduction. You'd get much more hill climbing power. You might not even need to do anything.

I have a customer close by my area who's running a single 260KV and he's on 10S but it climbs him up pretty much everything. He tried a 192kv and he couldn't even get up a hill. He's also about 240-265 lbs.

Try it.... No need to go 4wd :) I've been wanting to make one but it's just complete overkill and just bragging rights. Your also not bragging when you have to hold that 24 lb board.

Summary - LOW KV sucks..better off HIGHER KV (under 300-280KV) and adjust through gearing ratios. If you really want more "torque" which doesn't equal out to anything special. 230-260KV IMO is ideal..

If you have 2x 230-260KV motors.. You'll be flying..
```

---
## \#18 Posted by: chaka Posted at: 2015-11-17T17:15:12.024Z Reads: 142

```
You really dont want above 200kv with the VESC when running 12s.  I use 192kv motors and a single will get me up a 15% grade no problem at all. I think a lot off people don't understand that kv and power are not related. It really depends on how much copper by weight is used in the motor.

Check for yourself and see that the most powerful motors in a given size will be the heaviest. The only reason low kv motors tend to be higher output is due to the windings being smaller diameter and therefore having less empty space/more copper mass vs  the higher kv motors in the same class.

A far more likely cause of your friends poor hill climbing performance would be the batteries used. The sk3 192 kv motor will draw a huge amount of power if you try hard enough. If the pack can't keep up with the demand it will drop in voltage significantly. Motors with less copper will draw less amperage allowing the battery to keep chugging along leading us to believe the motor is more powerful.

Personally I would like an AWD off road board with 192kv's and a pack large enough to ride all day. Something with enough power to mix it up with motorcycles. Sure it will be heavy, it would be a specialized board and definitely not a campus cruiser. Just like a Honda R1000 weighs close to 500lbs while the typical moped weighs well under 200lbs.
```

---
## \#19 Posted by: torqueboards Posted at: 2015-11-17T18:39:41.239Z Reads: 133

```
I'm not talking about a 15% incline... 15% inclines are easy.. I'm talking about 20-28% incline. I know that the weight of the copper is what matters per the given motor.

I just don't see any benefit in a lower KV. If you want to lower the top speed go with a higher KV motor and change it through the gearing. Of course, higher KV can be too high as well. A balance in the middle is best.
```

---
## \#20 Posted by: claudiofiore88 Posted at: 2015-11-17T19:22:21.639Z Reads: 132

```
So just to clarify, a higher mass of copper windings results in a higher torque motor, not lower kv?  Does that mean I should focus on the watts rating and weight of the motor, not the lower kv?
```

---
## \#21 Posted by: longhairedboy Posted at: 2015-11-17T19:34:44.617Z Reads: 137

```
lower kv motors use thinner wire and more windings to achieve more torque at higher voltages but at a lower top speed, a side effect of which is less energy wasted as heat.

higher kv motors use thicker wire and fewer windings to achieve less torque at lower voltages but at a higher top speed, and because of the increased current/lower voltage traveling through thicker wire you end up with a bit more heat. 

This is why there is a balancing act that has to happen between the desired voltage of your system (6S, 8S, 10S, 12S) and your desired motors (~270kv,~245kv,~210kv,~190kv)

beyond that you also have to consider pulley ratios and wheel height. In my personal opinion the voltage should determine the motor kv and your body weight should determine your pulley ratio and wheel size as well as your voltage.
```

---
## \#22 Posted by: claudiofiore88 Posted at: 2015-11-17T19:52:19.156Z Reads: 141

```
You mean lower kv motors achieve more torque at lower voltages with a lower top speed, or am I mistaken?
```

---
## \#23 Posted by: longhairedboy Posted at: 2015-11-17T20:04:10.489Z Reads: 152

```
it seems counter intuitive but the way i wrote it is correct. On a 6S system running a 270kv motor will give you a higher top speed than a 245kv motor if the pulley ratios are the same. I have tested this in the real world, its not just math. On a 14/36 ratio the highest i ever got on my set of R-SPEC 245s was 27mph. I topped that with a set of NTM Propdrive 270s at 31mph and everything else was the same on the board. 

The same is true at 12S. If you run 170s you're not going to get the same top end as you will on 190s or 210s. The thing about 12S though is that you have tons more torque so you just swap torque back for top end in the pulley ratio or in the wheel height or both.
```

---
## \#25 Posted by: Sirshaunsta Posted at: 2017-12-21T22:57:25.509Z Reads: 74

```
To your original post, I am a 155lb rider, but I went with the best setup I could build, I'm sure if you have some coin to spend you can assemble 4 190kv motors at a 16/40 ratio they should be able to pull you and make it up hills in excess of 25 kmph
```

---
## \#26 Posted by: squishy654 Posted at: 2017-12-21T23:05:14.656Z Reads: 71

```
Kv literally means "rotations per volt", overall power of the motor is rated in watts, the gear its in or how that power is applied, is written in revolutions per volt (kv)..
```

---
## \#27 Posted by: Cobber Posted at: 2017-12-21T23:46:43.470Z Reads: 65

```
@Sirshaunsta @squishy654 you guys are replying to a dead 2 year old topic to a member who hasn't been active for over a year...  

<img src="/uploads/db1493/original/3X/0/8/082dfd919f76e4ccd2025b7e9619c7e4f79edd3d.png" width="690" height="387">

might be waiting a while for a reply ;)
```

---
## \#28 Posted by: Sirshaunsta Posted at: 2017-12-21T23:47:56.344Z Reads: 63

```
Ty I didn't check first
```

---
## \#29 Posted by: squishy654 Posted at: 2017-12-22T00:06:28.837Z Reads: 57

```
I noticed, and I replied for the audience..
```

---
