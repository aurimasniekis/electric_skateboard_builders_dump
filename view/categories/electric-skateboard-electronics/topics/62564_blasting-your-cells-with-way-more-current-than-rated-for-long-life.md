# Blasting your cells with way more current than rated for long life

### Replies: 15 Views: 524

## \#1 Posted by: Hummie Posted at: 2018-07-22T21:49:48.959Z Reads: 207

```
this is just a snip from a study posted on research gate and cant post the whole study.  There have been a couple similar.  

 It's been confirmed by an expert that while this test was done with lithium sulfur cells the results should be similar to all lithium cells![Capture|690x384](upload://kyn1iN9UTY1VOGA2mUJRxKk11u5.JPG)

i cant do math. based on the start of this strange repairing action happening at at least 9mA cm^-2...what current would that be for a single 18650?
```

---
## \#2 Posted by: Hummie Posted at: 2018-07-23T18:02:16.439Z Reads: 172

```
no one can do this math on the current density?
```

---
## \#3 Posted by: deltazeta Posted at: 2018-07-23T23:37:14.498Z Reads: 154

```
Needs more context. You can do some basic unit matching on the value to get some supposed values, but without knowing how they got the 9mA cm^-2 in the first place its just wild guessing.

i.e.
![33%20PM|534x128](upload://tgmA9ttLPoxFctfSuePv47JA6Qq.png)
![10%20PM|406x362](upload://izQrgGjKqqogC1ah7Ew7eHfR9Ga.png)
22mA is far too low to make sense contextually


I'd wager a guess that you'd have to know the surface area of the rolled sheets in a 18650 in order to get the value you're looking for
```

---
## \#4 Posted by: Benjamin899 Posted at: 2018-07-23T23:57:42.128Z Reads: 147

```
another thing to know would be what this healing treatment is and if it is worth it the hassle. i guess in our aplications the damage to the cells over time would be more severe. 
This is what i found from a quick search, interesting.
https://news.rpi.edu/content/2018/03/29/heat-temperature-heals-lithium-dendrites
```

---
## \#5 Posted by: Hummie Posted at: 2018-07-24T01:43:19.470Z Reads: 132

```
thanks yea it seems like its missing something.   i can cut and paste the whole study if anyone wants it or it would help with the math.  unfortunately this seems the only formula.

but the results of this heating procedure do have great benefits as it was said that this works on all lithium cells.  Ive also heard of another procedure using high speed pulses as apposed to a full charge cycle.   regardless of the details it makes me rethink charging and possible regen limits and the study i posted a pic from showed great results.  surprisingly its safer to blast your cells with high current sometimes.
```

---
## \#6 Posted by: deltazeta Posted at: 2018-07-24T21:45:36.111Z Reads: 99

```
I did a bit of digging into this and based on the whitepaper, I would definitely say finding the surface area of the lithium in a 18650 would give us at least something of a reasonable current. So looking into trying to find these industry secrets led me to a teardown video of a Tesla 18650(https://electrek.co/2017/03/22/tesla-battery-cell-breakdown/, https://youtu.be/CxS7XeIh_i4). I'm led to believe this is a panasonic cell, not exactly a samsung 30q, but the internal design of most high quality 18650s is likely somewhat similar. Video shows the "jelly roll" and mentions some estimates of dimensions, so here's what i'm working with:

* Length is ~1m
* Width is ~65mm

So with these much larger numbers and the same formula as before:
![46%20PM|690x240](upload://npTNzAMvrX3WEcuFsIhfCBANsg4.png)

And here I think we have something usable. As a sanity check, their baseline .75mA/cm^2 with these dimensions led to ~5A discharge, perfectly reasonable(even low) for a 18650 cell, especially one used for an electric vehicle. Here's where things get interesting, at 9mA/cm^2, a 18650 would have to be discharged at ~58A!!! While I'm completely unsure how this would work in practice, the theory is quite jaw dropping. 

As a warning, however, while lightly reading the paper and looking for 18650 information, I never saw this kind of technique translating to anything outside the lab. They mentioned testing with a conventional Li-S button cell, but that kind of power flow is much much smaller.
```

---
## \#7 Posted by: Hummie Posted at: 2018-07-24T21:56:46.947Z Reads: 89

```
i was asking on endless sphere and a similar technique is used on other types of batteries including lead acid and some others but more so with high current pulses I think and not a complete charge cycle.  
50 amps... wow

ive read other explanations of very fast chargers doing huge current up until half full and it's only as the cell becomes more full that the ions have trouble finding a place to fit and i think get hotter then, but charging from a very low state with high currrent regularly up to about 50 percent.  

i think this is super info, not that we really know for sure and it is based on your assumptions at this point but think how awesome would be...charge wayyyyy faster sometimes and ultimately be healing your cell damage and allowing greater energy storage and less likelyhood of an internal short and fire.  its the ultimate irony.  hope you find more!
```

---
## \#8 Posted by: Minim Posted at: 2018-07-24T22:06:22.301Z Reads: 82

```
This is how my tesla behaves when I charge on supercharger. If the battery is hot it charges with 120kW (max) up to like 50-60% and then it rolls off. At 80-85% I think it’s down to like 30kW and then it kinda stalls out there slowly towards max. I just took these numbers from memory but you get the idea. It also limits charging when the battery is cold. It limits regen to the battery when battery is cold also but when it’s hot I can do 60-70kW regen when braking. And for max power you have to use the battery heat function. I think the BMS is pretty advanced but this is just what I noticed when driving it. The battery is 7-8k 18650 cells so it’s just a big eSkate battery :D
```

---
## \#9 Posted by: Hummie Posted at: 2018-07-24T22:17:33.366Z Reads: 74

```
.if you knew exactly how much current it puts in the battery when charging at its max charge rate divided by that 7-8k.   id like to know.  then we could correlate it with the spec sheet, if there is one for the tesla cells and see if they're dumbing it down for the public and giving just a general charge rate as typical.   there really seems a charge rate that greatly differs based on state of charge, and then beyond that there's this crazy study where you just blast the cell till full charge (ill have to check on that to be sure again)
NICE CAR.
```

---
## \#10 Posted by: Minim Posted at: 2018-07-25T00:44:54.149Z Reads: 69

```
There are many people that have documented this. This is what I found when doing a quick search. This is from a model3 with a smaller battery than my model s but the curve look very similar. There are prolly some showing amps also as the screen on the car can show volt/amps instead of kW if I recall correctly.

https://teslamotorsclub.com/tmc/threads/supercharger-speed-116kw.107619/?utm_source=threadloom&utm_medium=email&utm_campaign=ed9&utm_content=iss30#post-2540001
```

---
## \#11 Posted by: Hummie Posted at: 2018-07-29T06:44:17.936Z Reads: 60

```

https://teslamotorsclub.com/tmc/threads/supercharger-speed-116kw.107619/?utm_source=threadloom&utm_medium=email&utm_campaign=ed9&utm_content=iss30#post-2540001 
if the tesla cell is 3ah cell, which it pretty much seems to be, and 125 miles is about half of the 265 miles stated full charge miles (so i read), you can make assumptions and wouldnt it then have to be charging at 6amps a cell as it's getting almost to half charge in a quarter hour?  


but I read 120kw is the highest rate the chargers do.and i get 3.5 amps charge rate a cell if 7000 cells so i still dont know what's the peak charge rate.  



https://www.amazon.com/Adjustable-Converter-Switching-Regulator-Transformer/dp/B07DZW79KM/ref=sr_1_7?ie=UTF8&qid=1532843332&sr=8-7&keywords=48v+adjustable+power+supply
this is the charger i want.   it seems to have what would be in effect a cc/cv do it yourself ability with the two knobs one for v and one for c.
```

---
## \#12 Posted by: Minim Posted at: 2018-07-29T07:22:59.364Z Reads: 53

```
This shows more accurate numbers while charging but I still don’t see cell/A. Replying from phone now so it’s a bit of hassle to search :confused: 

https://youtu.be/tQ5takpm4Xs
```

---
## \#13 Posted by: Holyman92 Posted at: 2018-07-29T20:30:48.185Z Reads: 38

```
For science I would not be opposed to opening up a 30Q cell... however I would have to go out to the sand trap on my property before even considering this in case of... well, lithium going unstable
```

---
## \#14 Posted by: Hummie Posted at: 2018-07-29T21:45:20.520Z Reads: 35

```
Or a good metal box.  Or polycarbonate to see.  clamp it down and then no worries maybe 
Or a different approach and put in the bottom of a hobby store rocket.  

I found and lost a paper on the web that was doing 6c,5c..and w temp sensors n claimed 5c was acceptable as it kept within the maker specs. But didn't see what specific ion cell they were using.  The easy fun way to find the answers is a test.   the 30q.  Hope u do.  

Be nice if u charge w a meter to measure the in-going capacity recording from some set low soc to 4.0 and then discharging on a board as u normally would immediately.   And maybe just an infrared temp at each rising volt.  

The power supply will be a lot (ill link one) but worth charging the whole board so you can discharge it and it's practical, and see how the cells heat each other while charging.  

Id rather fast charge to even a low voltage and not even bother going past maybe 60% charge if i could do it with great speed and still maybe even this would have greater all around safety and the cells lasted more cycles and kept their capacity. maybe. maybe the heat produced would be ideal for the cells as apposed to their typical cold state when charging

  But it sounds like you can have your cake and eat it from the study above and just blast more in to full charge.  they skip any concern for heat which is a big omission.  Id like to see you do that test too.

  if you have a place safe for a possible fire and smoke and are willing to pay for the charger and have a temp sensor and a way to monitor each cell (even 10 dollar stick onto balance ports) that's all that's needed.  30Q is 3ah and at 5c with a 12s4p pack...15 amps each cell and four in parallel..60amps.  PLEASE TAKE VIDEO!!    Or maybe just try one cell first at 15.  my supply will do 10 and maybe i'll just try that.  someone is supposed to step in and say you shouldnt do this.
only 50 amps but still.  wire in a wattmeter. 
https://www.jameco.com/z/RSP-2400-48-MEAN-WELL-AC-to-DC-Power-Supply-Single-Output-48-Volt-50-Amp-2-4kw_2106722.html
```

---
## \#15 Posted by: Holyman92 Posted at: 2018-07-29T22:21:04.265Z Reads: 30

```
I was saying I would dissect a 30Q and unroll it to give you guys the surface area
```

---
