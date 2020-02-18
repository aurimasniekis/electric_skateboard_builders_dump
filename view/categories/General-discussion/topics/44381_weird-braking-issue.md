# Weird braking issue

### Replies: 5 Views: 301

## \#1 Posted by: michaelcpg Posted at: 2018-01-22T22:05:16.698Z Reads: 65

```
This morning I was doing my usual half hour commute to work and just in the last couple minutes of riding, my brakes started acting a little weird. 

Occasionally when I went to apply a small amount of braking, the board would seem to push the brakes on a lot harder than expected but usually only very briefly. The battery was sitting at about 70%.

Can anyone give me pointers on what might suddenly start to cause an issue like this?

Specs:
- GT2B
- 2 Ollin 5065 motors
- 1 Ollin 4.12 VESC
- 1 Enertion 4.12 VESC
- 10S6P 25R battery
```

---
## \#2 Posted by: mmaner Posted at: 2018-01-22T22:37:32.054Z Reads: 55

```
Are the 2 VESC's connected via can bus or split ppm?  I could logically see an issue with can since they are 2 different VESC's which handle BAT MIN differently...maybe, hell I don't know.  Either way, I would rule it out by switching to split PPM and see if the problem goes away.
```

---
## \#3 Posted by: michaelcpg Posted at: 2018-01-22T23:05:16.095Z Reads: 43

```
Using split ppm currently
```

---
## \#4 Posted by: Deckoz Posted at: 2018-01-22T23:07:21.511Z Reads: 42

```
They could if ones on 2xx and the other is on 3xx(behaving diff to battery min)

What were your temps?

Have you gotten a rock in your motor and caused a short?
```

---
## \#5 Posted by: michaelcpg Posted at: 2018-01-22T23:14:39.928Z Reads: 39

```
Pretty sure they're both using same firmware version and all the firmware settings are the same. No idea what the temps were but they should be perfectly fine as I've done this path 100s of times with no issues and its largely downhill at the point where I started getting issues so nothing should be getting pushed particularly hard. 

I'm leaning towards it being a short somewhere in the motor so I'll be opening them up tonight to check but happy to hear other ideas still :)
```

---
