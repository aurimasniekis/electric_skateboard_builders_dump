# Question about homemade batteries (12s3p)

### Replies: 7 Views: 806

## \#1 Posted by: Gepson Posted at: 2017-04-18T02:43:02.118Z Reads: 148

```
Hi guys!

So first, a little introduction: I plan to build my first eSk8 build using Trampa motor mount for Caliber II, a SK3 149Kv motor from Hobbyking and a VESC V4.12. 
For the battery I have been lurking on the internet for a bit of time and I found that's its kinda difficult to source for a decent price here in Canada, it often involve buying from US or Asia and since Li Ion are classified as "HazMat" the carrier take a comfortable amount of money to carry the cells. And as a DIY enthusiast and an Electronic technician in real life I feel confident enough to build my own battery pack.

So my question is the following: I plan on recycling used cells from laptop batteries as it's often good quality cells and it brings down a lot of the cost, It might be hard to find the exact same brand for 36 cells so as far as i keep using cells that are the same capacity is it OK if it's not the same brand? 
I will charge my 12S with 2 6S balance charger so I wont use a BMS.

I hope this is not too much of a wall of text :) 
This community is awesome keep up the great work!

Edit: I didn't mention it but of course I'll use 18650 cells.
```

---
## \#2 Posted by: BigBoyToys Posted at: 2017-04-18T02:58:56.705Z Reads: 136

```
Im not one of the resident experts here, but I think your plan sounds just fine!
```

---
## \#3 Posted by: Namasaki Posted at: 2017-04-18T03:13:59.900Z Reads: 138

```
Several bits of advice here.
Laptop batteries may not have the current capability necessary for an E-skate.
And as you suspected it may be impossible to get 36 matching cells. That is matching capacity, current capability and internal resistance. Using a bunch of unmatched cells will cause the pack to discharge unevenly and cause damage to cells that drop voltage too quickly.
If I may be up front with you, you are starting off on the wrong foot here.
To build a safe, reliable battery with the performance e-skate requires, you will need to start off with brand new quality cells.
Then you will need a 60a spot welder and nickel strip to put it together. Some have soldered cells together with wire but the truth is, the cell get overheated in the process and can get damaged.
Next, you will need a bms at least for charging. Unless your planning to build 2 6s packs that you connect in series for operation and disconnect for charging.
If budget is the issue, you would be better off using a couple 6s Lipos in series and charge them separately with your hobby charger. At least that would be a less expensive option.
```

---
## \#4 Posted by: sl33py Posted at: 2017-04-18T03:16:55.206Z Reads: 123

```
[quote="Gepson, post:1, topic:21262"]
used cells from laptop batteries
[/quote]


The trouble with laptop batteries usually is amp output capacity.  When you look at the 30q / 25r / HG2 cells - they are rated to 15-20amps continuous discharge.  laptop batteries only need to output a few amps tops (look at the bottom of your laptop for voltage info - 19v 2-5amps usually or so) - not high output.

What that equals in real world - when you connect your cells in 3p, your are tripling the amp output ability - so capacity of 20a cells x 3p = 60 amps continuous - with peak being higher, but focusing on continuous discharge.

If you look at measured discharge amps you'll frequently see 30-40 amps draw for esk8 riders.  Not every single person will have that high, but i'd not short yourself the ability to provide those at a bare minimum.

Voltage sag and damaging your cells and poor performance...  that's what will happen unless you build a @Chaka 8p setup...  voltage sag will be huge - you'll get a fraction of the range.  Run ok (if you are lucky) on the flats and no guts for hills.  And possibly damage and unbalance the cells from over discharge.

But we should hear from one of the experts like @barajabali who makes packs and hopefully can chime in.

Not to knock the idea - but maybe as a "for now" or just to start setup until you get a better battery?
```

---
## \#5 Posted by: barajabali Posted at: 2017-04-18T14:47:05.746Z Reads: 99

```
Pretty much what @sl33py said. 

Laptop batteries will only work for you with huge packs for ebikes or cars where you can really stack cells up and get that amp rating high enough. I don't reccomend using old cells or even different cells for that matter just for consistency. Also BMS's are only to be used with brand new cells. 

I've built laptop packs way back in the day and they simply don't work. Not as in they work but it's a bad idea, no they do not work at all. The amp raring is too low even with a fully charged battery the vesc will shut down (or at least mine did) the cells will take you a few feet if you don't accelerate too hard then just shut off. They're meant to be used for really lightweight electronics
```

---
## \#6 Posted by: Gepson Posted at: 2017-04-18T17:30:44.643Z Reads: 85

```
Ahhh thanks guys, this is not the answer I wanted to get but i was really expecting it :p . It works on e-bike because they have some mechanical assistance for the motor that a skate doesn't have.
So I'll kill my creative mind right in the egg and go for a 2x 6S 5000mA Multistar. 
On a side note: i saw a lot of people giving conflicting information about spot welders and batteries, some argue that the electrical contact is not as strong as a good ol' soldering(which makes sense for me) but on the other hand you might damage your cell with too much heat. I saw a lot of people designing their batteries without spot welding and they seem to be just ok with it.
```

---
## \#7 Posted by: sl33py Posted at: 2017-04-18T17:42:20.659Z Reads: 82

```
Thanks @barajabali!  I knew it would work poorly if at all, but if it sagged enough to trip the low voltage cutoff in VESC it would un-rideable.  Good to confirm.  I've never tried this since i knew it couldn't supply enough amps to run.  But sounds like it wouldn't just run poorly - it won't run at all.  Risks aside about damaging cells...
```

---
