# Not getting enough torque up hills, small c rating?

### Replies: 13 Views: 730

## \#1 Posted by: Quinlanbrown Posted at: 2016-09-30T03:17:07.450Z Reads: 148

```
im running 4 zippys in searies pretty much the battery's everyone uses and when i start going up hills its fast at first then starts slowing down should i buy batteys with a higher c rateing mine are 10c 20c peak
```

---
## \#2 Posted by: Pathaim Posted at: 2016-09-30T03:19:00.210Z Reads: 148

```
what is the mah on your batteries? and what motor do you have, i run 10c multistar batteries and my hill climbing is fine. also do you have single or dual motors?
```

---
## \#3 Posted by: Quinlanbrown Posted at: 2016-09-30T03:29:51.017Z Reads: 144

```
i have a single sk3 6473 and im running 4 5000mah 3s
```

---
## \#4 Posted by: VladPomogaev Posted at: 2016-09-30T03:34:58.756Z Reads: 139

```
In series or in parallel? What's your voltage? What kind of motor are you using, and controller? I think we need more info please :)
```

---
## \#5 Posted by: mattdig Posted at: 2016-09-30T05:23:26.427Z Reads: 129

```
It might not be the batteries. What's the Kv of the motor, the gear ratio, wheel size, and your weight? Also what ESC are you using?
```

---
## \#6 Posted by: saul Posted at: 2016-09-30T09:33:17.798Z Reads: 114

```
4x 3s in series so 12s on 6374. I have the same motor 149kv and the same multistar 10c 5200mah packs. 

hills are fine for me but I do get slowed on long ones, i think its the vesc heat protection but not sure.

are you using vesc? what are you settings? details....
```

---
## \#7 Posted by: Quinlanbrown Posted at: 2016-09-30T12:06:50.303Z Reads: 99

```
192kv with 16t 32t and 97mm wheels but the thing is it will go up really steep hills fine then start slowing down even when I get to the top and it's flat there's not the tork is should have untell I give it a second
```

---
## \#8 Posted by: Quinlanbrown Posted at: 2016-09-30T12:09:07.672Z Reads: 95

```
I have 192kv but ya it must be the vesc, I couldn't program it but I'll try again also Imite get a heat sink for it with the setup I have I'm pretty much maxing it out
```

---
## \#9 Posted by: mattdig Posted at: 2016-09-30T14:02:54.442Z Reads: 84

```
You have a very high gear ratio and wheel size but also a low Kv motor so it might balance out. I think you're right, the VESC is overheating and just taking a couple of seconds to cool down. When my ESC overheats it at least beeps through the motor to tell me. Is there a setting to make it do that?
```

---
## \#10 Posted by: mattdig Posted at: 2016-09-30T16:35:55.474Z Reads: 71

```
You could also think about reducing your wheel size or gear ratio. Maybe drop to 90mm or 83mm wheels. You'll loose some top speed but if long hill climbing is important to you it will help a lot.
```

---
## \#11 Posted by: Titoxd10001 Posted at: 2016-09-30T16:55:12.773Z Reads: 65

```
Your gearing seems way to high for 97mm wheels. What speed are you getting like 45mph? You want to gear for the fastest youll ever go or even lower. So you should get a 40t wheel pulley for a speed of 35mph. Or get a 44t if you want to get one 3d printed. Also you may have to play with vesc settings for example my vesc was heating up because my settings where to high. If you want scary climbing ability though i think dual would be the way to go.
```

---
## \#12 Posted by: SteveS Posted at: 2016-09-30T16:58:24.168Z Reads: 62

```
I was having the same problem lat the top of long hills, but gearing down and getting heat sinks for the VESC solved  it.
```

---
## \#13 Posted by: saul Posted at: 2016-10-01T11:56:46.148Z Reads: 52

```
wow your gearing is really high.

I have a 149kv on 12s, 97mm wheels but 14/36!
i just put on some 80mm kegels and the torque is scary again :upside_down: but it actually over heats more on hills it seems...I think too many amps with the higher rpm...

the sweet spot might not be the highest..but yea way too fast of gearing to do hills...
```

---
