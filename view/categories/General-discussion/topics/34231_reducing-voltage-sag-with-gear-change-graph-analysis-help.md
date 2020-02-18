# Reducing Voltage Sag with Gear Change - Graph Analysis Help

### Replies: 59 Views: 2154

## \#1 Posted by: cody00 Posted at: 2017-09-29T00:59:52.338Z Reads: 175

```
After getting a HM-10 chip and using @emmaanuel 's iOS app, I have been trying to fine tune my board.  I have come to realize that I'm sagging more than normally would expect.  

The graph below is with a 10s3p (LG HG2) starting out at 40v.  Going up slight hills I'm sagging down into the 29-30v range to where the VESC resets.  On a 15min ride, I generally will have a couple of cutouts.  

I have 100mm wheels, with 16T/36T, Dual 6355 190kV,  and I weigh 205. 
I realize this isn't this probably isn't the most logical combination but I recently ordered some 40T to head in the right direction.

Is this a logical analysis of why the sagging is occurring down this far with near full charge?  Does the graph tell a different story?  Do you think the hop from 36T to 40T will have a decent impact on this sag?

<img src="/uploads/db1493/original/3X/4/1/4135ca4ffa2cb485c930765b76aa89714e80a80f.png" width="690" height="228">
**Going below 30V**

<img src="/uploads/db1493/original/3X/5/9/59623d104210f19b7a11ffc647a347a176ee6a98.png" width="690" height="225">
**This is where a VESC reset happened.**
```

---
## \#2 Posted by: Okami Posted at: 2017-09-29T06:14:43.684Z Reads: 153

```
That sounds like some crazy sag with not that bad battery pack (in theory)..

Is there a way for you to see what is happening in cell level? The drop in voltage looks a bit abnormal if u ask.me. though i would like to check your graph from pc as from mobile i cant see everything clearly.

Though i like your idea about.changing gears
```

---
## \#3 Posted by: scepterr Posted at: 2017-09-29T06:22:19.229Z Reads: 146

```
Using BMS? Specs?
Pics of battery, series, parallel connections would help too
Sagging to 3V/cell is not normal
```

---
## \#4 Posted by: willpark16 Posted at: 2017-09-29T06:29:37.062Z Reads: 141

```
I looked at your vesc settings you are drawing 30a to each motor on a battery that can output 60a max, you are essentially drawing max current from quite frequently damaging your cells causing this effect which is voltage sag, try more conservative settings
```

---
## \#5 Posted by: Okami Posted at: 2017-09-29T06:32:41.694Z Reads: 128

```
Thanks for spotting this. I had idea he is somehow overstressing the cells but couldnt make out the numbers in graph.. probably problem solved, either he needs to limit power vesc can take or upgrade his battery
```

---
## \#6 Posted by: DeathCookies Posted at: 2017-09-29T06:36:36.454Z Reads: 129

```
But his avg battery current (roughly estimated by the given graph) is about 20A max.
```

---
## \#7 Posted by: jmasta Posted at: 2017-09-29T06:38:09.576Z Reads: 132

```
Your voltage sag does not look normal for a 10s3p pack made from HG2 cells.  In the graph you are pulling about 7A/cell.  We can estimate the expected voltage sag from discharge charts.  The difference in the red line to the light blue line is the voltage drop for 7A/cell loading; reading off points at the 1.5Ah line:

10*(3.68-3.44) = **2.4V drop** under 21A (7A/cell) loading of 10s3p battery


---
 If you are actually pulling 20A per motor and not 20A total, your expected voltage sag would be:

10*(3.68-3.30) = **3.8V drop** under 45A (15A/cell) loading of 10s3p battery

---

http://lygte-info.dk/pic/Batteries2012/LG%2018650%20HG2%203000mAh%20(Brown)/LG%2018650%20HG2%203000mAh%20(Brown)-Capacity.png

It seems like you have another issue at hand.  Perhaps your serial connections cannot handle this load.  How is your battery constructed? Maybe you are unknowingly using nickel-plated steel, which has a higher resistance and would lead to a more severe voltage drop under load
```

---
## \#8 Posted by: cody00 Posted at: 2017-09-29T13:05:19.833Z Reads: 121

```
Thanks for the input guys .

Here is a graph file for http://www.gct-hp.de/VDLA/
http://s000.tinyupload.com/?file_id=05762327609852844307
(Ignore the GPS) :slight_smile: 

[I am using copper grounding strap for my battery connections.](http://www.ebay.com/itm/10-FEET-3-8-BRAIDED-GROUND-STRAP-GROUNDING-Bare-Copper-Flat-Braid-MADE-IN-USA/302414393994?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649)  I read other people doing this without issues and I used 3/8" with 40A rating which is equivalent to 8AWG which I believe people were using as well. 

I checked V of every cell before the build and then between each series after I built.  I'm not sure which direction i could go with testing it.  Charging, capacity,  and the distance i can go on the board all seem to be normal.


[Here are the exact details of my build.](http://www.electric-skateboard.builders/t/acorn-duster-loaded-vanguard-2x-torque-6355-190kv-10s3p/32585)
I am discharging without BMS with 100A Fuse Currently.
> **VESC Settings**
> Ackmaniac Custom Firmware 2.54
> Ackmaniac Custom BLDC Tool for Mac
> CAN link

> Master:
> Motor Max: 80A
> Motor Min: -60A
> Batt Max: 30A
> Batt Min: -6A
> Battery Cutoff Start: 32V
> Battery Cutoff End 30V
> Slow Absolute Max
> Use Max Watt (800 watt) ... Adjust for how im feeling

> Controller ID: 0
> PPM and UART

> Watt no reverse with brake
> Safe Start
> Multiple ESCs over CAN
> Enable Traction Control

> Slave
> Motor Max: 80A
> Motor Min: -60A
> Batt Max: 30A
> Batt Min: -6A
> Battery Cutoff Start: 32V
> Battery Cutoff End 30V
> Slow Absolute Max
> Use Max Watt (800 watt) ... Adjust for how im feeling

> Controller ID: 1
> No App
> Send Status Over CAN

<img src="/uploads/db1493/original/3X/d/0/d0df6a9310d01e3bf2a71caa60e17159ff57f22e.png" width="640" height="480"><img src="/uploads/db1493/original/3X/6/1/6188efb6e2e4b894a51633232fa41273191ba685.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/6/6/66f431474dcf44155f4dcb5abcb4b9b070f2dded.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/2/4/24819149924bee0d3bccdd842fdf5fa355aed93d.JPG" width="375" height="500"> <img src="/uploads/db1493/original/3X/e/f/effad1df56aef327a49423de52e5e41b2b652aac.png" width="690" height="329">(Not my image but how my battery is designed)
```

---
## \#9 Posted by: cody00 Posted at: 2017-09-29T13:58:15.068Z Reads: 109

```
After researching and looking at the graph more it just seems that possibly the internal resistance of these batteries are high means they are dying.  Maybe they were either bad or I damaged them in some way.  

Taken from LaserPointer forum.
> I've seen here and there posts about people having trouble with their batteries, some from DX (I've had issues, too) and other places, so now's a good time to post a simple test you can do to find the health of your rechargeable battery.

> For an example I'll use a common 18650 li-ion cell. When fully charged these carry a potential of 4.2-4.25V and when discharged 3V. This is true of any cell that hasn't shut down whether it's new or old and tired. So what is the difference between a new cell and an old cell? Internally a battery consists of an electrolyte/electrode interface where the potential is generated by chemical reactions. As the reactions progress forward and are reversed during charging, the interface slowly degrades. This degradation results in not only a loss of capacity but also an increase in what is known as the batteries internal resistance.

> **High battery internal resistance is a BAD THING for a number of reasons. First, it makes the battery output voltage drop when the battery is being used.** As soon as you take the battery out of the circuit to measure its voltage, the voltage rises and it seems OK again. Secondly, high internal resistance saps output power from the battery's already diminished capacity. This sapped power winds up as HEAT in the battery and can cause ugly issues and further degradation.

> **Measuring the battery's internal resistance is simple. All you need is a 4 ohm 5W power resistor or similar and a multimeter. Five common 1W 1 Ohm resistors in series would work. If you aren't measuring an 18650, choose a load resistance that will load the cell but not overload it. Capacity/3 should be ok.**

> 1) First, measure the battery's voltage when charged. This is V1
> 2) Next, connect your multimeter leads to each side of the resistor and briefly connect the resistor across the battery. Note the voltage reading, this is V2.
> 3) Measure your resistor to get its precise resistance, this is R

> 4) The battery's internal resistance (Ri) is calculated with the formula:

> Ri = (V1-V2)*R/V2

> Example: cell measures 4.2V unloaded, 4.0V when connected to a 4 ohm resistor has an internal resistance of 200 mOhms (0.2 ohms)

> A new high quality 18650 battery will have an internal resistance under 100mOhms.

> A used up 18650 battery will have a resistance 400mOhms or more.

> So, feel free to test a few batteries you have around and post what you find!!
```

---
## \#10 Posted by: Okami Posted at: 2017-09-29T16:31:43.504Z Reads: 97

```
Good tip. He needs to meausre internal resistance. Some chargers can do this, if u select right mode
```

---
## \#11 Posted by: scepterr Posted at: 2017-09-29T16:37:24.037Z Reads: 101

```
I would check the series connections. 
This sag isn't normal unless you've been cycling the cells daily for atleast 2 years. If your cell resistance was as high as suggested above you wouldn't be able to fully charge, it would get stuck at like 4.1-4.15 or even lower and start heating up like crazy, and drop voltage as soon as you remove from charger.
```

---
## \#12 Posted by: scepterr Posted at: 2017-09-29T16:38:32.668Z Reads: 101

```
I have 10yr old 18650s with a resistance less than 150mohms...
```

---
## \#13 Posted by: cody00 Posted at: 2017-09-29T16:49:17.421Z Reads: 97

```
Well these characteristics are definitely not happening.
I'm not sure where i could go with testing the series.  If you look at the battery image above, you can see the pattern of how i soldered the braid to make the series (image 1).  I then fold it over. (image 2)  In the back of my head, I wonder if this would be an issue.  I've also heard people preach about not soldering batteries.  None of them got so hot where I couldn't hold them - so i like to think that i didn't damage it.
```

---
## \#14 Posted by: scepterr Posted at: 2017-09-29T16:50:59.931Z Reads: 95

```
Check that the series connections didn't get burned
Also you don't have insulator caps on the cells?(nvm just saw them)
You do seem to have solder spray all over...
How is this not shorted 🤔
<img src="/uploads/db1493/original/3X/1/e/1e7afec2800364365ecd5cb8bb6d4533ba683406.jpg" width="640" height="480">
```

---
## \#15 Posted by: cody00 Posted at: 2017-09-29T17:19:49.826Z Reads: 92

```
sorry for my ignorance - Here is an unwrapped Cell.  Is the suggestion that I'm touching these two points?  
<img src="/uploads/db1493/original/3X/5/7/57a147e865411d4f84e43728e9e86e69f15485b7.jpg" width="673" height="500">
```

---
## \#16 Posted by: scepterr Posted at: 2017-09-29T17:22:40.926Z Reads: 92

```
Yes and if there are loose solder balls they can be randomly shorting and sparking, eating away at your connections.
```

---
## \#17 Posted by: cody00 Posted at: 2017-09-29T17:31:51.311Z Reads: 91

```
Time to take the battery apart i suppose - already talking with chiboards about getting a battery -  first time board building money suck
```

---
## \#18 Posted by: cody00 Posted at: 2017-09-29T18:01:17.448Z Reads: 90

```
Lets just say in theory - if it was one loose ball - That 3 battery section becomes the weak link and then becomes 10s2...  Bringing it down to 40A discharge .   40A/2 VESC would be about 20A which is about what I was getting in the graphs.  

Not sure if any of this is logical or im just rambling.
```

---
## \#19 Posted by: PXSS Posted at: 2017-09-29T22:58:09.523Z Reads: 86

```
You have a bad weld or solder joint somewhere in your battery. 
Do you own a multimeter?

You need to check the voltages across each group of parallel cells. If there is a group or groups out of balance then that would be where I wiuld start. 

If all is good on the initial test, charge your battery and measure all voltages again. If all is good, go for a ride, and measure your voltages after. If you have a bad solder joint then one or several of the groups will be at a different voltage than the rest. 

Another possibility but noy as likely, is a bad BMS if you have one. It could be turning off if it sees any of the limits being hit. 

My bet would be on a bad battery
```

---
## \#20 Posted by: pat.speed Posted at: 2017-09-29T23:24:42.437Z Reads: 79

```
Could you have damaged the cells when soldering then by leaving the iron on them for too longboard
```

---
## \#21 Posted by: scepterr Posted at: 2017-09-29T23:32:09.458Z Reads: 75

```
Yes-ish it's more about losing the voltage out of that series connection, drop from 10s to 9s and that also causes current spike so it all goes nuts
You could have 1 series pack bottoming out in voltage and the others spiking in voltage, total voltage will look reasonable, but each series could be way apart
```

---
## \#22 Posted by: Aeroquiv Posted at: 2017-09-30T01:15:15.808Z Reads: 72

```
Are you certain that your batteries are genuine HG2's? Those cells were extremely popular back in 2016 when LG couldn't keep up with demand. As an obvious result, China started producing a lot of knock-offs that looked convincingly genuine and was sold to 3rd party wholesalers for a tidy profit. Have you tested them prior to your build? I would do that just as a safety counter-measure for every purchase, because even if you trust your source, they're not perfect.

Oh, if you haven't seen it, here's a [blog](https://batterybro.com/blogs/18650-wholesale-battery-reviews/104619270-can-you-identify-the-fake-lg-hg2-18650-battery) testing a batch to identify fakes.
```

---
## \#23 Posted by: jmasta Posted at: 2017-09-30T01:35:59.595Z Reads: 64

```
Wow those are very elaborate fakes
```

---
## \#24 Posted by: cody00 Posted at: 2017-09-30T01:38:54.739Z Reads: 65

```
Voltage across all series is identical @ 40.32 V (I had went down the road and back since last charge).  Even when I'm on the board, if I'm not drawing current then it is expected charge.  

To me, this would lean more to possible a bad connection for 1 of 3 batteries in a series set.  In this case it would still read 40.32V but could get massive SAG like I'm seeing..  How I would test for this, I'm not sure...

Thanks for the site @Aeroquiv - It crossed my mind but i took the leap.  Everything I can tell from the te site you sent me shy of doing discharge test is showing that they are legit.  

----
```

---
## \#25 Posted by: scepterr Posted at: 2017-09-30T01:46:40.562Z Reads: 63

```
Yes total voltage could look normal, measure each series connection please.
```

---
## \#26 Posted by: cody00 Posted at: 2017-09-30T01:48:36.056Z Reads: 60

```
Sorry - I didn't type that right.. I measured each series separately and it was 4.03V across all
```

---
## \#27 Posted by: scepterr Posted at: 2017-09-30T01:55:39.530Z Reads: 59

```
All the series connections look good too?
```

---
## \#28 Posted by: cody00 Posted at: 2017-09-30T01:56:52.460Z Reads: 55

```
Yea, I've disassembled and inspected.  None loose.. no burns.  My last ditch effort might be to fire up the iron and just zap each one very quickly
```

---
## \#29 Posted by: Okami Posted at: 2017-09-30T01:59:35.643Z Reads: 58

```
If i were.u i would still check internal resistance. I think that should be good way to see where the cells stand.. maybe some of them is messed up? What happens on cell level at end of discharge? Are all cell groups at same level or is it like lipo with different levels of state of charge?
```

---
## \#30 Posted by: scepterr Posted at: 2017-09-30T02:05:30.388Z Reads: 56

```
Was that 4.03 after full charge?
@okami with 18650 they should be within like 0.005 after full if they are same cells, same resistance
```

---
## \#31 Posted by: cody00 Posted at: 2017-09-30T02:10:09.690Z Reads: 58

```
no there is about a mile on this charge.  They get a good full charge and I use a BMS for charging. 

@Okami : I suppose I could hook it up and discharge it down to see.  Maybe it would show a problem child.   I think I will try the internal resistance test as well.  Maybe I can do that test on each series so I dont have to completely disassemble
```

---
## \#32 Posted by: scepterr Posted at: 2017-09-30T02:11:36.478Z Reads: 57

```
Any chance you have a Foxnovo 4s or opus bt-c3100 charger? I would run charge/discharge cycle see if any heat up like crazy. 
I do think at this point it's worth tearing it down, testing cells individually and rebuilding
```

---
## \#33 Posted by: cody00 Posted at: 2017-09-30T02:16:27.465Z Reads: 59

```
I dont. I wish I had something to do this discharge cycle.  Ill play around and see what I can come up with
```

---
## \#34 Posted by: scepterr Posted at: 2017-09-30T02:18:31.483Z Reads: 57

```
You can grab one on Amazon, I swear by the Foxnovo 4S
<img src="/uploads/db1493/original/3X/0/e/0e7446d4ff9bf7cd671ea8e8a028eb1a286e3128.jpg" width="690" height="256">
```

---
## \#35 Posted by: cody00 Posted at: 2017-09-30T02:24:50.454Z Reads: 54

```
Thanks for the tip - looks like something good to have on hand - I really appreciate you guys trying to help figure out my issues.
```

---
## \#36 Posted by: scepterr Posted at: 2017-09-30T02:25:47.028Z Reads: 55

```
Every problem solved for 1 person, solves it for 100 more 😉
This is a unique one I would like to see solved
```

---
## \#37 Posted by: cody00 Posted at: 2017-09-30T14:32:01.714Z Reads: 56

```
I retouched every point on the battery with the solder gun in hopes it was something not visible.  Similar results riding a few hundred yards.<img src="/uploads/db1493/original/3X/5/d/5dddd785224b61ab8dee336928d3da48b47d5d76.png" width="690" height="176">


I just ordered some of these so I can do some test to batteries other than voltage.  I figure I only have to remove the outer connections of the pack vs completely taking it apart to isolate one cell.  
https://www.amazon.com/gp/product/B0087ZDH7I/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1
```

---
## \#38 Posted by: cody00 Posted at: 2017-10-03T02:11:55.680Z Reads: 51

```
I ended up getting this cheap battery tester which can also do internal resistance check.  
https://www.amazon.com/gp/product/B0178P8H9U/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1


After measuring the internal resistance for each cell.. nothing looks too off.. so i think...
<img src="/uploads/db1493/original/3X/e/9/e948f59391a0e423676af40578eb1e0f619354ba.png" width="690" height="329">


I'm very close to buying a new battery from @barajabali but I will kick my ass up and down the street if I buy it and it still does crazy voltage drops (meaning that it was something else like VESC acting funny). 

Anyone have any other ideas? - 

On my agenda as of now.. put the outter rim of the battery back on.  Hook back up to wiring harness.  Leave off the BMS since full charged... Test... Remove 100A fuse.. Test.. Switch BT HM10 to other VESC B.. Test to see if readings are consistent with VESC A.
```

---
## \#39 Posted by: cody00 Posted at: 2017-10-03T04:40:56.516Z Reads: 49

```
Battery put back together - Same extreme sag.
Fuse Removed - No Changes...
Battery Meter Removed - No Changes.
Motor B & Vesc B - By Itself  (Was the Slave) - No Changes... 

Are there any other options?
```

---
## \#40 Posted by: cody00 Posted at: 2017-10-03T15:43:25.907Z Reads: 46

```
Just ordered a battery from @barajabali (Chi Boards) - If this battery comes in and solves the problem then we know there is some type of issue with the battery pack that Voltage and Internal Resistance checks couldn't bring to light.  

Mimicking a 30A-60A load @ 40V and checking the voltage might have brought some clarity to this.  
Ive done some research on how to do this without going out and buying some expensive load tester.  
..."Get a 1500 watt space heater".. which should give a decent comparison.. 
If this is a bad idea - Stop me :slight_smile:
```

---
## \#41 Posted by: scepterr Posted at: 2017-10-03T16:18:32.397Z Reads: 44

```
I don't think a space heater would work, it's AC, unless you have an inverter. 
Are there any other esk8ers with a board near you, you could try the battery on ?
```

---
## \#42 Posted by: cody00 Posted at: 2017-10-03T16:40:03.019Z Reads: 42

```
Good call - I have a car inverter that might work - Thanks
```

---
## \#43 Posted by: scepterr Posted at: 2017-10-03T17:34:45.044Z Reads: 40

```
That likely only runs off 12V
```

---
## \#44 Posted by: cody00 Posted at: 2017-10-03T17:43:08.340Z Reads: 36

```
You're just raining on my testing parade @scepterr - There are no electric skaters here besides maybe a couple of boosted boards..
```

---
## \#45 Posted by: scepterr Posted at: 2017-10-03T17:44:06.012Z Reads: 33

```
I'm just trying to prevent fires ,😋
```

---
## \#46 Posted by: cody00 Posted at: 2017-10-03T17:49:18.481Z Reads: 33

```
At this point.. im secretly wishing this battery pack goes up in flames assuming that it doesn't catch anything else on fire.
```

---
## \#47 Posted by: scepterr Posted at: 2017-10-03T17:50:21.120Z Reads: 33

```
Any chance you're in or around NYC?
```

---
## \#48 Posted by: Okami Posted at: 2017-10-03T18:22:58.093Z Reads: 33

```
What would be interesting to see would be how hot do they really get.. though might be a bit hard unless u have someone with cat phone (infrared camera).. as im not sure how reliable would be to fit just a temp sensor in the battery compartment..

.. on a side note, it somewhat looks like it could really be counterfeit cells.. but im not sure is this the case, as it looks like they can offer decent punch but then during longer use get really terrible ?

Not saying your cells are not genuine.. but it sure looks like tough nut to crack lol.. 

I suppose yeh, if you got infrared camera it might reveal some spots which are problematic.. then it should be possible to see whenever the cells get hot or is it something else in the chain that drags the voltage down (gives huge resistance)
```

---
## \#49 Posted by: cody00 Posted at: 2017-10-03T18:50:07.122Z Reads: 35

```
[quote="Okami, post:48, topic:34231"]
might reveal some spots which are problematic.. then it should be possible to see whenever the cells get hot or is it something els
[/quote]

Yea might be worth looking at.  I could ride the hell out of it and punish it, remove the cover as fast as possible then use my temp gun to see if i find any hot spots.  

As far as counterfeit, they very well could be.  I tried to find a reputable seller that had "good" reviews but that was one of the shaky areas of my build.
```

---
## \#50 Posted by: Okami Posted at: 2017-10-03T18:56:28.112Z Reads: 33

```
So where did you order your cells?

Well.. u might try to do it with a temp gun but im not sure will you be able to compare the temperature in a decent way.. 

Though if you do find massive difference in temp between cells, then yeh, maybe you could find which cells heat up more (if there are such cells compared to the rest of the pack, though you said all of them measured just fine and none was out of place or so)

--

As about riding conditions - as i understood from your first post - the cutouts/massive sag also happens on flats right? u mentioned something like every 15mins.. or after 15mins during the ride..

Would be interesting to see whenever the gear change would improve the situation a lot, when do you think u will get the 40T gears for the wheels?
```

---
## \#51 Posted by: cody00 Posted at: 2017-10-03T19:57:23.108Z Reads: 35

```
I ordered them from ebay - based my decision upon reviews - but still an iffy situation.

The massive sag happens all the time (now that I can see the live stats on the phone).  After about 15min of riding, it will sag enough or I'll usually hit a hill to take it into the 30v range to cause a shutoff (which is what seems to be happening) - In the screenshot above, where it goes into sub 30v is when i lost all acceleration.   After searching the forums, I have found a decent amount of people with the same issue but never really found a solution (Search VESC cuts out on acceleration).  

I have the 40T and waiting on some longer belts which are on the way but after going through all of this analysis, I'm not sure that is the issue at heart.  I know that will give higher torque and will use less power starting out....But... Looking at the watts to amps to volts.. the dropout shouldn't be happening like it is.
```

---
## \#52 Posted by: Okami Posted at: 2017-10-03T20:39:22.862Z Reads: 30

```
yeh, ebay might not be the best place to order cells.. thats for sure :smiley:

I havent really looked into cutouts but i think most could happen due to limit being reached and this should happen more for bms.. not for vesc I think

Have u tried to really limit the current output.. like 2x lower as it is now?
```

---
## \#53 Posted by: jmasta Posted at: 2017-10-03T21:05:12.094Z Reads: 28

```
It sounds to me like you unfortunately bought counterfeit cells, especially considering the article posted earlier about all the fake HG2s
```

---
## \#54 Posted by: cody00 Posted at: 2017-10-03T21:16:54.303Z Reads: 28

```
I actually have stopped discharging through the BMS and then added 100A 58V fuse.. Then last night I removed the fuse to make sure there wasn't anything going on there.  That's a good idea. I'll set VESC at 5A each just to see what happens.....but im not hopeful.  

@jmasta  : i wont argue with that statement as it is possible.. however, I figured that some testing might be able to bring the issues to light.. They hold charge.. Low internal resistance etc.
```

---
## \#55 Posted by: Okami Posted at: 2017-10-03T21:23:07.582Z Reads: 28

```
5A might be too low. If cells are any decent 10A x 3 should be good. So 30A total, 15A per vesc or so. Cant see your original settings but i think.it was 60amp total, what is in theory max of what cells should output

Otherwise set at least 10A per vesc, 5A will be really lowish i think.. u still want to ride it after all
```

---
## \#56 Posted by: cody00 Posted at: 2017-10-03T21:25:59.687Z Reads: 31

```
yea original was 30Ax2 ..  At some point in this thread i cut it down to 25Ax2.  I'll chop it down to 10A for experimenting but ultimately will hope the Chi Boards battery is the end game.
```

---
## \#57 Posted by: cody00 Posted at: 2017-10-11T21:45:28.085Z Reads: 31

```
Just a quick update - Got 40/16 up and going now.  Although the system is a little snappier, it still does extreme voltage drops when accelerating.  

ChiBoards just sent out a new 10s3p - Will report back once I receive and get it installed.
```

---
## \#58 Posted by: cody00 Posted at: 2017-10-14T02:14:26.645Z Reads: 25

```
Received the new 10s3p battery from @barajabali ([Chi Boards](http://www.chiboards.com/)) today.  This happened to the fix to all my problems.  Even after extensive acceleration test, I could only get it to drop to 35.5v from 41v.

So that leaves me with the reasoning being faulty/counterfeit batteries or I damaged them somehow.  Even after voltage and internal resitance test, they still checked out okay.  

Thanks for the help and input everyone.
```

---
## \#59 Posted by: scepterr Posted at: 2017-10-14T03:33:57.324Z Reads: 24

```
Convert the "LG" cells into USB power banks, they'll be good enough for that, get some use out of them
You can get a housing with module that you can just pop 18650s into, they're no more than $10.
```

---
