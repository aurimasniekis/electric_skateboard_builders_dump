# 6S BMS wiring diagram help!

### Replies: 77 Views: 5184

## \#1 Posted by: ReeCorDs Posted at: 2017-11-24T15:53:55.930Z Reads: 173

```
Hello my friends!
i'm new in this forum and this is my first topic. I need your help: i like to build my own electric skateboard but i don't understand the wiring of the balance cables.

I got a 6S BMS with five pins and two 3S batteries with both four pins - how to wire it together?

Five pins only on the BMS is because it only carries the between cells connections and the ends of the battery packs are connected to the b+ and b- making a total of 7 conections.

I already made a diagram and it would be very awesome if someone could complete it! :blush:

Another question is if the voltage indicator is wired on the right place? 

<img src="/uploads/db1493/original/3X/6/7/674e5cf4c293f4d336856bd3abc9f0f5ab072e11.jpg" width="690" height="331">
```

---
## \#2 Posted by: FredrikHems Posted at: 2017-11-24T17:40:03.850Z Reads: 139

```
Not sure about the balance wires, but make sure you hook up your voltage meter after the switch. If not it will drain power from your battery even If its not turned on
```

---
## \#3 Posted by: ReeCorDs Posted at: 2017-11-24T17:44:49.181Z Reads: 136

```
Do i have to wire a second switch between the batteries and the BMS? There is already one switch on the ESC, does that mean that i need two power switches?
```

---
## \#4 Posted by: ReeCorDs Posted at: 2017-11-24T17:47:57.051Z Reads: 132

```
Is that correct? What happened with the two ground wires of the batteries?

<img src="/uploads/db1493/original/3X/8/9/891a84a9ee38f6c2bff91b54d87a0e2ae47e43dd.jpg" width="690" height="331">
```

---
## \#5 Posted by: FredrikHems Posted at: 2017-11-24T17:50:27.141Z Reads: 123

```
I think the balance wires are right, but i'm not sure.. @barajabali may know?  About the switch on the esc, What esc are you running?
```

---
## \#6 Posted by: ReeCorDs Posted at: 2017-11-24T17:51:18.677Z Reads: 121

```
This one: https://www.ebay.com/itm/Single-Motor-Electric-Longboard-Skateboard-Controller-ESC-Replace-Control-Modul-/322629605298
```

---
## \#7 Posted by: FredrikHems Posted at: 2017-11-24T17:55:00.984Z Reads: 119

```
Hmm.. If i were you, I would have made an loop key. As the voltage meter is supposed to go between the esc and switch
```

---
## \#8 Posted by: NiTroNooB Posted at: 2017-11-24T17:59:50.207Z Reads: 120

```
The wiring diagram is not correct. You need to connect the black wire from the battery on top to the 3rd pin on the BMS. You do not need to connect the last red wire of the battery on top since that is already connected to the BMS (thick red wire)
```

---
## \#9 Posted by: ReeCorDs Posted at: 2017-11-24T18:05:10.863Z Reads: 120

```
Thank you very much for your help! But i am a newbie and english is also not my mother tongue (i am from germany). You would be my hero if you edit my wrong diagram and upload it here? that would be awesome! :blush:

Is it correct now?

<img src="/uploads/db1493/original/3X/d/6/d6257705e68c95595fa72e73a5040642976c4302.jpg" width="690" height="331">
```

---
## \#10 Posted by: NiTroNooB Posted at: 2017-11-24T18:21:47.255Z Reads: 122

```
Almost correct :) Move the top two wires on the battery down one step. And you don't need to connect both the red and black wire to the 3rd pin.
```

---
## \#11 Posted by: ReeCorDs Posted at: 2017-11-24T18:26:20.433Z Reads: 118

```
Like that?
<img src="/uploads/db1493/original/3X/c/e/ce1f09b108ae383ee0114b98775a9cf92ac20fa3.jpg" width="690" height="331">
```

---
## \#12 Posted by: NiTroNooB Posted at: 2017-11-24T21:19:49.819Z Reads: 116

```
Yes, that looks correct :)
```

---
## \#13 Posted by: pat.speed Posted at: 2017-11-24T21:25:36.023Z Reads: 118

```
I second that it is correct now. @ReeCorDs what tool did you use to draw the diagram?
```

---
## \#14 Posted by: ReeCorDs Posted at: 2017-11-25T08:41:04.447Z Reads: 123

```
@pat.speed Thanks for your help! I am simply used Paint :smiley:
@NiTroNooB Thank you very much! And the three cables which are not connectet are just useless? So i do nothing with them :slight_smile:

I have two other questions if it's okay for you :smiley:

1. what for a charging cable do i need to charge my board? How much volts and amps? I will use a DC female power adapter.

2. where i have to connect my battery capacity tester on the ESC? I'm using this one:

<img src="/uploads/db1493/original/3X/5/b/5b31cd3f129b0b3313a9051cf598ed41468895b8.jpg" width="500" height="500">
```

---
## \#15 Posted by: pat.speed Posted at: 2017-11-25T10:56:53.104Z Reads: 112

```
You need 25.2v to charge the batteries and you can use any connector you want. I don't think you could use a volt meter with that esc because the switch is wired into the actually esc. You would need a separate antispark loop key or on off switch before the esc
```

---
## \#16 Posted by: ReeCorDs Posted at: 2017-11-25T12:24:52.829Z Reads: 111

```
25.2v and 2a is correct?

And for what are these two black and red wires on the esc? They are not connected to something. I mean not the thick ones
```

---
## \#17 Posted by: pat.speed Posted at: 2017-11-25T19:58:16.930Z Reads: 108

```
They are for powering an led button
```

---
## \#18 Posted by: ReeCorDs Posted at: 2017-11-26T09:13:04.359Z Reads: 105

```
How many amps do i need for charging?
```

---
## \#19 Posted by: pat.speed Posted at: 2017-11-26T11:02:24.496Z Reads: 108

```
No more than 5. Depends how fast you want it to charge. Most people use 2 or 4amp chargers
```

---
## \#20 Posted by: ReeCorDs Posted at: 2017-11-26T17:12:25.012Z Reads: 108

```
Okay, i will buy an anti spark switch. but i only want just one button to power my longboard on. when i simply remove the switch from my ESC and i wire the anti spark switch between ESC and battery, it should work, right? 

And after this i can wire my battery capacity indicator between switch and ESC :slight_smile:
```

---
## \#21 Posted by: pat.speed Posted at: 2017-11-26T21:25:16.873Z Reads: 99

```
I don't think that will work because you need the switch on the escto turn the esc on. I am going to be using this esc soon and I will just be having two switches an antispark loop key and the normal esc switch.
```

---
## \#22 Posted by: ReeCorDs Posted at: 2017-11-27T13:34:16.499Z Reads: 95

```
And when i will do it like that?

<img src="/uploads/db1493/original/3X/b/8/b87f1e4c7eb208a06c2e9274fe5706f30626a306.png" width="690" height="261">
```

---
## \#23 Posted by: pat.speed Posted at: 2017-11-27T21:05:24.175Z Reads: 96

```
It kinda makes sense to do it like that but I'm not 100% sure it would work. Actually I just had a really good idea. What if you get a different switch with 4 connectors that way you can switch on two things with one button! I think it's called a dpst switch. @vishal_tejwani would this work better do you reckon?
```

---
## \#24 Posted by: vishal_tejwani Posted at: 2017-11-28T04:21:12.751Z Reads: 90

```
Checkout meepo board esc review or meepo board review In that kerin(sorry if i miss spelled his name) assembles meepo board, and the board is turned on by the single switch, the esc has a voltmeter/ battery indicator output.

Soo if the esc is turned on the board will turn on soo will the voltmeter.

There is no need of antispark switch and xt60 loop key with this esc
```

---
## \#25 Posted by: ReeCorDs Posted at: 2017-11-28T06:39:54.369Z Reads: 86

```
Alright, thank you guys!

But there is one thing i dont understand... i watched the video of the meepo esc and yes, youre right! There is a voltmeter input but his voltmeter has four wires, mine just have two wires with positive and negative :neutral_face:

And is it possible to connect some 12v LEDs to the ESC? I like to assemble back and front light LEDs to my board :grinning:

And the last question: as you can see in my first post, i have two 3s 35c 11.1v 5.500mah batteries. Do you think it's enough to get a speed over 15mph and a range around 12 miles? :grin:
I will use dual hubmotors with 70kv each.

Thanks very much for your nice help! This will be my first built and i am very happy to get some nice answers for my noob questions! :yum:
```

---
## \#26 Posted by: pat.speed Posted at: 2017-11-28T07:55:56.103Z Reads: 80

```
I don't know if you will be able to connect led lights to the esc directly as you won't be able to turn them off unless the esc has a specific 12v rail. Otherwise you could just buy torches and turn them on and off manually with the normal buttons
```

---
## \#27 Posted by: ReeCorDs Posted at: 2017-11-28T08:26:22.160Z Reads: 81

```
Okay, thanks! But what do you think about by battery setup?

Maybe @vishal_tejwani can help me with my LED light question :slight_smile:
```

---
## \#28 Posted by: vishal_tejwani Posted at: 2017-11-28T08:55:08.762Z Reads: 80

```
Use step down converter taking power from bms if you don't have a bms you can use Battery too,

Bring VOLTAGE to 12 and use your leds
```

---
## \#29 Posted by: pat.speed Posted at: 2017-11-28T08:58:29.304Z Reads: 78

```
How big are your wheels
```

---
## \#30 Posted by: ReeCorDs Posted at: 2017-11-28T09:05:11.675Z Reads: 79

```
my wheels are 90mm
```

---
## \#31 Posted by: pat.speed Posted at: 2017-11-28T09:05:49.065Z Reads: 79

```
That will get you to around 25km/h on a full charge
```

---
## \#32 Posted by: ReeCorDs Posted at: 2017-11-28T09:06:05.577Z Reads: 77

```
Okay, thanks :-) I already got a 12v converter. but where to connect to the ESC?
```

---
## \#33 Posted by: ReeCorDs Posted at: 2017-11-28T09:06:33.518Z Reads: 80

```
And if i use 10S batteries?
```

---
## \#34 Posted by: pat.speed Posted at: 2017-11-28T09:10:25.209Z Reads: 81

```
About 42km/h. Although you must take into account that these escs have a speed limit. Or at least the normal motor version does. About the converter it needs to be connected to the main power leads on the battery. You will need a switch though to turn it on and off
```

---
## \#35 Posted by: ReeCorDs Posted at: 2017-11-28T13:25:08.053Z Reads: 84

```
okay, i think i will use two 5S batteries instead of 3S. But now i have the same wiring issue as before :sleepy: Maybe someone can help me out if its correct

<img src="/uploads/db1493/original/3X/4/3/43b0424b39b341b5802b465c85d33c34621405de.png" width="690" height="331">
```

---
## \#36 Posted by: pat.speed Posted at: 2017-11-28T19:57:56.919Z Reads: 82

```
Yeah looks good. You will need a 10s bms though
```

---
## \#37 Posted by: ReeCorDs Posted at: 2017-11-28T20:01:43.688Z Reads: 83

```
Alright, but how many amps do i need on that BMS? I got some with 10A, 20A or 35A
```

---
## \#38 Posted by: pat.speed Posted at: 2017-11-28T20:08:47.637Z Reads: 81

```
Are you going to bypass it?
```

---
## \#39 Posted by: ReeCorDs Posted at: 2017-11-28T20:17:12.289Z Reads: 80

```
bypass what? I just want to charge my lipos over it
```

---
## \#40 Posted by: pat.speed Posted at: 2017-11-28T20:19:30.262Z Reads: 80

```
Yes but will you be discharging through the bms
```

---
## \#41 Posted by: ReeCorDs Posted at: 2017-11-28T20:36:49.082Z Reads: 77

```
I don't understand this :sweat: i want to use it like my diagram. the batteries will power the ESC on and i want to charge the batteries through the BMS. Now, i do not understand how many amps i need on that BMS
```

---
## \#42 Posted by: pat.speed Posted at: 2017-11-28T21:09:07.422Z Reads: 84

```
A bms charges and also discharges a battery. If you want to discharge through the bms you need at least 50amps but if you only want to use it for charging you only need as many amps as you plan on charging it so for you about 5amps. Anything higher is fine as long as you only use a 5amp charger or less

Have a read of this


https://www.electric-skateboard.builders/t/a-final-word-on-bypassing-bms-for-discharge/18351
```

---
## \#43 Posted by: ReeCorDs Posted at: 2017-11-28T21:13:10.915Z Reads: 84

```
I understand but what is the advantage when i discharge it through the BMS? 

If i understand it right, on my latest diagram i posted here with the 10S BMS, i bypassed the discharging, right? So the wiring is right for just charging

EDIT: I edited the latest one, leaving P- alone is right for bypassing discharging? Like that:

<img src="/uploads/db1493/original/3X/3/2/32f793d7d2042a55da0edd35388679a32dce5bcd.png" width="690" height="331">
```

---
## \#44 Posted by: pat.speed Posted at: 2017-11-28T21:24:19.070Z Reads: 73

```
Yes that is correct for bypassing. If you are to discharge through the bms it will just stop the batteries from being over discharged
```

---
## \#45 Posted by: ReeCorDs Posted at: 2017-11-29T12:53:10.347Z Reads: 69

```
Okay and that is not critical to discharge without a BMS in this case?

And for wiring the charger: do i use the thick cables like the batterie's positives and negatives or like the thin balance cables?
```

---
## \#46 Posted by: pat.speed Posted at: 2017-11-30T11:17:33.975Z Reads: 66

```
What wires are you talking about exactly?
```

---
## \#47 Posted by: ReeCorDs Posted at: 2017-11-30T11:22:09.173Z Reads: 63

```
The wires, which come from the charging plug
```

---
## \#48 Posted by: pat.speed Posted at: 2017-11-30T11:26:46.782Z Reads: 64

```
If you mean from the charging plug to the bms then you would be best with about 16-18awg wires the large battery cables are over kill but the balance cables are a little small for my likings. In the middle would be fine
```

---
## \#49 Posted by: ReeCorDs Posted at: 2017-11-30T11:34:43.796Z Reads: 63

```
The battery cables have 12 AWG and the balance 22, right?
```

---
## \#50 Posted by: pat.speed Posted at: 2017-11-30T11:36:04.895Z Reads: 60

```
Yeah. If you have any spare 12awg use that or buy some 16ish awg cable for cheap. Make sure to get silicone cable though
```

---
## \#51 Posted by: tojo Posted at: 2018-03-21T18:34:04.805Z Reads: 39

```
[quote="pat.speed, post:42, topic:39169"]
A Final Word on Bypassing BMS for Discharge
[/quote]

Anyone can help me please ? I have an issue with a 6s BMS...
```

---
## \#52 Posted by: pat.speed Posted at: 2018-03-21T20:13:49.060Z Reads: 39

```
What’s the issue?
```

---
## \#53 Posted by: tojo Posted at: 2018-03-21T20:21:31.988Z Reads: 47

```
I have made this diagram ![IMG_2301|375x500](upload://fvAhhzpHZytRnBYSnT3bDEFcVLO.JPG)And it doesn't charge... What's wrong ? 
My BMS specified a 24v power supply it is normal ? 

Thanks for your response
```

---
## \#54 Posted by: pat.speed Posted at: 2018-03-21T20:32:04.020Z Reads: 46

```
P- is for the Vesc to connect to. Is there a C- on the bms?
```

---
## \#55 Posted by: tojo Posted at: 2018-03-21T20:46:48.280Z Reads: 46

```
No there is not... 
I need to bypass discharge because the bms support only 10A
```

---
## \#56 Posted by: pat.speed Posted at: 2018-03-21T20:53:49.908Z Reads: 45

```
Hmm I’m not sure. The diagram looks right if the C- and P- are combined. What charger are you using?
```

---
## \#57 Posted by: ReeCorDs Posted at: 2018-03-22T06:19:50.052Z Reads: 48

```
Look at my diagram in this topic! That is right! For bypassing, you have to leave P- alone. 

Next time, please just reading the whole topic ;-)

![Longboard diagramm - Kopie - Kopie - Kopie - Kopie - Kopie|690x331](upload://7gSiXRr10YrcGvrHOIj9k2YQm0l.png)
```

---
## \#58 Posted by: tojo Posted at: 2018-03-22T06:36:09.550Z Reads: 46

```
I'm using a 24v power supply bought on ebay, with an hoverboard charging port!
```

---
## \#59 Posted by: pat.speed Posted at: 2018-03-22T06:36:59.656Z Reads: 47

```
You need a 25.2v cc/cv power supply to charge with a bms
```

---
## \#60 Posted by: tojo Posted at: 2018-03-22T06:37:35.686Z Reads: 45

```
Okay but if there is not C- on my bms and only P- and B-, what do i do ?
```

---
## \#61 Posted by: pat.speed Posted at: 2018-03-22T06:40:59.275Z Reads: 43

```
The pads are probably just connected together as one
```

---
## \#62 Posted by: tojo Posted at: 2018-03-22T08:26:52.171Z Reads: 41

```
I read all the posssible existant subject on BMS (hours and hours). None solved my issue...
Like i said, There is no C- in my BMS...
```

---
## \#63 Posted by: krloz Posted at: 2018-03-22T09:15:27.100Z Reads: 37

```
Probably your bms is a combined input and output type. In that case your wiring would be ok.
You still need a 25.2v psu though. 
At 24v you won't get past 4v per cell
```

---
## \#64 Posted by: b264 Posted at: 2018-03-22T09:17:40.956Z Reads: 39

```
[quote="tojo, post:58, topic:39169"]
I’m using a 24v power supply bought on ebay
[/quote]

A power supply is not a lithium battery charger.  Which power supply?

[quote="tojo, post:62, topic:39169"]
There is no C- in my BMS
[/quote]

Which BMS?
```

---
## \#65 Posted by: tojo Posted at: 2018-03-22T12:27:18.054Z Reads: 35

```
So you say to me that if i have a 24v power supply, even if my diagram is correct,  it doesn’t charge at all ?
```

---
## \#66 Posted by: tojo Posted at: 2018-03-22T12:28:02.281Z Reads: 36

```
I have an hover Board charging port, so i bought on ebay an compatible charger which send 24v 
It’s A cheap BMS bought on eBay 6s 24v, i don’t Know more about!
Sorry the website block me 3h befor i can sending responses
```

---
## \#67 Posted by: krloz Posted at: 2018-03-22T13:27:03.219Z Reads: 38

```
Im not saying "at all".
What i am saying is to charge lipo or lion you need a power source of 4.2v per cell. Unless the bms clearly says it can up the voltage. Which is very rare. And this is assuming  no power loss in the bms. Which is not a bad assumption. 
So if the psu gives 24v it can only charge up to( 24v/6cells) 4v per cell.
Whoever sometimes lithium chargers for 6s are advertised as 24v or 22.2v when in reality they are feedings the 25.2v.
Check yours with a multimeter and no load
```

---
## \#68 Posted by: tojo Posted at: 2018-03-22T14:12:25.514Z Reads: 37

```
Thanks man! I will Check that! 
Is There a possibility that chinese cheap BMS don’t work?
```

---
## \#69 Posted by: krloz Posted at: 2018-03-22T14:52:03.891Z Reads: 39

```
[quote="tojo, post:68, topic:39169"]
Is There a possibility that ****** cheap ***** don’t work?
[/quote]

Corrected that for you. 
The answer is absolutely yes
```

---
## \#70 Posted by: b264 Posted at: 2018-03-22T17:47:18.764Z Reads: 39

```
[quote="tojo, post:66, topic:39169"]
I have an hover Board charging port, so i bought on ebay an compatible charger which send 24v

It’s A cheap BMS bought on eBay 6s 24v, i don’t Know more about!

Sorry the website block me 3h befor i can sending responses
[/quote]

Neither of those are model numbers or links.

I will say that no lithium-ion stuff is 24 volt so it's possible you have lead-acid chargers and BMS.
```

---
## \#71 Posted by: ReeCorDs Posted at: 2018-03-22T18:56:11.494Z Reads: 37

```
i had the same issue. The problem was: the charger was broken. Please check with a multimeter if you really get 24v out of your charger. Another problem can be the BMS. maybe that is broken.

Please check both things and then buy another BMS with C- B- and P-. I am also unsing a cheap 5$ china BMS and it just works fine. :slight_smile:
```

---
## \#72 Posted by: tojo Posted at: 2018-03-22T19:21:20.481Z Reads: 35

```
Okay, it was written for lipo battery, but i don’t have so Much trust! 
I think i am going to bought a new quality BMS, for charge and discharge, Like that i can put the regeneretive breaking at it max, is that right?
Do you have any BMS to recommend?

Thanks Again for your help, it’s really kind of you!
And excuse for my poor english i am french...
```

---
## \#73 Posted by: tojo Posted at: 2018-03-22T19:30:12.869Z Reads: 36

```
Okay man, thanks for the info! I will do that! Where did you buy your own BMS? Do you have the link ? 

And i looked for a 25,2v charger with a 3prong in Line output (compatible with my charging port) and i don’t fine anywhere...
What do you use for charging port ? 

@krloz Ahaha okay thanks man!
```

---
## \#74 Posted by: ReeCorDs Posted at: 2018-03-22T20:35:55.837Z Reads: 38

```
I am using a 10S BMS, that would not fit for you.

![grafik|281x500](upload://e2IDowySkSkuWKNgmGLeYqArsdc.jpg)
```

---
## \#75 Posted by: tojo Posted at: 2018-03-24T09:15:15.155Z Reads: 34

```
Okay man thanks for the picture! Where do you found the dc port with the waterproof cover?
```

---
## \#76 Posted by: ReeCorDs Posted at: 2018-03-25T18:08:32.342Z Reads: 37

```
on ebay. search for waterproof dc plug
```

---
## \#77 Posted by: tojo Posted at: 2018-06-22T20:36:05.888Z Reads: 24

```
Hi guys!
I have questions if you don’t mind!
I have a 6s battery pack (2x3S in series) since 2 month, can i add 2X3s in parralel to double the range (with two new and two old) ? If yes How i wire the BMS to the new, I use the same or i put another 6S BMS ?

Thanks in advance!!
```

---
