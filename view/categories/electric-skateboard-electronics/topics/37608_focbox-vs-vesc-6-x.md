# Focbox vs VESC 6.x

### Replies: 22 Views: 5792

## \#1 Posted by: Luuke Posted at: 2017-11-07T09:11:43.073Z Reads: 706

```
Hi,

I am thinking about using one huge single drive 190KV built, which is rated up to 90A.
Most 6374 motors are rated up to 70A I think.

Since Vesc 4.x can supply 50 constant, I wouldn't be able to use the potential of this motor.
This is why I am thinking of Focbox or Vesc 6.x

Both have direct FETs and aluminium case for head spreading.

FocBox
Voltage: 8V – 50V
Safe from 4 to 12S Batteries
300A Peak Current
60A Continous Current

Vesc 6.x
Voltage: 6V – 60V (Safe for 3S to 12S LiPo) 
Current: Continuous 80A, Burst 120A 

Which one would have more potential?

Some further information:
10S5P or 12S4P (30Q)
15T/35T
90mm Flywheel
```

---
## \#2 Posted by: Maxid Posted at: 2017-11-07T09:17:47.245Z Reads: 678

```
You are giving all the answers yourself already - not sure what you want to know in addition to that.

BTW: burst is meaningless and my Focbox on a single 149kv pneumatic was overheating all the time (admittedly gearing was not optimal but still)
```

---
## \#3 Posted by: Luuke Posted at: 2017-11-07T10:20:36.278Z Reads: 650

```
Why is burst current much lower for Vesc 6?
What is the duration for burst/peak current?

Is peak & burst current the same?
```

---
## \#4 Posted by: Der6FingerJo Posted at: 2017-11-07T10:37:00.429Z Reads: 639

```
I think there isn't some standard in the peak/burst current measurements, but you can picture it like this:
For fractions of a second, the ESC can withstand X amount of current. If you go for a millisecond it could probably handle 1000A and so forth. (well this is hyperbolic but you get the idea)

Then there is the question of what a "burst" is. The manufacturer could define it as a spike when you start from standstill, like below a second, or as short moment in which you pull the trigger hard for acceleration for 10 seconds or so.

I think the FOCBOX "burst" is the former, shorter, burst when starting a motor, while on VESC 6 it might be the 10 second burst you would actually manually control.
```

---
## \#5 Posted by: Maxid Posted at: 2017-11-07T10:42:23.832Z Reads: 608

```
Peak and burst are marketing terms and nobody knows what the conditions for either are. Go for the continuous and you get the idea of which one can handle more current. 
Keep in mind though that at 80A battery current a 10S4P with 430Wh would be drained completely in 9min - just o give you an idea that you will not really be using 80A for long periods of time in day to day use.
```

---
## \#6 Posted by: Luuke Posted at: 2017-11-07T12:24:56.438Z Reads: 580

```
That's true! It is something arround 9 Minutes... Insane!

But almost every dual drive System with 2 times 6355 would be the same, or even more (40A to 50A each motor)!
Ok, current would be splitted to two ESCs...
But the total power consumption is equal.
```

---
## \#7 Posted by: Maxid Posted at: 2017-11-07T12:33:30.544Z Reads: 564

```
Maximum total power is pretty meaningless - you will not use it continuously. No matter if you have one two or four motors on your board.
Your average consumption will be much much lower (somewhere around a couple amps)

What I want to say is: both ESCs will give you plenty of power as you won't be reaching their limits in normal riding conditions. If you go all out like @Nowind that might be a different story though :D
```

---
## \#8 Posted by: Maxid Posted at: 2017-11-07T15:06:39.980Z Reads: 528

```
BTW: there's also @esk8's new controller that seems to sit in between VESC6 and Focbox - personally I don't have experience with it but  maybe he can tell you something about what continuous current it can withstand.
Might be what you are looking for for a strong single motor setup - especially considering that it is quite a bit cheaper than a VESC6
```

---
## \#9 Posted by: chaka Posted at: 2017-11-07T16:02:26.540Z Reads: 495

```
Both units use the same driver and fets, same as our Ollin ESC v1.1. It comes down to which one has more thermal mass and surface area... Our version has more mass and surface area and performs better than both vesc6 and the focbox in constant current handling. We have even produced some custom OEM models with cooling fins and a fan and have reached over 80 amps constant for the Esurfboard crowd.

FYI, the VESC six only handles about 30 amps constant, slightly better than the focbox.
```

---
## \#10 Posted by: Maxid Posted at: 2017-11-07T16:10:13.976Z Reads: 475

```
@Luuke so now you have 4 options to choose from - thanks @chaka: seems like you are making this even harder for him :smile:
```

---
## \#11 Posted by: Deckoz Posted at: 2017-11-07T16:26:19.951Z Reads: 456

```
Well, in my eyes,  the vesc 6 isn't worth it. While its now measuring current across all three phases, which should be capable of ruling out time delay on phase readings...the vesc6 still can't do 100% duty cycle even though the DRV is 100% duty capable. What are you really gaining for all that extra cost?

Focbox, or ollin esc... Are plenty capable of anything you'd throw at it for a lot less cost. But if your stuck on the VESC 6. You could grab one of @stewii boards  for a price comparable to ollin and focbox instead of the stupid trampa price gouge lol.
```

---
## \#12 Posted by: Luuke Posted at: 2017-11-07T17:03:19.417Z Reads: 429

```
@chaka: VESC 6 can only handle 30A? focbox even less?
So Ollin ESC should be slightly better?!

@stewii: your version can handle the same current as the others, depending on the Heatsink?

 How much current can VESC 4.1x handle?
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2017-11-07T17:22:46.166Z Reads: 417

```
Whithout any kind of heat sink, yes those fet can only handle 30 amp continous per fet, Ollin vesc aren’t exempt of that rule either, but with a good heat dissipation  you can easily ramp up the max current, that why these type Vesc should come stock with a heat shink and not only has a option.
```

---
## \#14 Posted by: chaka Posted at: 2017-11-07T17:23:15.870Z Reads: 411

```
The key word is "constant" current. Intermittently you can draw more power but you will hit the thermal limit quickly and the software will throttle back and eventually settle at its max constant.

@JohnnyMeduse I tested both models with the heatsinks attached.
```

---
## \#15 Posted by: JohnnyMeduse Posted at: 2017-11-07T17:38:29.971Z Reads: 401

```
Can you show us the result... I would like to know, and the process behind, I just wonder how these test has been conduct and by who. Did you also use a third part, for being able to show some unbiased resuts ?
```

---
## \#16 Posted by: chaka Posted at: 2017-11-07T18:03:29.521Z Reads: 402

```
Various tests, no huge differences between all models without employing some type of active cooling. Really comes down to how much gate charge the drv chip is capable of. The higher the charge the lower you can get the FETs in terms of resistance. I suppose you could spread the gate charge through several small FETs like the toshiba or fairchild but I think we would only increase passive heat dissipation marginally. 

As for testing you can see... Vedder did a few and posted videos on it. Ambient temp should also be taken into account since it does play a role in power output when doing these tests. 

In order to truly manage 80 amps constant you need a tall heatsink with a blower/fan bolted to it. I know what it takes because I have done it. 

Luckily, 30 amps constant is a massive amount of power in a dual drive skateboard. 12s @ 60 amps (2x30A) with a good battery is around 46v nominal/full charge. Just under 2800 watts!
```

---
## \#17 Posted by: Deckoz Posted at: 2017-11-07T20:04:40.797Z Reads: 385

```
As Johnny said constant current can be manipulated by heat.

For example there's a bvedder video with him pushing 70A constant through the vesc6 doing a position hold on a motor for almost 10 minutes. Which I believe if I'm remembering right started thermal throttling at 8 minutes once the FETs reached 75C

That's a LONG time to hold that much current...and still thermally be OK ;) just depends on how much aluminum you have
```

---
## \#18 Posted by: Luuke Posted at: 2017-11-07T20:42:41.157Z Reads: 367

```
So if that's the case I can go with a Vesc 4 and install some massive (maybe active) cooling.
```

---
## \#19 Posted by: themegak Posted at: 2017-11-07T21:46:55.001Z Reads: 359

```
You know you will not want to ride at the peak of what your motor is capable right ?  Unless you are very heavy, all of this will be moot once you start riding as you will see that your board goes plenty fast at below 30 amps.  Unless you are a super speed freak who eats speed wobbles for breakfast.
```

---
## \#21 Posted by: krazor Posted at: 2019-03-16T03:42:36.565Z Reads: 107

```
define speed freak in esk8. i do about 40kmh and it feels pretty slow to me
```

---
## \#22 Posted by: AlanZhou Posted at: 2019-03-16T03:48:30.866Z Reads: 105

```
Read the fckn date... 🤦‍♂️
```

---
## \#23 Posted by: krazor Posted at: 2019-03-16T03:54:49.567Z Reads: 102

```
Yep lol didn't even realise. I don't brows forums much anymore haha
```

---
