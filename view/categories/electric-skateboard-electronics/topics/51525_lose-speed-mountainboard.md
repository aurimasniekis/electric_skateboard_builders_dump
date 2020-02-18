# Lose speed mountainboard

### Replies: 20 Views: 717

## \#1 Posted by: Devilmycry Posted at: 2018-04-07T23:37:51.112Z Reads: 93

```
Hi 
When my  battery capacity go down my top speed to like I 100% top speed 40mph at 20% 30mph 
Can I fix this if yes 
How 
Thank you 
12s7p 30q vesc 6 2 motor sk3
```

---
## \#2 Posted by: myreala Posted at: 2018-04-07T23:42:20.137Z Reads: 91

```
I think watt control might help with the torque and acceleration at low battery but not sure if it also helps with top speed.
```

---
## \#3 Posted by: RedEagle Posted at: 2018-04-07T23:57:52.537Z Reads: 84

```
You can't increase your top speed. This has to do with how motors work. Kv is directly related to voltage. So if you have a full battery your top speed will be higher and if your battery is empty your top speed will be lower.
Example:
42v x 190kv = 7980 revolutions (higher top speed) 
36v x 190kv = 6840 revolutions (lower top speed)
```

---
## \#4 Posted by: E1Allen Posted at: 2018-04-08T00:01:39.495Z Reads: 74

```
[quote="Devilmycry, post:1, topic:51525"]
Can I fix this if yes

How

[/quote]


Charge batteries, and repeat
```

---
## \#5 Posted by: SeanHacker Posted at: 2018-04-08T00:02:13.763Z Reads: 68

```
Just as stated above. Charge your battery. Then go again. ;)
```

---
## \#6 Posted by: Deckoz Posted at: 2018-04-08T00:15:14.627Z Reads: 63

```
Or set your watt limit to your output capable at a dead battery. Then it is the same across the charge..and you won't feel as let down.. lol
```

---
## \#7 Posted by: Devilmycry Posted at: 2018-04-08T00:16:41.355Z Reads: 64

```
Ok lol 
I can do everything on the setting vesc for change
```

---
## \#8 Posted by: Deckoz Posted at: 2018-04-08T00:18:07.005Z Reads: 62

```
What's your battery?
```

---
## \#9 Posted by: Devilmycry Posted at: 2018-04-08T00:19:25.452Z Reads: 59

```
12s7p Samsung 30Q
```

---
## \#10 Posted by: Idle Posted at: 2018-04-08T00:24:06.019Z Reads: 56

```
Wait.. 

40/30 Miles or Kilometers per hour?

Please post pics of mountain board.

Thank you.
```

---
## \#11 Posted by: E1Allen Posted at: 2018-04-08T00:24:25.108Z Reads: 55

```
Yeah but then he limits his top speed. Which is no fun
```

---
## \#12 Posted by: Devilmycry Posted at: 2018-04-08T00:26:07.439Z Reads: 52

```
Is 40 miles
```

---
## \#13 Posted by: Devilmycry Posted at: 2018-04-08T00:26:24.753Z Reads: 55

```
How I can do it
```

---
## \#14 Posted by: Deckoz Posted at: 2018-04-08T00:26:43.732Z Reads: 55

```
7p *20a constant current. = 140a bat max / number of esc (ie 2 ESC is 70a battmax per..but most ESC can only handle 50)

Discharged is. 12 * 3.35 = 40.2v battery cutoff, + 1v = 41.2v battery cutoff start.

40.2v * 140a = 5628W / # of esc ( ie 2 ESC is 2814w per esc)

Batt min 3Ah * 7 = 21A * 2C = 42A batt min / # of esc (ie 2 ESC is -21a batt min.

If you went off of full charge wattage instead of end of charge wattage. It will feel like it drops

Start voltage wattage = 7056W 
End of charge wattage = 5628W.. if you set this as the watt limit the whole battery feels the same.

 Also @E1Allen there's no way with 5600 watts at dead his top speed is gonna be limited. That's alot of watts...your talking minimal speed difference I think..

I think he is thinking top speed = acceleration..
```

---
## \#15 Posted by: Devilmycry Posted at: 2018-04-08T00:32:14.988Z Reads: 49

```
No everything is good acceleration torque 
Is my top speed going down when the battery going down 
Like 100% battery I can go 40MPH when the battery go to 20% I can go just 30MPH
```

---
## \#16 Posted by: E1Allen Posted at: 2018-04-08T00:32:46.528Z Reads: 47

```
Yeah. That's just from less voltage as explained above
```

---
## \#17 Posted by: Deckoz Posted at: 2018-04-08T00:32:48.966Z Reads: 46

```
Well... That's not gonna change. How much do you actually ride above 30??
```

---
## \#18 Posted by: E1Allen Posted at: 2018-04-08T00:33:45.643Z Reads: 43

```
Haha. That's what i was wondering as well.
```

---
## \#19 Posted by: Devilmycry Posted at: 2018-04-08T00:37:55.174Z Reads: 43

```
Ooo ok man 
A lot 
😎
```

---
## \#20 Posted by: E1Allen Posted at: 2018-04-08T00:59:10.733Z Reads: 38

```
[quote="Devilmycry, post:19, topic:51525"]
A lot

:sunglasses:
[/quote]

Sounds like if you want your top speed you're just stuck with the lower speed when your battery is almost empty.  

At 20% you're probably sitting on LVC while accelerating.
```

---
