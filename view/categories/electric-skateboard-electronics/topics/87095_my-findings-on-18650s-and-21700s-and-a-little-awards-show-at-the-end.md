# My findings on 18650&rsquo;s and 21700&rsquo;s and a little &ldquo;awards&rdquo; show at the end

### Replies: 31 Views: 1249

## \#1 Posted by: TowerCrisis Posted at: 2019-03-13T23:18:07.203Z Reads: 305

```
![Battery%20Data|690x313](upload://6k8TA8AYAtNZ8655LBQbKov5XuE.png) 

Here's a spreadsheet I've come up with

**All data below comes straight from the battery datasheets, via manufacturer:**

* Capacity (stdrd)
* Capacity (stdrd)
* Current (max cont)
* Current (rec)
* Cycles @ Max
* Cycles @ rec
* Voltage Range

**All data below comes from my calculations:**
* Wh/cm^3 (max current)
* Wh/cm^3 (rec current)
* A/Wh/cm^3 max
* A/Wh/cm^3 rec

I'll explain a few things that the data may not fully explain.

**Capacity:**

First of all, the "Capacity (stdrd)" spec is not really useful for us when we are exceeding this on our packs. What you should instead use to calculate capacity is the "Capacity @max" rating, as this is the true capacity of the cell when you are pulling the maximum amount of amps.

In this case, the 30Q is really only a 2.975 Ah cell when pulling 15A from it. This is actually quite good, indicating low internal resistance.

Cells like the 48G cell are poor performers when it comes to high current draw, since they drop from the 4.8Ah spec down to 3.84 Ah under a 9.6A load. However, this cell would shine when used in a high P count pack where current isn't the bottleneck.

The 30T, 40T, 50E, 30Q, 25R, VTC4, VTC5, and VTC6 all have a good capability to deliver amps without significant capacity drop relative to their starting capacity spec.

**Current:**

This is the manufacturers current specification. Here you can see some real differentiation between what is meant to be a high power cell and what is not. The 25R was never meant to be high power, it simply managed to function as one with reduced performance and without damaging the cell beyond repair. This is likely why the 30Q is heavily used instead of the 25R nowadays.

**Wh/cm^3:**

This is the watt hour density of the cell when used to its current maximum limit.

You can clearly see that there is not much overlap between the high current and recommended current cells. Ones that perform well in one category don't in the other.

So from this data you can conclude that the 50E, 30Q, and 25R are good cells to use when you expect to reach their maximum current capability. You can also conclude that the 48G, 50E, M50, HG2, MU1, and 35E cells would all be very good performers when in a high P count pack. They simply will add much more capacity relative to their competitors.

**A/Wh/cm^3:**

This is an interesting spec. I decided to add this as a way to differentiate which cells are good performers in the current category relative to their power density. This spec is also a good indication of the heat dissipation ability of the cell. Cells that perform well at the high current spec are able to output significant amounts of amps while running at similar temperatures as their competitors.

As you can see, the 30T, 40T, VTC4, and VTC5 are all good cells to use in low P count packs where you may be pulling excessive current from each cell.

These cells also perform well when in higher P count packs, along with the 30Q and the HG2.

**Lifetime**

This spec on'y really matters to those who want their pack to last as long as possible. The 50E, VTC4, and MU1 will all last a long time when using them at high current.

At lower current, the 48G, M50, and VTC4 will all last a long time.

Unfortunate, the 30T and 40T under perform at high current. However I expect them to last a long time at low current. If someone has this spec, please let me know!

**Here's my final input, all of which is my OPINION:**

**The long range commuter goes to the MJ1.** This cell simply can't be beat when it comes to power density and lower speeds. It has a lower current output, meaning you can't accelerate fast or climb steep hills, but it will take you FAR when in a high cell count pack.

**The lightweight pack goes to the 30Q.** It simply has a great power density at low and high current draw.

**The speed demon goes to the 30T.** This cell can output serious amps and will almost never be the bottleneck for most boards. 

**The pack to last goes to the VTC4.** This cell, simply put, has a great lifetime. Stay within its recommended limit of 10A and it will easily last you 1000 discharges till you hit 80% capacity.

**Special nomination goes to the 50E.** This cell just has such a good capacity for a cell that can deliver 10A. I was more surprised to see it have a cycle life of 500 to 80% for a 5A discharge. This cell is on par with the MJ1 in regards to the "long range commuter" choice.

**In conclusion:**

I don't think the 30Q is the end all, beat all, cell. It certainly has some very good specs, however I see many other cells outshining it in certain specific applications. Similarly, the 40T isn't a "larger, better" 30Q. It has some very different characteristics and downfalls that really differentiate them. Choose your cell wisely and you can get a pack that's truly tailored to your own needs.
```

---
## \#2 Posted by: moon Posted at: 2019-03-13T23:32:04.883Z Reads: 265

```
Have you taken a look at:

https://www.fogstar-wholesale.co.uk/product/sanyo-20700b/


https://www.fogstar-wholesale.co.uk/product/sanyo-2070c/
```

---
## \#3 Posted by: TowerCrisis Posted at: 2019-03-13T23:48:05.787Z Reads: 247

```
I can't find a datasheet on the 2070c

However the 20700B has a cycle lifetime of 500 to 35% capacity at a 12A discharge. A more reasonable spec is 200 to 71% (which it is capable of) However that is also at 12A.

I think it's downright deceitful to say that it is capable of 16A continuous. It's can last 300 cycles till it reaches 77% capacity, however that is ONLY at 8A.

Related to this: It will sag from 4.2V down to 3.7 under a 15A load.

Also for anyone confused, that website says that it is both an 18650 and a 20700 cell. It is indeed a 20700 cell.
```

---
## \#4 Posted by: Eboosted Posted at: 2019-03-13T23:53:49.109Z Reads: 226

```
[quote="TowerCrisis, post:1, topic:87095"]
Similarly, the 30T isn’t a “larger, better” 30Q. It has some very different characteristics and downfalls
[/quote]

I wonder why you say this? For me the 30T IS a much more efficient 30Q, same capacity but has more than double discharge capacity, it's just a tad fatter and 5mm longer, a 12s4p made of 30T is my dream come true, 50A for each 6380 rings the sweet spot for orgasmic torque
```

---
## \#5 Posted by: TowerCrisis Posted at: 2019-03-13T23:58:02.183Z Reads: 212

```
My bad, I meant to say 40T!

Main reasoning being that the 30Q has a better cycle lifetime and better energy density. However the additional current can't be beat when that's what you're after, hence why I nominated the 30T as the "speed demon" (with the 40T in a close second).

Edited my initial post to reflect this.
```

---
## \#6 Posted by: deucesdown Posted at: 2019-03-14T01:40:55.842Z Reads: 187

```
Thanks for putting this together. Can you add VTC5A? This is an important cell.
```

---
## \#7 Posted by: TowerCrisis Posted at: 2019-03-14T01:43:10.511Z Reads: 183

```
I took a look around for the datasheet but found limited information, so I skipped it. I'll dig deeper and try and add it in soon.
```

---
## \#8 Posted by: lrdesigns Posted at: 2019-03-14T02:14:30.487Z Reads: 183

```
[quote="TowerCrisis, post:1, topic:87095"]
The long range commuter goes to the MJ1.
[/quote]

Thanks for this suggestion, also longer cycle life then 30Q :+1:

Wish we had capacity @ max for it though.
```

---
## \#9 Posted by: TowerCrisis Posted at: 2019-03-14T02:28:00.875Z Reads: 181

```
Agreed.

If capacity at higher draw is abysmal then the 50E or M50 would be a good substitute.
```

---
## \#10 Posted by: thisguyhere Posted at: 2019-03-14T02:32:56.364Z Reads: 180

```
Great analysis. 

I think cost would be a good and valid metric to include, to see where energy density by cost breaks down to each cell type.
```

---
## \#11 Posted by: goldrabe Posted at: 2019-03-14T03:30:55.340Z Reads: 172

```
:arrow_up_small:

This! 

In Moochs testing the 35E was only capable of 8A reaching it's full capacity and under a 10A load the capacity advantage to the 30Q was negligible. So even in a 8P count the 30Q is the better all-rounder. The 50E looks damn good and has quite a good value too. On endless sphere they were mentioning that the 35E looses capacity more gradually when reaching the 500 cycles mark whereas the 30Q losses are more significant. 
Interesting read and thanks for collecting all the data.
```

---
## \#12 Posted by: Eboosted Posted at: 2019-03-14T04:44:37.599Z Reads: 175

```
A 12s8p made of mj1 would be great for a Trampa urban board 50A for each motor and a huge range
```

---
## \#13 Posted by: PXSS Posted at: 2019-03-14T05:42:49.728Z Reads: 167

```
I applaud your efforts but you're quite mistaken in a lot of points.

We do not draw upwards of 10+A per cell ***on average***. Yes we do hit those currents for maybe 30s to a minute at a time but you have to realize that the spec sheet is usually stating maximum current continuously. What this means is if that current was drawn for the entire discharge cycle, the cell would not die.

To prove my point, to discharge a 30Q at 10A continuous, you would drain the battery in a total of 18 minutes. When was the last time you drained your battery in 18 minutes or less? If you have never done this, then you've never run your battery at an average of 10A therefore using a curve meant to give insight into the discharge capacity of a cell at 10A continuously is flawed.
 
I have run 30Q batteries at 20+A continuously. That means discharging the battery in a grand total of 9 or less minutes. I have also burst them to 40+A for maybe 30ish seconds? Yes, this is possible, but active cooling and proper heat sinking is a must. 

Reading spec sheets is fine and kudos to you for spending the time reading them instead of just quoting numbers without trying to understand but it does not replace experience. If you really want to gain knowledge into how hard these things can run then start experimenting and recording all the data you can. Then go through that and try to understand what the numbers are telling you. Understand the application and how the data you are collecting applies to your intended purpose.

---

Also cycle lifetime quoted in spec sheets do not compare one to one ever. It needs to be taken in with context.

For example, 40T vs 30Q:
40T is rated to 250 cycles at these conditions:
charging at 6A per cell up to 4.2v
discharging at 35A per cell down to 2.5v
capacity after 250 cycles: 2400mAh

30Q is rated to 250 cycles at these conditions:
charging at 1.5A per cell up to 4.2v
discharging at 15A per cell down to 2.5v
capacity after 250 cycles: 1800mAh

Why are you comparing these two when one condition is 4 times as aggressive in charge and 2 times as aggressive in discharge. If you are going to compare these two you have to normalize the data somehow, whether you decided to take the cycle life at a specific charge and discharge current for both cells or whether you want to normalize by cell size, so if 40T is 43% larger in volume then the charge and discharge current ought to be 43% higher than the equivalent 30Q.

Not only this, but in your excel sheet for 30Q you are gathering your data from a pre-release presentation dated August of 2014 from Nkon if I had to guess. The actual spec sheet was released February 2015 and the numbers on there align with what I wrote above and not with what you have in your sheet. 

---

I could poke holes into your methodology all day long but I honestly do not have the time. The best thing you can do is actually test things out and compile a database where you can account for a multitude of variables and sort and filter data based on your particular needs.

This is a good start, but you have a very long way to go before you have something good. Learning to identify the issues with your method and assumptions will lead to a much better model. If you start poking holes at your own data then you'll improve much faster.

Good Luck
```

---
## \#14 Posted by: FranciscoV Posted at: 2019-03-14T06:37:39.606Z Reads: 148

```
![image|320x220](upload://qLh1wjapTNN5pTDieiTXokV0ipz.gif)
```

---
## \#15 Posted by: TowerCrisis Posted at: 2019-03-14T07:45:44.597Z Reads: 143

```
[quote="PXSS, post:13, topic:87095"]
We do not draw upwards of 10+A per cell ***on average*** .
[/quote]
I never said we do, so the rest of what you said in regards to this 10A thing is irrelevant. I fully understand how discharge ratings work. Nowhere did I claim we will be pulling 35A continuous from a 30T or 15A from a 30Q. I'm simply listing what the datasheets say.

Just because you don't actually pull that much current doesn't mean that it doesn't matter. It's still a valid comparison because it's an indication of which cell is more suited for high current draw, whether it be continuous or instantaneous.

[quote="PXSS, post:13, topic:87095"]
I have also burst them to 40+A for maybe 30ish seconds? Yes, this is possible, but active cooling and proper heat sinking is a must.
[/quote]

That's just foolish, IMO. You should never exceed their spec this much if you want a reasonable cycle life. You can heatsink the outside, but you can't heatsink the inner electrodes (which you have no way of measuring the temperature of, btw).

[quote="PXSS, post:13, topic:87095"]
Reading spec sheets is fine and kudos to you for spending the time reading them instead of just quoting numbers without trying to understand but it does not replace experience.
[/quote]
I'm not sure what you're saying here.

The datasheet IS the experience. You can sure bet that they've done empirical testing on these cells. That's where these numbers come from.

All throughout my data I **specifically** laid out the test parameters of each value.

[quote="PXSS, post:13, topic:87095"]
For example, 40T vs 30Q: 40T is rated to 250 cycles at these conditions: charging at 6A per cell up to 4.2v discharging at 35A per cell down to 2.5v capacity after 250 cycles: 2400mAh

30Q is rated to 250 cycles at these conditions: charging at 1.5A per cell up to 4.2v discharging at 15A per cell down to 2.5v capacity after 250 cycles: 1800mAh
[/quote]

Yes. That is true. My data for the 30Q cycle count was outdated, their current production matches that of the 30T.

I specifically said that these values are at the **maximum** continuous current. So anyone who actually reads the data can look over a few columns and see "oh, the 30T is rated to over twice the current. That must mean that it will have a significantly longer lifetime given the same current application."

That's the entire point.

[quote="PXSS, post:13, topic:87095"]
If you are going to compare these two you have to normalize the data somehow, whether you decided to take the cycle life at a specific charge and discharge current for both cells or whether you want to normalize by cell size, so if 40T is 43% larger in volume then the charge and discharge current ought to be 43% higher than the equivalent 30Q.
[/quote]
It is "normalized" in the sense that you use common sense and read the data that effects these values. You can't just look at one set of values and conclude one cell is better than another, ESPECIALLY when that value is heavily affected by another.

[quote="PXSS, post:13, topic:87095"]
if 40T is 43% larger in volume then the charge and discharge current ought to be 43% higher than the equivalent 30Q.
[/quote]
Yep, which is why I included the **last four columns of data** which compares the energy density AND current capability relative to energy density (which is a VERY useful metric.)

[quote="PXSS, post:13, topic:87095"]
Not only this, but in your excel sheet for 30Q you are gathering your data from a pre-release presentation dated August of 2014 from Nkon if I had to guess. The actual spec sheet was released February 2015 and the numbers on there align with what I wrote above and not with what you have in your sheet.
[/quote]
That's a little misleading. The ONLY value that's different between the 2014 and current 30Q is the lifecycle (250 to 60% vs 300 to 73%). The rest of the values are unchanged, which affects no other data. You're writing this like it completely negates the rest of the data.

[quote="PXSS, post:13, topic:87095"]
I could poke holes into your methodology all day long but I honestly do not have the time.
[/quote]
Similarly to how you clearly didn't have time to thoroughly look through the data, I don't have the time to compile a complete database of every possible value equalized for different variables.

[quote="PXSS, post:13, topic:87095"]
Learning to identify the issues with your method and assumptions will lead to a much better model.
[/quote]
This isn't a model. And I have made no assumptions, the assumptions are left to the *reader* to make based on the data I've laid out.

Maybe you've mistaken my "assumption" and "model" for the second half of my post, which I **clearly** labeled as such:

[quote="TowerCrisis, post:1, topic:87095"]
Here’s my final input, all of which is my OPINION:
[/quote]
```

---
## \#16 Posted by: Vanarian Posted at: 2019-03-14T07:57:43.175Z Reads: 119

```
https://giphy.com/gifs/korea-north-headlines-j9djzcMmzg8ow

Well mixing both of @PXSS and your data was refreshing anyway! Thanks respectively for your work and your input guys :beers:
```

---
## \#17 Posted by: PXSS Posted at: 2019-03-14T12:06:12.254Z Reads: 114

```
Lol yup.
10c
```

---
## \#18 Posted by: Darkie02 Posted at: 2019-03-14T12:14:33.294Z Reads: 128

```
Still trying to work out what cells to use in my next build. So this is helpful but capacity arguments are irelivent to me and this is over talked about to death all the time.

Running a dule 6355 what I think is normal for most diy builds (sorry single drives you have the powers to go fast and up hills and aceliration on you 6370 motors but the brakes are all ways a concern if its not the motor -A it’s the grip of urathane skidding on the road that’s what I found from experience. I just don’t trust it’s there and when it skids if I brake hard and I’m trying to be my own abs system it works but just IN MY OPINION. I feel as tho I just want more stoping power when some one steps out on you and I feel the only real argument for it is cost its a big saving on a build.)
 
Running 2 motors with its motor max at +35A -30to40A seems to be were I’m happy on my 10s

My vesc says it’s pulling up to +15A avrage burst of the battry so by the time I double for the second vesc and add a safety factor on then I’m pushing 2p safer to go 3p depending on the battry 

I’ve not really ruled out any of the battery’s above parity much all of them would work until you look at regen
T40 and VTC5a is rated to max 6A charge so a 3p would be 18A that’s 9A to each motor.
T30 Q30 CTV4 is rated to max 4A charge so a 3p would be 12A that’s 6A to each motor I’m thinking is just not enough. Yes these are continues charging not burst but there is just no data on burst the best I can fined is mooch results
 ![|653x737](https://www.e-cigarette-forum.com/attachments/7306814d-0192-4d39-bf71-4d6fc4674cd5-jpeg.782887/) 


https://www.e-cigarette-forum.com/attachments/7306814d-0192-4d39-bf71-4d6fc4674cd5-jpeg.782887/

witch then throw another spanner in the works of his max life charge rating saying you can charge the CVT 5/5a/6 happy take 2 times the change rating of a Q30 before it reduces life span the battery and the 30T/40T are only 1/3 better than a Q30 baring in mined there also that much bigger 5mm longer adds nothing as that's with to most builds 3mm deeper again adds nothing to most builds a 10s 4p pack (standers) will add 60mm in pack length so comparing a 420mm pack to a 360mm pack is about 1/8. not the 1/2 as much room again every one keep saying in lost Realestate to ES8 in my opinion.

I think im after a high regen cell as I fined my batt neg regen is the main limiting factor and the fault regularly comes up on the VESC as hitting the limit. I'm leaning towards the VET5a in a 3p 9s con fig but im open to any other suggestions people might have if i'm looking at this from the wrong angle when choosing a battery.
```

---
## \#19 Posted by: Vanarian Posted at: 2019-03-14T12:58:12.269Z Reads: 116

```
Why responding to me tho? 😂

Busy atm I'll take a look at it tonight haha
```

---
## \#20 Posted by: Darkie02 Posted at: 2019-03-14T13:08:58.647Z Reads: 123

```
Because that’s the reply button I was sub  consciously drawn I hit when typing?
```

---
## \#21 Posted by: banjaxxed Posted at: 2019-03-14T13:20:19.693Z Reads: 123

```
Good work. I think it's useful even if real life usage is different constant Vs burst, refering to imperical data and curating the info is extremely  useful for those who face choice


But you need to add this bad MF
https://www.npecell.com/product/molicel21700/

Mooch likes
https://www.e-cigarette-forum.com/threads/bench-test-results-early-samples-molicel-p42a-45a-4000mah-21700-great-30a-battery-beats-40t.884615/

Also the widely available and cheap for specs
#Sanyo NCR20700B
```

---
## \#22 Posted by: Maxid Posted at: 2019-03-14T13:24:51.742Z Reads: 116

```
Last time I checked the 18650 cells for my ebike pack I came away with the impression that there is basically no difference between a 30Q and Sanyo GA or the MJ1 (or any other higher capacity cell) because the benefit of that additional capacity comes only into play at a voltage level that I usually want to start charging the pack again anyway as the voltage starts to drop rapidly.

21700 cells are too expensive for little to no benefit compared to 30Q (You could just stick an additional 30Q in your pack and be probably better of)

But that's just my 2cts!
```

---
## \#23 Posted by: banjaxxed Posted at: 2019-03-14T13:26:03.903Z Reads: 114

```
Depends on the price

![image|627x304](upload://aH9rKuRzZgPmOK3HPJAhf1jLxTg.png) 
![image|661x265](upload://xnYABXyFJzBhSxxTnVhWSSErLW3.png)
```

---
## \#24 Posted by: Maxid Posted at: 2019-03-14T13:29:40.201Z Reads: 110

```
hm? 30Q all the way in your example

A 10S3P Sanyo has 12750mAh and costs 145.5€

A 10S4P 30Q has 12000mAh and costs 141.6€ plus will be the better pack (as I said the added capacity is meaningless because of voltage level plus the 4P will perform better in terms of voltage sag plus will withstand more cycles as you are not pushing the individual cells as hard)

Edit: Funny detail - both packs will have the exact same weight of 1836g according to the data on lygte-info (30x61,2g vs 40x45,9g)
```

---
## \#25 Posted by: Pedrodemio Posted at: 2019-03-14T14:53:52.843Z Reads: 103

```
To be honest if you really want to compare cells for out use case, you would have to run them at the same conditions 

For example, get the data from @bevilacqua , from the acceleration curve derive a current curve and put that in cells of various configuration that are equivalent to what they would experience on a battery pack of different sizes and cells

It’s a big and expensive project, but would certainly produce valuable data

Kudos for who has the money and time to do that

(@PXSS I know you can’t say much, but do you do something similar at work or not so extended like this?)
```

---
## \#26 Posted by: sayekim Posted at: 2019-03-14T15:23:04.132Z Reads: 99

```
[quote="Pedrodemio, post:25, topic:87095"]
run them at the same conditions
[/quote]

Yes exactly. I need to know how all the cells perform going like this. 

https://metr.at/r/JvaJK

![image|375x499](upload://7ViFEenDup1lgaxUg8MouggVZle.jpeg)
```

---
## \#27 Posted by: TowerCrisis Posted at: 2019-03-14T21:42:10.035Z Reads: 93

```
That's understandable, that information would be useful.

The only problem is I collected all this data by hand. If I were to curate it and equalize it for that specific use case, then it would be useless for any other different board.

If you guys want to be able to plug in your board specs and have it spit out battery choices, then it really needs to be organized like a database, with each battery having it's own curves for different uses.

It's just incredibly hard to do without a LOT of data, most of which isn't supplied by the datasheet.

For that kind of information you'd need to turn to data collection IRL to record the entire discharge cycle at various currents. Same goes for cycle lifetime unfortunately.
```

---
## \#28 Posted by: Pedrodemio Posted at: 2019-03-14T23:22:42.087Z Reads: 85

```
Yeah, it's a lot of work

I think the best we can do is look at all the data you compiled and also read the opinion of people that test a lot of batteries
```

---
## \#29 Posted by: lrdesigns Posted at: 2019-03-15T00:55:00.726Z Reads: 84

```
[quote="Darkie02, post:18, topic:87095"]
I think im after a high regen cell as I fined my batt neg regen is the main limiting factor
[/quote]

If you want really high re-gen within given specs I would suggest a high grade lipo. Some are "rated" for 5c or 10c charge! 

But back to lion 18560's, the charge rate is given as a constant rate from empty to full which will never happen in a skateboard. They can take a much higher burst charge. Problem is no one is making data on that use case. So long as the batteries are not getting hot I think you are fine. Also most people will set a higher regen rate (over spec) for safety over reduced cycle life. 

I for sure would rather less cycle life then crashing into a car at high speed cause I didnt have enough brakes.
```

---
## \#30 Posted by: SimosMCmuffin Posted at: 2019-03-15T07:10:02.531Z Reads: 78

```
https://lygte-info.dk/review/batteries2012/Molicel%20INR21700-P42A%204200mAh%20(Gray)%20UK.html

Never heard of Molicel before, but dang that's a pretty beastly cell.
```

---
## \#31 Posted by: Vanarian Posted at: 2019-03-15T07:49:20.258Z Reads: 77

```
There was a guy on E-S using them for years on his e-bike (his company sourced batteries from them), back in the days he was very happy with Molicell 👍🏽

I might still have his messages somewhere... Definitely this new one with 30A discharge & 4000mah is *very* interesting.
```

---
