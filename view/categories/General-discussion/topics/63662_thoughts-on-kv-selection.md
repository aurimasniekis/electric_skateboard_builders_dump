# Thoughts on Kv selection

### Replies: 37 Views: 649

## \#1 Posted by: Jmding Posted at: 2018-08-02T23:38:10.363Z Reads: 204

```
Motor Kv selection seems to be  a common question, and after lots of lurking I think I might have it generally figured out. Hopefully, I'm not wrong on the subject and maybe this thread will be worth adding to the stickied guide list. 

When you design your board, you generally have a top speed in mind, and will pick your motor, gear ratio, and wheel size to hit that target. So basically the question "what Kv should I pick" really boils down to
1) should I pick a high Kv motor and gear it up/use small wheels or
2) should I pick a low Kv motor and gear it down/use larger wheels 

The confusion comes from the fact that Kv is essentially constant/Kt, i.e. a high Kv motor will have a low Kt torque constant. Now some people think that this means high Kv motors have less torque than their low Kv siblings, but this is not the case, because the effect is exactly offset by the changes in gear ratio that you will make in order to achieve the same top speed.

Let's try a real world example, let's say 50 kmph top speed target, with a 10s LiPo:
Configuration 1: a 200 Kv motor at 36 V turns a 7200 rpm. Assuming 83mm wheels, that's 36V *200rpm/V *3.14 *83mm *60min/hr *1km/1000m *1m/1000mm = 112 kmph with no gearing. To get this down to spec, we have to gear down to 2.24:1. Now Kv 200 rpm/V *2*3.14radians/rotation *1min/60s = 20.93 A/N*m, or 0.04778N*m/A. Assuming the battery maxes out at 50A, the max torque at the wheel is therefore 0.048N*m/A *50A *2.241= 5.38N*m

Configuration 2:  a 300 Kv motor at 36 V turns a 10800 rpm. Assuming 83mm wheels, that's 36V *300rpm/V *3.14 *83mm *60min/hr *1km/1000m *1m/1000mm = 169 kmph with no gearing. To get this down to spec, we have to gear down to 3.38:1. Now Kv 300 rpm/V *2*3.14radians/rotation *1min/60s = 31.4 A/N*m, or 0.03185N*m/A. Assuming the battery maxes out at 50A, the max torque at the wheel is therefore 0.03185N*m/A *50A *3.38= 5.38N*m

So theoretical torque is the same regardless of what Kv we choose, because we will just pick a different gear ratio to compensate. How do we pick a motor then? Well, have you ever noticed how two sk3 6374's with lower Kv's have lower wattage ratings listed by Hobby King? I think that is because the way you actually achieve a lower Kv for a given motor housing/stator is by winding the stators with thinner and therefore longer copper wire. Long, thin wire has higher electrical resistance than short, thick wire, wasting more energy in the form of  heat losses, which not only decrease energy efficiency, but also cause increased wear on the motor.

So in short, the old adage that a low Kv/high Kt motor is good for torquey builds and bad for top speed is kind of off the mark, since your pulley gearing changes all that anyway. You should always pick the highest Kv available as long as you can find motor/wheel pulleys to support the intended top speed. 

Well... Except for the fac that the VESC (pre v6) seems to have an erpm limit of about 60k, so if your Kv is too high relative to your battery voltage, you risk damaging your speed controller. Also there's some thought that maybe needs to go into the possibly higher mechanical losses associated with a more dramatic gear ratio, maybe some weird inertial effects due to increased rotational mass of a larger wheel pulley too, I dunno, haven't hammered it out. But I bet these are minor effects, so in the end they can probably be ignored.
```

---
## \#2 Posted by: Hummie Posted at: 2018-08-03T00:43:12.916Z Reads: 174

```
as you say you can do adjustments with gears and it largely has the same effect as kv and then there's the limit of how big a pulley you can fit, and you dont want to use one smalller than 17 supposedly.    
with the lower kv you have thinner wire that gets hotter per amp but with a motor having a very high kv and very thick wire, it takes more amps to make the same torque.  the heat balances out in terms of getting the same amount of torque out.  but lower kv motors do have a lower power rating and it could be related to that or it could be the high speed and high kv motor are able to increase their speed and of course speed and torque is power.  it seems an easy win and just go faster and you have more power, but there is the other motor major loss besides copper losses, iron losses being  eddy currents and hysterisis which increase with speed.  you can design a motor for more speed but the design generally used by us probably has an ideal ratio of speed to torque that is an equal balance.  and an ideal most efficient speed to torque ratio.  not that youd want to sit at one speed all day
```

---
## \#3 Posted by: lrdesigns Posted at: 2018-08-03T00:51:46.677Z Reads: 165

```
I have had two setup ups with same size motor one 270kv and 140k geared to same top speed. 

Only change between setups was kv and gear ratio. 

Performance was similar. Hard to give a winer without data but it feels similar. 

The low kv setup is much preferable because it means I can have a larger motor pulley, this makes belts last really long. The motor pulley last much longer too. Also the wheel pulley is smaller so the pulley and belt have more ground clearance which helps them get damaged less form uneven ground or rocks.
```

---
## \#4 Posted by: Jmding Posted at: 2018-08-03T01:07:20.095Z Reads: 156

```
What pulleys do you have the low Kv motor set up with?
```

---
## \#5 Posted by: lrdesigns Posted at: 2018-08-03T01:17:57.602Z Reads: 152

```
Originally was 20/39 = 1.95:1
Later I changed to a new wheel pulley.
                    .. 18/36 = 2:1

The 270kv setup was 4:1 ratio!

I should mention I'm on 12s with 97mm wheels

I have not had a belt brake since changing to the low kv which was over a year ago.
```

---
## \#6 Posted by: Jmding Posted at: 2018-08-03T01:20:12.391Z Reads: 141

```
Did not know that belts broke that often. That's very good to know
```

---
## \#7 Posted by: Schulerbible Posted at: 2018-08-03T01:27:41.757Z Reads: 139

```
What wheels and motors are you using? Going 36T:18T with a dual 6384 setup (@170KV) on 100 mm wheels.
```

---
## \#8 Posted by: lrdesigns Posted at: 2018-08-03T01:28:41.723Z Reads: 135

```
They don't if your setup is good. If there is any slip between the belt and the pulley during hard braking it will shred belts pretty quickly. 

The small motor pulleys 12t to 15t wear out really fast, once the teeth are worn they slip and that will kill your belts. Idler pulleys can help to reduce slip also.
```

---
## \#9 Posted by: lrdesigns Posted at: 2018-08-03T01:32:23.757Z Reads: 132

```
[quote="Schulerbible, post:7, topic:63662"]
What wheels and motors are you using?
[/quote]

Racestar 5065 140kv, 97mm flywheel clones. But will upgrade to 100mm boa's soon. The racestar motors have proven very reliable even with lots of heavy rain usage. I would like bigger motors but I use the board to commute and its already so heavy to carry around.
```

---
## \#10 Posted by: Hummie Posted at: 2018-08-03T03:01:19.612Z Reads: 120

```
i know someone who uses belts on his bike and has had the same belt with for like 6 years.  is there possibly a better belt and are yours kevlar?  his latest bike has a belt with a pattern that is even new.  i dont know it on hand but i doubt motorcycles are changing their belts so often.  seems weird still no one has belts that last.  
does the belt ruin the cog or the cog the belt or what or both.
```

---
## \#11 Posted by: dareno Posted at: 2018-08-03T10:30:03.985Z Reads: 108

```
I would say yes great in theory but not really practical with street set ups.  I think the sweet spot has been found with the 200 kv mark. With larger wheels say pneumatics on a mountain board then yes you have some wiggle room pulley wise but then factor in size of the wheels......too much thinking.....

I'm drinking.
```

---
## \#12 Posted by: Silverline Posted at: 2018-08-03T10:51:30.759Z Reads: 103

```
I use Steel pulleys for the motor. It's so much stronger than the usual alu. And hold so much longer....

After 2000km on my Trampa AT, the steel pulley still looks like new, and never broke a belt yet.
```

---
## \#13 Posted by: professor_shartsis Posted at: 2018-08-03T19:52:22.970Z Reads: 93

```
[quote="Jmding, post:1, topic:63662"]
So basically the question “what Kv should I pick” really boils down to

1. should I pick a high Kv motor and gear it up/use small wheels or
2. should I pick a low Kv motor and gear it down/use larger wheels
[/quote]

Here's the comparison chart between 100kv and 1:1 ratio vs 200kv and 2:1 ratio. The electrical resistance on the 200kv is 1/4th the resistance of the 100kv assuming the same size motor and same copper volume because the 200kv winding wires are half the length and twice the cross sectional area compared to the 100kv.

The most obvious difference is the huge boost in efficiency while accelerating with the 200kv motor (green line top left chart) caused by the 75% reduction in motor heating (purple line, top middle chart). Also notable is the reduction in battery amps across the chart with 200kv (purple line, bottom right chart) for identical acceleration performance (yellow and red lines, bottom left chart)

Both charts assume 50v, 100mm tire, 60a motor amp limit, 60a battery amp limit, same size motors & copper volume.

https://image.ibb.co/gxkpae/100kv_vs_200kv_2.gif
(edit: click to enlarge)
```

---
## \#14 Posted by: Blitz Posted at: 2018-08-03T20:30:02.636Z Reads: 81

```
don't have time to read this now, But looks good! :D

Thanks @professor_shartsis
```

---
## \#15 Posted by: dareno Posted at: 2018-08-03T20:49:30.065Z Reads: 79

```
Where are my bloody glasses?
```

---
## \#16 Posted by: professor_shartsis Posted at: 2018-08-03T20:55:10.325Z Reads: 80

```
@dareno if you click it there's a bigger version.
```

---
## \#17 Posted by: dareno Posted at: 2018-08-03T20:59:21.312Z Reads: 79

```
@professor_shartsis thanks for this by the way but alas even the bigger version has me needing visual enhancement. :roll_eyes: I will find them though because this is a good resource!
```

---
## \#18 Posted by: ivanflo Posted at: 2018-09-10T05:32:11.706Z Reads: 68

```
So i guess high KV with gearing is the winner?

[quote="Jmding, post:1, topic:63662"]
erpm limit of about 60k
[/quote]
This i did not know! just started playing with my first build, better go back and correct the speed limit.
```

---
## \#19 Posted by: Jmding Posted at: 2018-09-10T05:40:55.312Z Reads: 70

```
Yeah, it's probably the way to go. I don't have a food understanding of the magnitude of things like eddy current and bearing losses, but in the absence of such knowledge, the best we seem to know is that higher kv = higher max current, and assuming you gear for the same top speed, that extra current is directly proportional to torque. So sk3 6374 200 kv with 80A current is capable of 8/7x more torque than the 150 kv, 70A version
```

---
## \#20 Posted by: BruSkater Posted at: 2018-09-10T06:27:15.670Z Reads: 70

```
What about increasing kv and reducing voltage to achieve same results? Like instead of using a 12s with 200kv we use 10s and 240kv.

What would be the difference on those setups? Would there be any differences in efficiency or torque?
```

---
## \#21 Posted by: Jmding Posted at: 2018-09-10T15:27:12.615Z Reads: 65

```
If you drop the voltage from 12s to 10s, and adjust your gearing to keep top speed constant, you lose about 1/6 of your torque. Some people will argue that your VESC will be less likely to fail at 10s though. I don't know for sure. I'm going 12s on my flipsky 6.6 driven build and will watch long term how it does.
```

---
## \#22 Posted by: Hummie Posted at: 2018-09-10T15:46:34.161Z Reads: 66

```
60,000 rpm, or maybe 60,000 erpm maybe would be the most efficient depending on the motor design and what loads are put on the motor.  

the low kv has thicker wire and can take more amps but at the same time it takes more amps to make the torque and ultimately is the same heat produced. A motors km is winding or kv/kt independent. 


10s need not be any less torque than 12s And it’s the amps that decide the torque. If u used an esc that could put out more amps Itll get more torque 
For ultimate efficiency Youd want to balance the copper losses with the iron losses but both are dependent on the situation and the torque and speed Of the vehicle.  U can reduce your copper losses with greater motor speed so less current needed with a gearbox to produce the same torque but then the iron losses hysteresis and eddy currents are increasing with the erpm so there is the limit there as these iron losses also produce heat. It would be nice to see a breakdown of the losses, whether copper or iron, and if u work with the grin motor simulator u can see a lot by comparing custom motors.  You can increase the poles there which is similar to having a gear or pulley.  There really would be an ideal rpm for a motor for maximum efficiency but how likely are u to sit at that speed? Unlikely and u need to account for acceleration and top speed and slower speeds and steep hills.  But if u wanted to set up a challenge where u wanted to get the most Mileage on a consistent maybe flat track at a consistent speed then u could tweek for that ideal speed
But at the higher erpm there is greater switching in the esc and losses there too
Really your best bet is a good aero tuck!
```

---
## \#23 Posted by: slick Posted at: 2018-09-10T16:41:24.852Z Reads: 66

```
yup...exactly what I experienced
```

---
## \#24 Posted by: Jmding Posted at: 2018-09-10T17:43:57.534Z Reads: 64

```
think you have a couple things flip-flopped

[quote="Hummie, post:22, topic:63662, full:true"]
the low kv has thicker wire and can take more amps but at the same time it takes more amps to make the torque and ultimately is the same heat produced.
[/quote]

other way around, high kv has thicker wire and can take more amps.  See the published specs for 6374 200 and 150 Kv motors.  200 Kv has 14 turns (i.e. thicker wire), 0.016 ohms winding resistance and 80A continuous current vs 18T, 0.021 ohms and 70A.
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-149kv-brushless-outrunner-motor.html
[quote="Hummie, post:22, topic:63662, full:true"]
A motors km is winding or kv/kt independent.
[/quote]

I agree that Km is independent of winding, but max current (and therefore max torque assuming you compensate for the extra speed with more gearing) is not.

[quote="Hummie, post:22, topic:63662, full:true"]
10s need not be any less torque than 12s And it’s the amps that decide the torque. If u used an esc that could put out more amps Itll get more torque
[/quote]

Keep in mind that if you run 12s, you get 20% more motor speed, which you can generally trade extra torque with gearing.  That's what I mean by "assuming you gear for the same top speed."  The amps are deciding the torque at the motor, but because you have a more aggressive gear ratio in the 12s setup, you end up with more torque at the wheel.  Since we're bumping up against the current limits on our motors, in general I think going up in voltage is always a good thing (assuming the ESC doesnt blow).


As for iron losses, yeah I really need to get around to educating myself on those, I dont even know whether (at our speeds) they are 10% or 10x as big as copper losses, but I imagine (by conservation of energy maybe? ehhh... really getting vague with my physics here :grimacing:) that they must ultimately manifest themselves as heat as well, and therefore are already reflected in the max current specs provided by the manufacturers.  Thus since the higher Kv motors are rated for more amperage, we can probably still assume that they are capable of more torque (net of gearing) despite the increase in iron losses.

I struggle to use the grin simulator because the motors we use aren't in the system, and defining custom motors is difficult because I dont know which numbers are important, and what values to use in many cases.
```

---
## \#25 Posted by: Hummie Posted at: 2018-09-10T18:03:19.274Z Reads: 59

```
O yea I flip flopped the kv and resistance as You say and more turns n resistance w the low kv but people often think u can get more amps in and more torque w the higher kv as it has fatter wire n less resistance but in equal measure it takes more amps for the torque n balances out. 



  And with 12s n gearing u can get more torque with still the same amp limit of the esc as you say

I’ll post up a comparison of efficiency of our motors using the custom motor option in the future. It can be worked to incorporate any wheel size n frontal area for wind resistance.  I’m assuming that a non-hub motor can be represented on there actually.  Hoping people will take it on too and we could get somewhere.  It’s a great tool

Don’t think the Vesc is up there..I’ll see if I can get them to put it up if not and it should be
```

---
## \#26 Posted by: Blitz Posted at: 2018-09-10T18:35:19.921Z Reads: 56

```
Oh I don't feel so good. Could you guys already give an opinion in the context of I think so?

Higher kv, lower voltage, same wattage and geared for the same speed, what do you think about that?
```

---
## \#27 Posted by: Hummie Posted at: 2018-09-10T18:39:39.337Z Reads: 55

```
With higher kv motors they need more amps to get same torque. That’s not a problem if ur esc can do higher amps and should be maybe almost as efficient , maybe depending on the esc efficiency. But with the same esc , with say a 100 amp limit, with 10s vs 12 u won’t get the speed that can then be converted by a gear to torque.  So less torque w 10s

But then again in use it could be more efficient depending on the speed ur using the motor.
```

---
## \#28 Posted by: Jmding Posted at: 2018-09-10T18:44:31.560Z Reads: 54

```
@Blitz, I dont see any good reason to not go at least 10s
```

---
## \#29 Posted by: Blitz Posted at: 2018-09-10T18:44:52.055Z Reads: 53

```
so your telling me 12s 100a is more powerful than 10s 100a?
```

---
## \#30 Posted by: Hummie Posted at: 2018-09-10T18:46:19.805Z Reads: 52

```
Yea because if u geared it to have the same top speed that 12s speed is converted to torque
```

---
## \#31 Posted by: Blitz Posted at: 2018-09-10T18:51:20.464Z Reads: 52

```


Let me rephrase so your telling me that 5040W (12s) is more powerful than 4200w (10s)? 

Or are you saying that a higher gear is worse than a higher voltage for a certain speed?

I got a motor that is 245kv and cannot be run at a high voltage due to ERMP limits.
but I can near max out its wattage with extra current.
 (lets pretend I got a focbox unity with a massive heat-sink.) 

Is that just as good as running a higher voltage? (lets also pretend that the motor doesn't heat up)
```

---
## \#32 Posted by: Hummie Posted at: 2018-09-10T18:54:49.419Z Reads: 52

```
[quote="Blitz, post:31, topic:63662, full:true"]
Let me rephrase so your telling me that 5040W (12s) is more powerful than 4200w (10s)?

Or are you saying that a higher gear is worse than a higher voltage for a certain speed?
[/quote]

Yes. 

Im saying the efficiency could be worse running 12s if ur not going faster than u were on 10s in its use
```

---
## \#33 Posted by: Hummie Posted at: 2018-09-10T19:00:24.884Z Reads: 51

```
[quote="Blitz, post:31, topic:63662"]
Is that just as good as running a higher voltage? (lets also pretend that the motor doesn’t heat up)
[/quote]

If u can put the extra amps in it will be able to put out the same torque and power as the 12s.  Maybe just as efficient too depending on how u ride ..maybe more.
```

---
## \#34 Posted by: Blitz Posted at: 2018-09-10T19:06:19.443Z Reads: 51

```
Thanks for explaining!
```

---
## \#35 Posted by: BruSkater Posted at: 2018-09-11T01:46:04.065Z Reads: 47

```
So, I was debating on whether go with 12s4p or 10s5p on a hummie deck... I guess that going with a 190kv motor with the 12s4p would be similar to a 245kv 10s5p (a little faster on the 245kv)... Would you recommend going 10s @Hummie?

Also what 6364 motor would you recommend? Sk3 or tacon 245k?
```

---
## \#36 Posted by: Jmding Posted at: 2018-09-11T03:36:02.965Z Reads: 47

```
I dont know if the quality of the Tacon is higher or lower than the SK3.  But assuming they are equivalent quality, 10s + 245 kv Tacon is the better setup there, unless you use a VESC 6 and can go above 60k erpm.
```

---
## \#37 Posted by: Hummie Posted at: 2018-09-11T04:01:59.272Z Reads: 46

```
answering your question i think it would depend on the esc and how heavy you are and what hills or power you would do.  Ive never had a temp shutdown riding around san Francisco doing laps on hills on 12s but some people have, and then putting more amps through the esc on 10s and getting it hot will decrease its life and I think be general electronics standards is being pushed beyond the usual safe margin in amps and voltage.  really we want oversized motors and oversized escs compared to the amps they can do and then its most efficient,  but what is more unsafe the voltage or the increased amps and heat..i think youre safer going with 10s for sure and pushing the motor and battery amp limits.  maybe even a cheap 4.2 from hobbyking on foc could be fine with that or maybe you still should go for the 6 to be safe.  

the tacon 245 is an awesome motor just by the looks alone.  and of the few motors ive taken apart its the only one with pressed bearings and shaft.  and the glue is very strong and thick.  the only thing I don't like are its motor leads which are just the magnet wire coming the whole way along out and to the plugs.  its stiff and easy to rub off the insulation and short.  its rare in that I think, but a super benefit is I think you could reterminate the motor to a wye.  almost all the motors for sale are wired delta termination for whatever reason, and with the magnet wire coming the full length you can find the starts and ends of each of the 3 wires and bundle either the starts or ends, soldered, and drop the kv by some math I forget.  instead of 245 my guess is....   .. 160.
```

---
