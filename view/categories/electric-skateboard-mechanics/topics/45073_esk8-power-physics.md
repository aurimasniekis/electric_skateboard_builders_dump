# Esk8 Power Physics

### Replies: 52 Views: 1870

## \#1 Posted by: ZackoryCramer Posted at: 2018-01-30T20:05:59.190Z Reads: 273

```
**Here is the original post:**

I am taking my lonely lunch time at school to write this so take it seriously.
I’ve labeled the givens and conclusions by number so we can accurately dispute the problem. If you have complaints about how I skate, put them here.

Given:
(1) P=F*V=T(torque)/t(seconds)
(2) The faster you go, the more more friction/frictional torque
(3) The power into the motor will always increase the faster you go.

Conclusion:
(4) A motor set to a high gear ratio (20/36) will max out its power input somewhere if it doesn’t reach max speed.

Thanks for reading, have a great day. :grinning:

**Here's my after comment**

My friend told me that not only is there a limit to the power, but the torque is also diminishing as rpm increases, therefore, bottle-necking power output. 

Hope this helps anyone in understanding power and torque limitation of DC motors. And of course...
Thanks for reading and have a great day. :grinning:
```

---
## \#2 Posted by: FredrikHems Posted at: 2018-01-30T20:22:44.560Z Reads: 246

```
Uhm.. Am I the only one that didnt understood a shit of this?
```

---
## \#3 Posted by: Mikenopolis Posted at: 2018-01-30T23:20:08.502Z Reads: 220

```
these new "kids" make the oddest posts and comments. Stuff like this is what make @GrecoMan repectable
```

---
## \#4 Posted by: ZackoryCramer Posted at: 2018-01-30T23:34:13.958Z Reads: 214

```
Bro I was just trying to get an answer as to why I was wrong.
```

---
## \#5 Posted by: JLabs Posted at: 2018-01-30T23:34:39.886Z Reads: 208

```
So then what’s the question?
```

---
## \#6 Posted by: ZackoryCramer Posted at: 2018-01-30T23:38:40.176Z Reads: 193

```
It was in the edit. Can you not see it?
I was confused as to why you can't max out power with a high gear ratio, then someone told me that the motor will lose torque as RPM increase bottlenecking the power output at high speeds. Was that stupid?
```

---
## \#7 Posted by: scepterr Posted at: 2018-01-30T23:41:24.011Z Reads: 186

```
On 13s2p with 20/36 gearing 90mm? wheels you won't be able to use the most power
```

---
## \#8 Posted by: ZackoryCramer Posted at: 2018-01-30T23:45:29.495Z Reads: 186

```
I thought so since 45mph requires a lot more torque than starting up. Is there like a graph or datasheet demonstrating the torque/power over RPM/volts, I just want to be able to use as much power as possible. Is 16/36 the way to go?
```

---
## \#9 Posted by: scepterr Posted at: 2018-01-30T23:46:40.227Z Reads: 182

```
I think there are charts somewhere here, yes you'll deff get more power out of 15-16/36
```

---
## \#10 Posted by: ZackoryCramer Posted at: 2018-01-30T23:48:51.732Z Reads: 180

```
Does efficiency decrease for lower KV motors? I heard people say hub motors are inefficient due to their low KV.
```

---
## \#11 Posted by: JLabs Posted at: 2018-01-30T23:51:27.515Z Reads: 176

```
[quote="ZackoryCramer, post:6, topic:45073"]
It was in the edit. Can you not see it?
[/quote]

![image|281x500](upload://xW06gz1dEzuP411Yyym7vz7LSE9.jpg)
```

---
## \#12 Posted by: ZackoryCramer Posted at: 2018-01-30T23:52:00.135Z Reads: 167

```
Click on the red pencil. Maybe it only works on pc.
```

---
## \#13 Posted by: Mikenopolis Posted at: 2018-01-30T23:57:59.073Z Reads: 168

```
we can see it...the point is that you withdrew the comment/question. Just go and post it back up so it appears up top
```

---
## \#14 Posted by: barajabali Posted at: 2018-01-31T00:00:58.261Z Reads: 168

```
Reverted. If you want this topic gone let me know
```

---
## \#15 Posted by: ZackoryCramer Posted at: 2018-01-31T00:06:08.332Z Reads: 171

```
Thanks but no thanks.
@Mikenopolis yea I just realized after failing to delete this post. But I'll keep it for others.
```

---
## \#16 Posted by: Mathias Posted at: 2018-01-31T02:15:13.204Z Reads: 167

```
The language is a bit cryptic and Torque / s is not a physically meaningful quantity. But if I understand correctly what you wanted to say, then you are right: The faster you go, the more power and torque you need (duh). You can use the usual calculators to estimate if what motor specs you need for your case:
http://vesc-project.com/calculators

But I don't really understand how you connect it to gear reduction. The way it actually connects: if you are not limited by specs of your components, the gear ratio doesn't matter for your example (speaking from physics point of view) because the motor will get you the same acceleration at a higher torque. The output power is the same, though, because the motors rpm is lower: 

P = F * v = T_wheel * w_wheel  (T is toque, w is angular velocity)
T_wheel = 1/R * T_motor (R is gear reduction)
w_wheel = R * w_motor 
so:
P = F * v 
= T_wheel * w_wheel 
=  T_motor / R * w_motor * R 
= T_motor * w_motor

As you see the power is constant and the gear reduction cancels out. But in reality that's not what matters, because what you didn't include in your calculation is that the motor efficiency is lower at low rpm and low toque load. That's why a high gear reduction is more efficient, and means that the INPUT power goes up. But it has nothing to do with friction. Just motor efficiency. So get the highest possible gear reduction / lowest KV that can give you your desired max speed. Then you are most efficient. 

[quote="ZackoryCramer, post:10, topic:45073, full:true"]
Does efficiency decrease for lower KV motors? I heard people say hub motors are inefficient due to their low KV.
[/quote]
No, the opposite. Hub motors are usually inefficient because their KV is **too high**. They are usually "geared", to run at 60+ km/h, because you can only get so much copper into a motor of a certain size, which provides a lower limit for the KV. This is the reason why you want to have a gear reduction for a BLDC motor in the first place.
If you run the hub motors at sufficiently low torque load (large motors, many motors, not too many hills or aggressive acceleration, ...) the overall efficiency of a hub setup can even be higher, because they make up for lower motor efficiency with their lower rolling friction (no belts).
```

---
## \#17 Posted by: ZackoryCramer Posted at: 2018-01-31T02:28:07.769Z Reads: 146

```
[quote="Mathias, post:16, topic:45073"]
motor efficiency is lower at low rpm and low toque load
[/quote]
What! I get 8w/mi efficiency when I go 5mph and only 20w/mi when 25+mph. I don't know about the motor your using, but I too thought the same, lower the speed, the less efficient. My experience proves that the slower you go, the more efficient. Did you ever test this yourself? 

[quote="Mathias, post:16, topic:45073"]
They are usually “geared”, to run at 60+ km/h
[/quote]
And for most hub motors, I think they are geared at only 48kmph. 60~70kv. kv * 60 * voltage * pi * wheel dia./1000 <- isn't that how you calculate kmph?
```

---
## \#18 Posted by: b264 Posted at: 2018-01-31T02:45:22.544Z Reads: 138

```
"motor efficiency" is not the same as "total efficiency"
```

---
## \#19 Posted by: Pedrodemio Posted at: 2018-01-31T02:47:41.628Z Reads: 137

```
In this case you are comparing different motors. If the amount of cooper on a motor is the same, the ratings are the same, be it torque, power, loses, efficiency ,etc, but they happen at different voltage/current for a given Kv

The case for why hub motors generally are less efficient is because the Kv is not optimal for a given voltage, if you get a hub motor of 300 Kv vs the same motor wound at 300 Kv but with a 3:1 gearing, the hub motor will need more current to achieve the same torque since Kt = 60/(2*pi*Kv)

That leads us to the losses, power is P = U I^2, but since we need 3 times the current we have 9 times more cooper loses 

But if we match a hub motor Kv to the voltage and desired top speed, we have no reason to say it is less efficient, in fact it can be more since the only mechanical losses is a pair of bearings
```

---
## \#20 Posted by: Mathias Posted at: 2018-01-31T02:50:56.449Z Reads: 131

```
[quote="ZackoryCramer, post:17, topic:45073"]
What! I get 8w/mi efficiency when I go 5mph and only 20w/mi when 25+mph. I don’t know about the motor your using, but I too thought the same, lower the speed, the less efficient. My experience proves that the slower you go, the more efficient. Did you ever test this yourself?
[/quote]

This is not what I or @ZackoryCramer were talking about. This if about the power/torque needed at a certain, fixed speed. Meaning doing the exact same riding with a different setup. About the **motor efficency**.
The overall energy/distance that you are talking about should be independent of speed for low speeds and quadratic with speed at high speeds when the wind resistance kicks in.
```

---
## \#21 Posted by: ZackoryCramer Posted at: 2018-01-31T03:03:35.796Z Reads: 115

```
How much difference is there between motor efficiency and total efficiency? 12wh/mi (sorry, I forgot the 'h' in "w/mi in the previous post") is a lot of energy to be lost. So does that energy all go to heat in the battery, vesc, and pulley?
```

---
## \#22 Posted by: Mathias Posted at: 2018-01-31T03:16:16.705Z Reads: 111

```
They are not even the same type of physical quantity, so you cannot answer "how much the difference is". Motor efficiency is the ratio between output and input power. In a good setup the motor efficiency should be >80%. The wh-milage depends not only on your speed, but also on your weight, your body dimensions, on the cloths you are wearing, the way you stand on your board... 

[quote="ZackoryCramer, post:21, topic:45073"]
So does that energy all go to heat in the battery, vesc, and pulley?
[/quote]
No. The motor efficiency (or lack of it) heats your motor alone. The VESC efficiency your VESC, etc... As overall electronics efficiency should be high, ~80% is the portion of your energy that's used to set you into motion (kinetic energy). And that's the portion that heats mechanical parts and the street (friction), but most of it is lost setting air into motion, and slightly "heating" you (air friction). Minus the part that you manage to recover with regenerative braking.
```

---
## \#23 Posted by: ZackoryCramer Posted at: 2018-01-31T03:23:59.727Z Reads: 98

```
Sure, but do you really get less efficiency going slower? My record was 5wh/mi going 2mph walking speed, and 26wh/mi at 30mph(standing).
```

---
## \#24 Posted by: b264 Posted at: 2018-01-31T03:38:20.145Z Reads: 98

```
Your battery will last more miles if you accelerate slower and keep lower top-speeds when under power.  You'll have to take physics classes and science classes to answer most of that, it's beyond the scope of a reply here.

The basics: don't use hub motors, stand, more cells goes further, figure around 18Wh/mi
```

---
## \#25 Posted by: ZackoryCramer Posted at: 2018-01-31T03:40:16.389Z Reads: 97

```
I knew that. I just wanted to know why @Mathias said

[quote="Mathias, post:16, topic:45073"]
motor efficiency is lower at low rpm and low toque load.
[/quote]

I don't trust hubs. I stand mostly when I just feel like cruising. I use 15Wh/mi as my standard. I am 110lb BTW
```

---
## \#26 Posted by: b264 Posted at: 2018-01-31T03:41:55.414Z Reads: 95

```
Because the number of magnetic poles in the motor is not infinite.  There are discrete steps, and the highest efficiency is when you aren't trying to dump a lot of power into it when it's between poles.  Spinning it faster allows you to put the power into it where it matters the most
```

---
## \#27 Posted by: ZackoryCramer Posted at: 2018-01-31T03:44:37.801Z Reads: 99

```
Wait. Are you saying that going 3mph on 190kv is fast enough to not "dump power between" poles, but fast enough to put the power into it where it matters? At what speeds are you talking "slow" and "fast?"
```

---
## \#28 Posted by: b264 Posted at: 2018-01-31T03:45:57.781Z Reads: 99

```
No; I didn't give any speeds or numbers, I'm just saying that at higher RPM, that's why.
```

---
## \#29 Posted by: ZackoryCramer Posted at: 2018-01-31T03:47:45.416Z Reads: 97

```
I am just going to stick with my experience that slower you go without the motor jittering is better the efficiency. :stuck_out_tongue:
```

---
## \#30 Posted by: b264 Posted at: 2018-01-31T03:48:51.466Z Reads: 93

```
I agree with you, but it's not because of the efficiency the motor is running at
```

---
## \#31 Posted by: Pedrodemio Posted at: 2018-01-31T03:52:59.602Z Reads: 89

```
When you go slow, low rpm, the motor efficiency is pretty low, since wind resistance is insignificant you only have rolling and frictional loses, which are also low, this way even a low efficiency you need very little power to move. You being efficient to move? Yes, but that doesn’t mean that you are using the energy efficiently
```

---
## \#32 Posted by: ZackoryCramer Posted at: 2018-01-31T03:55:20.501Z Reads: 90

```
So you're saying although you are inefficient at low speeds, you eliminated a lot of other factors such as wind and friction that would overpower the efficiency you gain at faster speeds?
```

---
## \#33 Posted by: Pedrodemio Posted at: 2018-01-31T04:05:25.699Z Reads: 94

```
Exactly, you need more power to go fast, let’s say you need 50 mechanical watts to go 3 mph, if your global efficiency, accounting loses in the motor, transmission and all the electrical system is 50% you need 100 electrical watts out of the battery

But at 20 mph you would need about 300 electrical watts, if your system is operating at the sweet spot at this speed, you could get 85% global efficiency and need 350 electrical watts out of the battery

Way more efficiency but not more economic, to find the sweet spot of your build you have to do exactly what you did, to consistent run at the same route without wind and different speeds and see where you get better consumption, if you wanna find at what speed you are more efficient you need another criteria, if I’m not mistaken Wh/((Km^2)/h) and see what speed gets a lower number
```

---
## \#34 Posted by: wafflejock Posted at: 2018-01-31T04:07:17.458Z Reads: 89

```
http://www.dtic.mil/get-tr-doc/pdf?AD=ADA577582

^ some charts showing efficiency of various motors

can see some of my anecdotal data here too:

https://metr.at/r/hmtOO
```

---
## \#35 Posted by: ZackoryCramer Posted at: 2018-01-31T04:07:26.441Z Reads: 90

```
My most efficient is 5wh/mile at 2mph. What's your's?
```

---
## \#36 Posted by: Pedrodemio Posted at: 2018-01-31T04:08:55.458Z Reads: 86

```
I never tried to measure, maybe in the future, where I live is hard to get a day with no wind or a consistent wind, but should be very low also
```

---
## \#37 Posted by: wafflejock Posted at: 2018-01-31T04:09:44.957Z Reads: 84

```
I'm most efficient when going down a hill and only apply regenerative brakes I'm not sure how fast I was going but my efficiency was through the roof :)  Point is it all depends on all the factors/variables/friction forces etc. at play not even counting batteries speed controller configuration details, motor etc.  Also depends what length of trip you are measuring.  Numbers can easily lie if you sample the right part of the data.
```

---
## \#38 Posted by: ZackoryCramer Posted at: 2018-01-31T04:11:38.536Z Reads: 90

```
Well, I assumed that we are talking about flat bike lane. no wind. The electronics should be consistent. How does trip length come into play?
```

---
## \#39 Posted by: wafflejock Posted at: 2018-01-31T04:12:26.224Z Reads: 91

```
I meant more in terms of altitude changes than length but as you ride for longer you are also adding more heat to the electronics system overall and things are running less efficient when hot for the most part.  My point is if you want to know about motor efficiency you need to isolate the motor.

Direct motor efficiency tests are in the document linked above but can search for ones with motors closer to what you're using or maybe find some third party tests of the exact motor you have.

---

If you are talking in terms of overall efficiency though which I think is what matters to most people then can check out data other people have obtained from their rides and different setups http://esk8race.com/
```

---
## \#40 Posted by: Pedrodemio Posted at: 2018-01-31T04:17:17.454Z Reads: 87

```
That’s where guessing gets trick, the things that could change with trip length 
- the motor gets warmer so the resistance decreases a little
- the internal resistance of the battery gets lower as it heats up so less losses here, but as the battery gets near the end the internal resistance climbs sharply so loses and gains here
- the oil in bearings gets less viscous lowering losses
- the belt gets hotter and more flexible resulting in less losses

But all these factors are so small and/or unpredictable that one would go crazy trying to figure all out, only with a very controled environment ( dynamometer inside a lab) you could isolate and measure each one. A gust of wind that hits you would make far more difference
```

---
## \#41 Posted by: Hummie Posted at: 2018-01-31T04:22:33.640Z Reads: 82

```
http://www.ebikes.ca/tools/simulator.html/

this is a full system efficiency calculator but pretty accurate for just the motor.  

the esc is more efficient at higher speeds as well as the motor.

heat increases motor electrical resistance
```

---
## \#42 Posted by: ZackoryCramer Posted at: 2018-01-31T04:23:39.177Z Reads: 82

```
Seems legit.
```

---
## \#43 Posted by: Mathias Posted at: 2018-01-31T06:14:02.461Z Reads: 82

```
[quote="ZackoryCramer, post:23, topic:45073, full:true"]
Sure, but do you really get less efficiency going slower? My record was 5wh/mi going 2mph walking speed, and 26wh/mi at 30mph(standing).
[/quote]

That's the opposite of what I said. 
Again: motor efficiency is **not** Wh-milage. 

[quote="Mathias, post:20, topic:45073"]
The overall energy/distance that you are talking about should be independent of speed for low speeds and quadratic with speed at high speeds when the wind resistance kicks in.
[/quote]
```

---
## \#44 Posted by: ZackoryCramer Posted at: 2018-01-31T06:51:40.364Z Reads: 74

```
Hey I just had a revelation. This whole time when I was talking about efficiency, I meant wh/mi when it reality it's just mechanical power out/electrical power in. Sorry for confusing everyone. I guess I meant range efficiency this whole time. I came from the drone world where we only talk efficiency as G/W in more practical units. Sorry!
```

---
## \#45 Posted by: SimosMCmuffin Posted at: 2018-01-31T06:52:02.371Z Reads: 77

```
I have also done some practical tests on how speed affects the power use and documented the results in my topic:
http://www.electric-skateboard.builders/t/speed-vs-range-practical-test-results/21015

I have then done some analysis and theory behind the operation.
```

---
## \#46 Posted by: pixelsilva Posted at: 2018-01-31T11:32:01.176Z Reads: 74

```
...I was lost since the first reply

> Uhm… Am I the only one that didnt understood a shit of this?

https://media.giphy.com/media/Rt23MIHkCJwdy/giphy.gif
```

---
## \#47 Posted by: SimosMCmuffin Posted at: 2018-01-31T12:12:06.291Z Reads: 74

```
[quote="Pedrodemio, post:40, topic:45073"]
the motor gets warmer so the resistance decreases a little
[/quote]

Doesn't the resistance increase, as the copper windings in the motor heat up?
```

---
## \#48 Posted by: Pedrodemio Posted at: 2018-01-31T12:33:20.204Z Reads: 75

```
Yeah, my mistake, sorry
```

---
## \#49 Posted by: longhairedboy Posted at: 2018-01-31T17:59:16.361Z Reads: 69

```
if you want to go 44mph you're going to need @Battosaii 's setup. It got my 130 pound son up to that speed without much issue at all.
```

---
## \#50 Posted by: Battosaii Posted at: 2018-01-31T18:35:58.440Z Reads: 68

```
16/33 gears 
107mm wheels 
Dual 6374 motors
12s4p battery 

Pretty much all you need 

Focbox is optional but recommended.
```

---
## \#54 Posted by: GrecoMan Posted at: 2018-03-05T12:24:56.039Z Reads: 55

```
but what if he’s right? 🤣
```

---
## \#55 Posted by: Sebike Posted at: 2018-03-05T12:50:37.790Z Reads: 52

```
Yes, I flagged the posts. That type of language doesn't belong here.
```

---
