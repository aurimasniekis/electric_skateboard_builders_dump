# Is my 6s 3p BMS wiring sheme correct?

### Replies: 56 Views: 2933

## \#1 Posted by: Zimbombe Posted at: 2017-08-25T09:21:00.301Z Reads: 174

```
Hi,

im in the process of wiring my esk8board and as i havent done much electric projects so far i would 
really apreciate if someone could look at my wiring diagramm and tell me if everthing looks alright.

Before it get´s to the point where somebody questions my research, i´ve been looking around in this forum for months
and tried my best to understood everything as good as i can. But if you see some missunderstandings on my side pease
be gently as i really tried understand everthing correct. 

I tried to orientate on this thread but wanted to make it fit my physical setup to help myself getting not confused while wiring it, so if my diagram has some crosscuts of wires it´s just because the wires overlap there.

https://www.electric-skateboard.builders/t/acceptable-diy-6s3p-bms-and-battery-setup/6114

I have 3 things i dont understand. 

1. The given shemes on how to wire this bms don´t show the usage of P-, from what i saw P- has to 
be connected to negative ESC. (i´ve put a red cicle on it to show what i mean)

2. What is the difference between "load" and "Charger" from the general sheme for this kind of bms ?

3. Should i use the switich of my ESC or wire one between the bms ?




<img src="/uploads/db1493/original/3X/2/b/2baa171afc75b2334ed9663061f51ae2e21ed95e.jpg" width="446" height="500"><img src="/uploads/db1493/original/3X/0/1/0159a665aabdd1037b2b8b3ec68c18185cd251fb.jpg" width="666" height="500">


Every help would be highly appreciated but please be gentle. Thanks in addition.


BMS: https://www.aliexpress.com/item/13S-100A-bms-2016-new-Li-ion-48V-100A-large-high-current-BMS-PCM-with-different/32759040792.html?spm=a2g0s.9042311.0.0.U44Zr7

Engine: https://www.banggood.com/Racerstar-5065-BR5065-140KV-6-12S-Brushless-Motor-With-Gear-For-Scooter-p-1110304.html?rmmds=myorder

ESC: https://www.banggood.com/FVT-CBWI120A-ESC-Brushless-Speed-Controller-For-110-and-18Series-RC-Cars-Skateboard-ESC-p-985970.html?rmmds=myorder

Charger: https://www.banggood.com/AC-100V-240V-DC-24V-4A-96W-Power-Supply-Charger-Converter-Adapter-p-970663.html?rmmds=myorder

Voltmeter: https://www.banggood.com/Battery-Capacity-Tester-with-LCD-Indicator-for-12V-24V-36V-48V-Lead-acid-Lithium-LiPo-p-991337.html?rmmds=myorder

Power Switch: https://www.banggood.com/DC-12V-19mm-Stainless-Steel-Illuminated-Latching-Power-Push-Button-Switch-p-1120942.html?rmmds=myorder

<img src="/uploads/db1493/original/3X/b/4/b4225cd6e8023d108cce884d871817922efdd102.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/a/6/a65ca294508897f4b778cba66a6ae1b3a3157876.jpg" width="375" height="500">
```

---
## \#2 Posted by: krloz Posted at: 2017-08-25T15:08:29.991Z Reads: 125

```
I dont quite understand your diagram. firstly it looks like you have your esc and chargers positive and negative to the same wires connected?
in any case this bms switches the negative side so you need the following.
a thick wire (10awg maybe) from the battery negative to the bms b-
your esc, charger and battery positive all conected together, with a thick cable (10awg again) between esc and battery. and im not sure about the escs switch but i would add a loopkey in between.
the negative from charge to your bms c-
the negative from esc either to the bms p- (this would be your load) if you desire undervoltage and overcurrent protection from the bms, or directly to the battery negative. (10awg again here)
I think that is all?
```

---
## \#3 Posted by: krloz Posted at: 2017-08-25T15:14:57.973Z Reads: 121

```
I dont know the bms you posted. it looks like it shares the c- and p- connections. if that would be the case, where I said
 [quote="krloz, post:2, topic:31448"]
the negative from esc either to the bms p-
[/quote]
it would mean 
the negative from esc either to the bms c-
```

---
## \#4 Posted by: Zimbombe Posted at: 2017-08-25T15:45:14.773Z Reads: 115

```
Thats what confused me the most, from what i understood and saw from other bms is that p- should be connected to engine or esc negativ but the wiring sheme i got from their site doesnt showed it.

Actually i would think this wiring would be correct, it´s confusing.

<img src="/uploads/db1493/original/3X/2/2/2216270daddcef9a8e9c6ca0f8257a5effa97203.jpg" width="446" height="500">

here is the how my esc looks like, it has seperate c- and p-.

<img src="/uploads/db1493/original/3X/d/9/d9195401b520f6753359257f3e5610f4803b3b1b.jpg" width="375" height="500">

can u tell me the difference between Charger and Load ? Thanks for taking your time.
```

---
## \#5 Posted by: rojitor Posted at: 2017-08-25T17:20:05.702Z Reads: 99

```
It is very confusing. Looks like a model S (charge and discharge on the same port) but it has C and P ports....
Either the diagram is wrong or is a model S. You should ask the seller.
I wired a 6s model S here:

[https://www.youtube.com/watch?v=_iKuUNYCXRk](https://www.youtube.com/watch?v=_iKuUNYCXRk)
```

---
## \#6 Posted by: rojitor Posted at: 2017-08-25T17:25:39.857Z Reads: 98

```
I checked the link you posted:

The seller wrote:

esta bms se utiliza para la batería de li-ion, los SERVICIOS de administración de los puertos de carga y descarga son EL MISMO PUERTO " P "

I am pretty sure it is a model S and you must wire charge and discharge to P
Ask the seller anyway. That thing is a mess.
```

---
## \#7 Posted by: krloz Posted at: 2017-08-26T08:47:24.839Z Reads: 90

```
[quote="Zimbombe, post:4, topic:31448"]
Actually i would think this wiring would be correct, it´s confusing.
[/quote]

That wiring is also wrong.  You have the positives of esc and charger to one port of the bms and the negatives of esc and charger to the other one
What you want is the positives of esc and charger to battery positive and the negatives of esc and charger to p-

What we might have here is a bms with shared charge and discharge ports (just learned the are called model s) built in a shared pcb layout.   Designed for either model s or for the "whatever You call the usual bms with separated ports". Just like they do with the cell count where they design the pcb for a big cell count and just add the balancing components for the particular count they are building for.

Editing for the bloody autocorrect
```

---
## \#8 Posted by: Zimbombe Posted at: 2017-08-26T13:11:07.693Z Reads: 83

```
I Found something in the description of the Bms which made it pretty clear.

"This bms is used for Li-ion battery pack, The BMS charge and discharge ports are THE SAME PORT "P-"

So i tried again to do a more understandable wiring sheme with your tipps in mind but this time i´m not sure what to do with C-. I also used thick strings to mark where i´ll use 12awg wire. But i guess @rojitor is right and C- will not be connected. 

<img src="/uploads/db1493/original/3X/2/3/23a7bba9b66ecfc165f344411cfc83c2872f9801.png" width="690" height="261">

Anyway thanks again for your Help

"1. Before you make the pack, please test and match the cell's voltage,capacity and resistance.
2.The diagram showed thick cable, please use the thick wire. 
3.The balance wire sequence is from B1-  B1- connect to general negative,the second wire connect the first series positive 
4.When you connect the balance wire, please unplug all the wires ,then connect the wires step by step.
5. Connection sequence: Connect B- wire to battery pack negative ,then connect balance wires and plug in. Connect P- & C- and 
and then test the general voltage and C-with battery pack positive voltage whether the same. if yes, then it's OK."
```

---
## \#9 Posted by: krloz Posted at: 2017-08-26T14:26:01.126Z Reads: 74

```
Boom. Now it's right

[quote="Zimbombe, post:8, topic:31448"]
i´m not sure what to do with C-
[/quote]
Just what you did in the diagram. connect nothing to it. Probably it goes to no where in the bms.

Nitpicking a bit now. 
You should add a switch to the vmeter do it doesn't drain your battery. 
Personal opinion.  Even if you use the esc switch. I would add a loopkey in case of emergency.  For a simple jankoff quick switch

And some of the wire  colours are technically the other way round, but as long as you follow the paths all is okay. Be sure to connect the esc charger and vmeter red positive to the battery+ and the blacks to the p-
```

---
## \#10 Posted by: Zimbombe Posted at: 2017-08-29T06:59:17.182Z Reads: 71

```
Yeah i got that wrong with the color sheme i really thought red is suposed to be negativ wire. Again something learned.

I've taken my time and wired everything up which was quite
Frustrating because all soldered conections were lose, i had to find another way to connect everything which looks horrible but works.

Systems are running and the board runs well BUT i don't know if my bms is properly Working. When i connect the charger nothing happens while its connected to p- .
So i gave it a try and connected it to C- and it themed to starting to load until a little bang scared the out of me and i cut it off. (In both cases, C- and P-, the balance leds were not working.)

And here i am again, dont know what to do and especially dont know how to figure out if my bms is working properly.

<img src="/uploads/db1493/original/3X/4/0/40511bdd1869071eaab75a428bb4db4c7646ced1.jpg" width="374" height="500">
```

---
## \#11 Posted by: Zimbombe Posted at: 2017-08-31T09:31:28.389Z Reads: 59

```
I decided to ask the seller how the bms has to be wired and this what he said. <img src="/uploads/db1493/original/3X/9/5/951cffbc63002e38cf60f04ee44471c245a24481.png" width="243" height="500">

So this evening i will check all bms connections with a voltmeter and wire to C- then.
```

---
## \#12 Posted by: Zimbombe Posted at: 2017-09-01T06:05:55.739Z Reads: 53

```
So yesterday i tried the hole evening to get my bms working but for some reason i was not successful. 

At first i checked my bms wiring just like @rojitor did in his video by and got 3,3V, 6,6V, 10,1V, 13,5V, 16,9, 20,2. I then reconnected my bms starting with B- then balancer plug then C-. And result is the same as before. The board works but it wont charge at all.

I'm now pretty frustrated and don't know how to go on from here. If somebody has a hint for me on what to do next i would highly appreciate. 

Thx in addition
```

---
## \#13 Posted by: krloz Posted at: 2017-09-01T07:21:28.271Z Reads: 49

```
Are you sure your charger is working properly
```

---
## \#14 Posted by: Zimbombe Posted at: 2017-09-01T07:55:37.761Z Reads: 54

```
Thats what i was thinking too but i'm not 100% sure how to check it. Shouldnt my voltmeter show 24V here ? Because it does not. 

But why does the green light shine whenever i plug it into my board ? And why should my charger be broken he is brand new, maybe because of the wrong wiring before ?
<img src="/uploads/db1493/original/3X/d/d/ddbc0f9e06086e249053279f87e41da96711cc6e.jpg" width="666" height="500">
```

---
## \#15 Posted by: krloz Posted at: 2017-09-01T08:46:09.541Z Reads: 52

```
Yes. Actually it should be outputing dc 25.2v to charge a 6s. I don't understand what led you are talking about
```

---
## \#16 Posted by: Zimbombe Posted at: 2017-09-01T08:57:11.454Z Reads: 53

```
Thats sounds not good, but i dont understand why it stopped working. 

I mean the led on the charger, whenever i plug the charger to my board it goes green.

 <img src="/uploads/db1493/original/3X/7/b/7b8bf206ab6a98febc98b50a06a1767159785631.jpg" width="690" height="478">
```

---
## \#17 Posted by: krloz Posted at: 2017-09-01T09:11:40.602Z Reads: 50

```
Can you measure the voltage between p- on the bms and battery+ with and without the charger plugged in
```

---
## \#18 Posted by: krloz Posted at: 2017-09-01T09:12:53.974Z Reads: 52

```
Wait.  I think I know what's up.  Can you try plugging the charger to the bms and DON'T connect the charger to the wall.  What is the led then?
```

---
## \#19 Posted by: Zimbombe Posted at: 2017-09-01T09:39:57.527Z Reads: 53

```
The V between C- and battery + is 20,2v same for P- and battery +. 

When i connect the charger only to the board this is the result.

<img src="/uploads/db1493/original/3X/2/a/2a70b1f833c897a269c85257bc2b21bfa79fcc58.jpg" width="375" height="500">

Again, thanks for taking your time mate.
```

---
## \#20 Posted by: krloz Posted at: 2017-09-01T10:29:30.731Z Reads: 50

```
Yeah.  I'm 99% sure your charger is broken.  The led is on because the bms is feeding power to the charger and I'm guessing it is not protected against power going in through the charger out. Maybe that is why it broke in the first place.  Didn't simmering pop once when you connected something?
```

---
## \#21 Posted by: Zimbombe Posted at: 2017-09-01T12:36:17.597Z Reads: 46

```
Like 3 days ago i wired charge/discharge testwise to C- and that was the only time i saw it charging my battery until a little bang scared the shit outta me so i cut it of again. 
Aaaaand one day i tested my charger by putting one of the voltmeter into the plug of the charger where a pretty big again scared the shit out of me, i guess it broke there.

Do you think i should just buy a new charger or is there still a problem with my wiring ? (Ignore the C- wiring, it's testwise)

And if i would buy a new one this here should work right ?

https://www.amazon.de/dp/B01A6LQMWW/ref=cm_sw_r_cp_apa_2cvQzbBEKTCFP
```

---
## \#22 Posted by: krloz Posted at: 2017-09-01T13:45:40.481Z Reads: 45

```
Your last diagrams I checked were fine.  As long as you corrected the wiring colours. Red is positive and black is negative.
About that charger I don't think It will fully charge your battery.  You have a 6s setup.  And a fully charged cell is at 4.2v. So as voltage is added in series you have 6x4.2v=25.2v
That's the charger you need.  One that outputs 25.2v dc
With that charger you will get only 24v/6= 4v per cell. Not fully charging is actually good for batteries l life  but you will not get full juice out of them. Up to you
```

---
## \#23 Posted by: krloz Posted at: 2017-09-01T13:49:21.960Z Reads: 45

```
I don't speak German so I can't be sure but it looks line this one would do

https://www.amazon.de/gp/aw/d/B06VVNX19Q/ref=sxbs_sxwds-stvp_1?__mk_de_DE=ÅMÅZÕÑ&qid=1504273681&sr=1&pf_rd_m=A3JWKAKR8XB7XF&pf_rd_p=1302052647&pd_rd_wg=LzPna&pf_rd_r=M8HPGAWVYDFXWXQ916BH&pf_rd_s=mobile-sx-bottom-slot&pf_rd_t=9701&pd_rd_i=B06VVNX19Q&pd_rd_w=tW1rC&pf_rd_i=25.2v&pd_rd_r=CEF9VBAGAXD15N2VZ0F1&pi=AC_SX236_SY340_QL65Just
```

---
## \#24 Posted by: Zimbombe Posted at: 2017-09-01T14:30:46.810Z Reads: 44

```
I've ordered both because i want to get this thing to work asap and the 25,2V one is from China. And as you said, under charging increases battery life which isint that bad.

I'll get back tomorrow when the charger from amazon arrives.

And again thanks for all your help.
```

---
## \#25 Posted by: krloz Posted at: 2017-09-01T14:32:42.827Z Reads: 44

```
You are very welcome.  As I said i couldn't understand much more than the specs from the description. Xd
Not a bad idea to have a backup anyway
```

---
## \#26 Posted by: Zimbombe Posted at: 2017-09-01T18:47:47.320Z Reads: 41

```
Before i break the next charger i wanted to check if i wired my charging port correct but i couldnt find info on how to wire it. 

This is my plug.

https://banggood.app.link/7e27cIwN5F

At the moment i have battery + connected to inner pin of the charger plug and Esc - to outer ring of the plug. I really googled a lot but i couldnt find anything reliable on how the polarity of 2.5 x 5.5 plugs has to be.

Wait i just found a picture...
Aaaand it looks like i was wrong ? 

https://goo.gl/images/qJnkde
```

---
## \#27 Posted by: Zimbombe Posted at: 2017-09-02T07:24:47.033Z Reads: 39

```
I´ve updated my wiring sheme in regard to my problem. 

<img src="/uploads/db1493/original/3X/f/b/fbb741b212cc8af395d3753c0d587f988aa74008.png" width="690" height="261">
```

---
## \#28 Posted by: Tampaesk8er Posted at: 2017-09-02T11:02:50.269Z Reads: 40

```
Is everything working now?
```

---
## \#29 Posted by: krloz Posted at: 2017-09-02T11:26:54.594Z Reads: 41

```
When the charger arrives check polarity with your multimeter. It could be both ways
```

---
## \#30 Posted by: Zimbombe Posted at: 2017-09-02T12:07:25.149Z Reads: 47

```
The charger just arrived and i think i should be fine to test it right ? <img src="/uploads/db1493/original/3X/a/c/accceab90da24e54b12846a1889097e9274ba4cb.jpg" width="375" height="500">

Edit: I've plugged it in and it thems to work. The cells are slowly getting voltage. But there comes the next question to my mind. How do i now if my Bms is really working properly ?
```

---
## \#31 Posted by: krloz Posted at: 2017-09-02T12:57:56.799Z Reads: 43

```
Measure each cell voltage a couple of hours after you think it finished charging. 
And do the same once each month more or less.  If all cells are 4.2 either it is a perfectly symmetrical pack or your bms is working.
```

---
## \#32 Posted by: Zimbombe Posted at: 2017-09-02T13:47:16.053Z Reads: 43

```
That sounds plausible, my bms has also "balance Led's" but i don't know when they will turn on, maybe only in the balance process. 

Right now everything looks good and is loading. 
THANK YOU VERY MUCH M8 !

If you have the time to go through my last questions for now that would be awesome if not, its also fine :slight_smile:

1. Do you have an solution on how to wire my voltmeter, so it turns of whenever i use the switch of my esc ? 

 2. Another nice dude from this forum told me that my battery will have to work very hard in this setup. I think he is referring to the 45A my battery has and the 36A my engine will max drain. Would an 6s4p solve the problem ? 

Again thank you so much for all your help also to the other guys !
```

---
## \#33 Posted by: Tampaesk8er Posted at: 2017-09-02T14:23:19.040Z Reads: 44

```
looking at your last battery setup pic, does this 6s setup work? i have 24 samsung 18650 batteries to build a 6s4p setup and your setup would work great if i build my pack as is in your pic.
```

---
## \#34 Posted by: krloz Posted at: 2017-09-02T14:43:14.460Z Reads: 45

```
I'm afraid I never had That esc so I can't say. Ask around in the forum maybe someone figured it out.  Maybe the switch switches on the full dc input to turn on something and you can turn on the volt meter as well but without having the esc I can't figure it out.  maybe open a new thread specifying the esc model. 
And about the batteries.  I have only used lipos but in general.  If your Max discharge (theoretically c rating of cells x pack amps) is not high enough you will get voltage sag and maybe trigger esc protections or at least not enough power. So in general more cells in parallel equals less sag and more driving distance but more weight
```

---
## \#35 Posted by: Zimbombe Posted at: 2017-09-02T19:50:55.251Z Reads: 39

```
Well i havent driven it yet but the engine is working as it should. From what i've calculated i should get around 20 kph max with 16 km range, which would be top notch in my opinion. 

But remember if you want use my wiring diagram that its for my bms and my battery will probably have to work hard as my engine max drains 34 A from my 45A battery pack.

I'll upgrade asap to a 6s4p or 5p setup.

@krloz

Thank for the hint i'll see what i can find in regard to my esc and probably upgrade my battery very soon with more in parelel wiring.

Btw that loading time with my 24V 3A charger is crazy. After 6 hours of loading from 20.2V to 21.2V.
```

---
## \#36 Posted by: krloz Posted at: 2017-09-02T20:51:40.066Z Reads: 34

```
That is quite slow.  Maybe the charger is over specked  and it is not giving 3A. What is the amp rating of your cells?
```

---
## \#37 Posted by: Zimbombe Posted at: 2017-09-03T06:52:11.661Z Reads: 36

```
They are rated with 15 A 

https://eu.nkon.nl/review/product/list/id/1852/category/23/

For some reason my multimeter stopped working yesterday.....anyway almoast 50 % Charge.
```

---
## \#38 Posted by: krloz Posted at: 2017-09-03T09:04:55.659Z Reads: 39

```
15A is the max discharge rating. I meant the capacity which is 3A (3000mA) and at 4p pack that is 12A. With a 3A/hour rated charger you should be getting to 90% charge and balancing in 5 hours more or less.

Edit. I thought you had a 4p pack. At 3p the math is 9A pack and around 4hours of charging
```

---
## \#39 Posted by: Tampaesk8er Posted at: 2017-09-03T13:07:37.136Z Reads: 40

```
Here is what they say.
HERE ARE POWERFUL 36V 4.4AH BATTERY PACKS MADE OF 20 BRAND NEW AND GENUINE SAMSUNG 18650 BATTERIES. I KNOW ALL YOU "DO-IT-YOURSELF" E-BIKE AND POWERWALL BUILDERS OUT THERE ARE LOOKING FOR AFFORDABLE AND HIGH QUALITY 18650 CELLS. THIS IS PERFECT FOR YOU. GENUINE SAMSUNG 2200MAH (MORE LIKE 2270MAH - 2310MAH) BATTERIES. HIGH DRAIN MEANING THESE ARE RATED FOR 10A CONTINUOUS AND 20A MAX PER CELL. SO THESE ARE MEANT TO HANDLE THE EXTRA POWER. DO YOUR RESEARCH AND REALIZE YOU ARE GETTING 20 BRAND NEW SAMSUNG 18650 CELLS FOR THIS PRICE. ALREADY SPOT WELDED AT 10S 2P WITH A SOLID BMS. I SEE YOU E-BIKE BUILDERS PAYING $190 FOR A 36V 10AH BATTERY. YOU CAN BUILD THAT WITH THESE FOR HALF THE PRICE. YOU JUST NEED A NEW CONNECTOR AND TO CONNECT THE 2 LEAD WIRES IN PARALLEL TO INCREASE THE CAPACITY. ALSO PERFECT TO DISASSEMBLE AND BUILD OTHER BATTERY PACKS WITH THE CELLS. LOOKING FOR A BULK ORDER? LETS DO BUSINESS! CONTACT ME BY CLICKING ON "ALARMHOOKUP" AT THE TOP RIGHT OF THIS LISTING UNDER THE SELLER INFORMATION BOX. THEN CLICK ON "CONTACT". I HAVE TONS OF THESE THAT I AM CURRENTLY RE-BUILDING INTO POWERWALLS. IF YOU NEED A LOT OF THESE PACKS I CAN SUPPLY YOU WITH MANY CELLS
```

---
## \#40 Posted by: Zimbombe Posted at: 2017-09-03T13:26:22.736Z Reads: 37

```
Ah ok i got you wrong there. I have to check the charging plug it possible some damage. 40% charge after 24h is kinda lame.
```

---
## \#41 Posted by: krloz Posted at: 2017-09-03T15:19:37.547Z Reads: 34

```
I don't understand what your question is
```

---
## \#42 Posted by: krloz Posted at: 2017-09-03T15:20:59.314Z Reads: 37

```
That is a terrible charging time. 
Maybe your parallel packs are terribly unbalanced. That could make your charging so slow. Can you measure the voltage of each parallel pack?
```

---
## \#43 Posted by: Zimbombe Posted at: 2017-09-03T16:09:11.150Z Reads: 41

```
Nah i think the cells are fine, i checked them several times yesterday and they were like perfectly balanced. All were within a range of 0.01 difference. Sadly my multimeter themed also to stopped working... i can't messure volts anymore but my e board voltmeter says now 80% charge and thats probably all i will get with 24v.


But as i said i think its either the charging plug who themes damaged from a spark, some bad wiring or the 24 V charger.
```

---
## \#44 Posted by: krloz Posted at: 2017-09-03T16:17:20.809Z Reads: 42

```
Yeah with 24v charger you won't get to max charge which is at 25.2v
```

---
## \#45 Posted by: Tampaesk8er Posted at: 2017-09-03T22:02:56.463Z Reads: 40

```
Sorry, someone was asking about the link i put up about a 18650 battery packs that i purchased on ebay so i copied and pasted the description of the battery pack.
```

---
## \#46 Posted by: krloz Posted at: 2017-09-03T22:26:19.791Z Reads: 39

```
No problem
```

---
## \#47 Posted by: rojitor Posted at: 2017-09-04T10:11:15.466Z Reads: 40

```
So... It was port C after all? The chinese intructions are kinda funny...
I hope you make that thing work once and for all. If the cells are new Sometimes they refuse to do full charge. You must go out for short runs and charge again. After a couple runs they will reach 4.2v. I see you have charger issues anyway. Keep trying.
```

---
## \#48 Posted by: Zimbombe Posted at: 2017-09-04T10:21:40.288Z Reads: 38

```
Yeah C- was the right way to go. I think the charging issues wont be a big of a deal. So thanks @rojitor for help, your video was pretty helpfull, the only thing thats left which is concerning me are the german laws but thats another story.
```

---
## \#49 Posted by: Tampaesk8er Posted at: 2017-09-04T17:12:11.556Z Reads: 36

```
Does your 6s battery setup works, if so, how many volts is it?
```

---
## \#50 Posted by: Zimbombe Posted at: 2017-09-04T19:28:26.794Z Reads: 37

```
Yeah it works, i just had my first quick ride and saw what the problem here might be. After like 2 mins the performance fall to like 25% but which could be a problem with the Voltage sag but, so 6s3p might not be a good Idea. BUT the performance los only last very short, i gave it a little pause and from then i had 15 min with 100%.

Tomorrow i will have a long ride at Tempelhofer Feld, the old Airfield and be able to tell more about it´s performance.

Edit: Fully loaded it´s 25,2 Volt.
```

---
## \#51 Posted by: chomp Posted at: 2018-01-08T17:33:15.459Z Reads: 27

```
I see you're using the Racerstar 5065. Same one I bought, I didn't notice you said anywhere..what mount are you planning on using? I'm having a hard time finding anything that would work besides the Evolve mounts since these motors have a 38mm bolt spacing.
```

---
## \#52 Posted by: Zimbombe Posted at: 2018-01-08T20:52:49.617Z Reads: 26

```
Hi m8,

you should check out the build thread i created later. You´ll find the mount i used and pictures of how it looked after i adjusted it. The pictures are in a comment of me.

https://www.electric-skateboard.builders/t/human-instrumentality-project-6s3p-single-racerstar-140kv-5065-custom-deck-battery-box-holder-fvt-120a-esc/32737

let me know if you have and further questions
```

---
## \#53 Posted by: Zimbombe Posted at: 2018-03-12T17:35:01.221Z Reads: 21

```
It would be awesome if somebody could check if my new wiring scheme of my rebuild esk8 
looks good, thx in addition. 

![Wiring sheme|551x500](upload://bFJdnP38Uazi6XGniqVt5IuVm21.png)

Edit: @rich or @krloz maybe ?
```

---
## \#54 Posted by: rich Posted at: 2018-03-12T20:43:33.304Z Reads: 18

```
Looks correct for me because I know this BMS, other people might be confused :laughing:
Do you have a wiring scheme for the balance leads to get sure?
Just to make it 100% perfect there is one motor phase wire missing :wink:
```

---
## \#55 Posted by: Zimbombe Posted at: 2018-03-12T22:21:38.796Z Reads: 18

```
[quote="rich, post:54, topic:31448"]
Just to make it 100% perfect there is one motor phase wire missing :wink:
[/quote]

Damn, i really thought there was no mistake hidden in my scheme..... ofc you are right about that.

[quote="rich, post:54, topic:31448"]
Do you have a wiring scheme for the balance leads to get sure?
[/quote]

I could do one but the battery pack is already wired and works fine, as u can see i decided to just use my old 18650´s for my first spot weldet Pack. 

thx for the help m8
```

---
## \#56 Posted by: krloz Posted at: 2018-03-13T00:00:07.682Z Reads: 18

```
Looks good to me assuming the bms in use is of the common charge and discharge pad type
```

---
