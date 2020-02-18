# Destroyed my Flipsky 4.12, help me figure it out

### Replies: 33 Views: 782

## \#1 Posted by: kalebludlow Posted at: 2018-09-26T08:41:06.539Z Reads: 209

```
Okay so I was just randomly playing with my board, which is currently in a state of repair. Was just spinning the motors up, one of them would spin some times and wouldn't other times. Then a loud pop with some smoke, and she's fucked. Can anyone help me figure out what I did wrong? This is my first time playing with VESCs, so I had battery amps set to like 30A![IMG_20180926_183707|375x500](upload://74VsiN524SFUI0bcX8MFkzrRpRV.jpeg)
```

---
## \#2 Posted by: kalebludlow Posted at: 2018-09-26T08:55:16.323Z Reads: 195

```
I know I've blown the DRV, just wondered if anyone had any idea of why it happened so I know to not do it again
```

---
## \#3 Posted by: amazingdave Posted at: 2018-09-26T09:04:34.227Z Reads: 194

```
If you were running it on the bench you may have exceeded the 60k erpm limit....
```

---
## \#4 Posted by: L3chef Posted at: 2018-09-26T09:07:18.068Z Reads: 195

```
Did you go full throttle without any load? 
What's your battery and motor values?
```

---
## \#5 Posted by: trampa Posted at: 2018-09-26T09:12:30.020Z Reads: 194

```
It's a clone and when you look at the placement of the FETs, it's not made very well. The two FETs (lower right corner are nearly touching each other).  It would not surprise me if this is not the only issue.

Settings, what did you do, vendor, brand?
```

---
## \#6 Posted by: kalebludlow Posted at: 2018-09-26T09:54:25.413Z Reads: 186

```
Does setting an ERPM limit in vesc-tool stop this? Or is it more of a soft limit?
```

---
## \#7 Posted by: kalebludlow Posted at: 2018-09-26T09:56:27.354Z Reads: 183

```
Yeah I did, that's probably what did it.

12s5p 30Q with SK8 6364 190kV on FOC

Motor Max 50A
Motor Min -30A

Batt Max 30A
Batt Min Regen -2A
```

---
## \#8 Posted by: kalebludlow Posted at: 2018-09-26T09:57:10.289Z Reads: 182

```
I can now see how it seems pretty clear this is my fuck up. I just want to be able to learn as much as possible to help in the future
```

---
## \#9 Posted by: amazingdave Posted at: 2018-09-26T09:59:40.451Z Reads: 182

```
Never blast it on the bench... and 12s foc is a very risky business...
```

---
## \#10 Posted by: kalebludlow Posted at: 2018-09-26T10:00:17.785Z Reads: 180

```
Time for that upgrade to VESC6 I think, before my build is even completed hahaha
```

---
## \#11 Posted by: trampa Posted at: 2018-09-26T10:13:39.726Z Reads: 175

```
And -2A on the battery min will not give you any brakes. This value defines the strength of the brakes at speed.
The motor min becomes more dominant at slower speeds! It doesn't help to use high motor regen values and low Batt Min Regen values. The braking energy needs to be stored somewhere. If you close that door, you will not have an brakes when you need them.

12S FOC is no issue if you use proper hardware. Clone HW 4.12 ESCs can't handle FOC at 12S really well. Chances are high that you fry the system.
```

---
## \#12 Posted by: kalebludlow Posted at: 2018-09-26T10:15:17.620Z Reads: 165

```
Not riding the board yet so not having brakes isn't an issue. What settings would you recommend for my hardware?
```

---
## \#13 Posted by: trampa Posted at: 2018-09-26T10:43:25.920Z Reads: 161

```
Twin or single?
```

---
## \#14 Posted by: kalebludlow Posted at: 2018-09-26T10:55:26.898Z Reads: 159

```
Twin 10chars
```

---
## \#15 Posted by: trampa Posted at: 2018-09-26T11:40:49.443Z Reads: 151

```
Run it in BLDC if you use HW 4.12
Assuming you use a 12s5p pack from 15A rated original Samsung cells:

Motor max 55 to 60A
Motor max Regen: - 30A
Battery Max 35A  (each ESC sucks 35 A, which results in 70A for the Battery).
Battery max Regen. -25A to -30A (about same as motor regen will result in more linear brakes)

The battery will not the high currents for a long time when you brake. These are very short spikes only.
```

---
## \#16 Posted by: dareno Posted at: 2018-09-26T12:50:02.194Z Reads: 141

```
That is not an over erpm issue.  That set up should not exceed the limit.  

[quote="kalebludlow, post:8, topic:69242, full:true"]
I can now see how it seems pretty clear this is my fuck up. I just want to be able to learn as much as possible to help in the future
[/quote]
That is a faulty vesc. 
  Get in  touch with them.  They are good people and will help you out.
```

---
## \#17 Posted by: kalebludlow Posted at: 2018-09-26T13:01:08.475Z Reads: 137

```
Well would I contact Flipsky directly or the random eBay seller I got it off?
```

---
## \#18 Posted by: dareno Posted at: 2018-09-26T13:06:04.023Z Reads: 139

```
[quote="kalebludlow, post:17, topic:69242"]
t Flipsky directly
[/quote]
These guys
```

---
## \#19 Posted by: baxtred Posted at: 2018-09-27T08:39:32.539Z Reads: 120

```
If you look at the data sheet for the 30Q, the max charge rate is 4A, so at a 5P pack, should be 20A.

I'd personally set this to -20A to not damage the cells by charging them too quick. I have -12A on one of my boards and feel like it's enough brakes for most situations. -20A should be plenty especially of you are used to "push" longboarding with no brakes.
```

---
## \#20 Posted by: baxtred Posted at: 2018-09-27T08:48:46.009Z Reads: 116

```
Adding onto my other comment. You should leave the motor max regen at -70A (or whatever your motor is rated too). The duty cycle will make motor amps high and battery amps low during slow speeds.

For a dual drive here's my recommended values (each esc will have these same values) 

Motor Max: 70 amps
Motor Max Regen: -70 amps
Battery Max: 37.5 amps
Battery Max Regen: -10 amps
```

---
## \#21 Posted by: Andy87 Posted at: 2018-09-27T08:50:20.668Z Reads: 115

```
Don’t forget that the max charge current for the cell found on the datasheet is for a full cycle from empty to full.
It’s not a problem for a short time to exceed this values

Edit:
Did understood why the duty cycle should make the motor amps high and the bat amps low during low speed?
If you have high motor amps your motor voltage will drop, that does not affect the battery amps and voltage (besides the voltage sag for sure)
Or did I get something wrong?
```

---
## \#22 Posted by: kalebludlow Posted at: 2018-09-27T08:53:48.656Z Reads: 113

```
They just got back to me, they said they couldn't do anything I would need to contact the seller
```

---
## \#23 Posted by: baxtred Posted at: 2018-09-27T08:55:29.001Z Reads: 112

```
@kalebludlow
 What KV is your motor by chance?
```

---
## \#24 Posted by: kalebludlow Posted at: 2018-09-27T08:56:36.491Z Reads: 108

```
190kv, little bit high for my battery I know, definitely time to move up to VESC6
```

---
## \#25 Posted by: baxtred Posted at: 2018-09-27T08:57:58.752Z Reads: 105

```
That should be fine. Was thinking you had a 280 KV or something crazy like that. I know they sell 6364 in high KV options and wasn't sure.
```

---
## \#26 Posted by: trampa Posted at: 2018-09-27T09:12:39.393Z Reads: 105

```
As I said, a short injection of high currents is not so much of a problem for the battery. The rated amps for charging are for longer charge periods. In the end yo want the brakes to work when you need them.
The Battery MAX Regen is the value that defines brakes at speed, assuming that the Motor MAX Regen is matched.

When you go slow the motor generates at lower voltage, which will be scaled up to charge voltage, while the currents will be scaled down on the battery side.

25V x 50A (Motor side) equals 50Vx 25A (Battery side).
If you generate at 25V you can have -50A braking, while the battery only sees 25A of Regen current.

Frank
```

---
## \#27 Posted by: baxtred Posted at: 2018-09-27T09:19:58.081Z Reads: 102

```
Here's a video with real-time overlay of what the VESC is doing. Input current is another name for battery current in this case.

https://youtu.be/bxSrCjUnLUc

You'll notice during the video that battery amps are always lower than motor amps, and the two approach each other as the duty cycle approaches 100% (during higher speeds). During low speeds, battery amps are low and motor amps are much higher. At around 0:35, you can see braking does the exact same thing. 

I guess a way to think of it is in power. The power (watts) that the battery provides will be directly equally to the power that the motor provides to the wheels (ignoring effeciencies). Let's say the battery and motor see 700W during acceleration. The difference is that the motor is doing 70a at 10v, while the battery is doing 14a and 50 volts, yet they are both using 700W. This large difference between motor and battery amps happens during acceleration from standstill or when the wheels aren't spinning very fast (when duty cycle is low). 

During acceleration, having a high motor amp value will give more punch. If both the battery and motor amps were set the same, during acceleration the motor will pull 35 amps, but the battery will only pull 10 amps wasting so much potential.

Kinda felt like I was talking in circles there. Hopefully that clears things up
```

---
## \#28 Posted by: Andy87 Posted at: 2018-09-27T09:33:46.791Z Reads: 98

```
Still don’t get it.
The thing with the input output watt is what I meant and in your first post thought you was saying wrong, but understood now that we mean the same 😅
I thought the duty cycle never can‘t exceed 95%.
I thought you just set max values, so why you should I lose potential if I set motor and bat amps close to each other?
If I set my bat max to 50a and my motor Max to 60a, why I can’t get 50 b, 55m amps with just a Duty cycle of 95% out? 
From what depends the duty cycle? From how hard I push the trigger or from the speed?
```

---
## \#29 Posted by: baxtred Posted at: 2018-09-27T09:44:53.174Z Reads: 103

```
The duty cycle is directly related to the speed of your wheels. Let's say your boards top speed is 20 mph. At 10mph your board is using a duty cycle of 50%, at 20mph its 100% (well 95% to protect the FETs), and 5mph its 25%. It doesn't have to do with how hard you push the trigger, just your current speed. 

If you set your battery to 50a and motor to 60a, you will get the most power at a high duty cycle. But when you are accelerating from a stand still (wheels aren't rolling very fast = low duty cycle). Your motor amps will be limited to 60a at let's say 25v, so 1500W. But your battery can produce 50a at 50v or 2500W. So you're only accelerating with 1500W. But if you set your motor to 80a, you'll be able to accelerate at 2250W and your battery still isn't exceeding its set 50a.

This is hard to explain... Lol

So yes, at 95% duty cycle your motor and battery amps will be the same. But you aren't always riding at top speed. For slowing speeds motor amps will always be higher than battery amps. Just watch the video, you'll notice that they are rarely equal and the motor amps can be twice as much as battery amps for most of his ride. Just set these values to what your motor and battery can handle. If anything multiply the manufacture recommendation by 0.8 if you want to be conservative. But don't make them equal!
```

---
## \#30 Posted by: Eboosted Posted at: 2018-09-27T19:33:20.701Z Reads: 88

```
If one of your wheels was spinning randomly then one of the hall sensors, or sensor wires was making bad contact, if you force the wheels pushing the throttle is this situation a large rush of current with flow into your VESC and surely will blow the DRV.

If you have studering on one wheel do not push the throttle all the way on the bench ever, disassemble the enclosure and make an inspection
```

---
## \#31 Posted by: Sebike Posted at: 2018-09-27T20:41:28.433Z Reads: 85

```
Sure, it's only for a short amount of time, but 2xvescs sending 2x30A=60A to the battery seems a bit high, even if it's only for a limited time. In his case that would be charging 12A per cell.
```

---
## \#32 Posted by: kalebludlow Posted at: 2018-09-27T21:34:09.662Z Reads: 84

```
This seems really plausible, closest to what actually happened
```

---
## \#33 Posted by: trampa Posted at: 2018-09-28T08:06:07.684Z Reads: 68

```
For anyone interested, I tried to explain things here:
https://www.electric-skateboard.builders/t/vesc-6-cooling-and-max-current/61944/9?u=trampa
```

---
