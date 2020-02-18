# Esk8 Battery/motor issues

### Replies: 5 Views: 379

## \#1 Posted by: Bananaman Posted at: 2017-08-01T22:05:47.470Z Reads: 56

```
First time builder I'm thinking about using just one Multistar High Capacity 20000mAh 6S 10C Multi-Rotor Lipo Pack to make charging easier, but I'm not sure how much power or range that will give to my motor. The motor I'm looking at is a Sensored 5065 Motor 270kv. Just looking for some guidance so I don't make the wrong decision.
```

---
## \#2 Posted by: Montiey Posted at: 2017-08-02T01:08:26.405Z Reads: 46

```
It will work, provided that both the ESC and motor can handle that voltage and give a decent performance.

You might find that 2 3s packs or smaller 6s packs are easier to install on a board. The thicker the battery, the more often it's going to hit the ground.
```

---
## \#3 Posted by: Tuomalar Posted at: 2017-08-02T12:43:19.770Z Reads: 30

```
I recommend higher C rate. 10c isn't enough imo
```

---
## \#4 Posted by: Brandtisco Posted at: 2017-08-02T12:56:25.884Z Reads: 26

```
With 10 C on a 20 Ah battery you could pump out 200 amps, so it should do just fine if you are not trying to skate up 80 degree hills.
```

---
## \#5 Posted by: TarzanHBK Posted at: 2017-08-02T13:12:22.211Z Reads: 23

```
multistar batteries do have really low C rate and are in reallity more like 5c, so these will sag a lot and die pretty quickly due to that.
There are a few people running them and are happy, but normally you should look for something more in the 30C+ range.

You can calculate range like this:

20aH x 3,7V x 6 cells = 444 Wh

You´ll need about 10 Wh/km so:

444 Wh : 10Wh/km = 44,4 km (this depends on riding style and riders weight and can vary)
```

---
