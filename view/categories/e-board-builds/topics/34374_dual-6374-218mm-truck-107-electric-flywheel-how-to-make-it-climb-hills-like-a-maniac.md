# Dual 6374, 218mm truck, 107 electric-flywheel, how to make it climb hills like a maniac?

### Replies: 20 Views: 1778

## \#1 Posted by: Fabar Posted at: 2017-09-30T14:54:34.513Z Reads: 310

```
First thank you all for your help. It really made a huge difference to avoid a bad experience buying a wrong board and I also had fun reading some funny, direct arguments here.  
I'm planning to build my board but really need something to climb hills, it's quite hilly around here (20% to 30%). With 10 miles of range I would be happy, with 140lbs maybe is not that hard.... 

So from many threads and a lot of reading that I have done here, if I understood it right, I think the best option would be:

Motors: dual 6374 @torqueboards  (thanks @Eboosted for explain your experience with 6374 and 6355)
trucks: 218mm @torqueboards (still not sure if I can fit the V4 mounting with a 107mm Flywheell and 15mm pulley)
Wheels: Superflywheel 107's ABEC11  (trying to avoid too mnay imperfections on the asphalt here, but don't wanna a offroad) still need to find where to buy them.....
pulley and motor mount (thanks @sl33py for your post, I can see that I can use 12mm belt and still have some space, just not sure if I can use V4 mounts from @torqueboards. 
battery: lipo 10S pack (from the experience of @Namasaki (thanks for that!) I'm planning to order 5 packs of this https://hobbyking.com/en_us/turnigy-5000mah-2s-7-4v-60c-hardcase-pack.html building a 10S pack)
BMS: again thanks @Namasaki   http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
remote control: http://www.ebay.com/itm/262779892776

VESC: I'm a bit confused about vescs, looks like it has more marketing in this part, I can't decide if I should pay a higher price for @chaka (not sure the full diference with Ollin 1.1 form the others as well) or FOCBOX from @onloop, whitch one would make difference, or just buy from DIY. I would like to hear someone with experience in FOC mode and if it's worth it?  Just afraid to fry my VESCs playing with these. 

Man!!! prices escalated quickly when playing with these.... heheheh... but as @onloop explained, a DIY is not meant to be cheaper, but make what you want.... so..... by the way I wanna play with a bamboo deck..... I still have to figure it out how to put this together to have some flex.....  for sure I will need to split in both sides... 

So thank you guys, any help I would really apreciate. I would buy from US, I wanna order as soon as possible.
```

---
## \#2 Posted by: Deckoz Posted at: 2017-09-30T15:23:43.151Z Reads: 283

```
The 107 superflys are offset, they have the same mounting depth as 83mm flywheels.

I run 100mm MBS wheels with 15mm belts on 180mm trucks with the tb v4 mount

The 218s would be good for having extra width and a pulley bearing as the axles are 10mm longer. But yes it should fit
```

---
## \#3 Posted by: E-Boarding Posted at: 2017-09-30T16:04:39.783Z Reads: 274

```
If money is not a problem go for the FOCBOX, I like FOC because its much more quiet.

Going 20-30% hills with 107 SuperFlys requiere a high gearing ratio and/or low motor kv and I recommend 2x 15mm belts
```

---
## \#4 Posted by: onepunchboard Posted at: 2017-09-30T16:14:51.569Z Reads: 259

```
lipo will give u so much power. just set to 80amp each motor, u will have more power than u can pull trigger. I get burnout on full acc from flat ground cuz im light, 130lb
```

---
## \#5 Posted by: Fabar Posted at: 2017-09-30T16:35:58.284Z Reads: 249

```
Thanks @Deckoz!  Good to know that mouting depth is the same. Just read your posts, what a crap to have a burned vesc.... how is going with your FOCBOX?
```

---
## \#6 Posted by: Fabar Posted at: 2017-09-30T16:41:09.759Z Reads: 246

```
Thanks @E-Boarding, my concern about FOC is burning my VESC as some of here have experienced.  For the 218mm trucks, @sl33py could only fit 12mm belts .....  not sure if I there is a way with a 15mm... but let's see ....
```

---
## \#7 Posted by: NickTheDude Posted at: 2017-09-30T16:41:18.121Z Reads: 239

```
What kV are you going with for your motors? Both kV and gear ratio are a direct tradeoff between torque and speed. Lower kV gives more torque, higher more speed. The bigger the difference in teeth between your pullies, the higher the torque.

The thing that's gonna haul ur ass up a big hill is torque, play around with [this calculator](http://calc.esk8.it/) and figure out what top speed you're looking for. The lower the top speed the more torque you will have in general.

Also you might want to consider 15mm belts because as you raise your torque output you have a higher chance of belt slip.
```

---
## \#8 Posted by: thisguyhere Posted at: 2017-09-30T17:06:10.921Z Reads: 238

```
i'm rocking this exact same setup, except with 12s4p liion pack and 15mm belts / pulleys.

if your intention is to climb hills the bigass 107mm wheels are really not the best choice as whatever pulley you throw at it, you'll still be contending with the largest diameter urethane wheels which lowers the reduction ratio.  having said that, i have yet to have encountered a hill i couldn't go up at full speed.  surprisingly, power draw going uphill with the dual 6374 backed by 12s voltage isn't considerably more than on flats.  may be anecdotal, your results may vary.  the 107mm are by far the most comfortable urethane wheels i've tried though.  also, go for the highest gearing you can find.  i'm running 15 / 40t, 15mm pulleys.  i sourced them from Titoxd10001 but he's out of them now.  so...may be a challenge finding them now.

i'm running unsensored bldc since running 12s, also too many people blowing out their vescs on foc.  i've tried psychotiller's sensored foc setups though and they're incredible.  completely silent and way smoother.  so in the hands of someone more capable, foc would be an option.

anyway, if you want to climb hills, my recommendation is to stay below 100mm wheels, and find the highest gearing possible.  also 15mm width pulley / belts if possible.
```

---
## \#9 Posted by: Fabar Posted at: 2017-09-30T17:23:50.476Z Reads: 216

```
@NickTheDude for now I'm planning to get the TB motor 190KV, but I'm open to lower it if I can find something else that could fit dual 6374 on 218mm trucks, that are the larger setups that I found here. Thanks for the calculator I was playing with it, but sometimes is not easy to find every part to fit the setup. The 15mm belts I'm still not sure if will fit with 218mm trucks. 

@thisguyhere wow!!! thats great!!!! I did not think to use 12s because i read some have burned the VESC as well.... hehehe.. so I was trying to play on the safe side.  What trucks are you using??  218mm from TB?  sl33py had mount TB with 12mm and 6374, but no chance with 15mm pulley.
```

---
## \#10 Posted by: E-Boarding Posted at: 2017-09-30T17:41:40.767Z Reads: 220

```
I'm running dual 6355 190kv with 15mm belts and a gearing ratio of about 15t:46t with 100mm Wheels

I'm at the limit with that:
when I would switch to 6374 there is no space for 15mm belts
when I would change to 12mm belt, they would slip and break very often (because of the torque and high gearing ratio)
when I reduce gearing ratio I would lose torque would not be able to go 30%, maybe 20%

And this is with 100mm wheels, it is getting worse with 107mm

so your motor kv is too high and maybe you've to compromise between 6355/6374 and 12/15mm
are you sure about that 30% hill, have you measured the incline and how long is it?
```

---
## \#11 Posted by: thisguyhere Posted at: 2017-09-30T18:17:04.932Z Reads: 213

```
TB 218mm trucks.  these trucks will fit dual TB 6374 motors with 15mm pulleys, or other motors that have a squared off barrel.  probably not the sk3 since they have kind of a nipple coming off the ends.

since this pic was taken wheels were replaced with 107mm but it's the exact same setup you're going after:

https://www.electric-skateboard.builders/uploads/db1493/original/3X/3/6/3682f947c3a30125221a6255c7374274e0136b3d.jpg
```

---
## \#12 Posted by: Namasaki Posted at: 2017-09-30T19:01:22.756Z Reads: 199

```
I am running dual 6374s unsensored in BLDC mode.
Ollin 4.12 Vescs
Motor max 80a
Batt max 50a
15/40 gears
90mm flywheels
I'm 195 lbs and it easily rolls me up some pretty steep hills.

The 107 Electric Flywheels has a center set core making them difficult to use with wide belts.
The 107 Super Fly's(just came out recently) have an offset core and might work with 15mm belts, I can't say for sure.
Still the fact is that larger wheels will increase speed and decrease hill climbing ability. Then again, that might not be an issue because of your weight. The difference between 195 lbs and 140 lbs is huge.
```

---
## \#13 Posted by: Fabar Posted at: 2017-10-01T03:22:37.919Z Reads: 186

```
@E-Boarding thanks ... I have recheck and at least a hill nearby here is 18%.... but all of them are not long distance, most of than around 500m. 

@thisguyhere thanks for the pic... this setup is great!!! do you have one with 107mm? are you using 107 Electric Flywheels or 107 super fly´s   :) ... ok I will get from TB and also the trucks and motor mounts V4. Hope everything fits perfect....

@Namasaki  thanks your post help me a lot......have you tried FOC mode?  

hey guys, is It worth it to put more money on FOCBOX or OLLIN 1.1 vesc because of FOC mode?  I'm not sure, reading many reviews, if this mode is already safe.... or may burn my vescs...
```

---
## \#14 Posted by: Namasaki Posted at: 2017-10-01T03:34:51.698Z Reads: 177

```
I have not tried FOC.
```

---
## \#15 Posted by: BigBoyToys Posted at: 2017-10-01T03:42:45.695Z Reads: 182

```
100% worth it to go FOC. I'd rather blow up my vesc than go back to BLDC lol. That being said, I have 3 boards on FOC and FOC box's and haven't had any failures that I attribute to FOC on them other than some random failures on the early batch of FOC box's. No problems since swapping them out for replacements.
```

---
## \#16 Posted by: thisguyhere Posted at: 2017-10-01T06:24:54.334Z Reads: 174

```
[quote="Fabar, post:13, topic:34374"]
do you have one with 107mm?
[/quote]

<img src="/uploads/db1493/original/3X/b/1/b1dce1987ce130323997fbc5a4cca3908a0c07dd.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/6/f/6f6df4bc453d7a0a79edcc991efde675e8c8ac30.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/a/8/a878703289dc0236778ff6ca3d04268f3db177c9.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/c/b/cb1dbb36b708640535ce7c7c1ff5e9b315a60d5f.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/1/c/1cbca7fb66b68926533321477660940cb316feb7.jpg" width="690" height="388">
```

---
## \#17 Posted by: PatRocks Posted at: 2017-10-01T06:54:05.153Z Reads: 160

```
Sick build!!!
```

---
## \#18 Posted by: E-Boarding Posted at: 2017-10-01T06:57:06.664Z Reads: 164

```
I will never go back to BLDC-Mode, this noise makes my ear bleed
FOCBOX ftw

18% for a few hundreds is fine, you won't need crazy torque for that, 2x6355 should be fine I think
```

---
## \#19 Posted by: Fabar Posted at: 2017-10-01T07:16:47.735Z Reads: 158

```
@thisguyhere wow!!! that's a great setup!!! really clean ... and probably one of the most powerfull.   How much battery do you have in that box?  Lipo?  
just read your post "Ate shit today and loop keys" ... wow... that's good to know!  
I'm struggling to find the 107 wheels and mounts for that... where did you get those?
```

---
## \#20 Posted by: thisguyhere Posted at: 2017-10-01T07:37:18.990Z Reads: 160

```
12s4p using lg hg2 liion cells, so 48 of those. 

I had to call ChrisChaput on his cell, and have my friend who lives a miles away from abec11 hq go get them in person. 

the mounts are enertion, it's too late but I just completed a sale for enertion clone mounts just recently. sorry.
```

---
