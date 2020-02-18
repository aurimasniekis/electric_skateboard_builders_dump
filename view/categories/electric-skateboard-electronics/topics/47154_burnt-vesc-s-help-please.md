# Burnt VESC’s help please!

### Replies: 32 Views: 1234

## \#1 Posted by: amazingdave Posted at: 2018-02-22T13:32:03.603Z Reads: 154

```
Hi.  

A student I’m working with has built a board, using a keda 190kv motor, scram board VESC and 12s battery. Following the same pattern that both my boards run without issues. 
The board has fried 2 vescs! In both instances it bench tested fine and then at slow speed on first run the VESC died... the settings on the VESC are correct as far as I can tell (same as my boards)

The Drv chip has scorching on the top face....

 what’s going on?!?
```

---
## \#2 Posted by: GrecoMan Posted at: 2018-02-22T13:39:31.765Z Reads: 151

```
post pictures of your settings please.
```

---
## \#3 Posted by: amazingdave Posted at: 2018-02-22T14:58:09.089Z Reads: 145

```
These are images of the Xmls saved from VESC tools.. 
app config are the first 3
Motor config the last 4![image|281x500](upload://9PyGgSYIoCXrDwBV5LyeMyC6wTJ.jpg)![image|281x500](upload://cYK26QyXsIzYuYwSkWlQFywLDbD.jpg)![image|281x500](upload://hzs9HozpWxrVu5K7MuuOlZMXBUW.jpg)![image|281x500](upload://y4n0HJRvYosfOp9Jpe3WR3yjqnS.jpg)![image|281x500](upload://t6nmJAIQi9aapvwnXFZdTrcvIwP.jpg)![image|281x500](upload://ytgJbhgO0H6L6p6iQdyPecwU3em.jpg)![image|281x500](upload://Awd1ghUG2gEgzj7Dc6aTi8hRo8c.jpg)
```

---
## \#4 Posted by: rojitor Posted at: 2018-02-22T15:46:32.613Z Reads: 123

```
Er.... I think grecoman means VISUAL settings....Not xml
```

---
## \#5 Posted by: GrecoMan Posted at: 2018-02-23T11:00:33.982Z Reads: 107

```
yea I meant screenshots of BLDC tool...🤣
```

---
## \#6 Posted by: Bjork3n Posted at: 2018-02-23T11:14:41.162Z Reads: 106

```
https://media.giphy.com/media/BmmfETghGOPrW/giphy.gif
```

---
## \#7 Posted by: amazingdave Posted at: 2018-02-23T11:40:43.217Z Reads: 102

```
I don’t use the bldc tool, I’m using vedders new VESC tool. Is there a way to view the settings easily in VESC tool? They seem spread across too many pages. There’d be more screen shots than the xml!!
```

---
## \#8 Posted by: Lumaci Posted at: 2018-02-23T11:47:48.440Z Reads: 102

```
You would not have to share all settings just stuff like battery settings motor settings and such.
```

---
## \#9 Posted by: GrecoMan Posted at: 2018-02-23T11:52:52.267Z Reads: 98

```
take a lot of screenshots. 

or buy a new vesc.
```

---
## \#10 Posted by: amazingdave Posted at: 2018-02-23T12:06:18.419Z Reads: 97

```
Buying a new VESC, but in the interest of me not killing it, please cast your eyes over these screenshots.... ta.  ![image|666x500](upload://8F7ZmYN88gypI2XWHFkJOazpZu5.jpeg)![image|666x500](upload://39c6FYTkLQPqptluGFI7ZUfkc0u.jpeg)![image|666x500](upload://lSDG37luAvov5lRSiApW0VuNPaT.jpeg)![image|666x500](upload://dIHXKtnmK0TPnfvbGpL8PZbuzgf.jpeg)![image|666x500](upload://yDUvn7tNbWASVzixSPByuMzfZ0M.jpeg)![image|666x500](upload://44pkCZfDM8Oaz129iGpOusdV4W2.jpeg)![image|666x500](upload://a9Q651ZHpC9B3tCKdmy37v4748H.jpeg
```

---
## \#11 Posted by: amazingdave Posted at: 2018-02-23T12:08:05.025Z Reads: 91

```
The VESC died within 3 minutes of first real use at low speed and light braking....
```

---
## \#12 Posted by: Blitz Posted at: 2018-02-23T12:11:43.914Z Reads: 93

```
Guys I am intrested also why and what went wrong. 

I have a keda motor and I want to use that New vesc tool :P
```

---
## \#13 Posted by: L3chef Posted at: 2018-02-23T12:13:07.859Z Reads: 95

```
Lipo or liipon? Your battery regen seems high
```

---
## \#15 Posted by: amazingdave Posted at: 2018-02-23T12:15:00.833Z Reads: 96

```
Lipo.....
10 char
```

---
## \#16 Posted by: laurnts Posted at: 2018-02-23T14:55:43.167Z Reads: 90

```
My best guess? motor phase wire short (unshielded / cut-off shrink wrap)...
```

---
## \#17 Posted by: Tomer Posted at: 2018-02-23T15:30:02.815Z Reads: 84

```
Happend to me, not a very pleasant experience. 
Although mine burnt immediately after I tried to detected it with VESC Tool.
He says that it got burnt after 3 minuets of use. Maybe some vibration make the motor phase wires touch
each other. 

Please upload photos of the motor.
```

---
## \#18 Posted by: ThermalM16 Posted at: 2018-02-23T18:02:14.186Z Reads: 78

```
Having high battery regen on 12s can put you close to the max voltage these VESCs are designed for. I've repaired several VESCs that were fried from braking downhill on 12s. It's possible on full charge with high regen current was enough to cause a similar situation. Usually this kills a FET which in turn kills the DRV in my experience.
```

---
## \#19 Posted by: amazingdave Posted at: 2018-02-23T20:06:23.279Z Reads: 68

```
What would you recommend as a max battery regen on this setup?
```

---
## \#20 Posted by: amazingdave Posted at: 2018-02-23T20:09:02.266Z Reads: 69

```
The motor looks immaculate, I’ve tried shorting each phase to another and all 3 whilst turning by hand and the motor gives the appropriate amount of resistance in all cases.... it may be as someone said that it is damaged insulation combined with vibration to make an intermittent short...
```

---
## \#21 Posted by: Blitz Posted at: 2018-02-23T20:14:17.433Z Reads: 68

```
If the wires were soldered on and heat shrink over this would not have happened right?

I'm thinking of useing the 5.5 bullets of my batteies or just direct solder.
```

---
## \#22 Posted by: Eboosted Posted at: 2018-02-23T20:24:03.263Z Reads: 62

```
I have a policy on DIY eboard building:

Buy extra spare parts every time, that'll save you months of waiting time for overseas shipments to repairs, replacement parts and more time shredding. 

Buy better quality parts when it's cost if slightly higher, you will buy them down the road sometime

This goes for motors, ESCs (specially VESC 4.12), extra battery cells and antispark switches
```

---
## \#23 Posted by: ThermalM16 Posted at: 2018-02-23T22:05:17.727Z Reads: 53

```
I believe people generally have -12 at most for 12s. I'm not 100% sure though
```

---
## \#24 Posted by: Clonkex Posted at: 2018-02-24T00:47:32.396Z Reads: 48

```
Why does regen current have anything to do with voltage? Not saying you're wrong, I genuinely don't know. I would have thought you determine regen current entirely by what capacity your battery is (for a 1-2c charge rate).
```

---
## \#25 Posted by: ThermalM16 Posted at: 2018-02-24T00:53:58.710Z Reads: 48

```
V=iR
Voltage = Current x Resistance

So the resistance is for the most part constant. The current and voltage are the main variables here. This basically makes voltage and current directly proportional to each other.

So if I use my power supply to run a VESC. I can spin a motor up and apply the brakes. In doing this I can get a reading of about 43V from my power supply that only outputs a max of 30V. This is with regen current set to somewhere around -40.
```

---
## \#26 Posted by: ThermalM16 Posted at: 2018-02-24T00:55:34.403Z Reads: 46

```
@Clonkex It's only really an issue on 12s or 13s if you have the ability to brake on dual motors
```

---
## \#27 Posted by: Clonkex Posted at: 2018-02-24T01:12:11.578Z Reads: 49

```
I'm still not sure how that works. This is my understanding:

The motor generates voltage proportional to speed. The faster it goes, the higher the voltage. When you're accelerating, at some point the voltage generated by the motor will be almost the same as the battery voltage and it won't be able to go faster (because the current no longer wants to flow to the motor when there's no voltage differential). This is why we have to use higher kv motors to reach higher speeds on the same gearing. I'm pretty sure that's correct.

This is where I'm confused. Why would the voltage ever increase with increased load? As I understand it, braking is the VESC allowing current to flow back to the battery. It regulates that current (with a duty cycle on the fets? not sure) so you don't blow up your battery and so you have controllable braking force. I'm not sure what resistance you would be talking about but the way I see it the main resistance is the fets. We'll assume for simplicity's sake that they're either off or on (lots of resistance or very little). When they're turned on, the resistance is low but the current is high. That means the voltage wouldn't change. Same thing when they're off, the resistance is high but current is low.

That might be oversimplifying it but I'm really not sure why voltage would increase with higher regen current.

What happens if you do the same test on your bench supply but set the regen current to -10?
```

---
## \#28 Posted by: GrecoMan Posted at: 2018-02-24T01:29:25.612Z Reads: 49

```
it’s why people get over voltage errors. sometimes, when braking hard on a full charge the voltage can spike high enough to throw a fault code, or fry components depending on severity
```

---
## \#29 Posted by: ThermalM16 Posted at: 2018-02-24T01:57:30.151Z Reads: 46

```
I get the same general result, just maybe 6V less or so. Honestly I'm just getting into this topic in my classes, but it looks like V=L(di/dt) which is the voltage equation for an inductor. Since a brushless motor is many inductors placed in a circular pattern, this equation is relevant here. So the inductance is pretty much a constant here, which leaves us with the derivative of current with respect to time. I also found a formula I believe is for 3 phase motors, but I may be wrong V=I*X where X=angular frequency * inductance (L)

To simplify all of that, voltage produced by an inductor will in fact increase as the current produced increases. 

To take an example, the inductance of one of LHBs motors is 13.7uH according to the VESC tool's FOC detection.  Lets say you have 40 amps of regen current, which realistically probably won't happen, but it's just an example.  So V = (40)*(5000)(13.7*10^-6)
Basically 5000 RPM is how fast your motor would be spinning in this example. However, I'm only getting about 2.74V when I calculate that. I can only assume it's the wrong formula, or you need to account for the number of inductors in the motor and multiply by that. If I do that, we have 14 in this motor, so now that's 38.36V

I know the motors aren't wired in series in a dual setup, but all I can figure is when you have two motors producing just shy of 40V a piece, bad things happen

If there are any Engineers on here who can correct me on that math or those formulas, I'd appreciate it. I'm only a second year, so I have a long way to go haha
```

---
## \#30 Posted by: Clonkex Posted at: 2018-02-24T03:35:24.849Z Reads: 45

```
That explanation makes me a lot more convinced haha. I have no formal EE training so that's now outside my area of expertise.

Why does 40V from the motor break a VESC though? I'm not sure which bit dies so I don't know which voltage rating to check. Is it the DRV?
```

---
## \#31 Posted by: b264 Posted at: 2018-02-24T03:37:05.922Z Reads: 43

```
[quote="rojitor, post:4, topic:47154, full:true"]
Er… I think grecoman means VISUAL settings…Not xml
[/quote]

If it's XML at least give us text so we can view it in a GUI.  An image of text won't do..
```

---
## \#32 Posted by: ThermalM16 Posted at: 2018-02-24T04:50:16.743Z Reads: 38

```
I can only assume somehow this when being fed by the capacitor bank can create more power or something somehow. I truthfully don't know how it happens, but the bottom line is something is exceeding its designed power limit and letting its magic smoke out.
```

---
## \#33 Posted by: amazingdave Posted at: 2018-02-24T06:37:15.973Z Reads: 33

```
Here’s a Dropbox link to the xml’s

https://www.dropbox.com/sh/tx0vnqmm716xuol/AABXWkz7Dr2TVbaTmBSNEV7ja?dl=0
```

---
