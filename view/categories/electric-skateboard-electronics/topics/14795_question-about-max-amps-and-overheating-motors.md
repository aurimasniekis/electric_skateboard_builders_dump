# Question about max amps and overheating motors

### Replies: 5 Views: 937

## \#1 Posted by: brakkeh Posted at: 2016-12-16T20:56:22.800Z Reads: 142

```
I've been searching quite alot the last few days but I could not find an answer. 

Max amp rating for lipo = Ah * C. So 5000mAh with 30C = 150A max, right? 
How come that I see a lot of people running this setup with a motor that can handle a maximum of 70~80A.

What is going on here? Is the VESC controlling the Amp's or...? 

Thanks in advance !
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2016-12-17T00:01:29.009Z Reads: 127

```
Are you wondering why people aren't using motor that are capable of drawing more amps? 

Yes they should handle 150a

At the moment I don't know anything about vescs. Sorry. I do think you can control the current on the vesc though. Anyone?

I'm guessing here about what you are asking... You should never run lipos or lithium ion batteries to their full potential. These motors that you see on this site are optimized for skateboards and really they are all you need.  They just don't draw that much. I would say never run the batteries more than 75-80% of their potential for more than a few seconds. There is a great thread on here right now where they are discussing battery cells and voltage sag. I love reading all these threads when people geek out. It speaks to why we don't run batteries full blast.
Check it out. http://www.electric-skateboard.builders/t/voltage-sag-what-is-the-most-suitable-battery-cell/14720/82

The batteries don't force power to the electronics. It's more like electronics take what they need from the batteries. So it's good to have a buffer. The batteries will stay cooler, last longer and compliment the setup that way.

Hope that helps and if I mucked it up someone can hopefully help both of us :slight_smile:
```

---
## \#3 Posted by: brakkeh Posted at: 2016-12-17T09:10:39.613Z Reads: 101

```
aaah, 

It makes very good sense to not let your battery work at full power. 
So i shouldn't worry too much about sending too much Amps at my motor because this isn't really possible because he can't ask that much? Something like that?

Thank you
```

---
## \#4 Posted by: i2oadsweepei2 Posted at: 2016-12-17T12:04:35.419Z Reads: 97

```
More or less yes. The motor and esc will take what they want from the battery or try at least whether the battery can handle it or not. Lipos and li-ions can be volatile. So spend a bit more money for quality cells that exceed the needs of the motor and esc. There are lots of threads here too that talk about setting the low voltage cut offs as well. So with all the above said if you run the cells too low you risk shortening their life and possibly worse problems. So if you are looking for a board that wil travel 10km build one than can travel 15 or 16kms. 

My example based on my variables is:
Me 210lbs or 95 kg's + 5-8lbs in my backpack
Dual 230kv motors
Dual TB's 12s esc's
16/36 gearing
83mm flywheel clones
10s1p 5000 mah (2x5s 5000mah turnigy nanotech 65-130c)
Cutoff set to 3.2v per cell.

I get 16kms consistently with the above setup and roughly 3% remaining in the packs. When I charge they take roughly 5000mah back after many uses. Nothing gets even remotely warm. Good quality cells. They are the heart of the system.
```

---
## \#5 Posted by: SirDiff Posted at: 2016-12-17T12:14:49.380Z Reads: 82

```
The escs we use aren't capable of delivering 150A continuous, and not many batteries can do so, only high power lipos. + A = + heat, we don't want (nor need) that. Vescs can't handle more than  60 amps, and even with that they get pretty hot.
```

---
