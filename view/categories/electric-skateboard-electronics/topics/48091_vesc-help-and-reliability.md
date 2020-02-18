# VESC Help and Reliability

### Replies: 10 Views: 626

## \#1 Posted by: mervmonster Posted at: 2018-03-04T02:07:25.737Z Reads: 78

```
Greetings, I am having some issues with VESCs and need some advice. Originally I had a 2 motor board that was geared a little too high (16 tooth motor-36 tooth wheel) but it was fast and fun. One of the DRV chips burnt out and I had that replaced. While I was waiting for it to be replaced I took the second motor off and road as a 1 wheel drive board. This quickly burnt out the second VESC. The VESC control software isn't showing any faults so I don't know if its repairable. Is there a way to improve reliability?
Any help is appreciated.
Setup: 
16 tooth motor, 36 tooth wheel
2 6355 230KV Torque Boards motors
2 VESCS from diyelectricskateboards
1 6s battery and 1 12s. I would switch back and forth.
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2018-03-04T02:13:44.691Z Reads: 74

```
Only first you burning your drv has nothing to do with your gearing  ratio and more to do that u ran 230kv at 12s and passed the erpm  of the vesc and blew the dvr
```

---
## \#3 Posted by: Lumaci Posted at: 2018-03-04T02:14:36.986Z Reads: 73

```
The gearing is fine, its the KV rating of your motors, for 6s its okay but 12s no.
```

---
## \#4 Posted by: NickTheDude Posted at: 2018-03-04T02:19:54.197Z Reads: 69

```
It's hard to say what problems you're having without knowing your VESC settings. The VESC is only as unreliable as you make it.
```

---
## \#5 Posted by: ThermalM16 Posted at: 2018-03-04T03:28:29.423Z Reads: 64

```
What symptoms is the second VESC having that is not showing any faults? Does it power up?
```

---
## \#6 Posted by: ZackoryCramer Posted at: 2018-03-04T04:11:32.378Z Reads: 53

```
[quote="mervmonster, post:1, topic:48091"]
2 6355 230KV Torque Boards motors
[/quote]

I wouldn't use 12s on motors with more than 200kv since they could break the erpm limit. Could be the reason why. :thinking:
```

---
## \#7 Posted by: Eboosted Posted at: 2018-03-04T04:47:43.890Z Reads: 44

```
Where you runing in FOC? Of you blew on VESC why you kept using the board? Why you didn't stop, uses the 6S battery and try to replace your motors for a lower kv one or you battery from 12S to 8S?
```

---
## \#8 Posted by: mervmonster Posted at: 2018-03-04T06:06:53.158Z Reads: 41

```
Eboosted. When the ESC blew, I did only use the 6S battery. This is a commuter board and my bike got stolen so I was trying to use it until I could find a decent deal on a bike. 

ThermalM16. The software connects to it and thinks everything is fine. When I try the throttle, the red light blinks three times and the motor does not turn. 

For settings, I was running the VESC stock settings that it came with but I adjusted the voltage cutoff to be higher. I was thinking about running FOC but I heard it was hard on the VESCs. I was also running dual using a servo splitter and not CANBUS because I couldn't get that to work. 

It sounds like in the future I should only run 6s and that will solve most of my issues. I was wondering if someone could help me with the ESC settings. I seem to set it to exactly what others have and it doesn't work. I am probably making a mistake somewhere. Any help is appreciated.
```

---
## \#9 Posted by: pat.speed Posted at: 2018-03-04T06:15:35.947Z Reads: 39

```
Is it possible he got the bugged firmware with the ramp up speed too high?
```

---
## \#10 Posted by: mervmonster Posted at: 2018-03-04T06:31:15.344Z Reads: 37

```
![Config 1|690x323](upload://bVq6A9UBdpFkCwiGKJtolO1GPC.JPG)

My next move was going to be running sensored. I was trying to before all this esc frying started. Whenever I hit the sensored option for BLDC it would get no throttle.
```

---
