# 6s2p battery capcity question LGHG2

### Replies: 58 Views: 3021

## \#1 Posted by: ralphy Posted at: 2017-02-22T22:45:47.907Z Reads: 162

```
So this is my first 18650 build and i got my cells from imr batteries.

I built two 6s2p packs. The cells came in at 3.51v char51 showed at 4% 

My charger is showing only about 4000mah going in to fully charge a pack Shouldnt it be closer to 6000mah?

<img src="/uploads/db1493/original/3X/e/0/e0f1ccfd0f6765d27c38eb1fbdb4256a3eb12438.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/f/f/ff7be97abfc9435582904f7c36ff09db2fa9ffd5.jpg" width="666" height="500">
```

---
## \#2 Posted by: Okami Posted at: 2017-02-22T23:05:36.598Z Reads: 155

```
Dunno if these are nmc type but try to discharge till 3.4 or 3.2v then charge and check what capacity u get ;)

I assume 250mah 'lost' per cell.

Extra 50-100mah per cell if u charge till 4.2v

Then another 100-200mah below 3,5v

--   

Nice charger! I got the same one!
```

---
## \#3 Posted by: ralphy Posted at: 2017-02-22T23:19:04.005Z Reads: 151

```
Nice thanks.

Im used to lipos that never go below 3.75v 

So i should always run these to 3.2v in the future? 

Whats the best way to extend their durability and capacity?

My lipos are stored at 3.75v so im not sure what to do with these.
```

---
## \#4 Posted by: Okami Posted at: 2017-02-22T23:22:02.956Z Reads: 143

```
Check graphs. Search lg2 discharge test

Not close to pc. Cannot help :slight_smile:
Some li ions can be taken till 2,5v but personally i think below 3.0v they are not usable much.

Would recommend 3.3-3.4v as lowest discharge and 4.1 - 4.15v  charge
--
Btw how u managed to get percentage display for reaktor? Mine does not show this in default..
--

https://www.e-cigarette-forum.com/forum/threads/lg-hg2-20a-3000mah-18650-bench-retest-results-a-great-20a-battery.714112/
```

---
## \#5 Posted by: Namasaki Posted at: 2017-02-22T23:43:54.530Z Reads: 127

```
Check the mah cutoff in your charger's settings
```

---
## \#6 Posted by: ralphy Posted at: 2017-02-23T00:37:24.467Z Reads: 121

```
Mine doesn show percentage. I got the percentage by using a handheld balance charge digital meter.
```

---
## \#7 Posted by: ralphy Posted at: 2017-02-23T00:38:15.669Z Reads: 122

```
Its not the cut off limit but thanks. Ill cycle them several times hopefully it improves.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-02-23T00:50:39.243Z Reads: 120

```
Oh, I remember now. Your charge is showing how much it put in the battery to bring it to full charge, not what the total capacity is.
My hobby charger does the same thing. The amount it shows at end of charge will vary depending on how low the cells where before charging.
It's been a while since I used my hobby charger.
```

---
## \#9 Posted by: PXSS Posted at: 2017-02-23T03:40:17.532Z Reads: 118

```
Liions run down to 2.5v/cell unlike lipos. You should set your lv soft at 3.0 at cutoff at 2.8. To prolong life also dont charge above 4.1v. 

Your charger has a profile for LiPo and Li-Ion. They are not the same. The low voltage cutoff is different. If youre only discharging to 3.3V then you're wasting a good 30ish percent capacity.

Storage for Li-ions is 3.55V. 
50% is 3.6V

E: Discharge profile
<img src="/uploads/db1493/original/3X/3/6/36f499f3a80ccadfe5def7a751947b0f00e12b91.PNG" width="690" height="387">
```

---
## \#10 Posted by: ralphy Posted at: 2017-02-23T04:05:47.044Z Reads: 110

```
Hey thanks! Thats good info, i would never think they would go that low. 

When you say lv soft at 3.0 and cutoff at 2.8v are your talking about the BLDC settings or the charger?

I only use my charger to charge i dont use it to discharge.
```

---
## \#11 Posted by: Namasaki Posted at: 2017-02-23T05:38:16.662Z Reads: 101

```
He's taking about BLDC settings
on the first page under Voltage Limits
Battery Cutoff Start 3.0
Battery Cutoff End 2.8
```

---
## \#12 Posted by: Okami Posted at: 2017-02-23T17:17:18.148Z Reads: 95

```
Report back once you charge your cells again!

Yes, my turnigy reaktor also does not show percentage.. it was a nice feature which accucel 8 charger had :slight_smile:
```

---
## \#13 Posted by: ralphy Posted at: 2017-02-23T19:08:00.314Z Reads: 95

```
<img src="/uploads/db1493/original/3X/c/8/c85c2d1c515770480943daaec43bbbac62f5c6f0.jpg" width="666" height="500">

I will modify them this is where they are at now.
```

---
## \#14 Posted by: ralphy Posted at: 2017-02-24T16:50:33.797Z Reads: 84

```
Took them down to 3.1v and the latest charge filled them 5650mah at 4.2v 

I think that's pretty good. Any thoughts?
```

---
## \#15 Posted by: Namasaki Posted at: 2017-02-24T18:34:37.823Z Reads: 81

```
Your charge is showing how much it put in the battery not what the total capacity is.
```

---
## \#16 Posted by: Okami Posted at: 2017-02-24T19:19:06.273Z Reads: 81

```
@Namasaki what you man with total capacity then? Do you discharge your cells completely till zero so they dont give up any more power?

Or you just meant that the discharge capacity is not the same as charge capacity?

---

@ralphy I think it is pretty good.. this way u should now know that below 3.1v there are the rest of the capacity more or less.. which would be around 350/2 = 175mah per cell or so right?
```

---
## \#17 Posted by: Namasaki Posted at: 2017-02-24T20:25:22.371Z Reads: 83

```
[quote="Okami, post:16, topic:18112"]
Or you just meant that the discharge capacity is not the same as charge capacity?
[/quote]
What I mean is that a typical hobby charger like the one I have, does not display a battery's  total capacity at the end of charging. Instead, it displays how much was added to bring the battery to full charge. 
Example:
If your battery's capacity is 6000mah and it is at 50% charge when you recharge it, your charger will display 3000mah. 
This is why @ralphy battery displayed a higher number after discharging his pack lower before charging it to full again. 
Unless he discharges his batteries to 0% which I think is something like 2.8v per cell, it is not going to display a full 6000mah no matter how many charge cycles you put it through.
```

---
## \#18 Posted by: Okami Posted at: 2017-02-24T20:38:42.330Z Reads: 80

```
@Namasaki well that is quite logical, indeed.. I just thought you had some more things to add to this.. :D 

Like, maybe, the ''losses'' or extra capacity which might be added to bring all the cells to the same level.. though I havent really looked into it, does it really makes a big difference to the mah rating the charger shows
```

---
## \#19 Posted by: Hummie Posted at: 2017-02-24T21:16:16.713Z Reads: 78

```
i was reading that when you speed charge you can jump up quickly to maybe 80 percent of full capacity and all is well but if you attempt to speed charge to full charge, even though the charger will cut off after a shorter time and the voltage maybe have been up to 4.2, the lithium chemistry needs the longer time to absorb the energy and it will drop to a lower voltage.    A better way to say it maybe: the voltage will rise quickly with a speed charge which is misleading as the ah put in it will be less and after the cell is pulled from the power source it will decrease more than if it had been put on the charger with a slow charge to full
```

---
## \#20 Posted by: Namasaki Posted at: 2017-02-24T21:37:01.857Z Reads: 74

```
When you say speed charge, do you mean 5a charge or higher?
```

---
## \#21 Posted by: Hummie Posted at: 2017-02-24T21:44:38.063Z Reads: 69

```
i don't know details but know it depends on the size of the cell of course.  I charge an 8ah pack at 8amps so im on the cusp I think but double that, if my charger could do it, I'd have a hard time getting to that top of the charge.  what I was reading made it out like it would take as long to get to a full charge even if you do it speedy as going speedy it blasts through the cc part of the charge but then the cells will have to sit for much longer on the later cv part for them to actually hold the energy.  something like that.
```

---
## \#22 Posted by: Namasaki Posted at: 2017-02-24T21:45:15.627Z Reads: 67

```
I was just trying to show @ralphy that the mah reading on his charger did not necessarily mean that there is anything wrong with his battery cells. 
As long as the pack charges to fulll voltage,  it's good.
```

---
## \#23 Posted by: Hummie Posted at: 2017-02-24T21:46:29.610Z Reads: 66

```
haha.  as long as the pack charges to full voltage it's good!  out of context it sounds like some crazy battery advice.  I'm imagining some nubie with their totally dead and abused battery sitting patiently at the charger.

have you ever tried to revive beat up or really low voltage cells?  If any cells have a voltage that's strangely low I call it done and don't bother .  anything that wont pop up to 3 volts by the next day.  if it wont I give up on it.  similarly my cells with holes in them show really low voltages and I give up on them of course


you've got your battery amps at 25 and motor at 40 @ralphy. that's very low.  especially with the voltage you'll be using at 6s....that's like 25 x22 max power in.  500 watts.  subtract losses and maybe 450.  you might be really disappointed.  you could increase the battery max amps to 40 at least and the motor...dare I say 200!

if you live near san Francisco Ive got a bunch of those cells Im getting rid of and you could bump it up
```

---
## \#24 Posted by: ralphy Posted at: 2017-02-24T22:41:44.101Z Reads: 60

```
It's a 12s 2p setup @hummie. So I'm happy with the power output. I will look into your advice on those settings and improving performance. 

I didn't know you had these cells I'm in Miami. I dropped like 150 bucks on 24 cells from imrbatteries in Texas. 


As far as fast charging like ions yes the first 70% can be done fast. That's how the Tesla supercharger stations work. They fill the cells up in 20min or so to 70% capacity . It's pretty cool.
```

---
## \#25 Posted by: Hummie Posted at: 2017-02-24T23:24:33.774Z Reads: 56

```
you're setting the amp limit at like 60 percent of the cell's stated peak discharge limit. I guess you could make the cells last longer that way but I'd rather have the performance the few cells you have are capable of.
```

---
## \#26 Posted by: PXSS Posted at: 2017-02-24T23:26:55.385Z Reads: 59

```
Fast charge just means you charge at Constant Current. Once you reach the CV phase the charger stops. You can do this at literally any current up to whatever the max current for your cells is. 
I usually do mine at 1c

The capacity you put in is always higher than the capacity you discharge. This is because your charger is not 100% efficient and there are some losses in the wires, etc. This also happens because your charger will balance the cells which pretty much entails charging the battery and discharging the cells with high voltage through balance leads until all of the cells are at the same level, the charger does not take this into account when giving you the amount of energy you put in. A simple way to see this is by charging not balanced and then balanced and you'll see the latter takes in more capacity even if they end up at the same voltage
```

---
## \#27 Posted by: Namasaki Posted at: 2017-02-24T23:33:52.001Z Reads: 56

```
[quote="Hummie, post:21, topic:18112"]
i don't know details but know it depends on the size of the cell of course.  I charge an 8ah pack at 8amps
[/quote]

My Lipos packs are rated for 25a charge. I charge them at 5a so I'm guessing that would not be considered fast charging.
```

---
## \#28 Posted by: Hummie Posted at: 2017-02-24T23:36:52.980Z Reads: 56

```
.I wouldnt say fast charging "just" means you charge at constant current, it also means you're charging at a high current.

@Namasaki what c rating are your cells?
```

---
## \#29 Posted by: Namasaki Posted at: 2017-02-24T23:40:53.671Z Reads: 55

```
[quote="Hummie, post:23, topic:18112"]
haha.  as long as the pack charges to full voltage it's good!  out of context it sounds like some crazy battery advice.  I'm imagining some nubie with their totally dead and abused battery sitting patiently at the charger.

have you ever tried to revive beat up or really low voltage cells?  If any cells have a voltage that's strangely low I call it done and don't bother .  anything that wont pop up to 3 volts by the next day.  if it wont I give up on it.  similarly my cells with holes in them show really low voltages and I give up on them of course
[/quote]


Ok, ya I guess that statement could be taken wrong. I meant within the normal amount of charge time.
```

---
## \#30 Posted by: Hummie Posted at: 2017-02-24T23:43:01.011Z Reads: 55

```
im starting to sound like grammar police.  

can you find your lipo charge rate?  it seems rare.
```

---
## \#31 Posted by: Namasaki Posted at: 2017-02-24T23:46:35.858Z Reads: 57

```
They are 5000mah 60-120c Lipos with 5c charge rate.
http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014
```

---
## \#32 Posted by: Hummie Posted at: 2017-02-24T23:49:09.099Z Reads: 55

```
weird my flightmax 8ah with 30c have a 5c charge rate as well.   so what's the math for this stated max madness.  5 times 5 for you.  25amps.
```

---
## \#33 Posted by: PXSS Posted at: 2017-02-25T00:06:23.447Z Reads: 53

```
For him its 25 for you its 40. And fast charging really is just cutting off the cv stage. There is no current defined that you should charge at for it to be fast, all companies do it at different rates. 

EG Tesla does 1C I believe, Android phones do 2C, Lipos can be done at 5C, liions at 1-2c. 

It really depends on the application. The one thing they all have in common when they say fast charge is that they cut off the cv phase
```

---
## \#34 Posted by: ralphy Posted at: 2017-02-25T00:06:37.137Z Reads: 49

```
The whole pack is running two vesc. Are you sure I can push that little pack to those limits per vesc ?
```

---
## \#35 Posted by: PXSS Posted at: 2017-02-25T00:09:40.752Z Reads: 49

```
No. You would kill your cells. 
25A per vesc is 50A total. Your cells are only rated to 20continuous and you have two in parallel which means 40A total. Your settings are fine, you might be pushing them a little
```

---
## \#36 Posted by: ralphy Posted at: 2017-02-25T01:03:58.007Z Reads: 49

```
I figured it was pretty much maxed out because I can't stay on the board if i hit full throttle from a stop. 

Top speed is at 23 mph and I'm 180 lbs 

I used to get 26mph with a 16000mah 12s1p lipo.
```

---
## \#37 Posted by: Namasaki Posted at: 2017-02-25T01:37:01.080Z Reads: 49

```
is your computer a Mac or Pc?
```

---
## \#38 Posted by: ralphy Posted at: 2017-02-25T04:57:42.331Z Reads: 48

```
Pc dude, i hate the fruit...... surface pro3
```

---
## \#39 Posted by: Okami Posted at: 2017-02-25T09:18:24.901Z Reads: 48

```
[quote="PXSS, post:26, topic:18112"]
The capacity you put in is always higher than the capacity you discharge
[/quote]

This is what i was talking about, at first I didnt know it but i think it later on becomes clear that you can get 'varied' amount of capacity when discharging.

Discharge rate and temperature influences this, so the cells are not as 'linear' as we would like to think :)
```

---
## \#40 Posted by: Hummie Posted at: 2017-02-25T17:50:36.328Z Reads: 47

```
sorry for my math above I thought we were working it out for one motor.  

As you say @okami, and I wonder how well a lipo being used under the typical low rate of discharge for its stated ability on a board will compare to a li-ion being pushed further towards it's discharge limit in capacity and also life cycles.
but can't you get really close discharge energy to the input energy if you draw at low amperage?  the conversion from chemical to electrical energy is probably the most efficient thing on the board possibly

The word "fast"..can mean anything I guess but in my mind a fast charger is one that would charge fast.  1c rate is pretty fast.
```

---
## \#41 Posted by: mmaner Posted at: 2017-02-26T02:49:52.704Z Reads: 42

```
I've got a surface pro 3 as well, love it.
```

---
## \#42 Posted by: Namasaki Posted at: 2017-02-26T06:31:02.408Z Reads: 40

```
I'm an Apple addict myself.
```

---
## \#43 Posted by: ralphy Posted at: 2017-02-26T14:11:26.411Z Reads: 40

```
In my line of work most of the programs are windows based. Apple products are great it just i cant use them for what I do.
```

---
## \#44 Posted by: ralphy Posted at: 2017-02-26T14:12:45.055Z Reads: 39

```
Picked mine up used a year ago on ebay for $250 due to a little crack in the corner of the screen. Best money i ever spent on a computer.
```

---
## \#45 Posted by: mmaner Posted at: 2017-02-26T14:58:09.055Z Reads: 42

```
[quote="Namasaki, post:42, topic:18112, full:true"]
I'm an Apple addict myself.
[/quote]

My condolences 😀
```

---
## \#46 Posted by: Namasaki Posted at: 2017-02-26T16:23:46.305Z Reads: 40

```
My first apple product was an iphone 2.
```

---
## \#47 Posted by: mmaner Posted at: 2017-02-26T17:15:45.207Z Reads: 40

```
Actually, mine too.  It was also the last Apple device I liked. From a manufacturing standpoint most Apple products are sub par.  From a software stand point, I'm just not a fan of closed source code.  I used to have a power Mac for Photoshop that I loved, but I absolutely cannot stand apples notebooks. 

I'm not saying you shouldn't use apple stuff, I'm just not a fan.
```

---
## \#48 Posted by: Eboostin Posted at: 2017-02-26T18:50:49.589Z Reads: 40

```
Why did you do 2 6S2P rather than 1 12S2P?

Was it only for the charging?
```

---
## \#49 Posted by: ralphy Posted at: 2017-02-26T19:07:57.419Z Reads: 39

```
Well yes for charging  and weight distribution on both sides of the board. but the 2 6s2p are wired in series when mounted on the board and they produce the power of a 12s 2p. 

Do you understand?
```

---
## \#50 Posted by: Eboostin Posted at: 2017-02-26T20:09:05.161Z Reads: 38

```
Yes, I understand. My question was more in terms of if there a compelling reason to go one way vs the other. The weight distribution will be the same if it's two rows, sounds like it was done more for the charger.
```

---
## \#51 Posted by: ralphy Posted at: 2017-02-26T22:41:15.435Z Reads: 36

```
Well safety. I rather handle two packs at 25v that I can connect independently than one 50v pack that can kill.
```

---
## \#52 Posted by: ralphy Posted at: 2017-03-02T14:57:28.537Z Reads: 37

```
Here are the 2 finished packs. Im not sure if there is a market for them but if anyone wants these built i have the resources to get it done and we can work out a price.

One thing i did different is i encased all the cells into a aluminum c channel once the circuit was spot welded and completed then i heat shrinked the whole thing. The aluminum protects the cells and helps with any heat dissipation. Rode 7 miles last night went from 4.15v to 3.85v.

Enjoy<img src="/uploads/db1493/original/3X/7/8/78e39b4a80907f99883bb60b576dff7a6f363e72.jpg" width="666" height="499">
```

---
## \#53 Posted by: Namasaki Posted at: 2017-03-02T16:07:21.773Z Reads: 34

```
Looks like a clean setup
```

---
## \#54 Posted by: ralphy Posted at: 2017-03-02T16:13:16.740Z Reads: 33

```
Thanks I'm really happy and I appreciate everyone's expertise!

Here is a shot of the welds ...Turned out really good with only 4-6 ohms per cell of internal resistance on the pack.  <img src="/uploads/db1493/original/3X/6/0/6015265b7992aaff5ef96730066f21978992034f.jpg" width="375" height="500">
```

---
## \#55 Posted by: Namasaki Posted at: 2017-03-02T16:31:33.798Z Reads: 32

```
That's low resistance for Li-ion
```

---
## \#56 Posted by: Maxid Posted at: 2017-03-02T16:37:47.272Z Reads: 33

```
those spots do not look good - and are you sure it is Ohm and not mOhm? Did your cells get hot? the second one on the left looks like it's plastic shield was seared.
```

---
## \#57 Posted by: Namasaki Posted at: 2017-03-02T17:20:22.021Z Reads: 32

```
I didn't notice that, your right it should be milliohms.
```

---
## \#58 Posted by: ralphy Posted at: 2017-03-02T18:14:00.289Z Reads: 31

```
Yeah sorry it's m ohms I'll get a pic. The welds are super solid. The cells didn't get hot but the negative  side shield did pull away on some.
```

---
