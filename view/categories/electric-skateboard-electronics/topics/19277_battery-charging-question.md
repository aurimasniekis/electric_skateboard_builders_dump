# Battery charging question

### Replies: 63 Views: 5124

## \#1 Posted by: Wschles Posted at: 2017-03-19T00:51:49.172Z Reads: 273

```
If 50% charge is the ideal state of battery equilibrium and charging less than 100% allows many more recharge cycles - then wouldn't it be ideal to ride down to 25% and charge up to 75%? Obviously if you have a long ride planned then fully charge and down to the min set by the vesc. But for every day 15-30 min rides would the above regimen be better?
```

---
## \#2 Posted by: Namasaki Posted at: 2017-03-19T01:20:55.517Z Reads: 255

```
According to Leo Leporte " the tech guy"
The life of a lithium battery is determined by a certain number of full charge cycles.
If you do a partial charge, it counts as only a percentage of that full charge cycle.
So if your battery is good for say 500 full charge cycles and you charge it to 75% full and discharge it to 25% or charge it to 100% full and discharge it to 50%.( I believe it is better to use the 100% to 50%)
Then your only using up 1/2 of a charge cycle each time you charge/discharge your battery.
So doing this, you will be able to charge said battery 1000 times before wearing it out.
The problem I find with this practice is that because you are effectively reducing your battery's range, you will have to charge your battery more often. So have you really lengthened the life of your battery? In my opinion, no.
But by charging to 100% and discharging only 50% will keep you safely away from an over discharge situation. 
My experience has been that charging a battery to 100% appears to have no adverse affect on the battery where as discharging the battery too low has immediate adverse effects on the battery.
Granted that there can be other factors which may affect the health and life of a battery like trying to draw more current than the battery can handle and causing it to overheat.
http://techguylabs.com/episodes/1022/how-can-i-make-my-batteries-last-longer
```

---
## \#3 Posted by: Ackmaniac Posted at: 2017-03-19T01:30:54.182Z Reads: 230

```
You are right. That would be better for the cells. 
But you have to realize that 300 full cycles on a 10S4P battery pack would be more than 10000 km. In worst conditions the battery should be good for at least these 300 cycles. But in reality it will be fine with more cycles because when we ride we are not even close to worst conditions. (As long as your settings are in the battery limits). 
And i don't think that there are many out there who did already 10000 km on one longboard battery pack. So you can safe some recharge cycles but i would recommend to not care about and just have fun. In the winter when you don't use it for a couple of weeks or months then you should bring the voltage down to 3.75V a cell. But otherwise it doesn't hurt that much. Just simply only charge the board when you know you ride the board that day or the next day.
```

---
## \#4 Posted by: Namasaki Posted at: 2017-03-19T01:36:39.867Z Reads: 202

```
One thing that I have noticed is that when Lithium cells are tested, they are allowed to rest between charging and discharging and I believe that this is a good practice when possible.
Something like 30 min after discharge and before re-charging.
And 15min after charging and before discharging.
```

---
## \#5 Posted by: Ackmaniac Posted at: 2017-03-19T01:47:47.672Z Reads: 188

```
I think that's only because of the temperature. But we don't use the cells contentiously with the maximum continuous discharge rate. To be honest, with quality high current discharge cells we only raise the temperature a little bit. So this is also something we don't need to worry about. If you want to do your cells something good then charge them with a low current. This takes longer but your cells like it.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-03-19T01:56:36.563Z Reads: 183

```
Good point, slow charging is the best way.
Although I think charging at 1C is safe for the most part.
```

---
## \#7 Posted by: Ackmaniac Posted at: 2017-03-19T02:19:26.176Z Reads: 182

```
1 C is already very high. For a 10S4P pack with 2500 mah cells this would be 10A. Most fast chargers have only 4A (0.4C). 
Best of course is a adjustable charger for current and voltage. 
A really nice 12S charger is the Graupner Ultramat 18. The build in power supply works with 100 watts. But with a external power supply you can use 300 watts. But i always charge my cells slowly so the 100 watts is enough. 
For my 1 kwh battery i need more than 10 hours but i simply leave it on over night. It also interrupts the charging every minute for a couple of seconds which is also good for the battery.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-03-19T02:53:54.831Z Reads: 173

```
I charge my Lipo packs at 1C but it's only 5a and they're rated for 5C. 
I use a lab power supply with adjustable voltage and current up to 60v 5a with CC and CV. IT works great as a charger and won't over charge.
```

---
## \#9 Posted by: PXSS Posted at: 2017-03-20T05:39:43.526Z Reads: 155

```
http://batteryuniversity.com/learn/article/how_to_prolong_lithium_based_batteries

Look at tables 2 and 4. 
That tells the whole story. 
By discharging only to 80% and charging fully, you get a 33% increase in life cycles. 
By charging only to 80% and discharging fully, you get a 200% increase in life cycles. 

Lithium Ion cells don't like being fully charged regardless of what others say. Battery University is a great place to learn and has tons of citations to academic research papers with real good stuff if you're looking to get really informed.
```

---
## \#10 Posted by: Wschles Posted at: 2017-03-20T11:11:03.407Z Reads: 152

```
It also says this initially in that article:
"The smaller the discharge (low DoD), the longer the battery will last. If at all possible, avoid full discharges and charge the battery more often between uses. Partial discharge on Li-ion is fine. There is no memory and the battery does not need periodic full discharge cycle"
Base on this I came up with my recommendation of 75-25 use zone.
```

---
## \#11 Posted by: PXSS Posted at: 2017-03-20T13:06:14.107Z Reads: 147

```
I'd say that it's more beneficial to charge to 65% and discharge to 15% but there is no data to support that. Charging to 75% and discharging to 25% is really good though!

<img src="/uploads/db1493/original/3X/8/a/8adfc7fecece06fda2f290a360e8866e77b2ae49.PNG" width="607" height="500">
```

---
## \#12 Posted by: Wschles Posted at: 2017-03-20T13:24:31.475Z Reads: 139

```
It seems like when I go from 100-50 the battery goes on forever. Yesterday 18 miles. Then from 50-25 only another 3-4 miles. At 25 starts slowing down and acts funky.
```

---
## \#13 Posted by: PXSS Posted at: 2017-03-20T13:27:37.779Z Reads: 132

```
Which battery??
```

---
## \#14 Posted by: Wschles Posted at: 2017-03-20T13:48:33.978Z Reads: 131

```
12s4p lithium ion cells. Kali built it!
```

---
## \#15 Posted by: PXSS Posted at: 2017-03-20T14:17:07.226Z Reads: 131

```
Do you know what cells were used??
@Kaly
```

---
## \#16 Posted by: longhairedboy Posted at: 2017-03-20T14:30:21.690Z Reads: 133

```
@Wschles yeah that doesn't sound good. You should be seeing more of a flat/linear drain between 90% and 20% than that.
```

---
## \#17 Posted by: Kaly Posted at: 2017-03-20T14:37:15.258Z Reads: 130

```
The cell use are Samsung 25R
The pack is a 12S-6P 

On The battery indicator this is an estimate reading since  that pack does not have a coulomb meter installed. 

the LED indicator have 5 leds the last red dot indicates empty. 
And the behavior is the soft cutoff voltage setting from the VESC. 

The setting can be change but I think 18 miles + 3-4 miles  to depletion is pretty good for a eMTB.
```

---
## \#18 Posted by: PXSS Posted at: 2017-03-20T14:47:16.999Z Reads: 133

```
What are the ESC settings right now? I agree with @longhairedboy that it should be more linear than that but it highly depends on how much power he's drawing. 25Rs are not great in delivering high amounts of current as voltage sag takes a toll on them specially past the 50% mark, this combined with high cutoff voltage can be cutting his range significantly but again it's all highly dependent on how much power he draws.

And as @Kaly said, the percentage meter is only an estimate based on voltage. So while the board shows 50% at no load, under load it could dip below 20%. 

<img src="/uploads/db1493/original/3X/1/7/175aa238c29a41af10556c8d75643665ce84030c.PNG" width="690" height="387">
```

---
## \#19 Posted by: Kaly Posted at: 2017-03-20T15:08:44.555Z Reads: 127

```
The issue here may be the LED  indicator. 
The one I use on my packs are the push button type with 5 LEDS that represents a range of voltage, which in turn this voltage represent an estimate of the capacity, one red led is for empty, the remaining  4 leds each represents a 25% range in voltage this is good to estimate on what **range** of the discharge curve you are. But not to properly track a discharge curve.
```

---
## \#20 Posted by: Kaly Posted at: 2017-03-20T15:10:36.388Z Reads: 129

```
@PXSS
A graphic is worth 1000 words ;-)
```

---
## \#21 Posted by: Wschles Posted at: 2017-03-20T16:45:50.102Z Reads: 121

```
This emtb board is INCREDIBLE!  As I've said the battery lasts an extraordinarily long time. If you compare to an Evolve GT all-terrain set up your lucky if you get 7 to 8 miles. I thought I was going to do more Offroad which is fun and enjoyable but I've still been doing more road riding and the overall experience is way better than a regular electric skateboard. The bindings allow you to carve like you are defying gravity.  Most of all Kaly is an incredible board builder. He is an engineer with fantastic knowledge of the intricacies of this wonderful hobby. I cannot recommend him any higher than I already do. You can certainly  do it yourself but I would recommend using an experienced builder like himself because he understands a lot of the complications and intricacies avoiding many of the trial by error that do it yourself builder will  experience.
```

---
## \#22 Posted by: Wschles Posted at: 2017-03-20T18:52:15.844Z Reads: 115

```
What do you think kaly about one of these?<img src="/uploads/db1493/original/3X/d/5/d5fbaf4a1b453f11d8e9503f9c4d40161c3d9480.PNG" width="281" height="499">
```

---
## \#23 Posted by: Ackmaniac Posted at: 2017-03-20T19:05:56.910Z Reads: 111

```
You can also buy a Bluetooth module and use my app to see the real timedata. Then you can define by yourself at which voltage the battery has which percentage.
```

---
## \#24 Posted by: Wschles Posted at: 2017-03-20T20:28:59.861Z Reads: 109

```
Do you sell the modules or have a link to it?
```

---
## \#25 Posted by: PXSS Posted at: 2017-03-20T22:44:52.852Z Reads: 107

```
Don't forget to mention it only works with android!
Otherwise I'd be all over it
```

---
## \#26 Posted by: Ackmaniac Posted at: 2017-03-21T00:29:51.103Z Reads: 116

```
Yeah sorry, it's only for android. If you don't have one I think it's worth the 3 dollars for the Bluetooth module and borrow a android smartphone from a friend. This way you can learn a lot about how your VESC works. 
More info here. 
http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286/935?u=ackmaniac
```

---
## \#27 Posted by: PXSS Posted at: 2017-03-21T00:31:57.834Z Reads: 115

```
Just port it to iPhone already!! Lol
```

---
## \#28 Posted by: longhairedboy Posted at: 2017-03-21T14:38:26.796Z Reads: 132

```
[quote="PXSS, post:18, topic:19277"]
25Rs are not great in delivering high amounts of current as voltage sag takes a toll on them specially past the 50% mark
[/quote]

it seems terrible on paper but in practice with the higher P counts (4 and over) its not as bad as it seems like it would be. There's no free lunch, so if you want more amp hours you lose discharge capacity, if you want more discharge capacity you lose amp hours, and if you try to do both by achieving some kind of balance you get various degrees of voltage sag. That's my observation anyway.
```

---
## \#29 Posted by: PXSS Posted at: 2017-03-21T15:47:01.596Z Reads: 129

```
They're just old and outdated. There's better options now that don't break the bank. 

Samsung 30Q from Nkon @ $2.75 if you're outside Europe. 3Ah per cell, much better power delivery than 25Rs. 25Rs sag as much drawing 5A/cell as the 30Qs do drawing 15A/cell. 

Sanyo GA cells are more expensive ($5 a cell). 
They have 3.5Ah/cell and sag just as much as 25R cells drawing the same amount of current.
```

---
## \#30 Posted by: longhairedboy Posted at: 2017-03-22T18:53:16.613Z Reads: 127

```
Where are you getting those prices and in what quantities? I'm not seeing that kind of pricing anywhere i would actually be willing to buy from. I don't buy cells from ebay or alibaba, i get them from lionwholesale usually but i try to make sure whoever i get them from are in the US and can actually stand behind a product without getting returns lost in China Post territory. 

the 30Q has a max continuous discharge of 15Amp, leaving a  60Amp pack in a 4P config. The 25R has a max continuous of 20amps and a sub-second burst capacity of up to 100Amps. That's the trade off. You either get more amp hours or more continuous current at a time. I'm betting voltage sag correlates with max continuous current because i keep seeing "better batteries" around that don't deliver their juice as fast or as hard. 

The Sanyo NCR18650GA deliver a whopping 10amps max continuous. Not interested. 

So yeah, by limiting their current draw within the cell, they have effectively not allowed you to draw the kind of power that not only results in voltage sag but also results in higher discharge capabilities and a lower amp hour spec. 

I guess that makes them better, i don't know. I build 80 amp packs and use a 60 amp BMSs and try to tune my VESCs to not launch like an out of control rocket, so the voltage sag I am actually seeing on the street just isn't anything i wouldn't expect. Out of any cell. 

So should I use 15amp cells with a higher Ah rating so that my volt meter doesn't drop a percent or two while I'm hitting the throttle? Or should i just let the hardware draw what it wants from a set of cells that are willing to give them their all?

It deserves a good pondering i suppose.
```

---
## \#31 Posted by: Maxid Posted at: 2017-03-22T20:51:04.878Z Reads: 114

```
he gets them from nkon.nl - a european supplier that also ships to the US apparently.

The current ratings don't mean anything. You need to look at the discharge curves. You will see that the 30Q don't just deliver 15A but can go much higher. You will also not drain them continuously at that current so the added capacity and less voltage sag make a big difference compared to the higher temperature increase they see at continuous high current use.

We actually need to get away from this "I build 80amp packs" as your basing this info solely on the rated current. It says nothing about the actual performance of the cells. 30Q would make a rated 60A pack but would kick your 80A pack's ass ;)
```

---
## \#32 Posted by: landonkun Posted at: 2017-03-22T22:36:30.708Z Reads: 114

```
I'm curious about those batteries myself. I might try them out in my next build.
But even on that nkon.nl site, 40 of them still works out to about $3.30 (cause no VAT). I want that $2.75 price :stuck_out_tongue:
```

---
## \#33 Posted by: PXSS Posted at: 2017-03-23T00:41:00.289Z Reads: 114

```
@longhairedboy 
I source 30Qs from Nkon and have them shipped to the US. 
I source GAs from Liionwhesale too. 

Stop looking at just the rating. That's the issue with a lot of people here, you see numbers and take them by heart without understanding the reasoning behind them is. Look up the spec sheets and read them if you have the time. The reason 30Qs are rated to 15A is because if you continuously run them at that current and charge them at 4A, after 300 cycles, you only get 73.8% of rated capacity. That's where Samsung decided to draw the line. In the same spec sheet they show that for 22A continuous and a temp cutoff of 70C and charge at 4A, after 250 cycles, they get 72.4%.

Similar stuff is done by Panasonic. You can run the cell at higher currents CONTINUOUSLY by sacrificing number of cycles you can run them for. Key word there is continuously. We do not do this unless you're climbing an endless 15 degree incline at 20mph. 

Check these graphs out, I've posted them several times:

First is Sanyo GA vs 25Rs:
This is continuous current running through them, the vertical difference between curves is voltage sag at that specific capacity. The red curves are GA and blue is 25R. From top to bottom 0.2A, 5A and then 15A. Henrik's battery holder failed on one of the 15A GA test, that's why it is cut short. The other one he stopped at 75C. 

<img src="/uploads/db1493/original/3X/5/b/5b616802d5299a6dc7a79a8c46504a9b4c7fbe77.PNG" width="690" height="387">

The takeaway here is that they have less voltage sag than 25Rs, aka they can deliver more power for the same throttle setting at the same discharge level. Also, if you were to throttle to 15A with 25Rs sag down to 3.2V which is most people's soft cutoff after 1.125Ah consumed. With the GAs, you sag down to 3.2V after 1.55Ah consumed. The gap widens if you bring the cutoff lower. 

---

Next 30Q vs 25R:
Same thing as before, Red is 30Q, blue is 25R. Top to bottom 0.2A, 5A, 15A

<img src="/uploads/db1493/original/3X/5/e/5e561358e769e2c21fc3821c337cbbf380668b2d.PNG" width="690" height="387">

Here, there is a big difference. The 30Qs drawing 15A sag down as much as the 25Rs drawing only 5A after 1.25Ah consumed (which is 50% capacity of 25Rs). At 15A and 1.25Ah consumed, the 30Q outputs 2070W, the 25Rs on the other hand output 1902W. At 15A, 25Rs sag to 3.2V at 1.125Ah, 30Qs sag to 3.2V at 2.125Ah, that is almost double!

As I said 30Qs are much better at delivering high power than 25Rs. GAs can deliver slightly more power while having 40% more capacity!

I hope this is clear, I've been writing this on and off throughout the day while flight testing lol.

---

I intentionally left out the 20A case.
Henrik tested the 25Rs a long time ago and he didn't measure temperature back then. We cannot say that the cell did not overheat as he didn't measure this. 
He didn't test GA cells at 20A because he thought they would overheat (and he broke his cell holder), rightly so, but again, we do not run continuously. 
He stopped the 30Q test early at 20A because of heating. He got through 2Ah before he stopped the test because the cells reached 80C. That would be. 6 minutes continuously at 20A per cell. 

---

It seems that Nkon's prices have gone up since I ordered
```

---
## \#34 Posted by: longhairedboy Posted at: 2017-03-23T03:11:49.442Z Reads: 95

```
That's a terribly convincing argument.  I think you've made a believer out of me.
```

---
## \#35 Posted by: PXSS Posted at: 2017-03-23T04:19:02.072Z Reads: 97

```
The more people get on board and spread the knowledge the less I will have to repeat myself and the sooner esk8 will leave behind using an overrated and outdated cell! :)
```

---
## \#36 Posted by: smurf Posted at: 2017-03-23T07:16:57.558Z Reads: 94

```
Clearly we need a battery FAQ so we don't have this conversation every week in  yet another thread
```

---
## \#37 Posted by: TarzanHBK Posted at: 2017-03-23T08:00:26.104Z Reads: 95

```
I wrote this 2 months ago in a battery thread and was wondering why companies like Enertion are still using the 25r.
I think it´s just the "we´ve always done it like this and keep doing it like that" thing.
Or maybe it´s the price point - 25R are slightly cheaper than 30Q.
```

---
## \#38 Posted by: Maxid Posted at: 2017-03-23T08:02:16.092Z Reads: 92

```
well at least he is trying:
http://www.electric-skateboard.builders/t/raptor-2-most-powerful-direct-drive-electric-skateboard-kickstarter/12694/1004?u=maxid
```

---
## \#39 Posted by: TarzanHBK Posted at: 2017-03-23T08:04:28.198Z Reads: 90

```
yep! So I think we have to spread the word of battery gods to the world and after a few months we´ll be having more people with cool packs on the street that also last longer :angel:
```

---
## \#40 Posted by: Maxid Posted at: 2017-03-23T08:05:37.845Z Reads: 89

```
I still feel bad about building myself a 25R pack :cry:
```

---
## \#41 Posted by: TarzanHBK Posted at: 2017-03-23T08:09:12.367Z Reads: 76

```
Like I told you, you had the chance to hopp in our group buy :D

But the 25r is still a good battery, it´s not like you´re having a bad pack now :slight_smile:
```

---
## \#42 Posted by: PXSS Posted at: 2017-03-23T12:10:22.191Z Reads: 78

```
I bet it'll come at a hefty price increase...
@smurf, I've been thinking about that but I don't think I have the time to write it...
```

---
## \#43 Posted by: Maxid Posted at: 2017-03-23T12:13:07.985Z Reads: 80

```
he says ~50-70USD - not that bad actually.
```

---
## \#44 Posted by: PXSS Posted at: 2017-03-23T12:14:56.059Z Reads: 80

```
What is the price difference per cell. If it's any higher than that, it's bs.
Lol, I bet you he saw multiple threads showing that 30Qs are better and decided he could make a quick buck. I just checked, the price difference between 25Rs and 30Qs in bulk is 30cents. For a grand total of $12 increase in cost. 

That's what pisses the crap off of me of people like that. Making money on other's work.
```

---
## \#45 Posted by: longhairedboy Posted at: 2017-03-23T14:23:20.677Z Reads: 79

```
[quote="PXSS, post:44, topic:19277"]
That's what pisses the crap off of me of people like that. Making money on other's work.
[/quote]

You're going to be pissed at him a while then. His entire model from the beginning was to leverage the DIY community to fund proprietary development and ultimately develop a product that leaves DIY behind and raises margins. It's playing out exactly as i predicted a couple of years ago. Its not an uncommon model, and at least one positive result was this community, not to mention a seriously elegant drive system. 

So i just checked pricing... NKON definitely has a great price on those 30Qs, so definitely worth switching over to them. Too bad when i loaded 50 of them in my cart they told me they didn't have shipping options for my address. I was just trying to see what the total would be with shipping from Europe. Weird. I live in a house on a street. I wonder if that's an issue? lol

Edit: nevermind, they have a seperate site for ordering from outside of Europe. They ship via FedEx and it might take 3 weeks for them to get here but it still seems worth it. The price is still really good. I'm just going to have to stay ahead if i want to reduce build times. One reason i like liionwholesale is because the shit is at my house within a week. That's not worth the premium, though.
```

---
## \#46 Posted by: PXSS Posted at: 2017-03-23T16:10:22.787Z Reads: 70

```
"Proprietary development" /sarcasm
```

---
## \#47 Posted by: longhairedboy Posted at: 2017-03-23T17:01:54.311Z Reads: 72

```
i know, i know... but i might know some things i can't talk about...
```

---
## \#48 Posted by: eLDoska Posted at: 2017-03-23T17:37:42.314Z Reads: 80

```
[quote="PXSS, post:33, topic:19277"]
As I said 30Qs are much better at delivering high power than 25Rs.
[/quote]

This is a wrong conclusion.
Let me explain why.
We have 2 cells: 25R and 30Q. Both are high current cells and both have end voltage: 2.5V
So we can discharge these cells to 2.75V without worring about their health. But for example let's take 2.9V limit as the safest. And let's take 3 graphs - 5A 10A and 15A because we power e-boards and not led-lights.

So let's start with Graph1. It shows us how much capacity is given by these cells from nominal (2500mAh - 25R; 3000mAh - 30Q) at 2.9V
<img src="/uploads/db1493/original/3X/a/e/aecc3d2a579224627578538cb7099bac3795d2e0.jpg" width="690" height="328">
25R (2,5Ah)
5A = 2.35Ah (-6%)
10A = 2.25Ah (-9%)
15A = 2.15Ah (-14%)
30Q (3.0Ah)
5A = 2.8Ah (-6.5%)
10A = 2.7Ah (-10%)
15A = 2.6Ah (-13%)
**Booth cells have almost the same results.**

Graph2. It shows us how big the Voltage drop is at 50% of each cell (1250mAh - 25R; 1500mAh - 30Q) 
<img src="/uploads/db1493/original/3X/7/e/7ec602cf90750fa18542a10e34c196da808176b9.jpg" width="690" height="385">
5A: 25R - 3.45V; 30Q - 3.55V (difference 3%)
10A: 25R - 3.28V; 30Q - 3.46V (difference 5.5%)
15A: 25R - 3.18V; 30Q - 3.38V (difference 6%)
**In real life it means that at 10S setup with 40km/h top speed with 30Q cells, 25R cells will give us 37.6-38.8km/h top speed. Can you feel this 1.2-2.4km/h difference?** 

Graph3. It shows the behaviour of both cells at 20A (1250mAh - 25R; 1500mAh - 30Q)
<img src="/uploads/db1493/original/3X/6/2/625d51edebad464ca2d76af44ceaff17b24326df.jpg" width="690" height="381">
25R - at 2.9V give us 2Ah from nominal 2.5Ah
30Q - overheated (70C) at 3.15V and gives at this voltage 2.1Ah from 3Ah nominal
(the same peak you can notice at 15A Graph1 after 2.9V)

**Conclusion**
 Both cells are good.
25R is a good cool cell for a good price. But it has larger voltage sag (compare to 30Q: minus 3-6% or minus 1.2-2.4km/h at 40km/h board). 
30Q is minimum 32% expensive and has 20% more capacity as 25R. Also 30Q are hotter as 25R so minimal setup for them is 4cells in parallel.

So in my oppinion "much better" is difference 10-15km/h at top speed. 1.2-2.4km/h is somthing that i can not feel, that means that both cells are good enough for e-boards.
```

---
## \#49 Posted by: Maxid Posted at: 2017-03-23T19:04:05.261Z Reads: 70

```
Why would you take the voltage sag at 50% of each battery? Makes no sense.

[quote="eLDoska, post:48, topic:19277, full:true"]
30Q is minimum 32% expensive and has 20% more capacity as 25R. Also 30Q are hotter as 25R so minimal setup for them is 4cells in parallel.
[/quote]

Where do you buy your cells? It is more in the lines of 25% more expensive but with 20% more capacity plus less voltage sag. How can you say no to that?
```

---
## \#50 Posted by: longhairedboy Posted at: 2017-03-23T19:21:22.764Z Reads: 70

```
While you guys are deciding what cells I should use, I'm going to open this fresh new box of Pop Secret i just picked up when i rode my old ass 25Rs  to Publix at 37mph while flipping the bird to a tailgator.
```

---
## \#51 Posted by: JohnnyMeduse Posted at: 2017-03-23T19:29:04.606Z Reads: 71

```
[quote="longhairedboy, post:50, topic:19277"]
i rode my old ass 25Rs
[/quote]

Are they WORKING... A need picture... these 25R should had burn down your board... :stuck_out_tongue_winking_eye:

[quote="longhairedboy, post:50, topic:19277"]
While you guys are deciding what cells I should use
[/quote]

WHAT are you trying to make money out of OTHER PEOPLE WORK ? :anguished:  :grin:
```

---
## \#52 Posted by: eLDoska Posted at: 2017-03-23T19:44:37.244Z Reads: 76

```
[quote="Maxid, post:49, topic:19277"]
Why would you take the voltage sag at 50% of each battery? Makes no sense.
[/quote]
You can take another % of nominal. The result will be +/- the same.
[quote="Maxid, post:49, topic:19277"]
It is more in the lines of 25% more expensive
[/quote]
25R - 2.15€/40cells 
30Q - 2.82€/40cells (25R+≈31%)
[quote="Maxid, post:49, topic:19277"]
How can you say no to that?
[/quote]
I dont say no to that if i will build 10s4p+ pack and when i will have 30% more money. :) But when i will build cheap 3p pack or my budget is small i will choose 25R.
```

---
## \#53 Posted by: longhairedboy Posted at: 2017-03-23T19:50:41.036Z Reads: 77

```
MEEE??? Take advantage of free information and share literally every thing i use it for to the benefit of the general public as well as making enough cash to sustain my hobby? NEVER. I'm insulted at the very idea. /s

https://www.instagram.com/p/BR9m9_xFBXt/?taken-by=longhairedboy

If you look closely, you can see that its not quite on fire yet. 

But let me tell you something. ONE of those cells will light a nickel strip up like a candle. Metal burns like paper for these guys. Luckily i've only had that happen once. I have, however, blown a few holes in soldering tips when my coordination failed me. I keep lots of tips around now. And the biggest fire extinguisher i could find at Lowes. 

I just bought a spot welder with a wand so building these will get a lot easier in a few days as i'll be eliminating the acrobatics needed to tack these together with the standard sunkko 788H front mounted welder.
```

---
## \#54 Posted by: Maxid Posted at: 2017-03-23T19:57:40.889Z Reads: 74

```
let me know where you buy them for that price
```

---
## \#55 Posted by: eLDoska Posted at: 2017-03-23T20:28:01.820Z Reads: 72

```
[quote="Maxid, post:54, topic:19277, full:true"]
let me know where you buy them for that price
[/quote]

nkon
.....
```

---
## \#56 Posted by: Maxid Posted at: 2017-03-23T20:29:49.351Z Reads: 73

```
just post a link dude
https://eu.nkon.nl/samsung-inr-18650-30q-3000mah.html they are far from 2.82€ a cell at 40cells
At least for me...
```

---
## \#57 Posted by: eLDoska Posted at: 2017-03-23T20:32:21.509Z Reads: 73

```
https://ru.nkon.nl/rechargeable/18650-size/samsung-inr-18650-30q-3000mah.html
```

---
## \#58 Posted by: Maxid Posted at: 2017-03-23T20:34:42.062Z Reads: 75

```
really weird: there has got to be something wrong here
<img src="/uploads/db1493/original/3X/6/e/6ef505b0fdcbe4c6ad43544487eb9ec613432c15.png" width="340" height="402">
```

---
## \#59 Posted by: fedestanco Posted at: 2017-03-23T20:57:16.282Z Reads: 71

```
Haha, lets buy the shit out of this shop!
```

---
## \#60 Posted by: landonkun Posted at: 2017-03-23T22:30:48.256Z Reads: 71

```
Haha what.
"I'd like two orders of 20... but please ship them together" :smiley:
```

---
## \#61 Posted by: Okami Posted at: 2017-04-06T21:50:24.637Z Reads: 64

```
@landonkun yeh I saw this glitch a while ago!

i believe @PXSS got to order them at a very good price! Since the price still stays low, even if you order 40pcs, I believe!
```

---
## \#62 Posted by: MaroonArcher Posted at: 2017-07-22T20:57:06.057Z Reads: 56

```
Hey guys, need some help.  My set up uses three 4 cell batteries that add up to 50.4v. I have a 12s bms for the board for charging. I wired everything up like the description showed. I have an aluminum cased charging brick with a fan and all that. The charging brick is shown is specs to charge to 50.4v yet my batteries aren't charging. I have all the wires connected right and the charging brick has the LED light on showing it's on but nothing charges.
```

---
## \#63 Posted by: Tweety90 Posted at: 2019-08-17T12:12:01.017Z Reads: 10

```
I am struggling with finding a way how to charge my battery only up to 80%. It's only because I want to increase lifespan, and because I am riding mostly short distances.
Is there a charger I can use to charge the 10s2p Sanyo Battery which I have in my Backfire G2 to a preset percentage? Is there some charger from hobbyking or somewhere?
```

---
