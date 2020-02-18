# First Build with $800 Budget

### Replies: 10 Views: 1262

## \#1 Posted by: jonatduarte147 Posted at: 2016-10-18T09:15:27.923Z Reads: 178

```
I've been reading and researching and I'm still super confused on a lot of the mechanical and electric jargon. Any help with this build would be greatly appreciated! I will be building my own board with 9" Caliber trucks and 83mm flywheels from ebay. I will be using this board to commute to school and work so the most important thing for me is range. I would prefer li-ion batteries because I've read that they are less prone to explode. Would an integrated BMS be possible in my budget? My area has moderate hills, so would a dual motor system be a good choice? I am also clueless on motor mounts and the pulley system. I read all of the stickied beginner guides but I'm still not sure about ESCs and how many I would need. There is a lot I am unsure about and would love some input. Thanks!
```

---
## \#2 Posted by: TarzanHBK Posted at: 2016-10-18T09:50:28.321Z Reads: 172

```
how heavy are you?
800 is not that much to build a dual.
liion with bms should be in your budget. Ask @barajabali for a custom made pack.

For a single drive:
go with a 190kv motor, like a 6374 + 10s battery + VESC + 12 or 15mm drivesystem

Depending on how heavy you are and how much you want to spend, go dual:
2x 190kv 6355 + 10s Battery + 2x VESC + 9mm drivesystem

These are standards, of course you can vary some parts, to serve your needs :+1:
```

---
## \#3 Posted by: jonatduarte147 Posted at: 2016-10-18T15:35:51.208Z Reads: 145

```
Thanks so much for the input! I weigh about 130lbs. Is the number of VESCs parallel to the number of motors? Like one VESC per motor?
```

---
## \#4 Posted by: NickTheDude Posted at: 2016-10-18T15:43:12.790Z Reads: 134

```
Yeah it's one VESC per motor. I'd definitely recommend single drive for your budget if you don't have too many hills to conquer. For dual drive you'll need twice the VESC's, pullies and mounts. 192kV 6374 SK3 if hills aren't a big deal. If they are go with the 149kV version. Definitely run in 12S. What kind of range/top speed were you aiming for?
```

---
## \#5 Posted by: jonatduarte147 Posted at: 2016-10-18T16:07:53.959Z Reads: 126

```
A top speed around 20mph would be nice. My area has decent hills, so the 149kV would be better for that? Would a single motor be able to get me up those hills? What capacity should the battery be if I'm looking for around 10-13 mile range? If there are any tools I can use to calculate this myself, I'd love to know them. Thanks for all the help!
```

---
## \#6 Posted by: Quinlanbrown Posted at: 2016-10-18T16:20:15.685Z Reads: 116

```
I have a single sk3 6374 and I can go up big hills no problem Ill be going up something really steep at like 10mph but I'm vesc starts go get to hot ad slow down so getting one with a heat sink would help I'm Gona build one
```

---
## \#7 Posted by: NickTheDude Posted at: 2016-10-18T16:47:39.801Z Reads: 118

```
To calculate top speed use this website: http://calc.esk8.it/

The VESC has a limit of 60,000 ERPM. And these motors are most efficient at higher RPM, so when designing you're board with that calculator, aim for 60,000 ERPM. 190kV with 12S gets pretty much spot on. After that you can alter your gear ratio to fit your top speed. Lower top speed will mean more torque, and better hill climbing ability.

Now, to calculate range, you need to determine the watt hours of you battery pack. Wh is equal to amp hours multiplied by voltage. 

For example a lithium-ion pack with 3Ah per cell, and 12 cells in series with 2 cells in parallel (12S2P) would have (12 x 3.7) x (2 x 3) = 266.4 Wh. 3.7 is the nominal voltage of a lithium ion cell.

A general estimation that people have come up with is that 10Wh will give you 1km of range. So I'd go with a single 192kV SK3, and a 12S battery pack, gear to fit the top speed you're aiming for, and pick your amount of cells in parallel to fit the range you need.
```

---
## \#8 Posted by: jonatduarte147 Posted at: 2016-10-18T22:15:01.092Z Reads: 96

```
So I've been looking at different prices and parts all day and I really feel like getting the space cell pro 3 would be the best way for me to go. I just don't want to worry about the battery, just plug and go. Here are the other parts I've found.

* Enertion Motor Mount ~ $60
* Turnigy Aerodrive 190kV SK3 Motor ~ $80
* Enertion VESC Standard ~ $100 -150
* Enertion 9mm wide drive pulley kit ~ $40
* Space Cell Pro 3 ~ $350

The base board I'm making will be about $130, so this should bring the total to about $760 to $810. I would still need to buy a remote and this will send me a little over budget which is fine. Any remote recommendations that are small and reliable?

I used the calculator and the top speed would be around 20mph and the Space Cell Pro 3 description says an 30km/18 mile range. Is this correct? 

I would appreciate any more feedback and thanks for all the input provided already!
```

---
## \#9 Posted by: TarzanHBK Posted at: 2016-10-19T07:35:53.840Z Reads: 79

```
you´ll be fine with a single motor at your weight.
But if you like to get a Enertion pulley kit, go for 12mm!
9mm is for dual drives.
```

---
## \#10 Posted by: jonatduarte147 Posted at: 2016-10-19T18:35:15.890Z Reads: 69

```
I'll get the 12mm then! Will this set up be fairly "plug and go" or will there be any soldering or anything else needed? I don't have soldering experience but my brother does. Are there any connectors I need to buy? Also, I've decided to switch to this battery instead of the space cell to bring costs down.

http://www.electric-skateboard.builders/t/meb-dirty-dervish-12s-stealth-battery-twin-esc-hub-motor/5104/37
```

---
