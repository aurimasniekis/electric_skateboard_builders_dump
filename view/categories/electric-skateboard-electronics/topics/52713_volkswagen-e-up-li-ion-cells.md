# Volkswagen E-Up! Li-Ion cells

### Replies: 51 Views: 2792

## \#1 Posted by: Nexo Posted at: 2018-04-18T23:01:04.743Z Reads: 362

```
hi there,

some time ago I was going through internet and looking for li-ion cells to make new battery for my EMTB

I was using lipos so far, but this is not a good source of power and I can clearly say that to EVERY PERSON that will try to use them to power high-drain builds: "this is crap".
They supposed to be 10C constant and 10Ah but reality was a bit different. Voltage sagging, puffing cells, unbalanced cells, etc.

I decided to go with li-ions and then I found THIS:
![liion|375x500](upload://5wZw9TGhvREmqOy4lq3JWdOKZpU.jpg)

Volkswagen's E-Up! electric car li-ion cells. 12 cells in a pack, configured as 6s2p, but that can be changed easily to 12s1p. 1 cell 3,7V, 25Ah, 5C constant, 10C peak, 147mm x 90mm x 25mm, +/-700grams each.
They are quite big, but that is not a problem with mountainboard.
![30739623_1571072239606820_5213870201744916480_n|690x388](upload://kXQVY60JF83YSls7DDM1RVEaUfB.jpg)

I got them loaded to 3,7V each and checked capacity. Here are the results when fully loaded:
![30740773_1572220192825358_3642022586428162048_n|690x388](upload://9S40AveyCFSVfbkx66mdKK1JP6o.jpg)

Now I need BMS, proper charger and a good weather to try it out :smiley:

What do you think about it? Did you try something like this before? Share your thoughts, suggestions, questions. :wink:
```

---
## \#2 Posted by: onepunchboard Posted at: 2018-04-18T23:17:08.459Z Reads: 347

```
so what is this chemistry? I suppose it is not the crystal cell, 
pretty good mha tho
```

---
## \#3 Posted by: Nexo Posted at: 2018-04-18T23:19:07.916Z Reads: 342

```
i found informations like this:

Lithium NMC.
```

---
## \#4 Posted by: Dyspro Posted at: 2018-04-18T23:26:51.717Z Reads: 337

```
So it's Lithium Ion with Manganese and Cobalt. Pretty solid transference.
```

---
## \#6 Posted by: onepunchboard Posted at: 2018-04-18T23:40:14.461Z Reads: 336

```
Sorry I read wrong chart but refer to here
http://batteryuniversity.com/learn/article/types_of_lithium_ion

it is Nikel Manganese Cobalt

it doen not seems to good for mtb cuz it's rated for 2c at max. 

for 2c 25ah u will get 100amp for 6s2p 50amp for 12s1p. which is okay I guess. 

but if it is indead 5c cells than u r golden. good luck
```

---
## \#7 Posted by: Dyspro Posted at: 2018-04-19T00:30:52.093Z Reads: 316

```
Yeah, having the nickel kind of neutralizes the fun.
```

---
## \#8 Posted by: Ackmaniac Posted at: 2018-04-19T00:35:47.782Z Reads: 307

```
They are heavy. With Samsung 30q cells you get roughly the same capacity (6P) with 270g instead of 700g.
```

---
## \#9 Posted by: squishy654 Posted at: 2018-04-19T01:35:47.043Z Reads: 294

```
Cost? 10 char
```

---
## \#10 Posted by: lock Posted at: 2018-04-19T01:48:00.202Z Reads: 292

```
Cool! 

I once came across a lithium-titanate battery pack in a similar form factor on eBay going cheap. Believe it was taken from a forklift or something. Discharge and **charge** rates were pretty awesome (like 150a charge!), but that was the only good thing about it. Energy density was low, the pack weighed 6kg, and the nominal voltage of each cell was 2.7v or thereabouts.
```

---
## \#11 Posted by: Nexo Posted at: 2018-04-19T01:50:09.460Z Reads: 285

```
Around 250$
```

---
## \#12 Posted by: onepunchboard Posted at: 2018-04-19T02:35:37.402Z Reads: 276

```
holly for the whole thing?
```

---
## \#13 Posted by: Der6FingerJo Posted at: 2018-04-19T06:32:33.067Z Reads: 268

```
[quote="Nexo, post:1, topic:52713"]
They supposed to be 10C constant and 10Ah but reality was a bit different. Voltage sagging, puffing cells, unbalanced cells, etc.
[/quote]

might be a bit off topic, but i assume you used the hobbyking multistar batteries because of the 10c. they really are crap and not at all 10C, more lik 2 to 3c. This is why nobody will recommend them to you. I know of some people that the 20-30C Zippys work fine and i'm personally using 12Ah 15C Graphene cells without any problems.
Maybe just a heads up for future lipo purchases.


On the other hand the VW cells look really awesome and i can't wait to see how they perform :D
```

---
## \#14 Posted by: telnoi Posted at: 2018-04-19T07:00:36.899Z Reads: 252

```
[quote="Nexo, post:1, topic:52713"]
I was using lipos so far, but this is not a good source of power and I can clearly say that to EVERY PERSON that will try to use them to power high-drain builds: “this is crap”.
[/quote]

Sorry to hear about your negative experience, but any lipo that is a true 30C or higher at 8000mah will blow away most Li-Ion setups when it comes to amp delivery (in my case 2S2P). The majority of amp hungry mountain boarders use Lipo.
```

---
## \#15 Posted by: Acido Posted at: 2018-04-19T07:48:37.020Z Reads: 237

```
25$ per cell
```

---
## \#16 Posted by: Nexo Posted at: 2018-04-19T08:15:29.702Z Reads: 235

```
@Acido, even cheaper actually, I paid 250$ for **12** cells :wink:

@Der6FingerJo @telnoi  I get your point guys, I used crappy lipos, so I got crappy results, but I think it is worth to try those VW's packs anyway. Then, maybe, I will be back to lipos, who knows :slight_smile:
```

---
## \#17 Posted by: Der6FingerJo Posted at: 2018-04-19T08:27:38.110Z Reads: 228

```
Yes of course, trying them will be great :D
```

---
## \#18 Posted by: Nexo Posted at: 2018-04-24T18:38:55.756Z Reads: 206

```
ok, I did a short test (weather in my city is horrible now)

I took my board for a ride, I did (according to google maps, forgot to switch on endomondo...) 17,5km = around 10miles.

+battery was loaded yesterday
+start-up voltage was 49,1V
+temperature outside 7 degrees Celsius, 44 Fahrenheit
+setup: EMTB, 2x6374 190Kv, 2xFOCBOX, motors set to 50A max, batt max 15A (just for safety, I am going to change it back to 65A and 25A)
+hills, hills and once again hills, some of them pretty steep (wheels were spinning)
+heavy and oversize load :smiley: board is around 20kg and mine "waaaaay over" 90kg

After that, when my face was frozen I came back home, battery voltage was **45,0V**.
![31224726_1577751188938925_428536460811960320_n|281x500](upload://lDdQQ6KPxXS1iL2tinbfF92axEt.jpg)
 I was completely shocked during that ride, voltage sagging during full acceleration was around 0,7 Volts! I am currently waiting for BT module so I will be able to upload some charts from BLDC app.

O checked each cell and they are balanced quite good: LV: 3,71V, HV: 3,75V.  << NO BMS so far

BEST. THING. EVER.

@Der6FingerJo I am in love with those VW cells :wink:
```

---
## \#19 Posted by: Der6FingerJo Posted at: 2018-04-24T19:10:04.037Z Reads: 185

```
That's great! :D And that is with a fairly high kv board too. 

A neighbour recently offered me one BMW i3 cell, but unfortunately he won't give me 10 of them to put in series :smile:
```

---
## \#20 Posted by: Acido Posted at: 2018-04-24T19:33:13.906Z Reads: 178

```
I wish i had the space for them....
```

---
## \#21 Posted by: Nexo Posted at: 2018-04-24T19:36:56.223Z Reads: 182

```
this board is ridiculously fast in that setup :stuck_out_tongue: ...or maybe it is just too fast for me, anyway, going over 40km/h on EMTB is a bit different than 40km/h on a longboard

@Der6FingerJo I found info that VW is actualy resigning their contracts with Sanyo for those 25Ah cells. They will use Samsung's 37Ah cells which are THE SAME SIZE THAT 25Ah...that means that maybe in a future I will be able to change my battery for even bigger without changing box :stuck_out_tongue:

@Acido yes, they are big, I thought that I will be able to use them in original enclosure, but no way...I designed a simple box that will make that 12s look like 2x6s lying on their side, that will make them a bit higher (which I dont care) but deifinitely less wide and it currently printing :slight_smile:
```

---
## \#22 Posted by: infiniti3d Posted at: 2018-07-27T09:19:50.085Z Reads: 163

```
Hey Nexo, great to see that you like these VW cells! I want to try them on a new project but cant find them nowere😞 Were did you get them from? Were the new or salvaged? Appreciate your help to get my hands on these, thank you...
```

---
## \#23 Posted by: offpist Posted at: 2018-12-09T08:56:06.732Z Reads: 136

```
Nice to see your enjoying the E-UP cells. (I believe i was the one to sell them to you)
I have lots more cells on stock so anyone located in Norway can contact me if you want cells like this. 

I now also have the Panasonic 37AH cells but, they are spot welded toghether at the terminals. That makes it more difficult to make an 1P battery, but i did make one 14S1P using an MIG welder.
```

---
## \#24 Posted by: Acido Posted at: 2018-12-09T09:01:34.048Z Reads: 132

```
What are the dimensions of panasonic cells?
```

---
## \#25 Posted by: offpist Posted at: 2018-12-09T09:15:02.502Z Reads: 133

```
14,7 cm x 9 cm x 2,5 cm
```

---
## \#26 Posted by: offpist Posted at: 2018-12-09T09:33:14.995Z Reads: 128

```
Here is an test i did, comparing the two cells.. remember, they are physically the size!

![E-golf|690x364](upload://rDuLl8URJo2RbnuodQZ0hZBAOIm.jpeg)
```

---
## \#27 Posted by: Acido Posted at: 2018-12-09T11:13:06.413Z Reads: 117

```
Nice, whats their condition?
I need a solution for a solar pack
Can you post some pics?
```

---
## \#28 Posted by: FredrikHems Posted at: 2018-12-09T11:15:01.816Z Reads: 114

```
I am in Norway :sweat_smile:
You have some more info and pics?
```

---
## \#29 Posted by: offpist Posted at: 2018-12-09T11:27:50.672Z Reads: 119

```
The car had only 5000 km on the meter when it crashed, so they are basicly like new condition.
Just to be clear, sending Lithium batteries over boarders are an nightmare as its considered dangerous goods. Needs to be packed and labeled accordingly, so i simply will not do it. 

I have sold to many Germans and they come here by car to pick up batteries.

For more info about the 37AH cells, check my add here:
https://www.finn.no/131343875
```

---
## \#30 Posted by: offpist Posted at: 2018-12-09T11:32:01.544Z Reads: 115

```
For small solar storage i recommenced 14S3P setup (48V, 5,7KWH).  If you need bigger i would look at Nissan Leaf cells. I once build an 14S10P setup for my house (arround 33KWH) using Leaf cells.
```

---
## \#31 Posted by: FredrikHems Posted at: 2018-12-09T11:36:14.920Z Reads: 111

```
Hva er pris per celle for 37ah panasonic versjonen? Hvis det var mulig å splitte de opp til enkelt celler. :blush:
```

---
## \#32 Posted by: offpist Posted at: 2018-12-09T11:40:00.391Z Reads: 107

```
I am only selling complete modules, and you get them in 12 cells 2500 kr/260 euro and 6 cells modules at 1250 kr/130 euro.  Cutting them up and selling cells one by one makes little sense.
```

---
## \#33 Posted by: FredrikHems Posted at: 2018-12-09T11:46:15.642Z Reads: 100

```
I see, do you know the C-rating of these? I cant see to find it myself.
```

---
## \#34 Posted by: Acido Posted at: 2018-12-09T11:57:22.999Z Reads: 102

```
Gls is the way to ship batteries
```

---
## \#35 Posted by: offpist Posted at: 2018-12-09T12:08:05.369Z Reads: 103

```
Hard to find the specs from Panasonic.
But i have customers that have tried up to 600Amps on one single cell.. 

Myself i have tried 4C continuous from full to empty and they did not get hot at all. 

I would not charge them more than 2C without temp monitoring and lowering current when about 90%SOC. Stay below 0,5C and your safe.
```

---
## \#36 Posted by: FredrikHems Posted at: 2018-12-09T12:27:36.258Z Reads: 106

```
[quote="offpist, post:35, topic:52713"]
specs from Panasonic.
[/quote]
Arent these from Samsung? :thinking:
```

---
## \#37 Posted by: Acido Posted at: 2018-12-09T12:29:45.571Z Reads: 99

```
I have just seen an article that VW changed their supplier from samsung to someone else i think panasoni
```

---
## \#38 Posted by: FredrikHems Posted at: 2018-12-09T12:34:08.430Z Reads: 100

```
I think it is opposite. They changed their supplier from Panasonic/Sanyo to Samsung.
```

---
## \#39 Posted by: offpist Posted at: 2018-12-09T12:42:57.050Z Reads: 99

```
Ah sorry. I sell both Panasonics (25AH) and Samsung (37AH).
```

---
## \#40 Posted by: FredrikHems Posted at: 2018-12-09T13:06:14.986Z Reads: 97

```
Okay. If I understood right, the Samsung (37ah) ones doesnt have screw terminals?
```

---
## \#41 Posted by: offpist Posted at: 2018-12-09T13:09:05.762Z Reads: 98

```
Correct. 
That makes the Panasonic cells much more easier for the DIY battery builder.

Then for an solar storage, you can build an 14S12P battery using 14 modules.
```

---
## \#42 Posted by: FredrikHems Posted at: 2018-12-09T14:13:13.179Z Reads: 92

```
Okay. So if you want to make a 12s1p battery with the 37Ah cells, you would need to cut the spotwelded strips and then solder the cells in the right orientation?
```

---
## \#43 Posted by: offpist Posted at: 2018-12-09T14:26:54.013Z Reads: 92

```
Correct, and its not an easy task, as the bus-bars are aluminium. If only they were copper. 
TIG or MIG welding is the way to to I guess.
```

---
## \#44 Posted by: FredrikHems Posted at: 2018-12-09T14:31:43.135Z Reads: 92

```
Damn it!, was hoping that the connections where copper. Aluminium is a pain to solder..
```

---
## \#45 Posted by: Acido Posted at: 2018-12-09T16:36:55.797Z Reads: 85

```
Even a bigger pain to weld...
```

---
## \#47 Posted by: taz Posted at: 2018-12-10T12:39:06.859Z Reads: 68

```
Not if you know what you are doing :wink:

![IMG_6266|375x500](upload://pvcWPofmdesTskMVDkdBJnsTyl6.jpeg)
```

---
## \#48 Posted by: Acido Posted at: 2018-12-10T13:49:53.308Z Reads: 63

```
Im okay at welding steel, tried to weld my cracked bike frame and had a really ugly time lol
nice work!
```

---
## \#49 Posted by: taz Posted at: 2018-12-10T13:51:47.628Z Reads: 66

```
Thanks. I am a welding engineer so if you need any tips I can give you some.
```

---
## \#50 Posted by: martijntje42 Posted at: 2018-12-10T13:53:34.421Z Reads: 62

```
you clearly don't!, alcohol free. it's Blasphemy.
```

---
## \#51 Posted by: taz Posted at: 2018-12-10T13:54:25.633Z Reads: 61

```
Why do you think I punished them by melting their butts off? :wink:
```

---
## \#52 Posted by: Acido Posted at: 2019-01-23T20:04:59.999Z Reads: 48

```
I need a new power source for my spot welder, do you maybe have an idea how much amps can they give?
Just realized they are 25ah 10c nvm
```

---
## \#53 Posted by: Tricohiba Posted at: 2020-02-15T12:16:09.831Z Reads: 8

```
Hi, i can also get Volkswagen battery modules and I was thinking to use them on My project. What kind of charger and bms you are using with them?
Br
Thomas
```

---
