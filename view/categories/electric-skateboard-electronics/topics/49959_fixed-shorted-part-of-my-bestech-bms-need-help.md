# (Fixed) Shorted part of my Bestech BMS. Need help

### Replies: 11 Views: 429

## \#1 Posted by: Tijmen Posted at: 2018-03-23T23:34:23.370Z Reads: 97

```
I noticed one group of parallel cells were 1v higher than the rest, so while checking group voltages I accidentally shorted through the balance lead connector and melted the connector closed. Ended scrapping two female pin headers from an old LiPo balance lead, and plugging that directly onto the pins on the BMS. 

Messed up somewhere along the line and made contact with the underside of one of those big metal bars running across the BMS.

Here's some pictures

![29340777_1644188872295815_2126292642_n|352x480](upload://yGuxCsB0TcRIqACRvg4N04bh7Np.jpg)

![29134243_1644212535626782_1181596379_n|480x360](upload://wMnGgEMNxWmttJZvXICbZsCaYnz.jpg)

The pins of the balance connector are now all black and I doubt any current is going to run through that properly. 

I need to know if the BMS is still functional considering part of the (solder?) is melted off on the underside of one of those bars.
What are those bars even for?

10S 80A Bestech BMS
```

---
## \#2 Posted by: Tijmen Posted at: 2018-03-23T23:38:09.019Z Reads: 95

```
Update: The molten underside is not actually directly attached to the bottom of one of those bars. It almost seems like that layer of solder isn't connecting to anything!
The reason the top of the bar is burnt is because when the connector shorted out, it disconnected and most likely flipped up and happened to rest right onto that bar
```

---
## \#3 Posted by: Eboosted Posted at: 2018-03-23T23:54:40.313Z Reads: 88

```
Using that BMS would be a really stupid decision, throw it away and get a fresh one. Too risky
```

---
## \#4 Posted by: Tijmen Posted at: 2018-03-24T01:04:20.934Z Reads: 79

```
Just fixed it and it runs and charges. Nothing major got damaged. Just the outside of some metals
```

---
## \#5 Posted by: thisguyhere Posted at: 2018-03-24T03:30:29.657Z Reads: 71

```
I've done exactly the same thing with the exact same module and keep using it despite the damage. 

after a few charge cycles one of the P group got drained to 0 volts. 

I'm not saying the same will happen but it did to me. 

if you insist on using it, check voltage drift across all P groups after each charge and discharge to make sure
```

---
## \#6 Posted by: Tijmen Posted at: 2018-03-24T14:13:36.513Z Reads: 56

```
I'm going to send this pack back to the guy who made it :/ Sad to see my board fucked after only 2 weeks... Shouldn't be this way. Thanks for the input!
```

---
## \#7 Posted by: banjaxxed Posted at: 2018-03-24T21:54:57.930Z Reads: 40

```
I think the bestech bus's will float charge that parallel back into line, imo you damaged the bms
```

---
## \#8 Posted by: Tijmen Posted at: 2018-03-24T22:06:54.853Z Reads: 39

```
The group was already 1v higher before I messed up with the BMS so there's a bigger issue somewhere. Pack will get looked at and BMS replaced for safety :slight_smile:
```

---
## \#9 Posted by: b264 Posted at: 2018-03-24T22:41:34.925Z Reads: 32

```
[quote="Tijmen, post:8, topic:49959"]
The group was already 1v higher before I messed up with the BMS so there’s a bigger issue somewhere.
[/quote]

Scrolled down to say this, you beat me to it.

Before the short, you had a big problem that should not happen if you're using a BMS and is a safety hazard.  Now, I would never use that BMS.  May not have before the short...
```

---
## \#10 Posted by: Tijmen Posted at: 2018-03-24T22:52:05.149Z Reads: 27

```
Could simply be a disconnected cell
```

---
## \#11 Posted by: b264 Posted at: 2018-03-24T22:53:01.567Z Reads: 24

```
If you physically find a disconnected cell, and the BMS hadn't been shorted, sure it might be trusted again...  Absent both of those, no way
```

---
