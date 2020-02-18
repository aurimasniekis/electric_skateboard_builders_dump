# Does The Order of The Sensor Cables Matter? Evolve gen 2

### Replies: 6 Views: 589

## \#1 Posted by: MaxMalouf Posted at: 2017-12-08T13:06:42.569Z Reads: 128

```
I'm upgrading the motor on my Gen 2 Evolve Board. The hall sensor cables on the stock motor are unusual. Is it possible to use the same esc with the standard format outrunner?

I have attached some photos of each connector.

Thanks, help is very much appreciated.

<img src="/uploads/db1493/original/3X/2/1/2129c82793868bbe60875d2ff574ca23c83ea3c2.jpg" width="374" height="500">

<img src="/uploads/db1493/original/3X/4/a/4ab19c36aa0d7f51310d00da940ed5d8e54586d6.jpg" width="374" height="500">
```

---
## \#2 Posted by: ikjahaa Posted at: 2017-12-08T17:13:29.368Z Reads: 97

```
I'm curious to know the answer to this question too.

But just outta common sense, I'd think yes?
They tell your esc in what position your motor is...

Ps,
Where did you find that extention cable?
```

---
## \#3 Posted by: evoheyax Posted at: 2017-12-08T17:45:39.088Z Reads: 95

```
I highly doubt they are using something other than the standard sensor protocol that all Brushless DC motors use.

black goes to black, red goes to red, and the center wires are your A, B and C sensor data lines. The order you put them in does not matter. Just black needs to go to black and red needs to go to red.

I you wana keep things simple, I would recommend using evolves sensor plug, since you have a male and female plug already. Leave yourself 2 inches for safety (in case you mess up soldering and need more wire), and solder one at a time. Cover each joint with heatshrink and your good to go :)

The one your using btw looks to have a temp sensor wire (which is why theres 6 and not 5). You don't need to connect the temp sensor, you can heatsrink the end of the wire so it doesn't short with any thing.
```

---
## \#4 Posted by: squishy654 Posted at: 2017-12-08T19:43:15.059Z Reads: 68

```
did you just say "brushless DC motor" ?  sorry, but that gave me a chuckle, lol

I mean I know that's what they are called but when I see it it makes me laugh, cus they are actually 3 wire phased alternating current motors, lol
```

---
## \#5 Posted by: MaxMalouf Posted at: 2017-12-08T23:04:18.069Z Reads: 50

```
All came with the board
```

---
## \#6 Posted by: MaxMalouf Posted at: 2017-12-08T23:06:45.768Z Reads: 49

```
Thanks for the help man.
```

---
