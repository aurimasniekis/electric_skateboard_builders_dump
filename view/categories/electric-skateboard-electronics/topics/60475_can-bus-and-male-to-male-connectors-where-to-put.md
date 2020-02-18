# CAN bus and Male to Male connectors - where to put?

### Replies: 13 Views: 580

## \#1 Posted by: plasteroid Posted at: 2018-06-30T02:11:40.300Z Reads: 101

```
Trying to get my dual motor VESC setup all hooked up. 

Hoping you guys can help out.

I'm pretty sure the white CAN bus goes here (pictured below)

Then I'm really not sure where the black Male to Male goes - does that hook to the Remote receiver somehow?
Sorry for all the noob questions. 

Thanks!

![image|423x500](upload://mEn6K2YPBun7sVtSJLidzfwSKVW.jpg)
```

---
## \#2 Posted by: caustin Posted at: 2018-06-30T02:30:24.509Z Reads: 94

```
Not sure if I interpret your question correctly, but the 3 wire red white Black is the ppm wire from one Vesc as noted but other end goes to remote receiver 

Looks like sensor wires also in the corner of picture so need to connect them depending on what motors etc
```

---
## \#3 Posted by: E1Allen Posted at: 2018-06-30T02:32:40.775Z Reads: 89

```
Might want to search and read up a little more.  Canbus goes vesc to vesc.  RX gets plugged into master vesc. With canbus both have to be plugged (powered up) in at the same time.  There's more to it than what I said though.
```

---
## \#4 Posted by: plasteroid Posted at: 2018-06-30T02:33:12.348Z Reads: 88

```
Yes, thank you. that makes sense.   
The white tipped black and white wire connects the 2 VESCs.   Then the black goes from one VESC to the Remote receiver.   Got it.
```

---
## \#5 Posted by: mmaner Posted at: 2018-06-30T02:38:51.905Z Reads: 83

```
This should tell you everything you need to know...

![vesc-diagram_1530326294055|585x500](upload://jViFxl8Vn2AxeVhTsMBjuvRbcQn.png)

Can bus is center left, PPM is bottom right.
```

---
## \#6 Posted by: plasteroid Posted at: 2018-06-30T14:10:16.065Z Reads: 63

```
Hey Mike - once you make the connections - do you guys do any kind of shrink wrap - water resistant coating over the VESC ?
```

---
## \#7 Posted by: mmaner Posted at: 2018-06-30T14:55:43.119Z Reads: 57

```
Some people do, I use 3m tape to secure it to the deck and just leave the factory heat shrink in it. 

I'm almost out of 5.5mm bullets or I'd make you some extensions. If you wanna get some on Amazon and send then to me I'll make them and send them back. 

Alternatively, @JLabs, @GrecoMan, @psychotiller and @torqueboards can make them.
```

---
## \#8 Posted by: torqueboards Posted at: 2018-06-30T15:35:02.819Z Reads: 56

```
Program both and plug in Can bus afterwards after it's been programmed and your ready to connect it. Just remember which one is master and slave.

Some people may end up damaging the canbus when trying to program both. It's not needed while you program.
```

---
## \#9 Posted by: Adam0311 Posted at: 2018-06-30T16:52:53.078Z Reads: 53

```
@Deckoz made a good video tutorial about setting up the canbus. I used it when building my dual board.

 https://www.electric-skateboard.builders/t/how-to-program-canbus-properly-video-tutorial/52606
```

---
## \#10 Posted by: banjaxxed Posted at: 2018-07-01T22:42:19.074Z Reads: 43

```
The canbus wire should only use two wires - only the center pins are used. In fact you can damage a vesc using all four pins
```

---
## \#11 Posted by: briman05 Posted at: 2018-07-02T12:46:54.094Z Reads: 38

```
The jst connectors only go in one way.  I would put some hot glue on the outside of the connectors once your vesc are configured this way they dont come undone by vibration but can still be taken off if you need to do work on the board
```

---
## \#12 Posted by: plasteroid Posted at: 2018-07-02T13:08:08.588Z Reads: 35

```
[quote="briman05, post:11, topic:60475"]
some hot glue on the outside of the connectors
[/quote]

Great idea - will do! Thanks
```

---
## \#13 Posted by: plasteroid Posted at: 2018-07-02T13:11:03.445Z Reads: 32

```
@banjaxxed - yes - this is the connector I'm using.   

![image|507x500](upload://jFiTw6Mh2bKONUyzXv8zAalfgq7.jpg)
```

---
