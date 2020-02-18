# Few things left to write in BLDC tool

### Replies: 17 Views: 1643

## \#1 Posted by: ninja Posted at: 2016-11-20T00:01:12.523Z Reads: 104

```
Hi! 
Can somebody tell if my numbers are correct in BLDC tool? So my setup is 8s 8000mah 30c with 245kv sk3 motor.
motor max 40A
motor min. regen -40A
battery max 25A
battery min regen 12A
```

---
## \#2 Posted by: Jinra Posted at: 2016-11-20T00:03:57.319Z Reads: 105

```
Those are conservative, but good numbers. I'd start with that and adjust if necessary. You can probably bump up the batt max a bit more. I'd personally just match it with motor max for now at 40A.
```

---
## \#3 Posted by: ninja Posted at: 2016-11-20T00:08:46.966Z Reads: 94

```
so batt max to 40A? also about motor detection numbers -should i put exact numbers what i'll get from detection? For an example if i'll get integrator limit 92.42 do i need put it exact or 90.00 will be fine?
```

---
## \#4 Posted by: Jinra Posted at: 2016-11-20T00:10:31.920Z Reads: 90

```
Round down int limit to nearest 5 and bemf coupling to nearest 50, it actually does this for you if you hit "apply" under "start detection".
```

---
## \#5 Posted by: ninja Posted at: 2016-11-20T00:11:53.206Z Reads: 83

```
thanx a lot:)
```

---
## \#6 Posted by: ninja Posted at: 2016-11-20T00:14:20.370Z Reads: 81

```
should i change min ERPM and min. ERPM for integrator limit?
```

---
## \#7 Posted by: Jinra Posted at: 2016-11-20T00:17:30.374Z Reads: 79

```
i wouldn't touch it, leave it at it's default values.
```

---
## \#8 Posted by: ninja Posted at: 2016-11-20T00:18:21.996Z Reads: 75

```
o.k. thanx
```

---
## \#9 Posted by: ninja Posted at: 2016-11-20T00:48:10.356Z Reads: 72

```
why my throttle on gt2b on 60% is already full speed?
```

---
## \#10 Posted by: Jinra Posted at: 2016-11-20T00:49:21.414Z Reads: 70

```
set control mode in the PPM tab to "disabled". Then check the "display" box and input your min and max pulsewidth. Apply and check your throttle, then you can turn the control mode back on.
```

---
## \#11 Posted by: ninja Posted at: 2016-11-20T01:07:36.193Z Reads: 70

```
I've done it couple of times. in display it showed on full throttle 100% with numbers 2,04 so i written that 2,04 in max pulse width. same did with full brake it showed 0% and 0,61. when i test it at the start it wont move because of safety features than it spins even on neutral position, so i need adjust trim on remote to stop motor, but then happens that problem i mentioned before!
```

---
## \#12 Posted by: Jinra Posted at: 2016-11-20T01:09:26.033Z Reads: 70

```
I think you have to rebind the remote to reset the neutral position. At least this is what you have to do with the winning remote, I'm not too familiar with the GT2B
```

---
## \#13 Posted by: ninja Posted at: 2016-11-20T01:10:50.824Z Reads: 68

```
you mean that i need to put that jumper in ?
```

---
## \#14 Posted by: Ackmaniac Posted at: 2016-11-20T08:02:19.707Z Reads: 59

```
That is the problem with the ppm adjustment in bldc-tool. That was one of the reasons for me to provide a mod. Because with that you also can define the center position.
http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-and-individual-throttle-curve/12286/1
If you want to get it running in the standard one you have to write down the ppm value in center, for example 1,54. Then at full throttle, which is 2,04 in your case. The calculate 2,04 - 1,54 = 0,50 and subtract that form the center 1,54 - 0,50 = 1,04. That is what you should enter for the minimum. Then your throttle will be at 50 % in idle.
But sadly you lost 0,44 of throttle range on the brake.
```

---
## \#15 Posted by: yaca Posted at: 2016-11-20T10:54:34.545Z Reads: 48

```
As I already told you, use BLDC-Tool 2.51. It's so much better.

Does GT2B has a throttle trim like the winning remote? Because this is also a posibility to adjust the neutral position to 50% on display.

Oh sorry just saw you already trimmed the throttle. What do you mean with "why my throttle on gt2b on 60% is already full speed?" 60% on display or 60% of throttle range (without brake range)? you run in current mode? you get full speed with just a little input of the trigger at the benchtest? That's normal. Even in real in current mode you won't use the entire throttle trigger range but more as at the benchtest. If you set motor max to a lower value the range will be higher, but is not always a good solution. In watt mode the range will be bigger.
```

---
## \#16 Posted by: ninja Posted at: 2016-11-20T12:20:21.654Z Reads: 47

```
Yeah, I will try it if somebody from my friends have Ubuntu. I have Windows for now, so i'll try to sort out trigger problem in BLDC tool 2.18. 

[quote="yaca, post:15, topic:13346"]
What do you mean with "why my throttle on gt2b on 60% is already full speed?" 60% on display or 60% of throttle range (without brake range)?
[/quote]

I mean, that I imagine range on my remote- from neutral to full speed, where neutral will be 0% and full speed 100%. So in that range on 60%on the bench testing it's already full speed, then from 60% to the 100% doesn't change everything.

So you are saying that  full speed with just a little input of the trigger at the bench test it's normal? And in real life it will be a bit better? I just don't want to ride at comfortable speed and then accidentally move trigger a 1 millimeter and than it goes on full speed!!

If i trimm trigger on remote while it's in bldc- nearest to 50% on display in bldc tool i can get 56%, but then if i'll press full throttle it will go up to only about 76%. Is this normal?

I run current no reverse with brake mode.

So if i set motor max to a lower value the range will be higher? How much lower i can make without causing some disadvantages?  what are disadvantages if I set motor max to a lower value?
```

---
## \#17 Posted by: yaca Posted at: 2016-11-20T12:30:21.050Z Reads: 42

```
You don't need Ubuntu. There is also a windows version for 2.51.

Max and Min pulsewith you set the numbers you get on display, than it shows 100% - try to go 99% at first to see if you got it. Neutral 50% you set with throttle trim or at version 2.51 you have to adjust at first the centre pulsewith.

About Motor max it depends on your hills you ride and how fast you want to accelerate. Just on flats you don't need so much amps but if you go steep hills you will need higher amps so lower motor max is not a good solution in that case. Try watt mode! I ride in watt mode with "ramp by current mode" but in the moment weather doesn't let me test it more. Try also to ride in current mode so you see the difference - it is similiar like throttle of a car.
```

---
