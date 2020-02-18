# Charging 9s liion

### Replies: 11 Views: 1115

## \#1 Posted by: Ryanliu Posted at: 2017-02-02T18:21:08.424Z Reads: 88

```
can i charge 3 liion batteries put in a 9s serial config to get 33.3v with a imax b6 charger without putting any of them back in parallel. I want to keep all 3 in a serial config to get 33.3v without re-configuring them. I want to just plug in the balance leads. 

IK how to charge 2 3s liions like this with a twin connector but can i charge the 2 of the three this way and charge the third one in the 3s port of the imax b6 while it is still connected to the other 2 in series. If so can u link a charger capable of this.
```

---
## \#2 Posted by: rubz Posted at: 2017-02-03T20:45:01.798Z Reads: 60

```
[quote="Ryanliu, post:1, topic:17100"]
can i charge 3 liion batteries put in a 9s serial config to get 33.3v with a imax b6 charger without putting any of them back in parallel
[/quote]


Simply said, no. Imax B6 will do maximum 6 cells in series.  You have two options: parallel charge them as 3S3P (but make sure to read into this first, because there are some rules) or charge them seperately (as 2x3S in series (so 6S) + 3S after that charge, or 3x 3S separately, or buy another 3S charger if you want to charge them all at the same time - either way you'll have to disconnect and reconnect some wires).
If you want to charge them simultaneously without ever disconnecting/reconnecting anything, I'd look into a BMS (battery management system).
```

---
## \#3 Posted by: Okami Posted at: 2017-02-03T20:55:16.739Z Reads: 58

```
You can buy Turnigy ''Reaktor'' 30A 1000w, it seems to be capable of charging 10s

Costs quite a lot $$$, best luck would be to find one on auction for sale as 2nd hand item :)

**https://hobbyking.com/en_us/turnigy-reaktor-30a-1000w-balance-charger.html**

<img src="/uploads/db1493/original/3X/e/e/ee2bba5c20027e3936039d2074f004536a81bfaa.png" width="300" height="27">

[Edit]

I think you need to get one more charger and just charge that one 3S pack seperately.. you wont need to make a parallel harness, just ''divide/split'' the serial connector.
```

---
## \#4 Posted by: Ryanliu Posted at: 2017-02-06T21:13:34.526Z Reads: 41

```
if i use a 6s charger and a 3s charger. Can i keep the batteries wired in a 9s configuration and charge the 2 3s batteries with the imax b6 6s charger and charge the 3rd 3s with a imax b3 lipo battery balance charger.
```

---
## \#5 Posted by: Okami Posted at: 2017-02-06T21:19:44.696Z Reads: 39

```
I think in ''theory'' this should work! If they are not connected in any way - why not..

You would need a seperate ''discharge port'' for each battery pack (3s and 6s) .. unless you unplug them from the ''circuit'' each time before charging..

You would need to make sure they do charge to the same voltage.. so you might have less ''flexibility'' with that 3s charger.. Otherwise.. i assume you could always ''switch out the cables'' and charge the seperate 3s pack along with another one..

X O  O

vs

O  O X

X - 3s pack / charger

O - 6s pack / charger
```

---
## \#6 Posted by: Ryanliu Posted at: 2017-02-06T23:37:33.426Z Reads: 34

```
ok so do i need the disconnect the batteries before i charge them? if not can i plz get a wiring picture/diagram?
```

---
## \#7 Posted by: Ryanliu Posted at: 2017-02-06T23:41:02.303Z Reads: 34

```
im guessing you use the twin connector to the 6s and balance leads and 6s charger and then just plug in the third 3s pack's balance lead to the 3s charger (all the while not disconnecting them from their serial config) if this is right i dont need a wiring diagram
```

---
## \#8 Posted by: Okami Posted at: 2017-02-07T00:35:03.932Z Reads: 32

```
Yeh, u could actually just go with ''twin charger'' adapter.. will make it a lot easier :slight_smile:

For that 3s pack I would recommend a seperate ''parallel lead'' so that you still get one connector exposed for charging and dont have to switch cables (takes time, not practical)
```

---
## \#9 Posted by: Ryanliu Posted at: 2017-02-07T01:57:05.736Z Reads: 29

```
<img src="/uploads/db1493/original/3X/5/0/500a4b6613da1b61e6b5e53612ff5d1805bd0b35.jpeg" width="375" height="500">

The 3s connected to the 3rd battery is a charger
```

---
## \#10 Posted by: Ryanliu Posted at: 2017-02-07T01:57:16.246Z Reads: 27

```
Will this work?
```

---
## \#11 Posted by: Okami Posted at: 2017-02-07T10:05:22.748Z Reads: 23

```
As i.remember twin charger had its own 'main plug'

If u can find something similar for 3s only you probably wouldnt need to tap into main leads for power delivery.

Have u tried to hook up just one battery to twin charger (i believe left side) and then start charging?

In such case u could perhaps cut half of 6s balance connector and make it as 3s. Wont be ideal but you would get away with 2 twin chargers without having to make parallel connection for 3s pack.

-  

Drawing looks correct, but you need 'main - discharge' plug for 3s battery. Chargers ask for main plug to be inserted. Twjn charger is unique in this way that it has 'its own' main plug.. this is what i was.talking about earlier..
```

---
