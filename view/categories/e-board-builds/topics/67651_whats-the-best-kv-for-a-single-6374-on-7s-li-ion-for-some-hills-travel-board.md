# Whats the best KV for a single 6374 on 7s Li-ion for some hills (travel board)

### Replies: 12 Views: 382

## \#1 Posted by: Lofidelity Posted at: 2018-09-10T20:34:06.835Z Reads: 130

```
Hey!

What would be the best Motor to buy for a single 6374 on a 7s2p Li-ion battery?

I want to build a light weight travel board that can handle some hills. Torque is much more important to me than speed. I'd be totally fine with 25-30kmh (15,5-18,5 mph)

Initially I thought 200kv would be a good idea but today I read that higher KV seems to be better and now I can't decide..

I was planing with a 16/36 12mm drivetrain

Thanks!
```

---
## \#2 Posted by: pat.speed Posted at: 2018-09-10T21:19:58.840Z Reads: 119

```
200kv seems good, according to the calc you will get about 33km/h at nominal voltage and you should be able to climb pretty decent hills with that setup.

The only thing left to worry about is whether the battery can handle enough power for hill climbing, what cells are used?
```

---
## \#3 Posted by: Lofidelity Posted at: 2018-09-11T08:28:41.475Z Reads: 105

```
thanks for the reply @pat.speed

I also used the calculator to config the setup. Like you mentioned it said I'd get around 33km/h theoretically but I wouldn't mind if it would be a bit lower in real world. 

The battery cells I used are Samsung 18650 30Q, which I read can handle up to 40A on a single drive. And I got a VESC 4.12
```

---
## \#4 Posted by: pat.speed Posted at: 2018-09-11T09:19:16.833Z Reads: 95

```
Thats's great then, looks like your all set for a load of fun
```

---
## \#5 Posted by: Lofidelity Posted at: 2018-09-11T09:25:06.591Z Reads: 93

```
OK, nice. Thanks!

I was really worried because I red yesterday that you should aim to run the motor close to 8000rmp because that's where it's most efficient. And I'll be miles away from that rating with the 200KV...

Thanks for the help :slight_smile:
```

---
## \#6 Posted by: Jmding Posted at: 2018-09-12T01:49:53.109Z Reads: 69

```
If you havent bought your parts yet, you should consider going 10s.  With a single motor, you want to milk as much power out of it as you can, and since too much current will cause it to burn up, that means you want to increase your voltage, and adjust your gearing to compensate.

I'd go 10s or 12s, 200 Kv, and gear it for a 25 mph top speed
```

---
## \#7 Posted by: faithfulpuppy Posted at: 2018-09-12T02:53:37.622Z Reads: 53

```
he specifically does not need that much speed. I run 12s on my board and for a lightweight travel setup (what he specified) 7s is definitely enough, especially assuming you're gearing it down to 15-19mph
```

---
## \#8 Posted by: Jmding Posted at: 2018-09-12T02:56:51.104Z Reads: 52

```
12s + gearing
```

---
## \#9 Posted by: Lofidelity Posted at: 2018-09-12T06:33:16.837Z Reads: 47

```
Is everyone really always flying at 40kmh/25mph?!

I've got a Mellow drive and ridden it for about 800km. The times I hit 40 I can count on one hand and it was always on smoothest underground and light traffic.
I feel 28-33kmh is my sweetspot.

That beeing said, if you want to build light, you gotta make compromises. A 7s2p is 700g a 10s3p is double that. And that would be what I'd need to max my motor at 3000W.

The travel build I'm talking about here is about 4.9kg. It has 29" mid flexing deck, a 6374 200KV, a swappable 7s2p, seismic trucks, and 83mm 75a flywheels. So you're getting a lot of in return for the weight. ANd that was what I was shooting for :slight_smile:
```

---
## \#10 Posted by: Jmding Posted at: 2018-09-12T07:40:37.316Z Reads: 42

```
Or you can go hobby LiPo instead of 18650, and not have to sacrifice output current or voltage to achieve low weight
```

---
## \#11 Posted by: Lofidelity Posted at: 2018-09-12T09:49:09.471Z Reads: 37

```
and travel around with a bulky LiPo charger?

But I appreaciate your help and suggestions :slight_smile:
```

---
## \#12 Posted by: Jmding Posted at: 2018-09-12T15:31:49.719Z Reads: 30

```
You can wire up the same BMS you use for 18650s and charge on-board with a laptop style charger as well, no different.
```

---
