# 6S &#124; 6364 SK3 245 kV Turnigy &#124; How to wire for charging &amp; for use with Loop Key?

### Replies: 3 Views: 1140

## \#1 Posted by: roamin Posted at: 2016-09-30T02:10:12.644Z Reads: 118

```
Hey gang,
I've been buying stuff left and right, but now I need some direction.

I have two 3S batteries in series, and I'm looking at placing an XT90-S loop key on the negative line to the VESC, to act as the ON/OFF key. Problem is, I have a parallel board from a friend for charging the batteries. How would I go about properly wiring this, between regular use and charging?

Do I need to get more bullet connectors that are the same size as the ones on my battery? I have a soldering tool for any connections I may need to make as well. What else do I need to get to complete the Electronics system? How should I wire this to effectively go back and forth between using and charging the board?

Also attached an image for any clarification, and for adjustment too. Much love :heart_eyes:<img src="/uploads/db1493/original/3X/6/b/6b68d3f32fea66b6ed1b0dff6d3458ccbe60bb84.PNG" width="690" height="398">
```

---
## \#2 Posted by: SteveS Posted at: 2016-09-30T03:04:03.132Z Reads: 105

```
One possibility on my recent build thread: http://www.electric-skateboard.builders/t/trampa-street-carver-sk3-6374-12s-vesc-and-trampa-mount-kit/10259
```

---
## \#3 Posted by: B4Me Posted at: 2016-09-30T11:16:42.519Z Reads: 88

```
I would charge your batteries as an 6s package as both the charger and battery config will be optimal at this..

What I did was to first create a connector which connects the 2x4pins connectors in series as:
Cell : pin
1 : 1
1 : 2
1 : 3
1 : 4
SHORT these two together
2 : 1
2 : 2
2 : 3
2 : 4

For the main connection between batteries you the cell 1's plus to cell 2 negative (the bullet on your drawing..

Connect the anti spark XT90 on the ESC part
and XT90 normal on your 6s batteries output

When charging connect the balance cable (with now 7 wires in!!! not 8) and the XT90 from the charger to the batteries XT90

And your on of is the anti spark XT90 and normal connector


I use this on my setup, works like a champ :slight_smile:
A sitenote.. the charger will only charge at 2,5-2 A now.. due to the 6S package.. but its still the max 50Watts
```

---
