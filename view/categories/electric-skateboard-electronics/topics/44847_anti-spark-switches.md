# Anti-spark switches?

### Replies: 5 Views: 2047

## \#1 Posted by: RosyRoseman Posted at: 2018-01-28T05:12:14.172Z Reads: 371

```
This may be a silly question; do I need an anti spark switch or loop key if I am using an 18650 pack with a BMS? If so, between which two components do I place the look key?
```

---
## \#2 Posted by: Apolo Posted at: 2018-01-28T05:17:21.485Z Reads: 373

```
Yes, it will be your way of turning off your board. A loop key is just an xt90 connector with one end shorted.
```

---
## \#3 Posted by: wafflejock Posted at: 2018-01-28T05:19:40.592Z Reads: 373

```
Some BMSes have a way to hook up a switch for turning power on/off, if you have one of those then you don't necessarily need a loop-key.  That said loop key is still a nice extra precaution even if you don't need it just as an easy way to turn the board on and off.  Loop key is just a part of the 12AWG wire that you make so you can remove part of the wire to leave the circuit clearly open (the antispark switches used generally use mosfets to allow the power to flow when "on" but the mosfets also fail "closed" or in an on position).  Since the circuit needs to be complete for power to flow where you put it isn't really that big of a concern but typically you just want to cut power between your batteries and any other components so putting it on the main leads between the battery and BMS or battery and VESC usually makes the most sense (I use mine between the two 5S batteries I'm putting in series to make a 10S, but really anywhere you remove a piece of the circuit between batteries and whatever they power will break the loop).

Using an anti-spark plug for the loop key is nice because then you don't get sparks and charring of the connector from inrush current that happens when first connecting.

http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204

---

Mine is not as pretty, not required for it to work:

![IMG_20180127_232542|375x500](upload://lGhbC4TDvdf5SxQogY8wb0tDlqv.jpg)![IMG_20180127_232515|375x500](upload://zkdWM2dooq9asmiQBbq9uLXZ70O.jpg)

---

Black wire and red wire going off screen to the left go to my VESC from the battery you could also put it on either of those if it's more convenient for your setup.
```

---
## \#4 Posted by: krloz Posted at: 2018-01-28T10:23:42.350Z Reads: 304

```
Totally agree on nearly everything wafflejock said.  
Except maybe This:

[quote="wafflejock, post:3, topic:44847"]
so putting it on the main leads between the battery and BMS
[/quote]

I wouldn't put the antispark in a mains wire between battery and bms because you would still have the balance wires between bms and battery and some(most) bms are not going to take that well. There are even some bms that are known to smoke if you wire them up in a wrong order.  So I think its better to put the anti spark between bms and others(esc, voltmeter...)
```

---
## \#5 Posted by: Acido Posted at: 2018-01-28T13:13:19.816Z Reads: 282

```
every bms smokes if you miss a wire as i know, they are great but also horrible parts of batteries at the same time
```

---
