# Skatey 800/fiik big dady/ superstar - Lead acid to LiPo conversion

### Replies: 90 Views: 4679

## \#1 Posted by: mountainboardlover69 Posted at: 2017-01-18T07:24:06.270Z Reads: 262

```
hi i have a skatey 800 i bougt it second hand 
but the lead accid batterys ar dead fist i wanted to put new in but i was like lipo is way better
but then i have a problem becous if the lead battery are empty they are 36v total and when they are full they are 45v
so that comes down to like a 10.8s battery so i wanted to get a 11s battery but that woud meen i need a 5s battery and those ar quid rare  so my question is is it better to use a 12 s or a 10 s ??????
```

---
## \#2 Posted by: Okami Posted at: 2017-01-18T19:17:46.234Z Reads: 239

```
Hard to tell. Depends on electronics and their limits. Might choose 10s for safety reasons.
```

---
## \#3 Posted by: mountainboardlover69 Posted at: 2017-01-19T07:38:00.783Z Reads: 232

```
wil that like 2v matter that much in speed ??
```

---
## \#4 Posted by: Okami Posted at: 2017-01-19T11:11:00.382Z Reads: 227

```
One of your options is something like this:

Buy 2x 6s Lipo's.

Leave one of them alone, but the second one, open up the pack, de-solder the wire/s from one of the terminals, then remove that cell from the pack.

Solder wires to the ''new'' last cell in that pack, which would be 5s now.

The hardest part would be to figure out how to charge this thing and how exactly do you need to wire the balance wires together.

----

Do you have lipo charger right now? Im asking because even with 11s pack, it looks like you get 46.2v. To make it ''totally standard' I would charge that 11s pack of lipos till only 4.1v per cell, then you would get 45.1v, you could charge them in Li-ion setting or just make a ''custom program for lipo'' to terminate charge at 4.1v.

--

This is a very labor intensive task, You might as well try to find 2x 4S batteries and 1x 2S battery, all in the same capacity range. You would get a really weird wiring and you would still need some soldering to make custom 3 battery connector but at least you would not need to take apart the lipo cell.

--

There is a thead about making lipo packs slimmer. Take a look there. Then you can judge will that be hard for you or not.

This is from theory, as I have not soldered / re-assembled lipo packs myself! But it should work, if you can make all the right connections!

---

Im sorry that I can not give you an insight about your skatey 800 circuit board limits. You might as well look at their lithium version (if they have one) and try to figure out whenever the electronics is the same..

Or - you could ask someone who is having the same board

Or - you could try to ask ''skatey company' itself, perhaps they are willing enough to help out

OR - you could try to look at the capacitors on the circuit (if there are any!) and try to figure out will they accept 49v instead of 45v (but I think this is not a reliable method at all!)
```

---
## \#5 Posted by: Okami Posted at: 2017-01-19T11:25:20.542Z Reads: 178

```
BTW - @mountainboardlover69 did you measure the highest voltage for your battery yourself?

I looked up how much volts per cell lead acid has.. It states that basically, 1.75v per cell is empty and 2.4-2.45 is full. Nominal is 2.0v. So to get 36v nominal, there are 18cells.

At 18cells - 2.40x18 =  43.2v 

http://batteryuniversity.com/learn/article/bu_214_summary_table_of_lead_based_batteries

So im not so sure anymore about 45v but if you got from somewhere that it is still safe, you might try with 11s and 4.1v charge, as I said earlier..

Otherwise.. 10S would definately be safer, if max voltage is actually 43.2v

You can try to ''feel'' what the max speed is when battery is half to empty.. that's what speed you would probably also get with Lipo's. 
lipo - (10x 3.6-4.2v = 36v-42v.) / 38 avg - / 37v nom
PB - 18x 1.75-2.4v = 31.5- 43.2v) -  ~37.6/38v average. / 36v nom
```

---
## \#6 Posted by: mountainboardlover69 Posted at: 2017-01-19T11:39:02.735Z Reads: 161

```
tnx for alll the ideas i have a 80w lipo charger and if the batterys are full my volt metter sais it is 44.5v
and the battery say there max volt is 15 v a piece soldering is not that hard for me  i lookt on the site and they sell a 36v 12ah lipo https://www.skatey.nl/skateboard/Skateboardp/skatey800/Skatey-800-Battery-Box-Complete-LITHIUM that one but i will never pay 800 euro for a 12ah 36v lipo  and here is the board that is in my board https://www.skatey.nl/skateboard/Skateboardp/skatey800/Skatey-800-Control-box-complete---microcomputer
i dont see a capacitors 
 i am gone give them a call today
```

---
## \#7 Posted by: Okami Posted at: 2017-01-19T14:25:40.253Z Reads: 165

```
You might wanna take a look at this:

http://www.electric-skateboard.builders/t/how-i-made-my-lipo-packs-slimmer/1415

http://www.electric-skateboard.builders/t/how-not-to-make-your-lipo-packs-slimmer-p/7216/6

Then decide do you want to remove one cell from the 6s pack to make it 5s..

---

Anyways, im not sure, but perhaps someone with more electronics knowledge could tell whenever you can over-volt the esc.. but generally it seems it does not work that great :slight_smile:
But to decide / see if it can take higher voltage, the ''components'' side should be seen.

In the picture you gave there are only circuit pathes no components on that side of the board..

--
So yeah, if you can, just stick to de-soldering one cell.. then you can cut balance connector a bit (so it fits 5s) port and stick in 5s port of that turnigy charger you got.. You will need to come up how to charge such battery.. so you either do 5s x 2 and later charge them in parallel, or you do 5s x 1 and 6s x 1 and then charge seperately..

Also would advise to get 10ah + size battery :)
```

---
## \#8 Posted by: mountainboardlover69 Posted at: 2017-01-19T14:38:33.776Z Reads: 128

```
i was planing on getting a 16ah so
```

---
## \#9 Posted by: Okami Posted at: 2017-01-19T14:48:27.411Z Reads: 123

```
That should be ok, for such board! I think 8-10ah is the minimum for emtb! :slight_smile:
Not sure how much energy your board eats.. but I can only do about 8-10km with my 8ah pack.. have not tried to go full distance so that is the max calculated one..

So you should be good for about 15km for sure :)

--
With 10s = 3.7x10 = 37v x 16 = 592 WH
592 WH / ~20wh (~15-20kph avg speed) = ~29 KM

Ok so Im not sure will you really get this much, but 15 - 20km should be really possible!
```

---
## \#10 Posted by: mountainboardlover69 Posted at: 2017-01-19T14:50:26.016Z Reads: 109

```
around per 3 ah 5 km
```

---
## \#11 Posted by: Okami Posted at: 2017-01-19T14:53:46.892Z Reads: 106

```
not sure about that.. depends on voltage, too (6s-12s..)

Forgot to mention - I have 6s, so only 24v

For energy you got to calculate WH

that is 24v X 8Ah = 192 WH, energy use per 1km = ~20 WH
192 / 20 = 9.6km

(usually WH is calculated from 3.6v (nominal) x 6 = 21.6v, but 24v is also ok for calculation)
```

---
## \#12 Posted by: mountainboardlover69 Posted at: 2017-01-19T14:55:12.984Z Reads: 101

```
i am just saing my battery hase 3 ah at this moment in i can max drive 5km wit it
```

---
## \#13 Posted by: mountainboardlover69 Posted at: 2017-01-19T14:57:38.205Z Reads: 101

```
i have a wat metter on my board i will look today 
i am in school now :sob:
```

---
## \#14 Posted by: Okami Posted at: 2017-01-19T14:59:03.109Z Reads: 101

```
Oh cool. ! Definately try to measure how much kilometers can you drive at what speed!

for me 1km  = (~0.9ah*21.6v) = ~19.5 Wh

You can check my previous post - I think you will be able to do even about 20km, since your voltage will be higher! I did calculation for 10s, 11s should be a bit more higher/bigger distance.
```

---
## \#15 Posted by: mountainboardlover69 Posted at: 2017-01-19T16:29:01.792Z Reads: 96

```
for me it is 23wh
```

---
## \#16 Posted by: mountainboardlover69 Posted at: 2017-01-19T16:36:35.311Z Reads: 102

```
there u go 
https://www.youtube.com/watch?v=NA7dj-_T6k0&feature=youtu.be 
sorry that there is no gopro film but my gopro in empty
but after 1.1  km it used 23wh and after 3.5 km 78wh
```

---
## \#17 Posted by: Okami Posted at: 2017-01-19T16:42:15.874Z Reads: 104

```
You should enable ''auto-pause'' function (if there is one) for your distance app! Otherwise you get incorrect average speed reading! 

Did you stop for a lot of time while riding? Im asking this, because at the end your avg speed was 13kph and consumtion is also based on speed!

----
Otherwise, 22-23wh seems reasonable, even with that ~15kmh average speed. Though I saw you rode over past 30kmh a couple of times.. :) that's quite speedy I think..at least for such emtb board

--

So from this you should be able to calculate the max range you should get!

Take your battery's voltage: 

10s = 37(lipo), 
11s=40.7(lipo) 

Then multiply (*) that by the size of the battery you intend to use, in your case: 16Ah (can take less, as perhaps not all capacity is gonna be used!)

So that brings us to:

 37v X 15AH = 555 WH + 37 WH (max in theory)
/  40.7V X 15Ah = 610.5 WH + 40.7 WH (max in theory)

10s / 15ah = 25km
11s / 15ah = 27.75km

--
If you go faster, you will probably be able to drive less kilometers
```

---
## \#18 Posted by: mountainboardlover69 Posted at: 2017-01-19T16:43:43.958Z Reads: 81

```
yes i know but there is non and i needet to srap my hole 6.4 inch phone to my board that aint easy
```

---
## \#19 Posted by: Okami Posted at: 2017-01-19T16:49:34.291Z Reads: 91

```
hah for sure..

so yes, go pro video would have been nice! Try to charge you camera before you go riding the next time! Video + App (distance) video would be nice 

+ can you tell / show what wattmeter do you have?

Did you install it by yourself ? or it was there already?
```

---
## \#20 Posted by: mountainboardlover69 Posted at: 2017-01-19T16:53:47.314Z Reads: 91

```
this one https://www.aliexpress.com/item/High-precision-RC-150A-Watt-Meter-Voltmeter-Power-Analyzer-Backlight-LCD-0-60V/32587810626.html?spm=2114.13010608.0.0.fT1Mvw
and u put it in my self
```

---
## \#21 Posted by: Okami Posted at: 2017-01-19T16:55:37.184Z Reads: 81

```
Nice! I have the same exact one on mine!

I watched your other video.. it looks like it is hard to start riding on this board? or the video was a lot older so it is not a problem anymore?

It looks like you could use some kind of ''bindings'' / foot straps for your board.. I saw you jumped off of it a few times.. with bindings it is easier to stay on balance while on the board.. at least for me it is a lot better to ride with feet straps!

Besides - do you plan to do a trampa version? I saw you looking for trampa deck..

-- One more note -- 

Haven't you considering installing vesc or any other esk8 esc into the board?

I think the board itself could be quite a good ''platform / base'' to use with other sorts of electronics!.. Of course you would probably need to get a different transmitter/remote control but at least you would lose that ''frequency noise'' which can be heard when you accelerate the board! Actually I think we are lucky (other esk8 builders) that we get to use brushless motors and some quality esc's! Otherwise our rides would be a lot noisier! 

My board also does give out a sound.. but it is a lot more subtle and I think it comes more from the motor than from the esc..
```

---
## \#22 Posted by: mountainboardlover69 Posted at: 2017-01-19T18:58:13.853Z Reads: 80

```
ug where to begin 
so i got this board cheap like 225 euro whel it is wat some call cheap for my it is a lot of money 
the steering was okay until i made my first crash the truck now steer weird if i trie to turn to the right
i can only make very big turns  and whell i just only make left turns  as u can see on my last video 
i contacted the makers of this board but they sold out of the front trucks because the new model's do not  have these truck's so  it kinda suck's and i can't rly find a other one the wheels are 10 inch an most truck's are for 8"

about that vEsc i dont rly se wy to upgrade and can vesc control motors wit a brush i them ?

about that trampa
whel it more a dream then a ting i am gone buy
i just dont have the money i get 180 euro a year  and a trampa  wil be like 1500 euro so that wil take 9 years :unamused: but soon i wil be abbel to work in a supermark or somting and i can make 20 euro a week 
20 x 52 = 1040 euro a year :grinning: so in about 2 years i wil have one super nice 

i dont rly care about that noise
and the board it self is shit a smal crash wil bend the truck totally 
so il just use this board until i have the money to get a new one 


btw my dad dose not like the idea of the bindings he thinks it is very un safe
```

---
## \#23 Posted by: mountainboardlover69 Posted at: 2017-01-19T19:14:33.412Z Reads: 74

```
ow and btw i dont know wy but i dont like the vesc i prefer the robben roxxy 100a idk wy
```

---
## \#24 Posted by: Okami Posted at: 2017-01-19T19:21:02.586Z Reads: 75

```
roxxy is also ok! 

You can try to make ''open style bindings'', like the ''freeboard'' has:

<img src="/uploads/db1493/original/3X/5/a/5ae1a45d5a23f3fc6d0a287ac7f6b19c2accc8bc.jpg" width="272" height="149">

So - for how much and from where did you get your batteries?
```

---
## \#25 Posted by: mountainboardlover69 Posted at: 2017-01-19T19:29:03.834Z Reads: 75

```
i dont have the lipo battery jet but i am planig on geting 2 of these https://hobbyking.com/en_us/multistar-high-capacity-6s-16000mah-multi-rotor-lipo-pack.html if the board can handel that
```

---
## \#26 Posted by: Okami Posted at: 2017-01-19T19:31:38.281Z Reads: 75

```
Be sure to buy the correct connectors also!

Balance harness

Parallel charging harness (xt60)
```

---
## \#27 Posted by: mountainboardlover69 Posted at: 2017-01-19T19:47:28.519Z Reads: 79

```
just mad some  bidding or a porto type 
<img src="/uploads/db1493/original/3X/e/5/e587c12971a852d31eb407f45d39136f6cfc83bc.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/b/4/b4cf0ab1de21c454c8119b72135f328f6520bb70.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/0/9/092e268818573222f3713e7b3d186546c1db22be.jpg" width="281" height="500">
```

---
## \#28 Posted by: Okami Posted at: 2017-01-19T20:02:20.061Z Reads: 78

```
hah, you are quite crafty / handy / practical!

Well, just make sure it is easy to step out of these!

So far I have only fallen like 1-2times.. without anything serious.. it was only because I tried to cross train tracks at a very slow speed! It is better not to ''chicken out'' and just have some speed when going over an obstacle.. 

--

I have bindings like theese:

<img src="/uploads/db1493/original/3X/5/7/571df2df0bdc0ef5dde8e9d8ca2bc3a37a0296f2.jpg" width="513" height="329">

If they are too too tight it wont be good for your feet also! They need to be a bit loose (at least I prefer them this way)

I have no problem getting my back foot out of them and stop with my foot, if I need to!

Not sure what happens if you tottally stop with your board at speed.. but it might depend on the situation!
```

---
## \#29 Posted by: mountainboardlover69 Posted at: 2017-01-19T20:23:31.051Z Reads: 79

```
i have lik fallen 3 times is because of speed wobble if u know wat that means 

btw just installed them
 <img src="/uploads/db1493/original/3X/c/2/c2973bf3a83f9a5e0e1978b3c3a86ef638f43248.jpg" width="281" height="500">
but me wit my dum ass installed them on the rong side (smart ass):smirk:
installed them to good way 
<img src="/uploads/db1493/original/3X/e/0/e0e88ba7d031132bda43a9aa84da4084bf68f1f7.jpg" width="281" height="500">
and holly sh*t the steering problem is no problem  any more 
gone make the other one tomorrow 
tnx man
```

---
## \#30 Posted by: Okami Posted at: 2017-01-19T20:32:18.154Z Reads: 76

```
hah im glad it solved your steering problem!

Be careful with speed wobbles! I've got only a small ones but I managed them because the speed was not very great and also because I was stable on the board! Without stability on the board it is hard to control it.

A lot of ''mountainboards''  dont have ''concave'' - ''river'' shape and they dont ''lock in'' the feet enough! Longboard decks are better in this manner, that the feet is more stable/in more control of the board, even without bindings!

Glad you fixed your strap! Otherwise you did mount it on the wrong size the first time haha! Now it should be easier to stay on the board!

Actually I think you made a good design! It seems that for ''left'' turn, you will lean / steer with your front fingers, then for the right turn you will be able to ''lean'' forward and hold yourself up with angle of your leg!

Dont worry if you dont understand my explanation! You can leave it out, I just tried to explain why I think your ''binding'' has a great shape/design and how will it improve your steering / turn making!
```

---
## \#31 Posted by: mountainboardlover69 Posted at: 2017-01-20T07:33:15.879Z Reads: 66

```
well wit my board there are non but when i go over a speed bump 
its like rly big speed wobble
```

---
## \#32 Posted by: Okami Posted at: 2017-01-20T18:03:02.370Z Reads: 66

```
I actually fell today (pictures later).. I fell because theere was not enough speed and I hit an ugly ice block.. almost fell into the canal lol :D I think if my board did not have any bindings and I would have jumped off there was a possibility for the board to go into water :confused:

Im glad it did not happen.. board just fliped around and I landed on my knee and on my palms..right palm is the worst one.. the rest is only a scratch..
```

---
## \#33 Posted by: mountainboardlover69 Posted at: 2017-01-20T20:45:01.587Z Reads: 69

```
just made my second binding <img src="/uploads/db1493/original/3X/e/4/e4460d14370de33a686b5663c399c753911e1399.jpg" width="281" height="500">
but this weekend my mom is gone help me to make so proper velcro bindings like yours
```

---
## \#34 Posted by: Okami Posted at: 2017-01-20T20:47:46.317Z Reads: 67

```
These also look good - I hope they are stiff enough!

When u make your velcro ones try to make them in a way that you can adjust.them.

Different boots / shoes will need different tension.
```

---
## \#35 Posted by: mountainboardlover69 Posted at: 2017-01-20T20:48:32.913Z Reads: 64

```
the new one not rly so that is why i am working on the velcro ones
```

---
## \#36 Posted by: Okami Posted at: 2017-01-20T20:51:02.272Z Reads: 63

```
Was the old one(in picture) just some thick wire with insulation (plastic around it)?
```

---
## \#37 Posted by: mountainboardlover69 Posted at: 2017-01-20T23:10:55.794Z Reads: 60

```
Nope haha it was bend PVC
```

---
## \#38 Posted by: mountainboardlover69 Posted at: 2017-01-20T23:13:58.280Z Reads: 72

```
So I am done making the new bindings 
Did not put them on the board yet
<img src="/uploads/db1493/original/3X/9/5/955b97cb8daa73885db3ee08f13a40ef987d9c90.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/9/0/90f1d6730712a2ca4d9e607249656e4c39c1b227.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/4/7/47902e1ae69874960f0b034822dc85c9df82acd7.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/d/6/d6e8c0a856e28ae039b7e18338318ea7ede46d7e.jpg" width="690" height="388">
```

---
## \#39 Posted by: Okami Posted at: 2017-01-20T23:29:02.005Z Reads: 71

```
Looks like you will have a tight (strong) fit around your foot!

Just try it out a few times and try not stop completely!.. Actually I think the best is to have the front foot available.. and only use ''belt'' / velcro un your back foot!

Take a look at this binding:


<img src="/uploads/db1493/original/3X/6/b/6ba897dd9fcba264a452768b452e435a7009e5cc.jpg" width="690" height="261">

Im not sure what happens when you fall with such board.. but it might be easier to get your foot out.. just watch out for big rocks or big potholes / gaps in the road when you ride and you should be safe!
```

---
## \#40 Posted by: mountainboardlover69 Posted at: 2017-01-21T12:21:25.879Z Reads: 70

```
https://www.youtube.com/watch?v=ur5BAwnjWBI&feature=youtu.be
new binding are noice
```

---
## \#41 Posted by: mountainboardlover69 Posted at: 2017-01-22T10:59:02.180Z Reads: 70

```
Speed wobble
 <img src="/uploads/db1493/original/3X/8/a/8ade2b70035f0f43dd9cbf41938e6c720dedc003.jpg" width="281" height="500">
1 night in the hospital
```

---
## \#42 Posted by: Okami Posted at: 2017-01-22T11:13:21.173Z Reads: 70

```
why did you fall? Were you going over a speedbump again?

I hope this is not because you made these velcro bindings.. as I said iti s better ot keep the ''front'' foot open - free, and only strap in the back foot..

--

Also - look how ''loose'' / open is your steering! You should try to make it stiffer.. = less chance of speed wobble also..There is a nut near these bushings, try to make it tighter!

-> 
<img src="/uploads/db1493/original/3X/9/4/94674ad0e4191e0d0543ab6334359425ec1d3c7f.jpg" width="690" height="492">

(on the left side - the nut)

I hope your mom will still let you ride after this one..
```

---
## \#43 Posted by: mountainboardlover69 Posted at: 2017-01-22T11:54:15.446Z Reads: 66

```
It was speed wobble I want to tell how but I don't know my mom Isn't mad  and nope it was not because of the bindings
```

---
## \#44 Posted by: Okami Posted at: 2017-01-22T13:46:46.153Z Reads: 66

```
Try to make your trucks / bushings more tight! I believe they are 'wobbly''. Is it easy to move / steer the board around while you are just standing and not riding it?
```

---
## \#45 Posted by: mountainboardlover69 Posted at: 2017-01-23T20:41:09.320Z Reads: 61

```
can test if it works i am still a zombie
```

---
## \#46 Posted by: mountainboardlover69 Posted at: 2017-02-01T08:59:02.656Z Reads: 60

```
batteries came in today :grinning:
```

---
## \#47 Posted by: Okami Posted at: 2017-02-01T22:15:29.321Z Reads: 68

```
Cool.. btw - if you can - change the topic's name.. change it to something like ''Skatey 800 - Lead acid to LiPo conversion''

Will be easier to later be found by others.. and just to understand better the topic in general..

---

Click on the icon.. right next to the topic..it should be like a ''pen'' / pencil icon.. scroll till the top of the page to be able to see it..

--

Hope your injuries have come better! I got my hand scratched the other day! .. part of the reason - too tight front bindings! Try to make it loose enough so you can pull out your foot if you need to jump off the board.. otherwise - the board will roll over.. along with you, if you fall / trip on an object.

PS - should have worn gloves.. didnt have any..

 **Wear gloves, if you ride with bindings! Will save your skin! Helmet also comes handy,** 

especially, if you fall on your face/ head when you fall!

 Just be careful.. these things are dangerous, if you dont watch where you are riding / or what you are going over! .. 

I hit an ice (reason I fell).. shouldnt have tried to ride over it in the first place :D
```

---
## \#48 Posted by: mountainboardlover69 Posted at: 2017-02-02T09:28:18.700Z Reads: 69

```
je i do always where gloves 
and a helmet (wel 1 time i tink i didn't but i can remember :) )

my wounds are mostly gone 
but i still can skate my doctor say in about one week i can try again :triumph:

so i have to leave my new batteries on the shelf

btw i stopt charing my batteries when thay are 4v per sell that means i have a total of 48 volts and 3 volt's wont let any ting explode i tink so   (and i hope so)
and i dont rly want to de solder a sell i mean the board is wit out a battery second han for around 170 euro and the battery is out of sale 145 euro so i tink the risk is smaller to do it at 4v instead of desoldering a cell so i am gone go this rout
```

---
## \#49 Posted by: Okami Posted at: 2017-02-02T10:35:46.116Z Reads: 65

```
Could you post a picture of what battery did you get ? How much Ah / capacity / discharge?
```

---
## \#50 Posted by: mountainboardlover69 Posted at: 2017-02-03T12:43:06.596Z Reads: 61

```
https://hobbyking.com/en_us/multistar-high-capacity-6s-16000mah-multi-rotor-lipo-pack.html
that one 2x in series
```

---
## \#51 Posted by: jga Posted at: 2017-02-03T13:08:04.448Z Reads: 62

```
I don't know how you manage to fall off that board! i have the same and never came even close to that. I have no bindings and would certainly not recommend them, at least you can jump off the board in case of problem  Your max speed must be around 30-32Km/h, so it is still manageable. As said by Okami try to tighten the two bolts on the trucks. Mine is quite stiff and the problem is more to turn in tight corners than the wobbling.

By the looks of things you seem to be willing to just exchange the batteries without touching the electronics. I am very interested as I am in the process of doing the same (lead-acid to Li-ion), but I thought I would have to change the ESC as well. See my other posts on the subject where you may find some information.
```

---
## \#52 Posted by: jga Posted at: 2017-02-03T13:14:37.479Z Reads: 60

```
http://www.electric-skateboard.builders/t/at-skate-conversion-from-lead-acid-to-li-ion-project/14777
```

---
## \#53 Posted by: mountainboardlover69 Posted at: 2017-02-04T10:31:08.958Z Reads: 61

```
about that esc as far as i know brusles ecs can take any battery aslong as it is about the volt thay like
but be carefull because driveing ur lipos under 3.3v per cell can harm u lipos but wit lead acid batterys u can drive them down totally 

if i was u i soud wait un til i have completely tested my board so u dont have to break a board :P if any ting bad happens
```

---
## \#54 Posted by: mountainboardlover69 Posted at: 2017-02-04T10:38:11.070Z Reads: 67

```
just done making the hole battery pack :P
<img src="/uploads/db1493/original/3X/3/e/3e9f71457401033f5d70bc2931380343c54007f3.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/1/a/1a7f22629fe4b9bb29f5b1faa46766ad2da56ac1.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/5/e/5e394cc9dcbda5a928ee5f4f22066e8ccbe2faa5.jpg" width="690" height="388">
```

---
## \#55 Posted by: Okami Posted at: 2017-02-04T20:59:11.517Z Reads: 61

```
Cool! You actually look quite smart for your age!

What is that other thing on the voltage display?

Here->

<img src="/uploads/db1493/original/3X/f/7/f7e2cf64e72e6e6839aab9679b12dcf0d90bc8d3.jpg" width="241" height="237">

---

Also - what charger do you have? How powerful is it?

--

Report (tell) later - whenever it works or not with the new batteries! 3V might still make a difference but let's see, once you attach it to the esc!


---

One thing about turning - do you have these things called ''risers'' for your board?


These are plastic thing/rectangular shape/ which are mounted between the deck (board) and the trucks/wheel axle..

If you have them.. you could try installing one with an angle! It is called a ''wedge''.. it helps eiter with turning or for stability! In your case - stability is the one you should go for, when you install them!

They look like these:

<img src="/uploads/db1493/original/3X/9/9/99e59038dd8fbe171e83e559d5354011d9f7b851.jpg" width="302" height="500">

I changed the ''position'' of the wedge and it made a big difference in how responsive ( turny) the board is.. Ive got no problems turning a bit sharper now!

--

Check this:

http://www.electric-skateboard.builders/t/swing-arm-steering-mechanism-for-the-regular-trucks-how-and-would-it-work/16876/10

<img src="/uploads/db1493/original/3X/7/0/709631677087b41526a915cb9fe26912bcae0231.jpg" width="250" height="361">
```

---
## \#56 Posted by: mountainboardlover69 Posted at: 2017-02-05T14:44:44.082Z Reads: 61

```
The weird ting on my volt meter is just because of the suterspeed  u don't see that in real live

A bout. That angled wedge  my truck are mounted berry weird 
<img src="/uploads/db1493/original/3X/f/9/f9e11a9f13cb13052c75a942aeb9567f2e98058d.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/5/4/54376bdaa6ce967d3f71306efe792609a96c93f7.jpg" width="690" height="388">
As u can see . And the trucks are the opesit way as the wedge the are bend the other way so
```

---
## \#57 Posted by: Okami Posted at: 2017-02-05T16:17:27.364Z Reads: 60

```
It's hard to see but now we know that u got spring trucks..

Yes mounting is a bit weird, hard to say will it be possible to insert a wedge there, unless you make one yourself.

---

Understood about voltage. I assume each volt meter shows voltage for one battery pack. ~24v each

---

You got some really grippy tires! No wonder u get such wh consumtion 

Probably performs really good on offroad roads! :)
```

---
## \#58 Posted by: mountainboardlover69 Posted at: 2017-02-05T17:28:31.342Z Reads: 62

```
 About the tires they are asome but a bit soft on the road if u want to rly take of u will make quit a big black mark :yum: 

And about mum charger here is a pic<img src="/uploads/db1493/original/3X/3/6/3665e54d9bf732c222ceb82c3ca55828f2c15c86.jpg" width="281" height="500"> 
They where 22.5v when they came  but me with my dump ass change them  and now  unloading them to get them to storage charge  witch takes 3 day ffs   I am planing on buying a new charger thinking about the ichager duo  or the reactor 2x300w
```

---
## \#59 Posted by: Okami Posted at: 2017-02-05T18:32:11.642Z Reads: 58

```
What happened with the charger? Why you set it to storage mode? U could have just canceled it I think..
```

---
## \#60 Posted by: mountainboardlover69 Posted at: 2017-02-05T19:42:34.682Z Reads: 60

```
No I was like ow my battery's are here let's change them 
Full and then when they were full I was o wait I aint gone use them in like to weeks and my charger can only charger to storage charge and not discharge to storage charge idk wy 
<img src="/uploads/db1493/original/3X/d/a/dac1cefd487cb16a8643c7fd10b4c1bdb04e9993.jpg" width="690" height="388">:heart_eyes:
More battery's  I got 6 now
```

---
## \#61 Posted by: Okami Posted at: 2017-02-05T19:57:56.043Z Reads: 57

```
Ok, got your point now!

uh 4 of them is sure a lot.. I think you can fit only 2 of them on the board right?
```

---
## \#62 Posted by: mountainboardlover69 Posted at: 2017-02-06T00:00:39.620Z Reads: 51

```
6 lol I know they are not my ones (2 of them are)  the are from a friend of my he has the same board as I have.
But he doesn't know shit about volts and amps so he asked me to do it for him witch I did
```

---
## \#63 Posted by: jga Posted at: 2017-02-06T14:18:38.551Z Reads: 54

```
I had a look at the ESC this week-end and it is quite complicated to have access without dismantling everything, so I think I will just connect the battery when I get it and see how it goes. It's not a LIPO it's a Li-ion 10S4P with BMS and anti-spark. So the voltage is the same as my lead-acid.
I have also changed the tires. i had the same as you and i bought more road-type tires, although they are still quite big (8" but very wide). I am sure you could fit MTB wheels on these trucks, but then you would have to re-think the pulley arrangement as it is a very specific system with a three bolts holder.
The whole thing seems of pretty good quality, but the parts are heavy.
```

---
## \#64 Posted by: Okami Posted at: 2017-02-06T22:29:39.272Z Reads: 59

```
<img src="/uploads/db1493/original/3X/c/2/c22a4b7c920b0fe86bf6ae31c2a2278c744621d7.jpg" width="689" height="322">

Either change the springs (tightness) or the - angle / wedge, For maximum stability, I believe the ''truck angle'' should be maximum parallel to ground.. Not like this:

 **|   /**

But like this:

**| ----**    

---

Also, did you fall when riding normally or when pressing the ''gas''?

I got extreme wobble today when I sqeezed the trigger waay much.. some ppl call this ''gunning''.. either way after the acceleration, if you let go of the trigger, the board starts to slow down rapidly and this causes the wobble.. at least it did in my case ;)
```

---
## \#65 Posted by: mountainboardlover69 Posted at: 2017-02-07T08:49:08.820Z Reads: 53

```
woud like to tel u bit i dont know any ting of the crash 
but that is normal for a severe concussion woud like to tel u tho
```

---
## \#66 Posted by: jga Posted at: 2017-02-07T09:39:19.934Z Reads: 50

```
That's the new tires I bought also.
What batteries do you have inside?

I am struggling to put the belt back on the wheel pulley. The access is not easy with the protecting plate
```

---
## \#67 Posted by: Okami Posted at: 2017-02-07T09:47:28.639Z Reads: 51

```
@jga Sorry it is from ebay. If it helps it's called eight balls or similar.
```

---
## \#68 Posted by: jga Posted at: 2017-02-07T10:02:44.866Z Reads: 53

```
Yes, I had recognized the Eight Ball deck :wink:
```

---
## \#69 Posted by: mountainboardlover69 Posted at: 2017-02-10T15:32:39.137Z Reads: 55

```
just order some safety gear 
<img src="/uploads/db1493/original/3X/4/8/48343d3714201ab6704c4ef5141dda262e749d3b.png" width="652" height="500">
```

---
## \#70 Posted by: Okami Posted at: 2017-02-20T10:26:49.743Z Reads: 51

```
@mountainboardlover69 Hey hi!

Did you have to pay Tax / customs when you received your batteries? Im planning to perhaps get something similar.. but I dont want to pay the EU customs tax :\ since they are only available from china (global) hobbyking site.. - the 6s 10ah multistar lipo
```

---
## \#71 Posted by: mountainboardlover69 Posted at: 2017-02-22T20:57:02.133Z Reads: 48

```
No i Dident have any taxes 👌
```

---
## \#72 Posted by: Okami Posted at: 2017-02-22T23:07:34.640Z Reads: 46

```
Did u get them from eu warehouse?

They dont sell these anymore for eu..
```

---
## \#73 Posted by: mountainboardlover69 Posted at: 2017-02-23T06:41:29.137Z Reads: 42

```
Nope got the from Hongkong
```

---
## \#74 Posted by: Okami Posted at: 2017-02-23T08:42:41.115Z Reads: 43

```
I assume they ship to NL from Hong Kong but not other countries then :/
```

---
## \#75 Posted by: mountainboardlover69 Posted at: 2017-02-27T09:07:38.131Z Reads: 40

```
idk btw my friend got did got inporttaxes
```

---
## \#76 Posted by: Okami Posted at: 2017-02-27T09:08:49.343Z Reads: 44

```
But u didnt right? I assume u was lucky then :) what's the distance with.new batteries? Have u tested?
```

---
## \#77 Posted by: mountainboardlover69 Posted at: 2017-02-27T09:10:32.216Z Reads: 43

```
je i dint got any taxes :joy: wel my friend never pay for the taxes thow i dont know how but he told me he didnt pay for the tax  4 monts later stil no bil for him idk how
```

---
## \#78 Posted by: TMID Posted at: 2017-12-04T13:39:22.741Z Reads: 34

```
Hey,

thanks for the information in the topic!
I have 2 skatey's the same one u have. The range is decent of the lead acid battery's but I want to have a better range. 
So after reading this topic I wondered what the range is of your board (with the lipo's)?
Also are the lipo battery's working better than the lead acid ones?
```

---
## \#79 Posted by: mountainboardlover69 Posted at: 2018-02-01T15:14:32.584Z Reads: 34

```
hey man sry i am a bit late but whit a 16ah battery around 1,5 hr drive time at nearly full speed for 90 % of the time , btw if ur still looking for some lipo batterys and ur close 2 the netherlands i can hook u op , i make custom batterys , hit me up if ur intrested
```

---
## \#80 Posted by: TMID Posted at: 2018-02-02T10:31:16.212Z Reads: 33

```
Hey I also live in the netherlands (Zeeland), and I am still looking for some lipo battery's for my skatey!
```

---
## \#81 Posted by: Leolivinlife Posted at: 2020-02-03T02:05:21.622Z Reads: 16

```
Sweet build dude !  @mountainboardlover69  How's the board running after all this time. I'm debating lithium ion vs lithium polymer. I'm leaning towards lithium ion because of the ease of charging and built in BMS.
```

---
## \#82 Posted by: Leolivinlife Posted at: 2020-02-03T02:08:54.465Z Reads: 17

```
I fell off my 1600w Mototec mountain board at about 20 mph onto concrete once. Hit both my knees and my right wrist. I was off the board for like 6 weeks while I recovered after that. Fortunately I had a thin jacket on and jeans so I didn't bleed to much but I 1000% agree with getting some safety gear. I wore a full face helmet, knee pads, and gloves after that. Got made fun of alot but I don't care lol
```

---
## \#83 Posted by: mountainboardlover69 Posted at: 2020-02-04T14:50:03.908Z Reads: 16

```
[quote="Leolivinlife, post:82, topic:16254"]
ototec mountain board at about 20 mph onto concrete once. Hit both my knees and my right wrist. I was off the board for like 6 weeks while I recovered after that. Fortunately I had a thin jacket on and jeans so I didn’t bleed to much but I 10
[/quote]

hey man i sold the board a year or 2 back, i would higly recomend the swap, well wort it, if u got the tools to build a 18650 pack go for it charging with a bms saves so mutch hassel :stuck_out_tongue:  and u can fit way more batterys in the box
```

---
## \#84 Posted by: Leolivinlife Posted at: 2020-02-04T16:26:27.790Z Reads: 15

```
@mountainboardlover69 thank you so much I really appreciate the feedback. I already took out 12 volt batteries to get a feeling for how like the board would be without them and I'm definitely excited. I think I'm going to end up buying a 10S4P Lithium-Ion from PitbullelectricSkateboards.com cause I can't find another seller that makes a pack that size for the same or less price. Do you think I can make my own pack for less and still be as reliable? 
![Screenshot_20200204-112418__01|281x500](upload://14wPLZDFdKlYsITjvbIF3FK5vdA.jpeg) 

Also, what range did you get out of it with that pack that you put in?
```

---
## \#85 Posted by: mountainboardlover69 Posted at: 2020-02-05T09:47:16.754Z Reads: 14

```
u wil draw about 25wh-30wh per km, but the pack in the pick can only discharge 40A my board could easly draw 70A so if i was you i woudent go for this battery
```

---
## \#86 Posted by: Leolivinlife Posted at: 2020-02-05T11:52:15.009Z Reads: 14

```
:exploding_head: Wow I'm so glad that I didn't get that one. This one is rated for an 800w motor. I don't see the A draw rating, but do you think it will be better cause it's rated for an 800w motor? 

https://www.amazon.com/gp/aw/d/B07Y8F5ZVW/ref=ox_sc_act_image_2?smid=A3D07RFBPK5QF8&psc=1
```

---
## \#87 Posted by: mountainboardlover69 Posted at: 2020-02-05T17:14:41.203Z Reads: 12

```
no, the 800w on my board was the normal draw the max draw I ever did was 75A so that would be closer to 3000W i think a 12s5p 30q pack would be a great option, not to big in price and some nice range and power :stuck_out_tongue:
```

---
## \#88 Posted by: Leolivinlife Posted at: 2020-02-05T17:50:36.156Z Reads: 11

```
I read somewhere that 12S would over volt the controller and potentially fry the system. That's why I was going for 10S . I'm really greatful for your advice as this is the first time I ever venture into anything electrical. So I need something that can handle up to 3000w? The previous batteries were 3 12v 9ah ![Screenshot_20200205-124943__01|384x500](upload://dgrwiR1aWFiRyAT6hIp1F0ipRXk.jpeg)
```

---
## \#89 Posted by: mountainboardlover69 Posted at: 2020-02-07T08:13:24.536Z Reads: 8

```
can u send me a pic of the full bottom of the board, yes i think 3000W would be good, my board took 12s totaly fine
```

---
## \#90 Posted by: Leolivinlife Posted at: 2020-02-09T00:09:01.175Z Reads: 6

```
Thank you for the help! I did some math and realized the $260 I paid for the board plus another $200-300 for a new pack did not make sense considering the outdated tech/size/weight of this board. I will buy a 12v to replace the one that's gone bad and ended up buying an N2G dual motor lithium electric longboard for $350 and I've got to say I love it and it only weighs 20 lbs! I'll fix the Mototec board and end up selling it. Thanks again guys!
```

---
