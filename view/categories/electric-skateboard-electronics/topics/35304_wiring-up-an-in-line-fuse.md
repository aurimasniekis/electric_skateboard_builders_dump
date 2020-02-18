# Wiring up an in-line fuse

### Replies: 27 Views: 2510

## \#1 Posted by: High-roller Posted at: 2017-10-11T11:16:03.794Z Reads: 357

```
What with all the various ways you have to burn out a vesc via overcharge, I thought I'd try to eliminate one by adding a fuse to my wiring.
Can someone please check me on this:
The xt60 plug in the top of the picture comes from the battery, down through the loop-key, and on to the vescs. Is where I've placed the fusebox correct?
Also, my battery is a 10s5p (12ah) so I got a 15 amp fuse. Is that right or should I have gotten one with a lower rating?
<img src="/uploads/db1493/original/3X/9/6/96dd46c12659f3be91a4aa4aefdbe7861f1697f6.jpg" width="375" height="500">
```

---
## \#2 Posted by: krloz Posted at: 2017-10-11T13:09:40.627Z Reads: 333

```
I think those car fuses are rated for up to 24V. I'm not sure it's good idea to feed it 42v. And 15Ah is VERY low.  You have to go higher than your max Battery amps
```

---
## \#3 Posted by: High-roller Posted at: 2017-10-11T13:13:33.762Z Reads: 333

```
Forgot to add- my battery is 36 volts, is that okay or still too high?
How do I calculate max. battery amps? Is that where the C rating comes in? As in : amps x C = max. battery amps?
If not, what fuse should I get?
```

---
## \#4 Posted by: krloz Posted at: 2017-10-11T13:22:41.979Z Reads: 362

```
You said your battery is 10S. that means it's nominal is 36v but the maximum voltage at full charge (4.2v per cell) is 42v. And the max is what you have to look for. 
A 24v fuse could work but when it blows it might not blow properly enough and not protect your electronics.  There are some specialised fuses rated for 58v in mouser for example.  

The amps have to be rated for the maximum current you might have or want.  The maximum current a battery can give is its amps capacity  multiplied by its c rating. If you are ussing a vesc  you can limit this value to something lower (max battery amps)thus this would be your Max amps
```

---
## \#5 Posted by: krloz Posted at: 2017-10-11T13:27:11.920Z Reads: 351

```
 Search and read

https://www.electric-skateboard.builders/t/what-fuse-do-you-use/6457

https://www.electric-skateboard.builders/t/how-to-fused-xt90-s-anti-spark-loop-key/16912

https://www.electric-skateboard.builders/t/what-fuse-to-use-for-100-amp-12-s-protection/17054

https://www.electric-skateboard.builders/t/fuses-correct-voltage-rating/29720
```

---
## \#6 Posted by: High-roller Posted at: 2017-10-11T14:57:17.173Z Reads: 282

```
The cells in my battery pack are Samsung 25r's. Their 3.7 volts each so shouldn't it be 37 volts instead of 42? 
Based on a quick read through the above links, most folks seem to be going for a 58v fuse, like you said. I was hoping to find one that would fit in the housing in the pic I posted.
```

---
## \#7 Posted by: psychotiller Posted at: 2017-10-11T15:27:09.505Z Reads: 264

```
Nope! they charge to 4.2v per cell.
```

---
## \#8 Posted by: krloz Posted at: 2017-10-12T06:53:40.336Z Reads: 245

```
I have never found a fuse so small it could take 58v sorry. 
As I said your cells are 3.7v nominal.  That means they are around 3.7v at medium charge (for simplification.  Read on nominal voltages if you need something more precise) so let's say at around 50% charge they have 3.7v. When they are completely depleted 0% charge they should be around 2.8-3v depending on the life you want to give them.  And when they are fully charged they are at 4.2v. You could go higher but that would damage your cells.  So on a fully charged 10s pack you have 42v.
[quote="High-roller, post:1, topic:35304"]
Also, my battery is a 10s5p
[/quote]

Your cells have a maximum of 20A discharge.  With 5 in parallel you can expect 100A maximum discharge from your pack.  If you want to be able to get all that juice out you need a 120-150 fuse.  Or lower if you set limitsl
```

---
## \#9 Posted by: High-roller Posted at: 2017-10-12T16:30:19.015Z Reads: 216

```
Woah, okay thanks, that clears up a few things. I hadn't considered the max. discharge properly.
So let's say I want my board to be able to climb hills decently but nothing too steep, and odds are I won't be going full speed very often- what would a good setting be? I see lots of people seem to set it at 60  amps.
For that matter just how helpful is the fuse? Since I have FOCboxes I assume that their heat-sinks would help somewhat prevent these problems, but how much?
```

---
## \#10 Posted by: b264 Posted at: 2017-10-12T16:32:49.160Z Reads: 207

```
Once you find the right fuse, it gets wired in just like another loop key.
```

---
## \#11 Posted by: High-roller Posted at: 2017-10-12T16:37:20.935Z Reads: 199

```
That's exactly the plan, put it in-line right after the key. I'm just trying to figure out what fuse to put in there, if there's even one that'll fit it. 
Someone told me that because these are automotive fuses they tend to take a bit longer to burn out if they're put over their rated current, which might be a problem for the electronics. Anyone know about this?
```

---
## \#12 Posted by: b264 Posted at: 2017-10-12T17:50:43.258Z Reads: 194

```
[quote="High-roller, post:11, topic:35304"]
put it in-line right after the key
[/quote]

I'd put it inline right before (closer to battery) the key
```

---
## \#13 Posted by: b264 Posted at: 2017-10-12T18:01:33.971Z Reads: 188

```
There aren't many fuses that are >45V and >100A that would physically fit in a skateboard.  I did [find one](https://www.digikey.com/product-detail/en/littelfuse-inc/142.7010.6122/142.7010.6122-ND/5234200) but the selection is very small.  
  
edit: none of those are in-stock, either...
```

---
## \#14 Posted by: High-roller Posted at: 2017-10-12T18:31:33.936Z Reads: 179

```
What's the difference?
Thanks for trying to find one anyway. I'll look around and see what there is. I'm really curious to know whether my focbox heat-sinks will be enough on their own, that way I could save myself some hassle.
```

---
## \#15 Posted by: krloz Posted at: 2017-10-13T09:29:17.999Z Reads: 177

```
[quote="High-roller, post:9, topic:35304"]
how helpful is the fuse?
[/quote]

The fuse is not there to limit the amps to the vesc and protect it from overt heating.  That's what the amps and temp limit are for.  I think the focbox is rated for 60A but not sure.  Fuses are there to prevent shorts from damaging your vesc and batteries.  A fuse "should" never blow under normal conditions while amp limits should quick in when you get near your limits like prolonged hill climbing.
If you are only using a single focbox limited to 60A you could do with a 80-100 Fuse as in normal conditions you would never get near that range meaning if it blows there was a short. 
Or If you are ever planning on going dual you could use a 120A fuse limiting both vesc to 50A or a 150A fuse going dual 60A (these would be me)
```

---
## \#16 Posted by: High-roller Posted at: 2017-10-13T10:31:20.925Z Reads: 165

```
This is perfect, thanks! 
I can only get 100 amp ones at the moment, and I have dual FOCboxes. If I set them to 50A will that be okay?
Bty, the size difference between a 100 and a 150 fuse is MASSIVE!
```

---
## \#17 Posted by: krloz Posted at: 2017-10-13T17:45:59.761Z Reads: 163

```
The Thing is. When you're fuse is so near to your maximum values thru could blow off when driving to your maximum.  100A is a beast of power.  But limits could be slightly overpasses while the vesc adjusts itself and fuses have tolerances.  Ie it really is 100A +- a small percentage.  And you really don't want your fuse yo blow if nor 100%needed. 
I would really leave a margin between your limited maximum and your fuse value of around 20% but that's up to you.

From Mouser Spain I can get these in 100 125 and 150A
http://www.mouser.es/Search/m_ProductDetail.aspx?Littelfuse%2f14256316122%2f&qs=sGAEpiMZZMsh2y49K8ANrTdpOrToc%252bEOWEps5yIgKK0%3d
```

---
## \#18 Posted by: High-roller Posted at: 2017-10-14T18:12:01.744Z Reads: 161

```
Thanks for the advice. I just ordered a set of four 150amp ones on ebay. As you say, better to have a safety margin.
http://www.ebay.com/itm/4-Pack-150-Amp-Mini-ANL-Fuse-Fuses-Gold-Plated-Inline-Quality-150A-/192124248960?hash=item2cbb7f6380:g:VHQAAOSwcj5ZVEAH
```

---
## \#19 Posted by: composites_r_awesome Posted at: 2018-01-21T11:19:10.135Z Reads: 140

```
Hi, how have your fuses been working so far?
```

---
## \#20 Posted by: Sebike Posted at: 2018-01-21T11:43:06.110Z Reads: 140

```
Aren't the fuse amp ratings also related to volts of the application, so that a 150A car fuse will blow at around 150 A when voltage is around 12v. Using the same fuse with higher volts will cause fuse to blow at lower amps, no?

I'd guess this would be related to max watts of the application, so that a fuse that blows at 80 A with a 10s system would actually equal a 280 A rated car fuse (12v). I might be totally off, but maybe someone with more knowledge could correct me? :smile:
```

---
## \#21 Posted by: SkaterBoy58 Posted at: 2018-01-21T14:51:21.043Z Reads: 131

```
Fuses are related to current only.
Current above fuse rated current heats up the element and when it is hot enough it melts and breaks the circuit
10A on a 100V curcuit has the same melting power as 10A on a 10V circuit.
Above is true for a simple wire fuse(such as auto fuse)
Cheers
```

---
## \#22 Posted by: Sebike Posted at: 2018-01-21T15:48:18.339Z Reads: 130

```
Thanks, that makes sense. 

But does a fuse with lower voltage rating cause a significant voltage drop then, or what's the point of using fuses with matching voltage rating?
```

---
## \#23 Posted by: krloz Posted at: 2018-01-22T18:32:21.389Z Reads: 126

```
Well. I haven't actually gotten to mounting them. Though I did buy and receive them already.  Bought from arrow to save in shipping and ended paying more in import fees but ohh well...

![20180122_192425|666x500](upload://daV8ubibkCyxW4C2g3jC6ZYzvNM.jpg)
Bought a bunch of these for a couple of different size battery packs. And planning to 3d print something to mount them. 

![20180122_192535|666x500](upload://4muYbfyVibNg4kUbaMNcnSTrZp6.jpg)
Also got a bunch of these to protect charging sockets and the vescs from other electronics failure. 

All rated to 58V and automotive category so pretty sure they will hold up to the power and vibrations
```

---
## \#24 Posted by: composites_r_awesome Posted at: 2018-01-22T22:15:08.004Z Reads: 122

```
Thank you SO much for the pics with a ruler next to them, helps a lot in getting better picture than dimensions alone
```

---
## \#25 Posted by: SkaterBoy58 Posted at: 2018-01-23T06:07:07.492Z Reads: 116

```
the volt drop across a fuse is proportional to its (very low) resistance and is nothing to do with the voltage rating.
```

---
## \#26 Posted by: SkaterBoy58 Posted at: 2018-01-23T06:09:33.137Z Reads: 115

```
The voltage rating is linked to the lenght of the air gap created when the wire element melts. I have used and blown a number of 12V auto fuses on a 42V circuit with no problems.
```

---
## \#27 Posted by: krloz Posted at: 2018-01-24T09:47:25.283Z Reads: 110

```
You are welcome.  It does also help me get an idea of what it's going to take up in the enclosure. 
Did anyone notice I fucked up with the hole size of the big fuses....I didn't.  I thought I ordered same size for both ratings
```

---
