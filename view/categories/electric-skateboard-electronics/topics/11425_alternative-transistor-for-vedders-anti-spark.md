# Alternative transistor for Vedder&rsquo;s Anti-spark?

### Replies: 13 Views: 1508

## \#1 Posted by: mclightning Posted at: 2016-10-19T08:57:52.260Z Reads: 169

```
Hi,

I am living in malmö, Sweden. There is a closeby electronics shop which has some transistors.

I found 2 potential options:
1 - 60V, 120A, 230W
http://www.electrokit.com/irfb3306pbf-to220-nch-60v-120a.54201?filters=t_v.0250v-9,tr_i.10a-20,t_p.100-106
2 - 40V, 185A, 163W
http://www.electrokit.com/auirfb8405-to220-nch-40v-185a.51435?filters=t_v.0250v-9,tr_i.10a-20


Can I directly use one of these instead of the IRFB7530?

BR,
Ahmet
```

---
## \#2 Posted by: chinzw Posted at: 2016-10-19T16:00:49.976Z Reads: 144

```
I think it should work just fine
```

---
## \#3 Posted by: sl33py Posted at: 2016-10-19T17:53:18.528Z Reads: 134

```
I don't think those will work.  You (@chinzw) seem to know a lot more than me, so maybe you can help clarify a bit.  

Besides the difference in pins 3 vs 7 (only need to to keep the gate separate from source - 3 vs 7 shouldn't matter), the 60v ones also have a huge difference in both amps and total watts.  (120A vs 7530 338A, and 230W vs 375W).  Especially as this is pretty over-rated and you won't actually be able to push 338A through 7530...

Given that the 7530's still fail infrequently, lowering the spec seems like you'd increase the failure rate?  

Where i really get lost is the importance of things like switching speed, gate resistance, avalanche energy, etc....  greek to me.

Personally - as the 7530 seems to work better than most (at least compared to other anti-spark switches i hear about failing frequently), i would think trying to find a more robust fet would make more sense vs the ones linked.  I was looking at a new OptiMOS transistor IPT015n10n5 100v w/ almost all improved specs, but the feet would need some redesign to easily fit.
```

---
## \#4 Posted by: chinzw Posted at: 2016-10-19T18:04:42.476Z Reads: 105

```
Yeah, its definitely a downgrade and won't be a 100% drop in replacement. The switching speed wont make a difference in this application as there's no switching frequency, just on/off. The resistance will change the power dissipation and efficiency.
```

---
## \#5 Posted by: smurf Posted at: 2016-10-19T18:22:27.820Z Reads: 100

```
I think it would be a fun project to make a anti spark switch on a through hole board.
As it would be so much easier than the surface mount stuff. But I don't know anything about proper component selection.
```

---
## \#6 Posted by: jmasta Posted at: 2016-10-19T18:44:32.777Z Reads: 95

```
The resistance Rds matters much more than the max power dissipation rating.  You should never even get close to that max value

I have spent some time looking for alternative MOSFETs to use in my anti-spark switch over the last few weeks.  I couldn't really find any thru-hole versions that would work at 60-70A with just two in parallel.  I will likely be using 4 in parallel in mine.
```

---
## \#7 Posted by: mclightning Posted at: 2016-10-19T19:17:28.353Z Reads: 91

```
It looks like I am going to with LoopKey with antispark resistor on positive power from batteries to vesc.
```

---
## \#8 Posted by: longhairedboy Posted at: 2016-10-19T19:37:25.052Z Reads: 88

```
I had these made recently with some IRFS7734s based on some advice i received because i'm not an EE:
https://www.instagram.com/p/BLl6ZZtAihf/?taken-by=longhairedboy
```

---
## \#9 Posted by: sl33py Posted at: 2016-10-19T19:41:52.706Z Reads: 85

```
[quote="jmasta, post:6, topic:11425"]
resistance Rds matters much more than the max power dissipation rating.  You should never even get close to that max value
[/quote]


Thanks @jmasta!  Good to know.  Have you looked at that infineon IPT015N10N5 then?  Looks more robust in almost all ways and Rds is really close to the 7530?
```

---
## \#10 Posted by: sl33py Posted at: 2016-10-19T19:50:39.506Z Reads: 81

```
Those look really good LHB!  Have you tested them yet and had any issues?

Seems like Vedder/Fechter's is still one of the better anti-spark switches!  Curious how the two compare (7530 and 7734).  I did a quick look on Mouser and did a compare, specifically trying to understand the difference in Rds @Jmasta mentioned:

Rds On - Drain-Source Resistance:  (7734 = 3.05 mOhms) (7530 = 1.4 mOhms)

Besides that the 7734 looks superior in almost all ways as well.  Only continuous drain amps slightly lower:

Id - Continuous Drain Current: (7734 = 197 A) (7530 = 240 A)

Love to learn this kind of stuff!
```

---
## \#11 Posted by: longhairedboy Posted at: 2016-10-19T20:01:40.781Z Reads: 78

```
i put the first one in my review unit this weekend. My only complaint with them is there's no 12v for the lighted switches. 

We'll see how they hold up, but i'm pretty confident they'll be good though. After having several of the flier type eswitches from various sources ($55-$65) fry into the op position on me after a short while at 12S and even at 6S, i decided to start ordering vedder switches but i got burned by a couple of vendors there too, with the mosfets failing into the ON position. So i asked around and a freind told me to upgrade to these fets and i'd have reliable 12S vedder switches. So i did.
```

---
## \#12 Posted by: sl33py Posted at: 2016-10-19T20:12:53.332Z Reads: 72

```
[quote="longhairedboy, post:11, topic:11425"]
We'll see how they hold up
[/quote]

Good luck!  Sounds like a good/better option than the Flier POS ones!

[quote="longhairedboy, post:11, topic:11425"]
After having several of the flier type eswitches from various sources ($55-$65) fry into the op position on me after a short while at 12S and even at 6S, i decided to start ordering vedder switches but i got burned by a couple of vendors there too, with the mosfets failing into the ON position.
[/quote]

Sounds like that can always happen - but shouldn't especially w/ the lower voltage 6s...  Look forward to hearing how these work out for you.  I have my last v1.3 (i reflowed) to go and kicking around getting a few more.  

Did you get a v1.4 gerber?  I see those are perforated under the FETs - i remember @Chaka was doing this to help with some folks heating the traces under load and they were lifting?  To help secure them he perforated them IIRC.
```

---
## \#13 Posted by: longhairedboy Posted at: 2016-10-20T03:37:38.217Z Reads: 63

```
yeah they're 1.4, but funny enough its the 1.3 silk screening layer that got uploaded so theres a bit of a misprint on the version number lol
```

---
