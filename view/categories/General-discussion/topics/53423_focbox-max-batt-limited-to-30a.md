# FOCBOX Max Batt limited to 30A?

### Replies: 18 Views: 917

## \#1 Posted by: zhud Posted at: 2018-04-25T03:49:34.427Z Reads: 213

```
Has this always been the case?

From Carl, this is the upper limit of the device. I find that odd considering it comes preconfigured to 40A. 

Anyone care to give some clarification?
```

---
## \#2 Posted by: SeanHacker Posted at: 2018-04-25T03:53:56.649Z Reads: 210

```
You're listening to the wrong guy. He's just a customer service rep trying to give technical advice here lately for some reason. 

I run 40A (30Q batteries) in each of my vescs (80A) all day long no problems. But it also depends on the type of batteries you have too.
```

---
## \#3 Posted by: zhud Posted at: 2018-04-25T04:01:55.775Z Reads: 208

```
I’m running 8s rated at 100A continuous. 

I really don’t understand why I couldn’t safely run 50A continuous through the FOCBOX, the specs rate it at 60A continuous. Am I wrong to assume that I have some headroom with leaving the extra 10A?

I’m al running the FOCBOX hard no doubt, it’s being used as a controller in a light duty e-bike.
```

---
## \#4 Posted by: Trdolan03 Posted at: 2018-04-25T05:11:01.496Z Reads: 194

```
Are they 60 motor amps or battery amps?
```

---
## \#5 Posted by: zhud Posted at: 2018-04-25T05:15:55.215Z Reads: 187

```
On the specs listing it is listed as Max Continuous Current: 60A

Considering this is listed with the battery specs, with Abs Max following, I think it can be assumed it is referring to the Max Battery settings... but I could be wrong.
```

---
## \#6 Posted by: CarlCollins Posted at: 2018-04-25T05:16:34.955Z Reads: 187

```
@SeanHacker
For your Information: Never replied to his thread here. Answered on the Support ticket.
Also I am just sharing the information which I'm getting from the tech team.
They advised me that Batt Max should be at 30A to play safe.
```

---
## \#7 Posted by: zhud Posted at: 2018-04-25T06:44:39.353Z Reads: 170

```
So let's say that I have set my Batt Max to 30A, would it be acceptable to set my Motor Max to the rated Amperage of my motor at 80A?

Would this be within acceptable current that the FOXBOX can handle, no overheating of the FETs permitting?
```

---
## \#8 Posted by: SeanHacker Posted at: 2018-04-25T15:48:19.320Z Reads: 156

```
Yes. You'll love the torque provided at Motor Max 80A if you're into that sort of thing. I just upped mine to 80A a few days ago after running 70A for a year or so. It feels great!
```

---
## \#9 Posted by: Bjork3n Posted at: 2018-04-25T16:29:31.753Z Reads: 143

```
Was it a big difference from 60 to 70? 
Running 60/30 now on the dual :slight_smile:

Been using 60/30 without any issues so far :slight_smile:
```

---
## \#10 Posted by: skatardude10 Posted at: 2018-04-25T17:12:46.125Z Reads: 135

```
If you are not pumping more amps out of the battery, how does increasing motor amps have any real effect? 

I guess I just don't understand the math/science behind it, and I can't deny that my VESCs logs do show motor amps much higher than battery amps, but how?

Is the effective power on the road derived primarily from your battery (which I thought), or from some combination of both?
```

---
## \#11 Posted by: egzplicit Posted at: 2018-04-25T17:18:32.592Z Reads: 133

```
Think of it in watts:

30A battery max * 36v = 1080W available power.

Duty cycle @ 60% means 30A * (36v * 60% duty cycle ) = 648W.

So there’s 440W left. That’s why motor amps can be higher than battery max. At 100% duty cycle the bat max will be the limit.
```

---
## \#12 Posted by: E1Allen Posted at: 2018-04-27T12:35:06.463Z Reads: 114

```
I've set my FocBox to 65 battery amps each.  For science.
```

---
## \#13 Posted by: zhud Posted at: 2018-04-27T20:45:32.780Z Reads: 103

```
Your battery can supply direct current flow to the FOCBOX, which utilizes PWM (pulse width modulation) to drive the motor. Because the PWM is not continuous, and provides intermittent pulses of current that can supply greater magnitudes of current to the motor via the MOSFETs and capacitors. You might recognize this as "Duty Cycle".

The reactivity of the capacitance increases with higher frequencies as they are frequency dependent and the resistance to current flow is reduced at higher frequencies. This is because of complex impedance of a capacitor. I won't go into detail about what "real" and "imaginary" impedance is, but it has to do with electron charge accumulation. 

Lets do some Laplace Transformations on the PWM frequency domain... lol, just kidding :joy: 

`** Let's just say that continuous current supplied to the FOCBOX is able to provide intermittent bursts of greater current to the motor.`
```

---
## \#14 Posted by: RedEagle Posted at: 2018-04-27T21:03:01.919Z Reads: 98

```
[quote="zhud, post:13, topic:53423"]
lol, just kidding :joy:
[/quote]

My mouse was _just_ hovering on the flag, waiting to strike.
```

---
## \#15 Posted by: zhud Posted at: 2018-04-27T21:26:26.819Z Reads: 97

```
NO BODE has time for that.

...alright, I'll stop
```

---
## \#16 Posted by: skatardude10 Posted at: 2018-04-27T23:41:57.864Z Reads: 89

```
Thanks for that explanation, that clears it up perfectly and makes sense! Not so much the second half making sense, but the second half is interesting to try to understand. Thank you!
```

---
## \#17 Posted by: Namasaki Posted at: 2018-04-28T05:25:48.263Z Reads: 76

```
I have been running my Vesc's Battery Max at 50a and Motor Max at 80a in BLDC mode for a long time with no problems.
```

---
## \#18 Posted by: flyb0i Posted at: 2019-09-18T17:29:43.551Z Reads: 17

```
[quote="zhud, post:13, topic:53423"]
Lets do some Laplace Transformations on the PWM frequency domain… lol, just kidding :joy:
[/quote]

HAHAHHAHAHA Love it.
```

---
