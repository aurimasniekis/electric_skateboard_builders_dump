# Budget build that can go uphill

### Replies: 11 Views: 1768

## \#1 Posted by: timmcgimpsey Posted at: 2017-05-19T04:53:42.799Z Reads: 154

```
Hi
First, if i am asking any stupid questions that have already been answered, please tell me!!! Also a link to the threads would be helpful.
Anyway i am aiming to build a long board that is fairly cheap to get me to work and back. Unfortunately, i live on top of a hill. It is a pretty constant 10-15% grade with some 20% bits. The climb is about 700m long.
I have decided on either a single motor board with a 6374 192kv motor on 12s, (or 9s) with a vesc, or a dual setup with 6355 190kv motors on 6s with cheap rc car esc's. Which of these setups be better for climbing hills? at this stage i am leaning towards the dual motors. I am not to worried about top speed, but 20 Mph would be nice. I am about 70kg.
I dont really want to spend much more than 300 usd on this project, but i already have 8 3s 8000MAh lipos from another project, and i already have a longboard. I plan to make the the motor mount(s) myself which wont cost very much.
Any ideas other people have would be much appreciated.
Thanks
Tim
```

---
## \#2 Posted by: aigenic Posted at: 2017-05-19T07:20:56.118Z Reads: 140

```
Ok...so you weight 70kgs...6374 shoul be ok on 12s, maybe even 9s...try this calculator, it is a little old, but if you will be patient you can get your max incline from it: 
http://www.elektro-skateboard.de/wiki/wissenswertes/strom-spannung-reichweite-vii

300 USD is not much...you wont get in this budget with dual...Maybe if you have a skateboard with useable trucks already...

Dual motors are certainly more powerful than single and better for hill climbing, but they cost much more...

Making your own mounts might be difficult if you are not skilled, try using tested types of mounts like the enretion motor mount or DIY's. If your trucks hasn't square or hexagonal axles than I would choose a mount similar to APS (alien power systems) because in case you wouldnt be able to mount it properly, you can just weld the round part that goes on the truck and you are done :)

Also check if your C rating on the batteries is high enough...

_Sorry for my English :/_
```

---
## \#3 Posted by: timmcgimpsey Posted at: 2017-05-19T07:57:12.327Z Reads: 128

```
Hi, Thanks for the reply. That calculator is really useful!
I should be fine on a single 6374 motor.
I have decided to use a single motor on 12s with a vesc, and if it doesn't have enough power I can upgrade to a dual motor system in the future.
I have access to a CNC mill and I have reasonable cad skills so I'll use that to make the mount. My trucks are callibre 2, so Im going to use a clamp design.
Thanks for all your help
Tim
```

---
## \#4 Posted by: bartroosen12 Posted at: 2017-05-19T09:19:11.093Z Reads: 114

```
I guess a vesc on 12S must be a good option, you will have like 2000W-2500W which must be enough.
What kind of batteries do you have, because if you got 8 packs that would be perfect to make a 12S2P 16Ah. That will be a sick battery! Pretty nice man
```

---
## \#5 Posted by: timmcgimpsey Posted at: 2017-05-19T09:37:30.164Z Reads: 113

```
 They are just cheap Zippy Flightmax 3s 8000Mah batteries from hobbyking.  They are what I use on my Camera drone.
At 600g a peice, im not sure if I want 8 of them on the bottom of my longboard!
If I want that many Wh, I think I'll invest in some 18650 li-ion cells to keep the weight down.
```

---
## \#6 Posted by: pennyboard Posted at: 2017-05-19T09:46:54.567Z Reads: 111

```
If you want to keep your budget under $300, I think you can do it. You mentioned already having trucks, the longboard, and the batteries. I say definitely use the batteries you have, and you should only need 4. I use 4 zippy 3s 5000mah lipos on my board and get 14 miles of range, so with 4 of your 8000 mah batteries, you should see around 20 miles, and all 8 on the board (which would be 12s2p), would get you around 30-40 miles, which is way more than you reasonably need.

Assuming you machine the motor mount yourself, you'd need gearing for the wheel and motor ($46 from torque boards), a motor (~$70 on hobby king or $90 from torque boards), a vesc ( $100 for torque boards vesc), a controller (GT2B on amazon $25), flywheel clones ($25 on amazon) and miscellaneous wiring and enclosure stuff. 

Should be do-able in around $300, just make sure you get really low gearing to climb hills on a single. With 12s batteries, you could go as low as 10/36T gearing, which would give you insane torque, especially if you have a 6374 motor, and you'd still have a 22 mph top speed with that 10/36T gearing.
```

---
## \#7 Posted by: DeathCookies Posted at: 2017-05-19T10:40:29.733Z Reads: 92

```
If he wants to use 10/36 he probably Needs a idler
```

---
## \#8 Posted by: pennyboard Posted at: 2017-05-19T16:42:35.500Z Reads: 87

```
What's the reason behind that? Is it just to push the belt down to that it makes contact with more of the teeth on the 10T pulley? I've gone 10/36T before without an idler and it was fine.
```

---
## \#9 Posted by: timmcgimpsey Posted at: 2017-05-24T08:50:36.464Z Reads: 74

```
I have another quick question, 
I really like the look of boosted boards with 2 separate battery cases at each end. If I go with a dual diagonal setup, can I have a separate battery and vesc/esc at each end of the board and only joined together by a servo cable for receiver? Are there any issues with throttle response with long receiver cables?
Thanks
Tim
```

---
## \#10 Posted by: TarzanHBK Posted at: 2017-05-24T08:55:32.752Z Reads: 73

```
teeth skipping. I have an 13t motor pulley without idler and do have skipping sometimes. So aim for 6 or more teeth in mesh
```

---
## \#11 Posted by: pennyboard Posted at: 2017-05-24T14:45:32.720Z Reads: 62

```
Ah that makes sense. Yeah I run a 13T without idler and have teeth skip sometimes when braking down hill. Any advice on how to install an idler pulley on torque boards motor mount?
```

---
