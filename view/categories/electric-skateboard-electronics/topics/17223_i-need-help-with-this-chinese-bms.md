# I need help with this Chinese Bms

### Replies: 16 Views: 2021

## \#1 Posted by: IsTalo Posted at: 2017-02-05T00:25:02.870Z Reads: 90

```
Can Anyone explain me how to wire my bms for just charging?

<img src="/uploads/db1493/original/3X/2/d/2d7c850d6cf52f267f87b3d0dc00db4f3dbcc03a.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/a/b/ab48d7f94fe61ec80e0ed53824a1f946161991da.jpg" width="690" height="411">
```

---
## \#2 Posted by: rpn314 Posted at: 2017-02-05T00:53:36.827Z Reads: 84

```
Yep! Couple of quick questions while I start to draw out a diagram. Do you have a 6s or a 7s pack? (I think this BMS was made for 7s). Did this come with balance wires? (bare wires on one end that all go into a connector on the other that plugs into the white port on the left)
```

---
## \#3 Posted by: IsTalo Posted at: 2017-02-05T00:57:03.768Z Reads: 81

```
My Battery is 6s, I bought the 6s Bms, maybe the picture in different, but still the same wiring, my battery have the balance wires
```

---
## \#4 Posted by: barajabali Posted at: 2017-02-05T01:00:47.548Z Reads: 79

```
Main pos terminal on battery to main positive on connector

Main neg to B-

P- to negative connector terminal 

Wire balance leads according to the main negative lead 1 being 3.7 2 being 7.2 etc till you hit 6 at 22.2
```

---
## \#5 Posted by: IsTalo Posted at: 2017-02-05T01:06:28.138Z Reads: 76

```
[quote="barajabali, post:4, topic:17223"]
Main neg to B-
[/quote]

Could you explain better. I put my Negative cable of the battery on B-?
```

---
## \#6 Posted by: barajabali Posted at: 2017-02-05T01:12:50.549Z Reads: 72

```
Yes the main negative terminal from battery to b-
```

---
## \#7 Posted by: rpn314 Posted at: 2017-02-05T01:16:05.547Z Reads: 68

```
I'm drawing but had a question. @barajabali isn't there also usually a 3rd neg input on the BMS for charging? 1 input for charging, 1 for discharge (to load, VESC or switch in this case), and 1 for the battery pack?
```

---
## \#8 Posted by: barajabali Posted at: 2017-02-05T02:03:04.191Z Reads: 59

```
Oh yea I forgot the charging

Charger negative to p- same port

Charger positive to main positive terminal
```

---
## \#9 Posted by: IsTalo Posted at: 2017-02-05T02:04:35.905Z Reads: 63

```
But how I put my Bms for just charging?
```

---
## \#10 Posted by: rpn314 Posted at: 2017-02-05T02:17:40.329Z Reads: 66

```
Basically as long as your switch is connected straight to the battery it'll won't handle discharging (and so just charging).

I've just never seen a BMS that handles both charging and discharging through the same location (solder point). Assuming I understood that part correctly, here's your diagram.
<img src="/uploads/db1493/original/3X/e/a/ea93b3bc36ed6b7d67485d1a28e276b570f99f31.png" width="684" height="500">
```

---
## \#11 Posted by: IsTalo Posted at: 2017-02-05T02:22:48.643Z Reads: 55

```
It won't blow my BMS during my run with the Skateboard? The bms is only 20a
```

---
## \#12 Posted by: rpn314 Posted at: 2017-02-05T02:24:58.836Z Reads: 54

```
If you're only charging with the BMS, you could have a 5 amp BMS and it wouldn't matter. It doesn't care about discharging (which is usually what the amp rating is referring to).

I will note that there is some danger here and you need to triple check that your VESC settings are properly set in order to not go under voltage, since you no longer have the additional cutoff protection that the BMS would add
```

---
## \#13 Posted by: IsTalo Posted at: 2017-02-05T02:35:32.687Z Reads: 50

```
Okay, sure. So in this esquematic after Power Switch goes Vesc?
```

---
## \#14 Posted by: rpn314 Posted at: 2017-02-05T03:08:59.445Z Reads: 48

```
In simple terms, yes. Switch could mean lots of things (like a loop key or some variation on vedder's anti-spark switch), but that would then go to the VESC.

Vi agora que você é brasileiro! Bem vindos ao esk8! Morei em Recife por dois anos (mais de três anos atras)
```

---
## \#15 Posted by: IsTalo Posted at: 2017-02-05T03:11:24.524Z Reads: 49

```
Oh, Legal, But Let's talk in English to practice, It's a bit difficult to me understand somethings that's why I ask too much. But you helped me with this chinese Bms.
```

---
## \#16 Posted by: rpn314 Posted at: 2017-02-05T03:12:30.691Z Reads: 46

```
No worries, ask as much as you want! I'm a little better at English anyways :slight_smile:
```

---
