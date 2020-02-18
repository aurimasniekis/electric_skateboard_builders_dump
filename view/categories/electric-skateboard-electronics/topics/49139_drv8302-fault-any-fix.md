# DRV8302 Fault&hellip; Any Fix?

### Replies: 21 Views: 833

## \#1 Posted by: Snowi Posted at: 2018-03-15T00:11:33.825Z Reads: 118

```
I already checked for burn marks... nothing. Checked for punctures in wires, nothing. Is this something I can fix or need to be replaced?
```

---
## \#2 Posted by: abenny Posted at: 2018-03-15T00:12:34.984Z Reads: 117

```
you'll probably want to post close up pics and summon the wizard...
@JohnnyMeduse
```

---
## \#3 Posted by: Snowi Posted at: 2018-03-15T00:14:23.460Z Reads: 114

```
close up pics of what exactly?
```

---
## \#4 Posted by: E1Allen Posted at: 2018-03-15T00:15:29.569Z Reads: 113

```
The vesc. Specially the drv chip
```

---
## \#5 Posted by: Snowi Posted at: 2018-03-15T00:15:42.582Z Reads: 113

```
which one is that? lol
```

---
## \#6 Posted by: E1Allen Posted at: 2018-03-15T00:19:03.698Z Reads: 109

```
![IMG_4598|281x500](upload://9Cly3VU165ju98gDJSsgV7ZeBsU.jpg)
```

---
## \#7 Posted by: bevilacqua Posted at: 2018-03-15T09:45:23.497Z Reads: 88

```
Is it when braking? Witch ESC Brand? FOC or BLDC mode?

I solved mine with this (on FOC): 
http://vedder.se/forums/viewtopic.php?t=68
```

---
## \#8 Posted by: Snowi Posted at: 2018-03-15T13:50:28.796Z Reads: 76

```
I think the skateboard stopped working when I was about to brake. I used diyelectricskateboard's VESC. And I used BLDC
```

---
## \#9 Posted by: bevilacqua Posted at: 2018-03-15T14:04:31.436Z Reads: 70

```
You can still connect it to the Vesc-Tool right?
```

---
## \#10 Posted by: trancejunkiexxl Posted at: 2018-03-15T14:04:53.390Z Reads: 70

```
make sure to include a screen shot of your setting if you can, could speed things up getting it diagnosed..
```

---
## \#11 Posted by: Snowi Posted at: 2018-03-16T01:21:58.973Z Reads: 60

```
What do you want me to screenshot?
```

---
## \#12 Posted by: RedEagle Posted at: 2018-03-16T01:24:28.280Z Reads: 60

```
Your motor and pwm settings.
```

---
## \#13 Posted by: Snowi Posted at: 2018-03-17T17:33:01.334Z Reads: 51

```
Sorry for late response but this is my motor and pwm settings
![image|690x406](upload://yqaESaJnzeVZeizp0qtvX0L1MF2.png)
![image|690x405](upload://xQEOW68x7bOwiJg00NTUtaMq7Wk.png)
![image|689x409](upload://d6iklC8tAtixbDFeja2HWlI8hRV.png)
```

---
## \#14 Posted by: Acidfie Posted at: 2018-03-17T23:50:14.277Z Reads: 41

```
ERPM Limit to 100'000. Keep it at 60'000.
```

---
## \#15 Posted by: RedEagle Posted at: 2018-03-18T00:13:47.912Z Reads: 39

```
[quote="Acidfie, post:14, topic:49139, full:true"]
ERPM Limit to 100’000. Keep it at 60’000.
[/quote]

As stated set the erpm limit to 60.000. Everything else seems fine.
What are the specs of your board? Upload a pic of the vesc & the motor advanced tab.
```

---
## \#16 Posted by: Snowi Posted at: 2018-03-18T00:21:06.841Z Reads: 37

```
I got two turnigy 5000 20C batteries connected in series, turnigy 213kv 6364, and diy vesc 4.12

![image|690x379](upload://tzlzCYuA5Le3Zi3C6LOh5lGy1eC.png)
```

---
## \#17 Posted by: RedEagle Posted at: 2018-03-18T00:31:55.794Z Reads: 35

```
Your settings are okay. Although your batt max settings are a bit low in my opinion. Does the motor spin when you push throttle?

You have three options:
1. Solder on another drv yourself
2. Let somebody else repair it for you, like @JohnnyMeduse 
3. Buy a new vesc
```

---
## \#18 Posted by: Snowi Posted at: 2018-03-18T00:50:02.871Z Reads: 34

```
There is no way of fixing it without modifying or repairing the physical VESC?
```

---
## \#19 Posted by: RedEagle Posted at: 2018-03-18T00:51:45.315Z Reads: 34

```
You'll have to replace the drv chip on the vesc. If you have experience with soldering you can try it yourself.
```

---
## \#20 Posted by: Acidfie Posted at: 2018-03-18T08:39:22.695Z Reads: 27

```
DIY VESC? 




10char
```

---
## \#21 Posted by: bevilacqua Posted at: 2018-03-18T09:18:01.381Z Reads: 24

```
Maybe try the fix I mentioned in my first post (C18-Mod), if it doesent work ship it to a repair guy.
```

---
