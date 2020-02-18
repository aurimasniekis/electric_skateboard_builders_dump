# Will this loop key work?

### Replies: 24 Views: 1561

## \#1 Posted by: moe_lester Posted at: 2017-03-26T12:58:33.689Z Reads: 215

```
Hey will this loop key work, im using xt90 s connector. 

<img src="/uploads/db1493/original/3X/2/c/2c03ee2cff86b44c3c1b1594b6abf901b3f6a535.jpg" width="375" height="500">
```

---
## \#2 Posted by: moe_lester Posted at: 2017-03-26T12:59:54.327Z Reads: 207

```
Because i know some people been say loop keys have been burning or not working properly, so im bit nervous about wiring it up as i might make a mistake.
```

---
## \#3 Posted by: Smorto Posted at: 2017-03-26T13:05:56.425Z Reads: 202

```
Yes, it will work.
```

---
## \#4 Posted by: moe_lester Posted at: 2017-03-26T14:18:57.852Z Reads: 187

```
thanks but will it eventually burn out, because I've read a few posts about loop keys smoking up and breaking??
```

---
## \#5 Posted by: JLabs Posted at: 2017-03-26T14:31:21.856Z Reads: 186

```
I have never had a loop key go up in smoke. As long as the solder joints are good nothing should happen. If it's a cold joint or not a good connection it will eventually wear away and cause sparks.
```

---
## \#6 Posted by: saul Posted at: 2017-03-26T14:42:12.832Z Reads: 179

```
I make mine the other way around. 
Male xt should be the passive side, the key. They're also cheaper so you can make extras..

The female with anitispark circuit is less likely to get shorted, you really have to try!!!! So that should be on the power side.
```

---
## \#7 Posted by: Smorto Posted at: 2017-03-26T14:46:12.849Z Reads: 175

```
True but very rarely would it ever get "shorted" by accident. Plus the female XT is easier to plug in. Also, even if both prongs somehow got touched, it would only complete the circuit, not a "short".
```

---
## \#8 Posted by: Smorto Posted at: 2017-03-26T14:46:44.985Z Reads: 170

```
I agree 100% with @JLabs. Nothing should happen except for a bad soldier joint or other user-error.
```

---
## \#9 Posted by: saul Posted at: 2017-03-26T14:54:06.515Z Reads: 163

```
Yes but it would complete the circuit without the spark protection. Kinda the whole point....

It's just better practice but either way works.
```

---
## \#10 Posted by: Smorto Posted at: 2017-03-26T15:10:18.409Z Reads: 148

```
Im not disagreeing with you but I'm just trying to prevent people from thinking that not using the Male XT as a key will result in smoke/fire. Like you said, either way works :slight_smile:.
```

---
## \#11 Posted by: mmaner Posted at: 2017-03-26T15:13:41.089Z Reads: 148

```
I've been using an XT90-S on my main build for months and a double kick build for a couple of weeks. I've never had a spark and both work beautifully. 

Connect the XT90-S in line with the POS wire after the battery but before everything else and you will be good.  Hundreds of people have done this with no issues.
```

---
## \#12 Posted by: moe_lester Posted at: 2017-03-26T17:30:49.839Z Reads: 129

```
great thanks
```

---
## \#13 Posted by: jmasta Posted at: 2017-03-26T18:22:49.411Z Reads: 125

```
What AWG are those wires? They look really small...
```

---
## \#14 Posted by: moe_lester Posted at: 2017-03-26T20:26:27.250Z Reads: 123

```
16awg

yh they look small, i don't know why they look bigger online
```

---
## \#15 Posted by: jmasta Posted at: 2017-03-26T20:34:39.758Z Reads: 120

```
Are those 16 AWG wires your main power lines?  If so I'd recommend using 10 AWG, or 12 AWG at least.  16 AWG is only rated to about 22A

Keep in mind these are conservative numbers, but this chart is a good guide. You can exceed these values because we are not continuously pulling high current

<img src="/uploads/db1493/original/3X/c/4/c4cc8db36722f31e5b7b94e7001dad72a13c55b9.png" width="290" height="500">
http://www.powerstream.com/Wire_Size.htm
```

---
## \#16 Posted by: moe_lester Posted at: 2017-03-26T20:45:18.231Z Reads: 106

```
ok I'm gonna change them now thanks, could I use copper core awg wires btw ?
```

---
## \#17 Posted by: jmasta Posted at: 2017-03-26T20:52:42.825Z Reads: 114

```
Yeah those will work fine. Silicone wires are usually preferred, since they are more flexible and the insulation has much higher heat capacity (won't melt during high temp soldering). But they are more expensive and not as readily available

The copper core are smaller for the same current capacity.  The wires stay in place, which can be a pro or a con depending on the situation
```

---
## \#18 Posted by: moe_lester Posted at: 2017-03-26T21:00:12.552Z Reads: 117

```
Cool great advice. 

Im also having trouble using my controller for setting up my vesc. Its PPM on the bldc tool right or is it UART?  

Anyway when i accelerate with the controller the motor literally jumps like crazy, what have i done wrong?

I connect the vesc and uploaded the right firmware, what do i change so my motor reacts normally to my acceleration? 

<img src="/uploads/db1493/original/3X/4/3/4320fdf1fb90cc60c6de67b949a55c99a4dadd62.jpg" width="374" height="500">
```

---
## \#19 Posted by: Namasaki Posted at: 2017-03-26T22:49:48.119Z Reads: 108

```
About your loop key. I can't tell if you have it before or after the charge port wire. 
You want it after the charge port wire.
```

---
## \#20 Posted by: Eboostin Posted at: 2017-03-27T03:44:47.654Z Reads: 102

```
Do you put the positive side of the loop key to the battery or the negative side? Or does it not make a difference?
```

---
## \#21 Posted by: mmaner Posted at: 2017-03-27T04:22:20.952Z Reads: 100

```
I've seen at least one person do the NEG leg, but I do the POS leg, that should prevent drain but I'm not so sure anymore.
```

---
## \#22 Posted by: Blasto Posted at: 2017-03-27T04:36:22.248Z Reads: 96

```
let me OCD a bit here.

having a powered up vesc, with no heatshrink, resting on a pair of clamps... maybe not the best idea

<img src="/uploads/db1493/original/3X/8/b/8bd65ea2027f157ce102251c41df16a2eb16bcd9.jpg" width="674" height="494">
```

---
## \#23 Posted by: wmj259 Posted at: 2017-03-27T06:01:40.772Z Reads: 86

```
Nice remote!!
```

---
## \#24 Posted by: moe_lester Posted at: 2017-03-27T07:29:23.895Z Reads: 83

```
Its got heat sink just cant see it. 

Does anyone now why my motor is going crazy when i barely accelerate through my controller....when i accelerate through the keyboard  on my laptop its fine. So does amykne nkw what i have to adjust?
```

---
