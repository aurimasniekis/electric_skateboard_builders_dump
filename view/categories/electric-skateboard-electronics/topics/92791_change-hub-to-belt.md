# Change hub to belt

### Replies: 14 Views: 321

## \#1 Posted by: rod_r Posted at: 2019-05-04T22:56:41.907Z Reads: 124

```
I've searched this but can't find a direct answer.
I have a prebuilt running a single 70mm hub off a 7s battery. All I know about the hub is that it's 400w, and I don't know the kv rating.

Thinking of switching to a single belt so I can use better wheels and go up to 80 or 85mm. Because this is such a low spec setup, I can't afford to lose speed or torque. I know bigger wheels generally mean more speed, less torque, but I can't get a handle on how the two will differ running off my battery.

All I really know is that I need to make sure the motor is rated for 25.2v and will probably by a 5065 and that I'll probably need something at the low to mid range kv rating.
```

---
## \#2 Posted by: ZachTetra Posted at: 2019-05-04T23:08:18.038Z Reads: 118

```
If it's a prebuilt than the ESC will be made for hub motors (always in the 50-150kv range), if you run a belt off it than you're probably going to exceed the ERPM limit and the board will cap at low speed

Recommendation is get a new ESC to go with the motors and wheels, you can go cheap and dirty with a non programable ESC and motor kit which will set you back about $150 brand new (ESC, remote, trucks, mounts, motors, belts, pulleys, wheels all assembled and shipped) or you can do DIY and get a pair of Caliber II style trucks and mount to carry a motor of choice and a VESC to run it but you pay more for control, customization, and quality

Cheapest I can find are these $125.62...it won't be long for this world but it'll go

($81.41) https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F372613215069

($44.22) https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F223429431642
```

---
## \#3 Posted by: rod_r Posted at: 2019-05-04T23:44:20.582Z Reads: 90

```
Thanks. That's great info. Wasn't thinking about ERPM, although have just recently read about that.

A while ago I went the other way and turned a 10s prebuilt 80mm belt drive into a 90mm hub from DIYelectric but it lost too much torque.

Assuming I change out the esc, do you have an opinion on how the belt system will compare for torque and speed, assuming say 80mm wheels?

Edit. Looked at the links. I have been looking at thouse but wasn't sure if they were compatible. Only issue I have is the wheel pulley probably won't work with decent wheels like Abec so partially defeats the purpose of doing it to get nicer wheels
```

---
## \#5 Posted by: ZachTetra Posted at: 2019-05-04T23:57:33.528Z Reads: 74

```
If you get the dual version it will feel better and you can swap wheels, otherwise you'll need a pulleys with the same teeth profile and count to replace it, if you get new belts you can change the ratio

Performance is dependent on the voltage, kv, ratio, and diameter, you can get speed in exchange for torque but the max power is capped
```

---
## \#6 Posted by: professor_shartsis Posted at: 2019-05-05T01:45:45.926Z Reads: 55

```
[quote="rod_r, post:1, topic:92791, full:true"]
I’ve searched this but can’t find a direct answer. I have a prebuilt running a single 70mm hub off a 7s battery. All I know about the hub is that it’s 400w, and I don’t know the kv rating.

Thinking of switching to a single belt so I can use better wheels and go up to 80 or 85mm. Because this is such a low spec setup, I can’t afford to lose speed or torque. I know bigger wheels generally mean more speed, less torque, but I can’t get a handle on how the two will differ running off my battery.

All I really know is that I need to make sure the motor is rated for 25.2v and will probably by a 5065 and that I’ll probably need something at the low to mid range kv rating.
[/quote]

Suppose you want to optimize for climbing 5% slopes at max possible speed with 250lbs rider + board, (1) 190kv motor, 0.05ohm, 30a battery current limit, 25.2v battery voltage, 85mm tires:

https://i.ibb.co/19kfRrn/7s-85mm.jpg

^then 2.09:1 is a good gear ratio for 20.23mph up 5% slopes (21.66mph no load wheel speed).

https://i.ibb.co/JzPfSG9/7s-85mm-190kv.jpg

^on the left it shows "how fast you could go" in mph at the optimal ratio... the right chart shows which ratio you need to achieve that maximum possible up slope speed.
```

---
## \#7 Posted by: rod_r Posted at: 2019-05-05T02:32:43.316Z Reads: 48

```
That's fantastic. thanks for that info.

I used the esk8 calculator and it seems the only variable that changes the erpm [ mentioned in the other guys answer ] is the kv rating, so it seems to me i could change to a belt system of any ratio and wheel size so long as i make sure the new motor does not exceed the existing motor kv., [ although i completely understand how you show a ratio of 2.09:1 is a good setting...even if im ony 158 lbs ].

I found my battery/esc online as a pack and it doesn't specify hub or belt.

EDIT: ok, now i see based on the spec of my board, the hub must be very low kv, probably lower than any decent belt motor
```

---
## \#8 Posted by: professor_shartsis Posted at: 2019-05-05T03:49:51.584Z Reads: 45

```
[quote="rod_r, post:7, topic:92791"]
I used the esk8 calculator and it seems the only variable that changes the erpm [ mentioned in the other guys answer ] is the kv rating, so it seems to me i could change to a belt system of any ratio and wheel size so long as i make sure the new motor does not exceed the existing motor kv.
[/quote]

well you can see from this comparison of some typical hubs (73kv, 84mm tire) vs belts (190kv, 100mm tires), the only requirement necessary to achieve nearly identical performance characteristics from either system is the correct gear ratio with geared systems and the correct tire size with the hubs.

https://forum./uploads/default/optimized/2X/9/97cd2cde4b2d17806940f8afdd09e5e2ade6af78_2_1054x998.gif
```

---
## \#9 Posted by: b264 Posted at: 2019-05-05T05:06:29.708Z Reads: 36

```
You don't really have a clear upgrade path with china hub motors, except for changing everything but the battery.
```

---
## \#10 Posted by: rod_r Posted at: 2019-05-05T05:17:33.279Z Reads: 35

```
Yeah, that's becoming apparent. I thought there might be some room to swap but probably the only reusable item is the battery, and even that's not ideal. Probably better to use until it breaks and maybe start making a diy list
```

---
## \#11 Posted by: professor_shartsis Posted at: 2019-05-05T14:31:10.391Z Reads: 29

```
[quote="rod_r, post:10, topic:92791"]
I thought there might be some room to swap but probably the only reusable item is the battery, and even that’s not ideal.
[/quote]

you can get roughly the same performance you have with the hub now using a higher kv motor, bigger wheels and switching hub to belt-- all you should have to do is set the gear ratio with the higher kv, belt and bigger wheels such that you have the same no load wheel speed (mph) as you have now with the hub. the higher kv and gear reduction will make a same-size motor slightly more efficient giving slightly longer range-- this is because increasing the kv with a same-size motor lowers the electrical resistance. or the higher kv could give slightly higher theoretical performance-- this can be seen in the moving chart above (the higher kv lower resistance motor can propel a rider to a slightly higher peak theoretical top speed on a given slope). this theoretical "speed boost" by using a higher ~190kv motor instead of a lower ~73kv hub is on the order of a less than 1mph increase in peak theoretical top speed for a given slope (assuming optimal gearing or tire size for that slope) on a typical 2-motor board that is carrying a person.
```

---
## \#12 Posted by: AlanZhou Posted at: 2019-05-05T14:33:05.571Z Reads: 22

```
[quote="ZachTetra, post:2, topic:92791"]
50-150kv range
[/quote]

50-130 kv 😉
```

---
## \#13 Posted by: rod_r Posted at: 2019-05-05T20:16:42.556Z Reads: 16

```
Really appreciate this info. I see how that works. Finally, is the wheel size vs gear ratio a sliding scale.? I was looking at 85mm wheels, so guessing the ratio would drop to approx 1:1.5
```

---
## \#14 Posted by: professor_shartsis Posted at: 2019-05-05T20:23:58.958Z Reads: 16

```
![image|520x500](upload://4HRJDpJohwV0oIZLaRo2jfJ1aRt.jpeg)

^this one is for 85mm tires, 25.2v, 190kv single motor (tire size shown in the top right)
```

---
## \#15 Posted by: professor_shartsis Posted at: 2019-05-05T23:49:33.766Z Reads: 12

```
[quote="rod_r, post:7, topic:92791"]
even if im ony 158 lbs
[/quote]


the difference 50lbs makes (200lbs vs 250lbs):

https://i.ibb.co/0cJ0yvg/50lbs.gif
```

---
