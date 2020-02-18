# Recommendations for buying 18650s

### Replies: 24 Views: 4269

## \#1 Posted by: Paalmb Posted at: 2018-02-12T16:18:53.153Z Reads: 396

```
Hi there. 
So i am “leaping” into using The 18650 batteries and going to build my own battery-pack. Going for a 10s2P kind of type. 
So many sellers om ebay have different kind of batteries, but i have read that not All is worth spending money on... some are fake, used and not god. 
Any recomendations? Sites? Sellers?
```

---
## \#2 Posted by: rojitor Posted at: 2018-02-12T16:26:10.556Z Reads: 393

```
Where do you live?
```

---
## \#3 Posted by: Paalmb Posted at: 2018-02-12T16:29:12.426Z Reads: 380

```
I live in Denmark
```

---
## \#4 Posted by: moon Posted at: 2018-02-12T16:39:05.851Z Reads: 375

```
[quote="Paalmb, post:3, topic:46191, full:true"]
I live in Denmark
[/quote]

try nkon.nl

Genuine batteries and reputable company
```

---
## \#5 Posted by: Blitz Posted at: 2018-02-12T16:45:38.797Z Reads: 372

```
Samsung q30 cells are the premo stuff there 3000mah 15a but people say they feel like 20a
so 10s2p pack 6000mah 30a But that might be a bit weak on acceleration and Hillclimb 
10s3p would give 45a I reccomend if possible get another 10cells
```

---
## \#6 Posted by: ZackoryCramer Posted at: 2018-02-12T16:45:55.025Z Reads: 363

```
Samsung 30Q 👌🏻
```

---
## \#7 Posted by: Latemate Posted at: 2018-02-12T16:49:20.112Z Reads: 358

```
Where in denmark?
```

---
## \#8 Posted by: darkkevind Posted at: 2018-02-12T16:52:32.859Z Reads: 345

```
Sony VT6 are the best 18650 on the market.

Sanyo 20700B if you have the room and the budget are the way you want to go....
```

---
## \#9 Posted by: Paalmb Posted at: 2018-02-12T16:55:27.946Z Reads: 338

```
I live in esbjerg
```

---
## \#10 Posted by: b264 Posted at: 2018-02-12T17:10:59.079Z Reads: 327

```
How many amps do you want to draw from it?  At 2P your options may be limited but I have no idea how much power you will need.  What will you be running with it?  How many motors?  Which ESC[s]?  How many watts do you want to draw?
```

---
## \#11 Posted by: Paalmb Posted at: 2018-02-12T18:15:14.280Z Reads: 315

```
One belt drive with a Sk3 6374 190 kv. 
Do not know How much amps i have to draw.... 
i am satisfied with my current power-suply with two 6s 5000mah in parallel. 
I have a Vesc.
```

---
## \#12 Posted by: b264 Posted at: 2018-02-12T18:27:42.701Z Reads: 311

```
It's not the capacity, like Ah (ampere*hours) but current, like A (amperes) somtimes expressed as a "C" rating like "20C" which means "20 times the 5000mAh, or 100A"

2P with Samsung 30Q will get you about 30A continuous draw or about 1110 Watts

That's okay for single-wheel drive (not for dual) but you'd need to set your esc up to limit battery current to around those values if your battery is only 2P deep

At 2P deep, the Sony Konion US18650VTC6 cells can deliver 60A but they are 20% more expensive

Also using less than 100% of your rated capacity can help your system run better, with less sag, for a longer lifespan
```

---
## \#13 Posted by: Paalmb Posted at: 2018-02-12T20:01:03.108Z Reads: 291

```
I see! 😄Thank you for sorting that out.👍 it is complicated. 
 I have been Looking at the Samsung INR18650-25R 2500mAh - 20A. 
It is not 3600mAh... but i Think i will manage. I will use it to commute to/back to work. Around 12 km pr day.
```

---
## \#14 Posted by: Bor.inc Posted at: 2018-02-12T21:05:57.307Z Reads: 282

```
I am realy not an expert on Lithium ion cells but I have heard from many that the samsung 30Q cells are prefered because The INR18650-25R do have some voltage sagg.
But maybe an expert can help you better
```

---
## \#15 Posted by: b264 Posted at: 2018-02-12T21:21:47.993Z Reads: 277

```
The experts won't say [much publicly](https://www.electric-skateboard.builders/t/have-a-potential-supplier-of-the-new-samsung-30t-21700-cells/43020/37), so we have to stumble around in the dark.  help @PXSS

You might be better off using 30Q than 25R though because the specs on paper don't tell the entire story.  But since that's what we have, and what specifications are literally made for, then we must use those.

Also all the 18650 prices just recently changed, so everything in that old thread is already mostly obsolete
```

---
## \#16 Posted by: nske Posted at: 2018-02-12T21:35:25.155Z Reads: 277

```
Has anyone build a pack using LG HG2? I'm surprised I haven't seen any reference -I have been using them for Vaping mods and been very happy -they should be at least on par to the S 30Q and can usually be found cheaper.
```

---
## \#17 Posted by: PXSS Posted at: 2018-02-12T22:15:59.952Z Reads: 283

```
What do you want to know?
I have posted plenty about 25Rs vs 30Q. I do not mind linking you to said threads/posts and answering questions. I cannot provide test data for different batteries as much of my stuff on that is work (and government) related...

You can read this thread:
https://www.electric-skateboard.builders/t/what-is-the-downside-of-single-18650-cells-with-high-higher-ah/17296
```

---
## \#18 Posted by: PXSS Posted at: 2018-02-12T22:26:13.967Z Reads: 284

```
Here is an important post from that thread, most of it is lipo vs liioons
[quote="PXSS, post:24, topic:17296"]
For example here is the discharge curve for 25R cells which are the standard vs 30Q cells:

![IMG_1652|690x387](upload://2KPbKzC81LhD3Y5SuEm94aVyHKF.PNG)

Top curve is 0.2A, second is 5A and third is 10A
In a 4P pack, this would correspond to 0.8A (close enough to no load), 20A, and 40A. As you can see, the 30Q cell has less sag at 10A than the 25R does at 5A! In fact, after 50% capacity the 30Q has the same voltage sag at 15A than the 25R at 5A. That means that you see the same voltage sag when pulling 20A on a 10S4P 25R pack than you do pulling 60A on the 30Q pack! That is laughable.
[/quote]

---
Another post where I explain it:
https://www.electric-skateboard.builders/t/battery-charging-question/19277/33

[quote="PXSS, post:33, topic:19277"]
I source 30Qs from Nkon and have them shipped to the US. 
I source GAs from Liionwhesale too. 

Stop looking at just the rating. That's the issue with a lot of people here, you see numbers and take them by heart without understanding the reasoning behind them is. Look up the spec sheets and read them if you have the time. The reason 30Qs are rated to 15A is because if you continuously run them at that current and charge them at 4A, after 300 cycles, you only get 73.8% of rated capacity. That's where Samsung decided to draw the line. In the same spec sheet they show that for 22A continuous and a temp cutoff of 70C and charge at 4A, after 250 cycles, they get 72.4%.

Similar stuff is done by Panasonic. You can run the cell at higher currents CONTINUOUSLY by sacrificing number of cycles you can run them for. Key word there is continuously. We do not do this unless you're climbing an endless 15 degree incline at 20mph. 

Check these graphs out, I've posted them several times:

First is Sanyo GA vs 25Rs:
This is continuous current running through them, the vertical difference between curves is voltage sag at that specific capacity. The red curves are GA and blue is 25R. From top to bottom 0.2A, 5A and then 15A. Henrik's battery holder failed on one of the 15A GA test, that's why it is cut short. The other one he stopped at 75C. 


![IMG_2|690x387](https://www.electric-skateboard.builders/uploads/db1493/original/3X/5/b/5b616802d5299a6dc7a79a8c46504a9b4c7fbe77.PNG)

The takeaway here is that they have less voltage sag than 25Rs, aka they can deliver more power for the same throttle setting at the same discharge level. Also, if you were to throttle to 15A with 25Rs sag down to 3.2V which is most people's soft cutoff after 1.125Ah consumed. With the GAs, you sag down to 3.2V after 1.55Ah consumed. The gap widens if you bring the cutoff lower. 

Next 30Q vs 25R:
Same thing as before, Red is 30Q, blue is 25R. Top to bottom 0.2A, 5A, 15A

![IMG_3|690x387](https://www.electric-skateboard.builders/uploads/db1493/original/3X/5/e/5e561358e769e2c21fc3821c337cbbf380668b2d.PNG)

Here, there is a big difference. The 30Qs drawing 15A sag down as much as the 25Rs drawing only 5A after 1.25Ah consumed (which is 50% capacity of 25Rs). At 15A and 1.25Ah consumed, the 30Q outputs 2070W, the 25Rs on the other hand output 1902W. At 15A, 25Rs sag to 3.2V at 1.125Ah, 30Qs sag to 3.2V at 2.125Ah, that is almost double!

As I said 30Qs are much better at delivering high power than 25Rs. GAs can deliver slightly more power while having 40% more capacity!

I hope this is clear, I've been writing this on and off throughout the day while flight testing lol.

I intentionally left out the 20A case.
Henrik tested the 25Rs a long time ago and he didn't measure temperature back then. We cannot say that the cell did not overheat as he didn't measure this. 
He didn't test GA cells at 20A because he thought they would overheat (and he broke his cell holder), rightly so, but again, we do not run continuously. 
He stopped the 30Q test early at 20A because of heating. He got through 2Ah before he stopped the test because the cells reached 80C. That would be. 6 minutes continuously at 20A per cell. 

It seems that Nkon's prices have gone up since I ordered
[/quote]

---

Read this topic, starting around post 80ish
https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014/85
```

---
## \#19 Posted by: PXSS Posted at: 2018-02-12T22:42:08.325Z Reads: 238

```
I have posted extensively about the subject.
You can look up 30Q vs 25R and look for the posts made by me. It's all from like November 2016-April 2017.

If there is anything specific you want to ask that I may have not covered before, you can ask away. I will respond as long as it doesn't delve into my work.

---
E: More reading material:
https://www.electric-skateboard.builders/t/vesc-voltage-cut-off-values-considering-voltage-sag/15390/11
https://www.electric-skateboard.builders/t/li-ion-18650-battery-comparison/11015/20
https://www.electric-skateboard.builders/t/lifepo4-batteries-in-evolve-gt/15558/66
https://www.electric-skateboard.builders/t/battery-calculator-spreadsheet/16172/15
https://www.electric-skateboard.builders/t/understanding-10s4p-18650-battery-packs/3032/45
https://www.electric-skateboard.builders/t/battery-questions/18712/16
https://www.electric-skateboard.builders/t/voltage-sag-what-is-the-most-suitable-battery-cell/14720/63
```

---
## \#20 Posted by: b264 Posted at: 2018-02-13T00:08:24.486Z Reads: 180

```
Thank you @PXSS this should keep us busy for a long time
```

---
## \#21 Posted by: ZackoryCramer Posted at: 2018-02-13T02:26:00.190Z Reads: 167

```
I am 🙋🏻‍♂️. Although 30q are found for a bit cheaper, hg2 does kick in a few more amps according to the specs sheet. Just got myself a box of 30Q’s for 75 cents off each cell. 😃 The esk8 public generally  stick with 30Q’s so we should stick with them. 🐟🐳
```

---
## \#22 Posted by: Deckoz Posted at: 2018-02-13T03:12:52.290Z Reads: 168

```
Hg2 we're kicking 30q ass in 2015... But every hg2 I've gotten since 2016 has fallen on it's face with far fewer cycles then the 30q and alot higher IR. 

LG changed it's manu process, hg2 aren't what they used to be.

And also @PXSS  great collection of posts 🤘
```

---
## \#23 Posted by: PXSS Posted at: 2018-02-13T03:20:20.251Z Reads: 166

```
HG2 loses out on voltage sag at every current draw. 
They might run 3-5deg celcius cooler than 30Q but you are giving up performance. 

![image|690x387](upload://ud9Lozjnnrudgp8kjMRCen1Fynb.png)
```

---
## \#24 Posted by: Paalmb Posted at: 2018-02-16T12:00:50.003Z Reads: 138

```
Thank you All for your reply’s! I have a  shipment with 20x30q’s coming my Way soon! 
Now The Hunt begins to find a bms and a chargingport for my laptop charger
Have a Nice Day!
Ride safe!
```

---
