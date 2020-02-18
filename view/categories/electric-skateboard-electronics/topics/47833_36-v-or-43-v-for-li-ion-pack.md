# 36 V or 43 V for Li-Ion pack

### Replies: 17 Views: 483

## \#1 Posted by: Alex.Scheff Posted at: 2018-03-01T11:47:11.237Z Reads: 81

```
Hello, I'm struggling to build a 10s or 12s battery pack, what is better, 36V or 43V? (Propably 8p with 80A discharge)
Thanks
Alex
```

---
## \#2 Posted by: Latemate Posted at: 2018-03-01T11:51:41.004Z Reads: 79

```
That depends on what you want. Which parts you are going to use, can the parts handle 12s?

You are going to have alot more power with 12s, also less heat from the cables. 

If I were to recommend you something knowing nothing about your setup, id say go with 10s.
```

---
## \#3 Posted by: Acidfie Posted at: 2018-03-01T12:04:03.089Z Reads: 70

```
VESC works up to 60V, but better stay around 12S
```

---
## \#4 Posted by: Alex.Scheff Posted at: 2018-03-01T12:11:20.655Z Reads: 64

```
I will use two vesc from maytech (up to 60V) two motors from alienpowersystem (max 42V max 60A 2400W 190kV)
and now I try to find out what battery constellation to get the best out the motors
```

---
## \#5 Posted by: Acido Posted at: 2018-03-01T12:39:16.603Z Reads: 55

```
36 is nominal voltage of a 10s pack
42 is maximal charged voltage of the 10s pack
So basically you are talking about the same thing
```

---
## \#6 Posted by: Acido Posted at: 2018-03-01T12:40:10.429Z Reads: 55

```
If you put proper cables like 10 or 12AWG you wont have any problems with heat
```

---
## \#7 Posted by: Alex.Scheff Posted at: 2018-03-01T12:42:50.797Z Reads: 50

```
Oh youre right :roll_eyes: thank you very much
```

---
## \#8 Posted by: Latemate Posted at: 2018-03-01T14:09:02.356Z Reads: 42

```
I dont have any problems with heats but you are right ohms law is cool.
```

---
## \#9 Posted by: Namasaki Posted at: 2018-03-01T15:56:03.448Z Reads: 37

```
[quote="Acidfie, post:3, topic:47833, full:true"]
VESC works up to 60V, but better stay around 12S
[/quote]


Did you mean stay around 10s?
```

---
## \#10 Posted by: Namasaki Posted at: 2018-03-01T16:02:40.041Z Reads: 36

```
10s is good for dependability.
12s is more for cutting edge performance but can be hard on electronics and motors.
```

---
## \#11 Posted by: Acidfie Posted at: 2018-03-01T16:03:00.823Z Reads: 34

```
10S @ 4.2V = 42V
12S @ 4.2V = 50.2V

VESC can handle Voltage up to 60V - **BUT** better stay at 12S because that would be the Voltage Spike Cutoff Limit of the VESC.

I just wanted to say if you go high voltage, stay at 12S **DO NOT** try 13S or whatever, just because the VESC **CAN** handle 60V.

More Power = More Heat - simple as that


If personally think 10S ist the best, the 12S is just the little push to the edge that is not necessary
```

---
## \#12 Posted by: Alex.Scheff Posted at: 2018-03-01T16:05:03.229Z Reads: 31

```
@Acidfie @Namasaki I will propably make a 10s6p with the LG INR18650HG2 (max discharge 20A) so I have enought power and mAh
```

---
## \#13 Posted by: Namasaki Posted at: 2018-03-01T16:06:00.013Z Reads: 31

```
Thanks for clarifying.
I agree with your preference for 10s. I ran 12s on my first 2 builds and had problems with heat in the motors and electronics.
```

---
## \#14 Posted by: Alex.Scheff Posted at: 2018-03-01T16:06:47.936Z Reads: 31

```
Oh okay another reason to go with a 10s
```

---
## \#15 Posted by: Namasaki Posted at: 2018-03-01T16:09:07.465Z Reads: 29

```
easier to find inexpensive chargers for 10s
```

---
## \#16 Posted by: Namasaki Posted at: 2018-03-01T16:11:29.162Z Reads: 29

```
[quote="Alex.Scheff, post:12, topic:47833"]
I will propably make a 10s6p with the LG INR18650HG2 (max discharge 20A) so I have enought power and mAh
[/quote]


Take a look at the Samsung 30Q. It currently seems to be the most popular cell for battery packs here.
```

---
## \#17 Posted by: Alex.Scheff Posted at: 2018-03-01T16:15:44.344Z Reads: 28

```
Yes I will take a look, thank you very much
```

---
