# Can a shorted motor blow a VESC?

### Replies: 18 Views: 914

## \#1 Posted by: Eboosted Posted at: 2017-07-01T05:24:58.198Z Reads: 177

```
Is there a way to check if a motor is shorted using a multimeter before connecting it to a brand new VESC?
```

---
## \#2 Posted by: Namasaki Posted at: 2017-07-01T05:30:26.486Z Reads: 175

```
I just recently received 2 new 6374 motors and it seemed they had a lot of drag in comparison to my 6355 so I was wondering the same thing. "Are they shorted?"
So I got my wife to hold the wires and short them together while I was spinning the motor and sure enough the brakes came on and stopped the motor. 
I guess the big motors just have a lot more drag.
```

---
## \#3 Posted by: Jinra Posted at: 2017-07-01T05:32:54.088Z Reads: 171

```
If the can has tension when you turn, it's shorted. You can easily test this work a working motor by touching any of the two phase wires, it'll be noticeably harder to turn.
```

---
## \#4 Posted by: Eboosted Posted at: 2017-07-01T05:36:36.062Z Reads: 168

```
I've been running 6374s for almost 1 month now, I'm pretty sure they do have more drag but I'm not sure if the drag came from the 15mm belts or the 6374s
```

---
## \#5 Posted by: Namasaki Posted at: 2017-07-01T05:39:26.965Z Reads: 160

```
I was spinning mine without belts or pulleys. The motors themselves do have more drag than the smaller motors.
Guess longer magnets do make a difference.
```

---
## \#6 Posted by: Eboosted Posted at: 2017-07-01T05:46:30.781Z Reads: 151

```
So, just to check if I understood correctly:

If a motor spins freely with the 3 phase wires disconnected and not touching each other then the motor is not shorted. 

If I connect 2 phase wires, leave one disconnected, spin the motor by the hand and feel drag, then the motor is working properly, not shorted. 

If feel drag on a motor with the 3 phase wires disconnected and not touching each other, the motor is shorted. 

All tests should be done with no power from the battery?
```

---
## \#7 Posted by: Eboosted Posted at: 2017-07-01T05:49:05.012Z Reads: 138

```
We're you comparing motors with the same KV? I read lower KV motors have more drag than higher KV motors. 

I can noticeable feel my Kaly 6355 230kv motors have less drag than my Torqueboards 6355 190kv
```

---
## \#8 Posted by: Jinra Posted at: 2017-07-01T06:11:11.175Z Reads: 131

```
Not connected, but touching each other. So just touch any of the two connectors on the motor (metal bits) and it should have drag (shorted). If they're all not touching and there's still drag, then it's shorted somewhere in the system.
```

---
## \#9 Posted by: lrdesigns Posted at: 2017-07-01T06:19:14.003Z Reads: 127

```
Lower kv = more drag is not true. I have low kv motors with little drag and high kv motors with high drag. Same size different brands. I think it has more to do with the type of magnets and how close they are to the stator. 

But yes a shorted motor could destroy an esc or a burnt esc could destroy a motor. :tired_face:
```

---
## \#10 Posted by: Namasaki Posted at: 2017-07-01T06:43:23.170Z Reads: 115

```
I was comparing 6355 190kv with
6374 200kv
The 6374 200kv have more drag Than the 6355 190kv but as @lrdesigns stated it's because of the magnets not the windings
```

---
## \#11 Posted by: Ixf Posted at: 2017-12-27T22:15:17.935Z Reads: 80

```
This was super helpful btw.  I was getting nervous about installing new vesc as I didn't know if the motors were causing their failures
```

---
## \#12 Posted by: Deckoz Posted at: 2017-12-27T22:19:50.851Z Reads: 79

```
You can measure the ohms between phases. You will need a meter that can detect milliohms. Ohms on a shorted leg will be significantly different then measurements between other phases.

The results can mean phase to phase shorts directly, or shorts through the stator due to epoxy worn off and the enamel of the windings melted. They will give different results.  Stator shorts are smaller ohm gains, phase to phase is large ohm gain.
```

---
## \#13 Posted by: Ixf Posted at: 2017-12-28T04:01:47.108Z Reads: 62

```
I don't have access to a meter that can detect millohms :( Is the turning method described by Jinra sufficient
?
```

---
## \#14 Posted by: Eboosted Posted at: 2017-12-28T04:03:05.920Z Reads: 57

```
No it's not. I did have drag touching any combination of phase wires but the motor was shorted or busted somewhere.

Edit:
Changed didn't with did
```

---
## \#15 Posted by: Ixf Posted at: 2017-12-28T04:07:46.396Z Reads: 54

```
Interesting... I feel a big difference in drag when the phase wires touched.  Also using this method to double check https://www.youtube.com/watch?v=7sP3dqRA4js
```

---
## \#16 Posted by: Deckoz Posted at: 2017-12-28T05:10:11.776Z Reads: 52

```
You can use a 10 ohm resistor in series with the meter and the phase in measurement to measure the resistance of the phase...

Look here

http://www.radiocontrolinfo.com/brushless-motor-efficiency/brushless-motor-winding-resistance/

The important piece with any way you chose to measure the phases is that they have similar values. An odd value could mean a short you can't "feel". Sure spinning by hand is a good indicator. But if your blowing fets on an esc and the motor "feels" fine. It doesn't hurt to test the phases
```

---
## \#17 Posted by: Ixf Posted at: 2017-12-28T05:55:07.083Z Reads: 46

```
Got a 404 on the link.  I have a really crappy meter that came in a package with my soldering iron... i'll see if i can borrow a better one.
```

---
## \#18 Posted by: Deckoz Posted at: 2017-12-28T10:03:36.369Z Reads: 42

```
Maybe this then

https://www.google.com/url?sa=t&source=web&rct=j&url=http://www.radiocontrolinfo.com/brushless-motor-efficiency/brushless-motor-winding-resistance/&ved=0ahUKEwitsYuh-KvYAhWlYt8KHYIFA_sQFgiIATAO&usg=AOvVaw2zZrtRAcwrThC7gF6r0hAK
```

---
