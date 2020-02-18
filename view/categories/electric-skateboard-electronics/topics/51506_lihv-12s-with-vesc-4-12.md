# LiHv 12s with VESC 4.12

### Replies: 10 Views: 656

## \#1 Posted by: amazingdave Posted at: 2018-04-07T18:58:06.642Z Reads: 118

```
I’ve been running my board at 12s with no problems for 300km.  The batteries I used for this build are LiHV which are full at 4.35v per cell however I’ve only been charging to 4.2 per cell out of fear of a fried VESC.

Question is do I need to grow some balls and charge my batteries fully gaining 3Ah across the series pack or am I right to keep playing it safe?

I love the raw power available at 12s so let’s not revisit the 10s /12s debate....
```

---
## \#2 Posted by: Acidfie Posted at: 2018-04-07T19:08:47.581Z Reads: 116

```
What VESC you're using?

@Deckoz using 13S Li-Ion = 54,6V fully charged

you 4,35 * 12S = 52,2

depends on the VESC, low quality can be an issue but voltage should be not _that_ problem..

still, its risky while braking getting overvoltage, but i dont see this as a problem
```

---
## \#3 Posted by: Deckoz Posted at: 2018-04-07T19:09:42.951Z Reads: 112

```
LiHV puff when you charge them to 4.35 regularly... In my experience they last longer then lipo when only charged to 4.20 in regards to life cycles.

As far as 52.2v on a vesc... 54.6v here(13s)
```

---
## \#4 Posted by: amazingdave Posted at: 2018-04-07T20:01:20.724Z Reads: 102

```
Using this VESC, max temp I see in telemetry is 39C https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.co.uk%2Fulk%2Fitm%2F183166720873

My main concern was over voltage on braking...
```

---
## \#5 Posted by: Acidfie Posted at: 2018-04-07T20:17:20.923Z Reads: 93

```
OT: this fu**ing seller sent me the wrong motors once and never responded again when i told him. they never came from uk, they came from china so i had to pay VAT and toll.. 

its 4.12 so it **can** handle this voltage, but i would never use a low quality VESC with that high voltage.. but since you're using 12S i think those 2 volts more should cause no issue imo
```

---
## \#7 Posted by: amazingdave Posted at: 2018-04-07T20:58:34.752Z Reads: 79

```
I had trouble with a drv faulting VESC from them... I opened a Paypal dispute and they eventually refunded the VESC and then sold me another for £40 delivered as an apology!! They had been crap till I opened a dispute...
```

---
## \#8 Posted by: amazingdave Posted at: 2018-04-07T21:08:05.522Z Reads: 75

```
I figured I could mainly run at 4.2 and then go for 4.35 just for very long trips...
```

---
## \#9 Posted by: helpmebuild Posted at: 2019-09-01T03:32:04.414Z Reads: 25

```
did you ever try them on 4.35 i bought the biggest lihv i could find for 12s and wondering if the voltage spiked over 60 on you i havent finished the build yet
```

---
## \#10 Posted by: amazingdave Posted at: 2019-09-01T17:19:05.354Z Reads: 20

```
I never ran them at more than 4.2 and was just happy with the overhead for full charge braking.
```

---
## \#11 Posted by: helpmebuild Posted at: 2019-09-09T19:03:47.053Z Reads: 15

```
It was fine on my trampa vesc6.![20190906_204109|374x500](upload://wh1sz7FpCcWjDAu7jIgVJJQkALa.jpeg)
```

---
