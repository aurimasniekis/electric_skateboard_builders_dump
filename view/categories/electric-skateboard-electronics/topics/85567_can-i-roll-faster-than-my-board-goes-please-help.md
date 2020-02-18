# Can i roll faster than my board goes? please help

### Replies: 25 Views: 533

## \#1 Posted by: Nedtrampz Posted at: 2019-02-27T13:37:02.124Z Reads: 206

```
Can my free roll speed exceed the max speed i get from my battery..? 9s x 170kv only gets me like 35km top. Basically i wanna know if its ok to roll faster down hills with it?

I have a vesc 4 running 9s thru a 170kv 6374. 

Thanks
```

---
## \#2 Posted by: Nedtrampz Posted at: 2019-02-27T13:38:35.719Z Reads: 205

```
Ive noticed braking comes on real sudden. But other than that it seems to be ok?
```

---
## \#3 Posted by: Grozniy Posted at: 2019-02-27T14:14:00.109Z Reads: 196

```
Belt drive can't roll faster due to belt drag.
```

---
## \#4 Posted by: Deckoz Posted at: 2019-02-27T14:49:54.938Z Reads: 186

```
no its not ok to roll faster down hills. 

- esc has a setting for limit max erpm with negative torque, this only works if you hold the throttle going down a hill, it wont let you go faster
- if you let go of the throttle and gravity accelerates you past your max, and you hit brake or throttle, you'll be lucky if 1 anything happens, 2 if it does happen and the motor doesn't sync your likely gonna get tossed the fuck off
- if you go faster then your max down a hill, and you aren't applying throttle, well don't touch throttle, slow down by other means until you are within your range.
```

---
## \#5 Posted by: Vanarian Posted at: 2019-02-27T14:58:28.960Z Reads: 179

```
IIRC There's also the risk to generate higher voltage from your motor than your battery's nominal which, if you don't have a brake chopper installed by any means, will fuck everything up (including a chance to fuck you up too).

You can check with a calculator your absolute max (no load).
```

---
## \#6 Posted by: Battosaii Posted at: 2019-02-27T15:15:48.676Z Reads: 170

```
I've seen some boosted guys hit 34mph down hill I guess they didnt touch the throttle or brakes till they were in range. Honestly seems very sketchy.
```

---
## \#7 Posted by: Deckoz Posted at: 2019-02-27T15:18:57.660Z Reads: 164

```
Yea, as well since its transients are gonna be huge when the esc tries to sync and maintain control, over-voltage is likely. Its how I killed my first set of escs, going faster then my erpm down a hill, with gearing and 190kv motors that would have put its generator voltage at 63 volts, when I tapped the brakes it would have been in the 70v's easily from transients.
```

---
## \#8 Posted by: venom121212 Posted at: 2019-02-27T16:27:02.670Z Reads: 141

```
Shameless pitch for @hyperIon1's rheostatic brake. I have it installed with no issue. I haven't pushed it on a lengthy downhill run on full charge but I do unplug, roll down my driveway and a quarter mile stretch, and have no issue.
```

---
## \#9 Posted by: Lambjr088 Posted at: 2019-02-27T16:28:36.780Z Reads: 136

```
So for these types of situations is it best to just brake slow when u start the downhill roll?
```

---
## \#10 Posted by: venom121212 Posted at: 2019-02-27T16:38:27.522Z Reads: 132

```
Correct <thhgg>
```

---
## \#11 Posted by: Sn4pz Posted at: 2019-02-27T16:56:29.977Z Reads: 125

```
[quote="Deckoz, post:7, topic:85567"]
n a hill, with gearing and 190kv motors that would have put its generator voltage at 63 volts, when I tapped the brakes it would have been in the 70v’s easily from transients.
[/quote]


woah woah this is super important and awesome. How the heck do I calculate this?????

Would a high gear ratio equate to more or less back voltage...? (probably more? :man_shrugging:)
```

---
## \#12 Posted by: Deckoz Posted at: 2019-02-27T17:25:35.178Z Reads: 107

```
same way you calculate your speed..

10s, 83mm wheels, 15/36 loaded takes me to about 26mph I was going 39-42 down a hill. 

Use this, in reverse

https://www.electric-skateboard.builders/t/im-loosing-my-frikkin-mind-here-help-to-calculate-top-speed/40136/4?u=deckoz

42 / 0.000037 = 1135135.13 mm/min 
83 * π = 260.752190mm circumference
36 / 15 = 2.4:1 Reduction Ration 
1135135.13 / 260.752190 = 4353.31005 Wheel RPM
4353.31005 * 2.4 = 10447.9441 Motor RPM
10447.9441 / 190kv = 54.9 volts

granted I think i had measured those motors trough cli at 170kv

10447.9441 / 170kv = 61.4584948 volts
```

---
## \#13 Posted by: Sn4pz Posted at: 2019-02-27T17:43:11.990Z Reads: 97

```
merci mr deckoz
```

---
## \#14 Posted by: Vanarian Posted at: 2019-02-27T17:46:15.485Z Reads: 94

```
You run mostly at nominal but your battery's max tolerance is top voltage. Transient voltages spikes go high easily even at normal levels (that's how most people here burned their DRV).
```

---
## \#15 Posted by: Sn4pz Posted at: 2019-02-27T18:01:19.002Z Reads: 90

```
I did the calculations with my normal top speed and all that jazz, is this right? I can smash the breaks at regular operation speed and not worry about absurd voltage spikes?

![image|395x376](upload://8bdzo7Ciqf7PUU1jB1GvqAFSGCn.png) 

E: my top speed is subject to change in the future, as I want to try a high ratio with smaller pneumatic wheels.... I plan on moving up to the 8 inchers when I tire(heh) of burnouts :D

E2: 35mph takes me to 53V, interesting :man_shrugging:
```

---
## \#16 Posted by: Gamer43 Posted at: 2019-02-27T18:56:38.416Z Reads: 78

```
The ESC is also a three-phase full bridge rectifier (thanks to the MOSFET body diodes); you will feel braking torque (equal to your acceleration) kick in at your boards max speed (+ ~1.4V), meaning you cannot exceed the max speed of your battery+motor+gearing by very much because the motor acts as a generator and the ESC rectifies the BEMF and sends current back into the battery. If you attempt to brake while this is happening, you might run into overvoltage conditions and possibly overcurrent conditions.
It is best to avoid these conditions, as at higher speeds, more power needs to be returned into the battey.
```

---
## \#17 Posted by: Vanarian Posted at: 2019-03-07T21:31:18.106Z Reads: 59

```
[quote="venom121212, post:8, topic:85567"]
Shameless pitch for @hyperIon1’s rheostatic brake
[/quote]

Got a link for that thing ?
```

---
## \#18 Posted by: venom121212 Posted at: 2019-03-07T22:04:54.066Z Reads: 57

```
Of course
https://www.hyperionesk8.com/products/rheostatic-brake-dynamic-brake-for-escs
```

---
## \#19 Posted by: Vanarian Posted at: 2019-03-08T13:47:14.736Z Reads: 41

```
Thank you ❤️
```

---
## \#20 Posted by: Nedtrampz Posted at: 2019-03-08T14:08:56.555Z Reads: 35

```
Tell that to my 45kmph dh dude aha. My setup only gets me 37kmph.. tops! 

Thanks for trying tho i guess...
```

---
## \#21 Posted by: Nedtrampz Posted at: 2019-03-08T14:11:28.998Z Reads: 36

```
Ok man thats great but will it harm the esc doing this? I have no dramas slowing down manually before hitting the brakes.
```

---
## \#22 Posted by: Nedtrampz Posted at: 2019-03-08T14:19:57.197Z Reads: 36

```
What if u just slowed the regen rate right down. I know it would effect braking but it would protect the battery for sure
```

---
## \#23 Posted by: Battosaii Posted at: 2019-03-08T14:22:46.621Z Reads: 36

```
Where would you wire that? Before the ESC? Is it just an array of capacitors? I want to know how it works lol
```

---
## \#24 Posted by: Deckoz Posted at: 2019-03-08T14:37:06.243Z Reads: 34

```
its probably a brake chopper circuit
```

---
## \#25 Posted by: venom121212 Posted at: 2019-03-08T14:43:56.294Z Reads: 33

```
Yep before the esc in parallel with battery. I just used a parallel xt60 connector. They're set to 57v so anything over that sent back to the battery for regen will bleed out through the rbrake circuit instead of blowing your battery or bms limits and leaving you without brakes on a hill.
@hyperIon2 knows most about it.

I can't recommend these guys enough. The customer feedback and innovation I've seen so far has been top notch. Both batteries I have built by them are extremely high quality and have built in charge port fuses (this is a necessity in any battery build). Keep an eye out for these guys this year.
```

---
