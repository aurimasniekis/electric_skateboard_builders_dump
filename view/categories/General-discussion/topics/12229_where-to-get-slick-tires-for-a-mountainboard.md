# Where to get slick tires for a mountainboard?

### Replies: 27 Views: 3981

## \#1 Posted by: Okami Posted at: 2016-10-31T23:27:22.915Z Reads: 298

```
Hi there! Has anyone found a place where to order slick tires for a mountainboard, except those ''skike'' wheels?

I found such wheels: 

<img src="/uploads/db1493/original/3X/2/7/279db2bc51039ab6117d907d1aa906ee06f64d0d.jpg" width="667" height="500">

They seem to be about **6.25 in size** and **1 1/4 wide.**

---
Too bad the auction ended not in my favor.. though, I would love to know is it possible to get any replacements for these tires! ..

Not even sure how much inches they are.. Though, I would also need ''whole kit'', hubs included.. as the board which had these wheels got away from me :\
```

---
## \#2 Posted by: Ackmaniac Posted at: 2016-10-31T23:40:00.796Z Reads: 281

```
Could be that these are these tires.
https://www.semed.de/reifen-und-schlaeuche/reifen-grau-profil-c-179-7x1-3-4.html
```

---
## \#3 Posted by: Okami Posted at: 2016-10-31T23:53:26.364Z Reads: 285

```
the ones in the picture look waaay thicker.. I have not compared the numbers, but the tire should be 1 1/4 thick, I think (the one in picture I posted). My current ones measures 2.5 / 2.8 in wideness..

Im not sure which number is for thickness, for the ones you showed.. Though, the picture is wrong if the tire size is below 2.5 for wideness.

-----
Yours look a lot like these:

http://www.trampaboards.com/innova-inline-street-tyres--7-inch-tyre-p-12772.html

The second option is these:

https://www.atbshop.co.uk/mountainboard-accessories/mbs-roadie-tyre

----
Though - they are still not as thin as the ones I posted.. I really wonder where did the guy get such a board! And is it still possible to get such hubs/wheels.. at all..
```

---
## \#4 Posted by: Ackmaniac Posted at: 2016-11-01T00:02:44.275Z Reads: 262

```
on their website they have the same picture for different sizes. But i think you may find the tires with C-179 7 1 1/4 maxxis in google. At the moment i make my self some plans to build a Street/Offroad board. So no hardcore offrod. Just want to take my dog out in the woods on easy walking paths. So mainly they should perform well on the road. But i am conserned about the durability. So is there any good tyre which performs well on the road and lasts long?
```

---
## \#5 Posted by: Okami Posted at: 2016-11-01T00:04:30.049Z Reads: 248

```
Well, a good consideration should be made (in my opinion) for best tire type and wideness choice because it will affect how much wh per km your setup / system is going to consume.

My tires / setup consumes quite a lot.. so Im already looking at the possiblities to get smaller / slicker tires.. 

I wont be able to give you much info, all I know it is better to use 4ply tire instead of 2 ply, because of durability.

---

I think this is close to the tire you showed, just with better specs supplied in the page:

http://www.mobilitydirect.com/Foam-Filled-Tire-7x1-3-4-p/tq295040.htm
```

---
## \#6 Posted by: Ackmaniac Posted at: 2016-11-01T00:10:37.711Z Reads: 228

```
Do you have a specific number how much wh you need per km. With my 90mm ABEC 78a dual drive enertion R-spec 6355 i need around 10 - 11 wh per kilometer. With my single drive 90mm ABEC 75a SK3 6374 i need around  9-10 wh per km. But i would not say that the dual needs 10% more. I would say i drive the dual harder because it is so sick.
```

---
## \#7 Posted by: Okami Posted at: 2016-11-01T00:15:43.267Z Reads: 227

```
Some other peple already suggested that with mountainboard you get about 40% less range.. So if you got 10km, we would only get 6km.. or so..

I still have to take more precise measurements but last time I tried to calculate the wh per km, it was in 19-20wh per km (this was done by taking the distance driven and dividing it with Ah put back into the cells, so there might be quite a big deviation, for example, If I did not charge the batteries fully, or they were already a little bit empty before I started to measure the distance..)

----

I also took it for a ride yesterday (with working wattmeter).. riding 2km quite fast (average speed 23kph), It consumed about 1900mah. i dont remember the exact number but it was less than 2000mah.. So yeah, quite close to 20wh/km (actually ~23/24wh, when converted (24.6 assuming max voltage x 1.9ah)

So, for avg speed of ~15kph, consumtion is ~19wh/km, with average speed of 23kph  = ~24wh / km

The calculation might be a little bit off, as I said - I need to do more tests :slight_smile:
For now I do know it consumes about 10-20A when normally cruising (~10-15kph).. As I looked into the screen while riding and it showed such consumtion.
```

---
## \#8 Posted by: Ackmaniac Posted at: 2016-11-01T00:24:13.504Z Reads: 203

```
i guess the tyre pressure has a huge impact on the consumption.
```

---
## \#9 Posted by: Okami Posted at: 2016-11-01T00:26:14.299Z Reads: 211

```
Glad you mentioned it, Will have to take into consideration all of these factors when I document my energy consumtion for my build! 

Right now tires are not at maximum pressure.. should increase it, to see what effect it takes on the **wh consumtion..** Im also close to 90kg.. so someone with 70kg might also have better wh per km .
```

---
## \#10 Posted by: Ackmaniac Posted at: 2016-11-01T00:33:21.849Z Reads: 216

```
If you have a VESC it would be the best to start the board and ride a track with a specific speed. Maybe adjust the max speed to have the same speed for different tests to have a good value to compare it. And then don't switch off the board when you are finished. Instead connect the vesc to your laptop and read the wh draw and wh charged and the tacho ABS value. Then you can calculate 

km = tacho ABS / ((magnets / 2) * wheelPulley / motorPulley / (wheelsizeInMM * 3.14159265359d / 1000) * 60 / 3.6)

wh/km = (wh draw - wh charged) / km
```

---
## \#11 Posted by: Okami Posted at: 2016-11-01T00:36:01.053Z Reads: 201

```
Unfortunately, I dont have vesc right now (not on this setup).. 

Though, I do have Watt meter and also a smart charger which can tell how much ah it has put back into battery..

I do realize now that VESC is perhaps the ultimate/best Energy use analyzer, as it is possible to directly export all of the values to the pc!

Though, for now I will have to use the ''simple'' methods.. and just measure the distance driven, wh/ah consumed and also average speed from gps app.. 

---

Will probably use your calculation sometime in the future! Thanks for sharing it!
```

---
## \#12 Posted by: Okami Posted at: 2016-11-01T00:37:22.344Z Reads: 185

```
Will probably try to take different measurements at different speeds! Also have to increase the pressure of the tires, to see would it take serious effect on the wh consumed, too!
```

---
## \#13 Posted by: Ackmaniac Posted at: 2016-11-01T00:41:47.855Z Reads: 176

```
Would be very interesting to see the different value at different tyre pressures.
```

---
## \#14 Posted by: Okami Posted at: 2016-11-01T00:42:46.381Z Reads: 186

```
Yeah, that would put some extra effort, so will see If I can manage to take a few little tests before I add pressure to them.. Portable pump would be the best, I believe.. as all the fuel stations around my place does not have a good runaway / straight road to test the parameters in safe / steady environment.
```

---
## \#15 Posted by: trampa Posted at: 2016-11-02T22:02:02.602Z Reads: 175

```
These are the ones we could offer. Most people don't dare to inflate them to 65+ PSI. They roll like a dream, when inflated to that pressure. Tyre pressure makes all the difference! If you really clean your bearings and use speed cream + sack off the inner rubber seal, you will have a board rolling very efficient. Make sure your hubs can handle that pressure! Ours do.

http://www.trampaboards.com/innova-slickcut-street-tyre--high-pressure-street-tyre--8-inch-tyre-p-12771.html

http://www.trampaboards.com/innova-inline-street-tyres--7-inch-tyre-p-12772.html

http://www.trampaboards.com/innova-inline-street-tyres--8-inch-tyre-p-12202.html

Frank
```

---
## \#16 Posted by: Okami Posted at: 2016-11-02T22:48:43.571Z Reads: 160

```
Thanks for the great info! Can you tell how much 65 psi is in bars? Idont want to make the same mistake again - I already overinflated my wheels once and the hubs just did not hold the pressure of the inner tube.. walls started to show bend marks.. had especially bad it with one hub where the screw holders just broke off..

Dont ask me how i fixed this! :smiley:
```

---
## \#17 Posted by: Okami Posted at: 2016-11-02T22:49:49.011Z Reads: 155

```
[quote="trampa, post:15, topic:12229"]
and use speed cream
[/quote]

Could u tell.me more about it? Where do you apply it?
```

---
## \#18 Posted by: trampa Posted at: 2016-11-03T08:26:28.547Z Reads: 150

```
4,5 Bar = 65 PSI. Google it! Some questions can be answered by yourself, using search engines.
Speed cream is basically a thin teflon based lube.The rubber bearing shields can be removed, using a small screw driver to peal them off. Only the outer ones are really needed. Re-lube once a while. Pressure and lube make all the difference.
Your board will roll 200% better.

Frank
```

---
## \#19 Posted by: Maxid Posted at: 2016-11-03T08:32:03.984Z Reads: 146

```
[Let me google that for you ;)](http://lmgtfy.com/?q=65psi+in+bar)
```

---
## \#20 Posted by: trampa Posted at: 2016-11-03T08:38:56.932Z Reads: 156

```
Wich hubs did you use? Ours withstand that kind of pressure with ease. We even tried 125 PSi to test out the extreme. 
I thougt the hub will implode - the tire ripped apart though.

Frank
```

---
## \#21 Posted by: Okami Posted at: 2016-11-03T17:45:15.900Z Reads: 150

```
I had ''star hubs''. Can show a picture.

The are made for 9'' tires, so not to confuse with 8'' ones, which have a different shape..

Tires were rated for 50 PSI.

Sorry for the laziness, I was from phone, though I still dont know how to calculate these two measurements on my own in the head :D

<img src="/uploads/db1493/original/3X/e/9/e909b0a4740492edcca4ef2274d633b694c4526a.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/6/5/65ed6213c9aad626f0ca4a6a62e8e0c6fd8904fe.jpg" width="255" height="198"><img src="/uploads/db1493/original/3X/0/0/003f9a3bd8c79b6310c7cee6171293985e588931.jpg" width="502" height="500">
```

---
## \#22 Posted by: trampa Posted at: 2016-11-10T12:38:40.204Z Reads: 133

```
These hubs are a very very old design, still found on cheap boards. They look strong but are in fact the opposite.

Frank
```

---
## \#23 Posted by: Okami Posted at: 2016-11-10T12:44:31.405Z Reads: 133

```
Aluminium would be great. Though, I had them on when I got my board, plus, the tires were in great shape, by buying aluminium ones I would not be able to use the tires.. 

Agree that aluminium hubs are way to go.. bearings ''rattle'' in these plastic hubs, as they does not fit perfectly into the bearing hole / place. I think evolve riders actually experience something similar.. they call it ''rattle snake'' :D as that's the sound it makes in some cases.
```

---
## \#24 Posted by: trampa Posted at: 2016-11-17T11:56:56.516Z Reads: 123

```
Our Superstars have alloy spokes and a plastic rim. This has proven to be the best design. Top spec plastic is more flexible and will go back to shape after deformation. Alloy would need to be quite thick and would be heavy. 

Frank
```

---
## \#25 Posted by: mccloed Posted at: 2016-11-17T21:19:52.700Z Reads: 120

```
6" Aluminum hubs? http://psychotiller.com/product/6-billet-wheel-hubs
```

---
## \#26 Posted by: GhettoFab.rictation Posted at: 2017-11-14T17:46:51.730Z Reads: 93

```
Hey do you know which of your inner tubes are better for top speed?
```

---
## \#27 Posted by: trampa Posted at: 2017-11-14T18:03:58.426Z Reads: 91

```
They are all the same if it comes to speed. The thicker ones are less vulnerable to punctures.

Frank
```

---
