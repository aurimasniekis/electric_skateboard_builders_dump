# HELP PLEASE! I need more speed and torque

### Replies: 13 Views: 378

## \#1 Posted by: Klaxs Posted at: 2018-06-22T11:27:18.727Z Reads: 119

```
Hello everyone, I am building a mountain board with wheels of 8 "with a ratio 60/20 htd5M and the maximum speed that I get are 23 km / h, when the inclination is 10º the speed is ridiculous 5km / h. My weight is 70 kg. I have tried different configurations but I can not find the solution. I need 30-35 km / h. According to esc.calc you should get more than 50 km / h.
Attached the battery, motor and esc I'm using. 

![motor%201|623x459](upload://oBxwxjQ5AuSvXyuUM5f6Uiigwvo.jpg)
![esc|375x500](upload://lnNanlfZx6AaitEfHBJn3M0GZJJ.jpg)
![battery|264x500](upload://5z5eAkPzGdlxrDTL02WMZheiw0l.JPG)

I think that the problem may be in my motor. Would it be enough to change my motor to this Hobbyking?

![motor%202|690x248](upload://67me6pbKwLibplq1Dseow4BnAdp.jpg)

Thank you very much everyone for helping me and sorry for my English
```

---
## \#2 Posted by: PartyPoison Posted at: 2018-06-22T11:50:31.460Z Reads: 104

```
Change esc to vesc
```

---
## \#3 Posted by: capfirepants Posted at: 2018-06-22T11:53:58.258Z Reads: 105

```
Yes. Probably the esc. The motor looks fine. Battery probably is too, cant say 100% eithout knowing what cells are inside.
```

---
## \#4 Posted by: Klaxs Posted at: 2018-06-22T12:58:48.397Z Reads: 93

```
Is posible that the máx current and the máx power motor is important? 65 vs 100. 2600 W vs 4400 W

You know a good Vesc in a europe store? Hobbyking for example?
```

---
## \#5 Posted by: pat.speed Posted at: 2018-06-22T13:17:46.015Z Reads: 85

```
Dude please read more before buying stuff. That battery is no good for esk8, the max current draw is 10amps or 360w.

That esc is for hub motors so that is another problem, but it could work with those motors if you are lucky.

Lastly that gearing is not right, it need to be around 4.5-6 :1 gear ratio, atm you only have 3:1 so that gearing will give very little torque, and then combine with the lack of power from the battery, that’s why you can’t go faster than 20km/h and can’t get up a hill. 

In the end you need a new battery for sure, possibly a new esc (it could work so I’d give it a go) and a new gear ratio (try 15:60 or 15:72).

Please read more before picking more parts, that’s the main cause of issue in this hobby, people buying crap parts that don’t work properly because they don’t take the time to read enough... rank over
```

---
## \#6 Posted by: Klaxs Posted at: 2018-06-22T13:45:48.995Z Reads: 77

```
Hello friend, thank you very much for your response. My esc works perfectly with pulley motors. I bought that battery because other users recommended me, I feel it is not good for my construction. The gear ratio was precisely to get more speed, but I knew it was not a good solution. Could you help me with an good battery? In the forum I found a lot of information to build your own battery, but not one already finished ... Thanks!
```

---
## \#7 Posted by: Acido Posted at: 2018-06-22T14:18:55.409Z Reads: 75

```
Get a 10s3p 30q at least and a vesc/ better esc
```

---
## \#8 Posted by: telnoi Posted at: 2018-06-22T14:27:22.656Z Reads: 71

```
[quote="Klaxs, post:6, topic:59716"]
My esc works perfectly with pulley motors.
[/quote]

It outputs 25a...which is nothing if you are after both torque and speed, especially when using a single drive on an mtb.

Since you bought the cheapest components possible I suggest you go with 2x 8000mah 35c or higher lipos (don't choose a cheap ass ebay brand or multistar) to reduce the price, along with a chinese vesc6 derivative that delivers 60a or more.
```

---
## \#9 Posted by: Acido Posted at: 2018-06-22T14:33:50.266Z Reads: 67

```
You need to spend $$$ to get a nice working e skate its not cheap
If you are cheaping out on everything its going to fail and you will have to spend more money and time to make it work
```

---
## \#10 Posted by: Klaxs Posted at: 2018-06-22T14:47:31.900Z Reads: 59

```
It has become clear to me that I have failed to purchase all the components, so I would like to know your opinion of a good combination motor, vesc, battery. I do not need to climb hardly inclination, I always travel on hard ground, speed 30-35 kmh and distance of at least 20 km
```

---
## \#11 Posted by: Adam0311 Posted at: 2018-06-22T14:58:59.385Z Reads: 53

```
Dude, as @pat.speed said spend 20-30 minuets reading through other MTB builds and another 20-30 minuets using the search function to read about different batteries and battery builders. You will be much better off with a little bit of knowledge as to WHY each component is right for your build.
```

---
## \#12 Posted by: pedro Posted at: 2018-06-22T15:24:32.845Z Reads: 44

```
your battery discharge is 10 A. if you make a correctly calculation power=Volts*Amp= (36V or 42V)*10A=360 watts or 420 watts, but your motor only accept 36V so you using 360 watts.
your batteries max discharge is 40A but it's only instantaneous, you can get P=26*40=1440 watts (during few seconds)

You have to see the discharge from esc to. for example if the esc can only discharge 5A, you only get P=36*5= 180 Watts
```

---
## \#13 Posted by: pat.speed Posted at: 2018-06-22T20:59:42.601Z Reads: 31

```
Do you ride on the roads or dirt and grass? If you are on roads the esc will be ok for now, if not you might need a new one. I would also suggest a lipo setup as it can deliver more amps, HobbyKing is a good place to buy, just don’t get multistar batteries. You need at least 5000mah and 10s. 

Once you have a good battery the board will “work” then you just need to fix the gear ratio, so it is 15:60
```

---
