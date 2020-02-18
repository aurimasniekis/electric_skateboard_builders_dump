# New build help on parts

### Replies: 9 Views: 938

## \#1 Posted by: Tricky Posted at: 2016-07-11T14:30:32.919Z Reads: 87

```
Hello to all 
Well this will be my 1st bord build I'm in the UK with not a lot of hills, the bord regarding performance I'd like a bit of both torq and speed, it will be a duel build, but I'm hoping you can all put me on the right track, parts I'm looking at 
Hobby King
2 x Sk3 245kv motors what size trucks will I need with the 2 motors ?
I'd like to ride the bord for an hour or more, and was looking at the zippy battery's, but don't no what or how many will do, also pully kits or parts, wear to order in the UK or other?
And what about the vesc a reliable one, or do I have to use 2??
Any help please with links to parts
Thanks Rich
```

---
## \#2 Posted by: Brando Posted at: 2016-07-11T14:51:44.353Z Reads: 84

```
If your want good battery life with duel motors, you should aim for around 10,000mAh. You can increase mAh by hooking batteries up in parallel. Keep in mind, 11.1V 3S 5000mAh batteries in parallel will give you 10,000mAh, but the voltage will still be 3S 11.1V, which will be pretty slow (around 10mph). If you want to increase volts to 6S 22.2V, you need to wire the batteries in series, but then it will still be at 5000mAh. So I would just buy four Zippy 3S 5,000mAh packs and have two pairs of batteries in series and then put those two pairs in parallel with each other. This would get you a 6S 10,000mAh at 22.2V for speed and range. I dont know how much you know about electronics but I can make a diagram for you if you want.
As for the vesc's, you will need one for each motor.
I dont know much about the mechanical parts like trucks so I just bought a mech kit that came with trucks, pullys, gears, risers, bolts, wheels, and a motor mount. Here is the mech kit: diy-electric-skateboard-kits-parts/torqueboards-single-motor-mechanical-kit/
BTW having four batteries can get messy with carging, so you would go with only two 3S 8000mAh in series which would give you 6S for speed and 8000mAh for ~10 miles of range
```

---
## \#3 Posted by: Tricky Posted at: 2016-07-11T18:53:00.730Z Reads: 61

```
Hi thanks for that, if you don't mind yes please for that diagram regarding the battery's 
Thanks again Rich
```

---
## \#4 Posted by: IanSwitz Posted at: 2016-07-12T02:24:49.970Z Reads: 47

```
Youll have too use 2 vescs if you want two motors.
```

---
## \#5 Posted by: XvDarkVAngelvX Posted at: 2016-07-12T03:09:18.623Z Reads: 43

```
What would be a great ESC with R-spec Dual 190kv motor?
```

---
## \#6 Posted by: Tricky Posted at: 2016-07-12T06:02:13.094Z Reads: 31

```
Why would the 190kv be so good, can you explain please
```

---
## \#7 Posted by: XvDarkVAngelvX Posted at: 2016-07-12T08:30:39.531Z Reads: 28

```
Was asking maybe someone would tell me. I do know that 190kv would be good for torque more than speed. Great for inclines. 👌
```

---
## \#8 Posted by: Brando Posted at: 2016-07-13T14:46:04.287Z Reads: 22

```
This is my design. I have two 3S 5000mAh batteries in series which gives me a 6S 5000mAh total.
That bit of the circuit with the loop key and XT90 is just my way of disconnecting the circuit. That can be replaced with a traditional on off switch.
Sorry for the late response, I thought I had notifications turned on for this thread😭
<img src="/uploads/db1493/original/2X/3/35d772a9cdff2c34a2ddb698fa4f4e3e1bfbc623.png" width="690" height="312">
```

---
## \#9 Posted by: Brando Posted at: 2016-07-13T14:54:50.177Z Reads: 20

```
Motor kV rating indicates how fast the more will spin. As @XvDarkVAngelvX said, lower kV will be more torque, but will be slower. 190kv is a pretty good speed, but I opted for a 230kv because my area is not to hilly, and I need as much speed as I can get because I only have a 6S battery setup.
As for the ESC, most will recommend a vesc, but it will have to be programmed with a computer and special power supply, so you need to be tech savvy. I was lazy and just got DIY's 6S ESC and the $15 programming card. This way I can easily set settings like acceleration and speed on the go and I also saved some money.
My esc: diy-electric-skateboard-kits-parts/single-motor-120a-6s-esc/
Esc east programming card: diy-electric-skateboard-kits-parts/torqueboards-esc-programming-card/
```

---
