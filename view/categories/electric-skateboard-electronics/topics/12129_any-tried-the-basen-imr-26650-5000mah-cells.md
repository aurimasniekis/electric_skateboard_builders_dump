# Any tried the BASEN IMR 26650 5000mAh Cells?

### Replies: 27 Views: 3800

## \#1 Posted by: evoheyax Posted at: 2016-10-29T19:02:09.878Z Reads: 223

```
So I'm looking at alternatives to the 18650s, as I either get high amps and low capacity or high capacity and low amps. To get both, you need a massive pack. So I found these 26650 cells which are rated to 50 amps continuous and have 5000 mAh!I can fit a 12s3p of 26650s in the same space as a 12s4p with 18650s (I build my decks to have 27mm of space inside in height anyways). So here's the comparison:

18650 LG HE2:

- 12s4p
- 80 amps continuous
- 504 Wh

26650 BASEN IMR:

- 12s3p
- 150 amps continuous
- 756 Wh

Basically, I could get almost double the max continuous amps, and 1.5 times the range. And it would fit in my board as is right now. But this seems too good to be true... Is it? Am I over looking anything? Has anyone tried these cells before? Thoughts?
```

---
## \#2 Posted by: Namasaki Posted at: 2016-10-29T19:10:28.117Z Reads: 219

```
Are you sure that they're 50a continuous and not 50a pulse?
```

---
## \#3 Posted by: evoheyax Posted at: 2016-10-29T19:12:39.124Z Reads: 216

```
https://www.google.com/url?sa=i&rct=j&q=&esrc=s&source=images&cd=&ved=0ahUKEwie59D224DQAhXGhlQKHTWWBkYQjRwIBw&url=http%3A%2F%2Fwww.ebay.com%2Fitm%2F2-BASEN-IMR-26650-HIGH-DRAIN-50A-60A-5000mAh-RECHARGEABLE-BATTERY-3-7v-w-case-%2F371687201846&bvm=bv.137132246,d.cGw&psig=AFQjCNGcYH2Hy9xFMsjDQ55RyEQdGMWhrg&ust=1477854694456061

It says it right on the cells. 60a pulse, 50 max continuous.
```

---
## \#4 Posted by: Namasaki Posted at: 2016-10-29T19:19:39.494Z Reads: 204

```
I would not not trust those batteries on eBay. 
They look like counterfeit. 
The Basen black 26650 is a 4500 mah battery with 60a pulse and 25a continuous. 
I built a 10s2p pack with them and it worked fine on flat ground but the voltage sagged a lot going up hills.
```

---
## \#5 Posted by: evoheyax Posted at: 2016-10-29T19:24:32.238Z Reads: 200

```
https://liionwholesale.com/products/basen-4500mah-26650?variant=14135870212

Says the 4500 mAh is 40 continuous. Are you sure its really 25?
```

---
## \#6 Posted by: Namasaki Posted at: 2016-10-29T19:25:21.370Z Reads: 200

```
Oh, wait, I just found them on Basen website. 
They must be new. 
Still hard to believe they can handle 50a cont but only 60a pulse. 
http://www.basengroup.com/product_view.asp?id=60
```

---
## \#7 Posted by: Namasaki Posted at: 2016-10-29T19:26:41.014Z Reads: 197

```
Some claim it's 40a. 
I talked to a factory rep at Basen. He said 30a
Mooch tested them and rated them at 25a
```

---
## \#8 Posted by: Namasaki Posted at: 2016-10-29T19:27:54.666Z Reads: 200

```
I just gave up on Li-ions and went back to Lipos because of voltage sag. 
And I didn't want to have a 6-8 pound battery
```

---
## \#9 Posted by: IDVert3X Posted at: 2016-10-29T19:29:37.501Z Reads: 193

```
They are rated at 50A, but in reality, they are more like 25A from what I have seen on other forums and real world testing.
```

---
## \#10 Posted by: evoheyax Posted at: 2016-10-29T19:55:40.491Z Reads: 189

```
So are there any 26650 cells out there with real continuous ratings that are more than 25a?

Looking through what Mooch said about 26650s, and he seems to think they are all vastly over exaggerated... I'm looking for 100 amp con or higher for the whole pack, as I'm trying to reduce sag...
```

---
## \#11 Posted by: sl33py Posted at: 2016-10-29T20:31:35.763Z Reads: 188

```
A123 systems ANR26650M1-B 2500mAh - 70A

Not sure what the measured discharge amps are, but they are higher, with the cost in capacity at only 2500mAh.

Digging further - this looks like an excellent cell for us, if you do some in parallel for better mileage.

Mooch:
[quote]This is an extraordinary cell that I am rating at 30A. My maximum vaping amps (MVA) rating is 70A. The two cells I received from EnerCig and the two from Nkon appear to have come from the same batch.



The datasheet has a "maximum continuous discharge" rating of 70A in the 
datasheet. But at that temperature, about 85°C, the cell will have a 
significantly reduced cycle life. This rating is an absolute maximum, 
not a level you should operate the battery at for every cycle. To allow 
direct comparison against other batteries I am rating this cell at a 
level, 30A continuous, which limits the temperature to 60°C to ensure 
good cycle life. Above this temperature the cell's aging accelerates 
significantly. The cell can easily be pulsed at levels above 80A though.



This cell's lithium-ferrous-phosphate (LFP) chemistry is the safest of 
the Li-Ion chemistries we use. While this should never be used as an 
excuse to do so, these A123's can take a lot of abuse before going into 
thermal runaway. If they do go into runaway their reaction isn't as 
violent as the other chemistries.



The voltage of this cell is very steady for most of the discharge, very 
similar to LiPo's. This is great for unregulated/mechanical mod users. The iJoy 4200mAh 26650 is a better choice for vaping at up to about 40A though.[/quote]
```

---
## \#12 Posted by: lox897 Posted at: 2016-10-29T20:33:21.080Z Reads: 169

```
What sl33py said. A123 26650 are 70a continuos and not too bad in capacity
```

---
## \#13 Posted by: sl33py Posted at: 2016-10-29T20:38:26.650Z Reads: 171

```
A couple caveats it seems...  primarily the reverse construction and 3.3v nominal not 3.7v!
[img]https://www.e-cigarette-forum.com/forum/attachments/image-png.608917/[/img]
[quote]
Things To Be Aware Of

- Their nominal voltage is 3.3V. This means they can't be used in regulated mods
 and their much lower voltage, when drawing a lot of current from them, 
probably limits their use to series unregulated/mechanical mods only.



- These batteries require a 3.6V charger! You cannot charge them to 4.2V.



- At high current levels the nominal voltage drops to as low as 2.5V.



- Unregulated or PWM mods using a MOSFET for button protection may not 
be able to use just one of these cells or use them just in parallel. The
 nominal voltage will be too low to turn many MOSFETs on fully at higher
 current levels. This can cause them to overheat and burn out.



-The "button" end of the cell is the NEGATIVE terminal, not the positive.



- The metal case of this cell is the POSITIVE terminal, not the negative like the other cylindrical cells we use.



- Due to the need to operate these in series, and their "reversed" 
polarity construction, I strongly recommend that only experienced vapers
 with in-depth knowledge of Ohm's Law, battery safety, and understanding
 of the ratings and requirements of this cell try using it. If you have 
questions that you cannot otherwise find the answers to, I urge you to 
not use this cell.

[/quote]
From:
https://www.e-cigarette-forum.com/forum/threads/a123-anr26650m1-b-2400mah-3-3v-26650-bench-test-results-an-extraordinary-battery-with-issues.770987/
```

---
## \#14 Posted by: evoheyax Posted at: 2016-10-29T20:41:15.117Z Reads: 159

```
So it seems like 26650's might not be the solution after all... I wouldn't really gain anything and maybe loose range since I would be at 7500 mah with the A123 instead of 10000 mah with the 18650s.

Lipos seem to be better in the short run...
```

---
## \#15 Posted by: Namasaki Posted at: 2016-10-29T22:14:40.708Z Reads: 158

```
http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014
```

---
## \#16 Posted by: johnny_261 Posted at: 2016-10-30T08:13:22.015Z Reads: 148

```
I can agree with @Namasaki , I have a Basen 6s2p pack and while the range is great on flat, of course it does have a lot of sag.  Maybe 3p might be okay at 12s, but likely you will still have some sag.

I haven't fully tested the range, but on this 6s2p I feel like I can get 15-20km.

My daily commute is 9kms and depending on if I do a route with hills or not, I have between 50-70% when I'm back home.

Basically I think it's safe to assume that you can only get the amount of amps as an 18650 from these cells. So if its the same space as 12s4p, go with that for less sag.
```

---
## \#17 Posted by: Namasaki Posted at: 2016-10-30T12:30:35.486Z Reads: 135

```
I think voltage sag is one of the main challenges we face with esk8 design. 
Even my 10s 60C Lipo pack capable of 300a cont sags a little when going up hills. Still, much less than anything else I've tried so far.
Accelerating up a 15% grade, total voltage only drops around 1 volt. That's only 1/10 volt per cell.
```

---
## \#18 Posted by: rpn314 Posted at: 2016-10-31T02:41:50.213Z Reads: 123

```
@Namasaki is definitely the master. Specs seem a little out there, and I would be very wary of any Li-Ion batteries on ebay, but the brand and size are not unheard of (@Namasaki's build) : http://www.electric-skateboard.builders/t/diy-battery-pack-using-basen-26650-hi-drain-li-ion-cells/4973.
```

---
## \#19 Posted by: barajabali Posted at: 2016-10-31T03:19:54.314Z Reads: 117

```
Let's get @anorak234 opinion on this I just built him 2 6s1p packs and I'm curious how they're riding?
```

---
## \#20 Posted by: anorak234 Posted at: 2016-10-31T03:24:56.942Z Reads: 114

```
One is riding great (the perfectly balanced), haven't done extensive testing with the other yet because it's been raining on/off in the bay area recently. Gets about 4.5 miles of range (1000mah/mile). Both of my packs are with the 4500mah 26650s
```

---
## \#21 Posted by: barajabali Posted at: 2016-10-31T03:51:46.945Z Reads: 108

```
Oh snap you're getting 4.5 miles per pack? That's crazy.  Is it on that short board with the bindings?
```

---
## \#22 Posted by: anorak234 Posted at: 2016-10-31T03:55:06.338Z Reads: 106

```
Yep. Rides like a dream - especially with the bindings. Starts at 24.4 and ends at 21.6, no problems in between. To be fair it is on flat ground, medium speed. I'll post test runs if i can get some in this week
```

---
## \#23 Posted by: johnny_261 Posted at: 2016-10-31T05:44:09.193Z Reads: 106

```
Just did some range testing on my board today.  Got 21kms on a 26650 6s2p.

Capacity is good on these cells, voltage sag is bad...
```

---
## \#24 Posted by: anorak234 Posted at: 2016-10-31T18:20:51.798Z Reads: 98

```
I'm with you there - trying to figure out if I can reconfigure my esc it seems to stop temporarily if voltage sag hits nominal voltage
```

---
## \#25 Posted by: barajabali Posted at: 2016-10-31T19:31:41.999Z Reads: 91

```
I thin if you ran your packs in Parallel you'd have less sag
```

---
## \#26 Posted by: longhairedboy Posted at: 2016-10-31T19:52:45.658Z Reads: 89

```
[quote="Namasaki, post:8, topic:12129"]
And I didn't want to have a 6-8 pound battery
[/quote]

I've been thinking about that too. My 12S4P packs weigh 5 pounds, which makes me wonder what 12 10ah lipos would weigh and what kind of footprint that would have. Cycle life is a trade-off though from what i understand.
```

---
## \#27 Posted by: evoheyax Posted at: 2016-10-31T20:32:14.325Z Reads: 84

```
The same here. I'm half temped to go back to lipos because I can fit a larger pack with lipos than lion in the same space. I need to make a decision soon though as I need to build another battery pack soon for my next board to test the vesc-x with.
```

---
