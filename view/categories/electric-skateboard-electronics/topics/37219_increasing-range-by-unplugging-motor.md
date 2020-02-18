# Increasing range by unplugging motor

### Replies: 33 Views: 1594

## \#1 Posted by: LordChaos Posted at: 2017-11-02T23:50:41.843Z Reads: 287

```
Hey guys i built my board so i can upgrade to dual motors when i move out to San Francisco. 

If i deiced to unplugged the phase wires so only one motor is running to decrease power consumption and increase range would that be harmful to my second vesc as it would ask for power but not send it anywhere right?
```

---
## \#2 Posted by: baxter Posted at: 2017-11-03T01:19:59.366Z Reads: 281

```
I have considered doing this as well. I would remove the drive belt @LordChaos to reduce resistance too, assuming you have a satellite setup.

I’m always a bit reluctant to do this out of a fear of frying a Vesc.

Has anyone, (maybe an EE) got a wiring diagram available to indicate where a switch might be located on a circuit to allow this?
```

---
## \#3 Posted by: psychotiller Posted at: 2017-11-03T01:24:30.083Z Reads: 274

```
Proven that 2 motors are actually more efficient than 1 because one motor will pull more amps under stress than 2 will.
```

---
## \#4 Posted by: ShutterShock Posted at: 2017-11-03T01:26:03.066Z Reads: 269

```
It shouldn't be harmful at all. However, Do nOt let the phase wires touch while riding!

You'll end up flat on the ground. The VESC will provide power to the motor phase leads, but since there is nothing connected, it won't draw anything. You could also just unplug that VESC from the internal power if you wanted to be super sure. But if you're thinking that it will like blow up because there's no where for the power to go, that will not happen :slight_smile:
```

---
## \#5 Posted by: ShutterShock Posted at: 2017-11-03T01:27:16.051Z Reads: 261

```
I second this, I didn't really notice any difference in range once I upgraded, due to how much more distributed the load is.
```

---
## \#6 Posted by: psychotiller Posted at: 2017-11-03T01:31:36.408Z Reads: 244

```
Would be the same with horses pulling a wagon. One horse wont go as far as 6
```

---
## \#7 Posted by: LordChaos Posted at: 2017-11-03T03:21:56.919Z Reads: 227

```
oh that is great! i was basing the decreased range from the Eskate range calculator which say 2 motors use more watts per mile
```

---
## \#8 Posted by: FredSaberhagen Posted at: 2017-11-03T03:40:36.721Z Reads: 211

```
Yes but say you only had one bale of hay.  How long could you feed that team of 6 horses?  Might make it farther feeding just the one horse and pulling your wagon slower
```

---
## \#9 Posted by: psychotiller Posted at: 2017-11-03T03:52:57.222Z Reads: 204

```
6 horses burn less calories per mile than one towing you and your bail of hay.
```

---
## \#10 Posted by: jmasta Posted at: 2017-11-03T17:50:53.110Z Reads: 185

```
[quote="psychotiller, post:3, topic:37219, full:true"]
Proven that 2 motors are actually more efficient than 1 because one motor will pull more amps under stress than 2 will.
[/quote]

Is that always true though?   One big motor is more efficient than two smaller motors. If you look at the torque curves, motors have pretty poor efficiency under low loading 

I've never had a dual-drive, but my SK3-6374 single-drive averages 12 Wh/mi. I've recorded a peak efficiency of 8 Wh/mi while also traveling at 20-25 mph.  The typical average is 16 Wh/mi
```

---
## \#11 Posted by: ShutterShock Posted at: 2017-11-03T17:59:37.663Z Reads: 170

```
Are you using the hm-10 and ackamaniacs app?  Mine averages out to 12wh/mi for dual vesc dual 6355 190kv on 12S
```

---
## \#12 Posted by: psychotiller Posted at: 2017-11-03T18:03:56.926Z Reads: 169

```
True. But 2 small motors is still more efficient than one small motor. (apples don't taste like oranges, but may smell like oranges if left in the same bag?) C'mon man...
```

---
## \#13 Posted by: FredSaberhagen Posted at: 2017-11-04T03:00:43.895Z Reads: 146

```
What he's saying is that he agrees with you- for higher loads, two motors better than one.
Conversely at low loads one motor is better 
For long range, what do you want to be at, low loads low speed or multiple motors at a higher speed (peak efficiency on the power band)

Only problem with that is wind force (basically dominating your losses) increases with the square of velocity so you really need to go low and slow for a max range and then one motor works better

Better way to put it:  you will gain efficiency with multiple motors as you go faster.  But for each mph the wind force will eat your efficiency gains several times over :-)
```

---
## \#14 Posted by: ryan_pogi Posted at: 2017-11-04T03:26:44.271Z Reads: 132

```
Just want to confirm this.
1 of my belt on my BoostedBoardV2D+ broke, and ordered some replacement belt.
But I still wanna use the BoostedBoard. While waiting for the replacement, I disconnected the motor without belt.
I say it increases my range significantly.  I just remember cause Boosted used to have a single drive.
```

---
## \#15 Posted by: Hummie Posted at: 2017-11-04T04:41:48.798Z Reads: 128

```
current u need to produce forward momentum can be halved between two motors and since the copper losses are current squared times resistance any reduction in either current or resistance is a boon and the losses will be decreased.  Generally to decrease this dominating loss you want MORE motor.  
 The only reason you'd be more efficient with less motor would be if ur motor or motors were too big to begin with and your main inefficiency therefore would be iron losses. This is the generally accepted guideline for motor sizing and efficiency
```

---
## \#16 Posted by: LordChaos Posted at: 2017-11-05T01:34:48.131Z Reads: 116

```
Thanks for all the replies it great to see all the feedback, Knowing this now i wish i have go to dual motors sooner stoked to see the lift off power when i rock dual 6374s
```

---
## \#17 Posted by: uigiroux Posted at: 2018-02-10T12:31:50.408Z Reads: 98

```
Does anyone know what the diameter of the Turnigy 6374 stator is?
```

---
## \#18 Posted by: Skitzor Posted at: 2018-02-10T12:37:34.150Z Reads: 99

```
that should be a 8mm and mentioned in the specs
```

---
## \#19 Posted by: Nordle Posted at: 2018-02-10T12:50:00.410Z Reads: 97

```
8mm is the shaft, a stator is something different:p i have one laying around at home, i will measure it tonight.
```

---
## \#20 Posted by: uigiroux Posted at: 2018-02-10T13:21:21.778Z Reads: 88

```
Thank you!  Can you get me the diameter and length please?
```

---
## \#21 Posted by: Skitzor Posted at: 2018-02-10T13:42:01.722Z Reads: 77

```
So you actually mean the bell ? I actually read shaft lol
```

---
## \#22 Posted by: GrecoMan Posted at: 2018-02-10T13:42:35.111Z Reads: 75

```
no...

he means the stator 🤣
```

---
## \#23 Posted by: Skitzor Posted at: 2018-02-10T13:45:21.422Z Reads: 74

```
I'm probably thinking too practical. is he looking for an inside constraint rather than an outside.
```

---
## \#24 Posted by: GrecoMan Posted at: 2018-02-10T13:46:05.217Z Reads: 74

```
stator is the inside part with all the windings

bell is the outside part with magnets in it
```

---
## \#25 Posted by: Skitzor Posted at: 2018-02-10T13:47:55.144Z Reads: 71

```
Yeah I get that. but unless he's looking for a sensor ring or something, why would it matter. the bell always covers it
```

---
## \#26 Posted by: GrecoMan Posted at: 2018-02-10T13:49:00.663Z Reads: 71

```
he’s probably trying to compare stator sizes to different motors. bigger stator = more copper = more powa!
```

---
## \#27 Posted by: Nordle Posted at: 2018-02-10T14:16:07.925Z Reads: 64

```
Doesn't matter at all what he's doing. If you can't read a question or understand the question, what is the purpose of answering?
```

---
## \#28 Posted by: Skitzor Posted at: 2018-02-10T14:18:20.371Z Reads: 65

```
Maybe rephrasing the question so the answers can be on point. (ignoring my reading mistake). If it was relevant information I would assume it's mentioned in the specs.

Edit: The stator of a sk3 192kv 6374 is spec. as 5045.
```

---
## \#29 Posted by: Nordle Posted at: 2018-02-10T14:44:28.762Z Reads: 64

```
[quote="Skitzor, post:21, topic:37219, full:true"]
So you actually mean the bell ? I actually read shaft lol
[/quote]
I'm sure it was a missreading, stator is very similar to shaft or bell. No sarcasm involved.
```

---
## \#30 Posted by: E1Allen Posted at: 2018-02-10T17:40:59.066Z Reads: 57

```
My helicopter will have increased range running on one engine in flight vs two.  But having that second engine running is required... Oh well.
```

---
## \#31 Posted by: PXSS Posted at: 2018-02-11T18:03:04.807Z Reads: 53

```
Comparing poatoes to oranges?
```

---
## \#32 Posted by: uigiroux Posted at: 2018-03-05T15:57:36.775Z Reads: 44

```
I forgot I had posted that question, lol.  Yes you are correct in what I was essentially asking.
```

---
## \#33 Posted by: meesie Posted at: 2018-06-19T12:51:01.136Z Reads: 25

```
back to topic: using 1 or 2 motors won't make a huge difference. 1 motor will use say 30amps to get me going, 2 motors will use 15amps EACH. there might be a slight difference but that would be something among the lines of 1mile on 50miles. if you want to increase your range, go slower or upgrade your battery.
```

---
