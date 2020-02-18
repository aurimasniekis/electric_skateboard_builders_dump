# Help: Why is my BMS balance wire melting on custom Evolve GT battery build?

### Replies: 47 Views: 4165

## \#1 Posted by: HGsystem Posted at: 2018-02-22T11:09:13.545Z Reads: 309

```
Hello Everybody!

Thanks to all the information on this forum I have succesfully built my own custom battery for Bamboo GT. I used VTC6 cells in a 10s5p config making a 15ah battery. I lengthened the case and stacked the BMS on the VESC to make room.

MY PROBLEM:
It rides great with no voltage sag and double the range...BUT I CANT PUSH THE MOTORS PAST ABOUT 45 AMPS (ie no hills!), when i do the BMS B0 balance wire melts and the board shuts down. The B0 sense/balance wire is the one the goes to the negative end of my first battery pack in parellel. I have replaced the B0 wire a few times now but every time i push the motor hard (up steep hills etc) the same thing happens, the wire melts and the board shuts down.

Any thoughts from the forum on how to fix this melting B0 wire issue? 

I dont think this makes sense, but is my battery “too powerful” ? Another strange observation I have made is that on a second Evolve GT I have that I took apart I noticed that the B0 sense wire is actually cut (by the factory) and only the 10 remaining B1-B10 wires are used....I have tried just not connecting the B0 wire on my build but the board will not turn on unless I also use this wire. Very strange that from the factory Evolve has some GT boards that require 11 balance wires to be used and then some that only 10 are used.

Thanks so much for everyones input, I am also including a few pics of my build for viewing pleasure.
```

---
## \#2 Posted by: HGsystem Posted at: 2018-02-22T11:16:28.263Z Reads: 303

```
![IMG_9008|690x335](upload://fa85CN2zNmVxHOAKd2Li7ptfKFA.jpeg)![IMG_9011|666x500](upload://6OUCrkPD32FfyQswU1gl87uqhx1.jpeg)![IMG_9027|375x500](upload://vpHT3NOe3PoYGmHmslZ9SwiPMPB.jpeg)![IMG_1911|282x500](upload://vPci8U6C2c2EN16dgtiUrxCbfYN.jpeg)
```

---
## \#3 Posted by: SimosMCmuffin Posted at: 2018-02-22T11:37:19.663Z Reads: 287

```
If the wire is melting, then that means that it has quite a lot current going through it. I suspect that the discharge current is going through both of the negative terminal wire and B0 balance wire.

Can you draw a diagram of the BMS wiring?
```

---
## \#4 Posted by: BoostedBuilder Posted at: 2018-02-22T11:46:00.986Z Reads: 282

```
I believe these motors have a 35A - 40A max current limit, why would you want to push 45A through a 50mm, 150KV motor in the first place? Don't they get boiling hot when you push them? I don't think that the Evolve system is designed for such a powerful battery. We are talking about 100a continuous current with these cells in a 10s5p configuration.
```

---
## \#5 Posted by: krloz Posted at: 2018-02-22T12:12:49.472Z Reads: 274

```
There is not such thing as a very powerful battery.  If I made a 10s20p pack out of 30q wicu can push 300A discharge that in no way means that it is going to push 300A to my motors at all. That depends entirely on how you configure your esc. You will however have a hell of range. If this wouldnt be the case absolutely every board would have a range of approximately 1 hour, or straight up melt...

To week batteries however actually are a thing.  

So assuming you have your wires properly dimensione, it looks like your bms is taking too much of its negative out of the b0 on the balance instead of the b- thick wire. Check this last cable
```

---
## \#6 Posted by: HGsystem Posted at: 2018-02-22T12:50:15.256Z Reads: 270

```
@SimosMCmuffin
Please see attached drawing. 

@BoostedBuilder
I should have clarified when I say it starts melting around 45a that is for the combined two motors, i.e. it starts melting with about 25a going to each motor. And my understanding is the same as krloz— the amps out to motor is limited by the esc so I cannot “overamp” the motor

@krloz
I think it makes total sense the the b0 cable is taking too much load instead of the thick b- wire...so how do I take the load off the b0 cable? FYI i am using the same gauge wire that the evolve originally was built with: 16gauge for the b- wire and 22gauge for the balance wires.

As a side note: I dont understand the purpose of the b0 wire— it seems a liability, but as I said this is how this board was originally configured and it does not turn on if I dont connect the b0. It is very interesting that the second GT board I have the b0 wire is cut off the BMS harness (maybe to address this very issue??) but it obviously does turn on without the wire used.
```

---
## \#7 Posted by: HGsystem Posted at: 2018-02-22T12:51:04.519Z Reads: 257

```
My BMS layout:![IMG_1912|690x411](upload://25FK6SpRr2M1de7581RyhoR0M2v.jpeg)
```

---
## \#8 Posted by: HGsystem Posted at: 2018-02-22T13:06:36.880Z Reads: 253

```
I am also attaching a more closeup view of the negative end of pack #1 where you can see the b0 and b- wires
![IMG_1913|690x396](upload://uE4sDK7Ca0U78PmCOTyEUuRXKlV.jpeg)
```

---
## \#9 Posted by: SimosMCmuffin Posted at: 2018-02-22T13:21:04.106Z Reads: 244

```
What if you cut the B0 wire and add a 100 Ohm resistor in-line to it?
```

---
## \#10 Posted by: krloz Posted at: 2018-02-22T13:35:31.762Z Reads: 243

```
Dont do that. The b0 is used for monitoring cell voltage.  You would screw with the protections.
```

---
## \#11 Posted by: krloz Posted at: 2018-02-22T13:38:32.587Z Reads: 242

```
If you are absolutely certain the b- is correctly soldered and has continuity I would recommend to decrease the b0 wire gauge.  But this would only move your problem to a path inside the bms. All power should be traveling through the b- and b0 should only be used to measure cell voltage and balance cell, usually around 50mA.
If you are positive about b- wire I would consider swapping the bms
```

---
## \#12 Posted by: SimosMCmuffin Posted at: 2018-02-22T13:49:47.025Z Reads: 242

```
Can you take a close-up from the marked area?
![image|437x395](upload://hEgUQ6aMNXEscUmPQm5IkCsQFWN.jpg)

EDIT: If possible try to get the markings from the top of the chips
```

---
## \#13 Posted by: SimosMCmuffin Posted at: 2018-02-22T13:55:13.681Z Reads: 239

```
Yea, it's used for monitoring cell voltage, not passing load discharge current.

I'm quite familiar with BMS' and in fact I'm developing an open source one for the community. Having a 100R inline in the cell inputs is not anything dangerous. In fact my current working prototype has them and they are also in the battery stack monitor ICs reference design.
http://www.electric-skateboard.builders/t/flexibms-first-prototype-kicad-project-files-released-flexible-configuration-and-charging-bms/46117

![image|690x340](upload://hX7gu55kK636JLa8YZIfxFDnqHW.png)
![image|689x390](upload://9M5IT3hGx1A4SHum8oirP7d6GvM.png)
```

---
## \#14 Posted by: Kug3lis Posted at: 2018-02-22T17:25:57.526Z Reads: 215

```
Resistor of around 100Ω is used to terminate direct signal and as a small fuse or etc for MCU designs ;)
```

---
## \#15 Posted by: Fiori Posted at: 2018-02-22T20:29:17.707Z Reads: 210

```
No. Evolve BMS has a 65AMP max ouput. That's less than 33amps per motor, which is fine. 

Something has to be hooked up incorrectly here. I used really thin wires for my charging port, and for my bms leads. I haven't had any trouble with melting of wires so far at all.
```

---
## \#16 Posted by: longhairedboy Posted at: 2018-02-22T20:35:18.736Z Reads: 216

```
[quote="BoostedBuilder, post:4, topic:47142, full:true"]
I believe these motors have a 35A - 40A max current limit, why would you want to push 45A through a 50mm, 150KV motor in the first place? Don’t they get boiling hot when you push them? I don’t think that the Evolve system is designed for such a powerful battery. We are talking about 100a continuous current with these cells in a 10s5p configuration.
[/quote]

Doesn't work that way. If it did, replacing the 7.5Ah shit-pack with a 12ah 10S4P 30Q pack would also be a problem as it is capable of 60 amps or more. This is not a problem, i can assure you of that. I've done about 30 of these mods now. 

[quote="krloz, post:5, topic:47142"]
There is not such thing as a very powerful battery.  If I made a 10s20p pack out of 30q wicu can push 300A discharge that in no way means that it is going to push 300A to my motors at all. That depends entirely on how you configure your esc. You will however have a hell of range. If this wouldnt be the case absolutely every board would have a range of approximately 1 hour, or straight up melt…

To week batteries however actually are a thing.
[/quote]

That is correct. 

[quote="HGsystem, post:7, topic:47142"]
My BMS layout:
[/quote]

That wiring diagram is correct. Its possible that you didn't follow it precisely. I know you have probably already done this, but check your wiring one more time. 

Grab your volt meter. Put the negative probe on pin 0 of the balance lead. Then put the positive probe on 1. It should read 3.6 or something, then pin 2 should read 7.2 or close, then each one shouolld be progresivley more by around 3.6 volts at half a charge. if you progressivley move up and the numbers don't get progressively bigger, you have a miswire.
```

---
## \#17 Posted by: pat.speed Posted at: 2018-02-22T20:39:07.526Z Reads: 203

```
Is it possibly that the connection between the main negative lead is faulty and thus the esc is drawing the power through the b0 lead instead
```

---
## \#18 Posted by: Eboosted Posted at: 2018-02-23T00:07:52.908Z Reads: 199

```
Hello, that problem seems to be to difficult to fix for me.

I have an Evolve Bamboo that had died on me last week, I went to check all electronics and it seems the BMS is dead already.

[img]https://i.imgur.com/E6TLB0E.jpg[/img]
[img]https://i.imgur.com/LNGan9H.jpg[/img]

However, this is a good thing for me, I'm sick of the throttle sensitivity, one motor no engaging randomly, low torque at medium speed, I don't like to reengage speed at half throttle when I want to continue accelerating after I left the throttle off.

Dead board, no parts can be purchased through Evolve:
[img]https://i.imgur.com/d4pXxoi.jpg[/img]

This is the perfect time to replace it with a couple of Focboxes and 6374s, a BMS and a Mini remote.

Problem fixed forever

You should do the same.
```

---
## \#19 Posted by: laurnts Posted at: 2018-02-23T01:43:18.251Z Reads: 184

```
My assumption is that the broken BMS / Cut off wire of the main powerline. This enforces high current flowing through the balance port instead of the low gauge wire.
```

---
## \#20 Posted by: darkkevind Posted at: 2018-02-23T12:10:45.823Z Reads: 183

```
From the photo, your BMS is definitely wired up correctly.

In that photo though, there's no discharge wires? Do you have the main discharge wire connected to P- or B-?
Are you bypassing the BMS for discharge and if so, in that case do you have the neg main discharge wire connected to the B- wire and also connected to the B- on the BMS?
```

---
## \#21 Posted by: HGsystem Posted at: 2018-02-23T12:40:12.104Z Reads: 182

```
THANK YOU everybody for your comments so far. Sorry for the delay in responding to your diagnositc questions, I live in Japan so my awake hours are different from yours :slight_smile:

@krloz 
Decreasing the b0 wire guage would have never crossed my mind to decrease current going through it, I would have thought that would only make the problem worse by making it even hotter and melt faster. If anything I would have thought to increase the gauge of the b0 to make it run “cooler”. Can you explain your reasoning?

@SimosMCmuffin
Can you please explain why adding an in-line b0 100ohm resistor would help? Does it cut down on current going through it and redirect it to b- wire? Does doing this affect the b0 sense function when I add the resistor? I am including the closeup view of the BMS that you requested. The b0 attachment you can see is a little browned/melted from the many wire melts that have occured on this lead. Is adding a resister effectively the same thing as down gauging the wire as per krolz’s suggestion (they are both adding resistance to the lead right?) or the electrical effects different of these two options?

@longhairedboy
Here are my BMS leads volt meter readings: b0-0v, b1-3.68v, b2-7.35v, b3-11.03v, b4-14.7v, b5-18.38v, b6-22v, b7-25.7v, b8-29.4v, b9-33.1v, b10-36.7v, battery pack voltage-36.7v. Since you have done so many of these evolve packs now, have you noticed like I have that some of the evolve BMS units do not have b0 wired and some do? 

@darkkevind
Sorry for the confusion, in the original photo I had not soldered all the other discharge wires in yet. No, I am not bypassing the BMS. I am attaching the final BMS layout below where you can see the b-/c-/p- discharge wires correctly attached.

SO, here are my new set of questions:
1) What is the purpose of b0? Not all BMS units have a b0 and I thought the cell balancing of pack #1 is already accomplished with b1.

2) I have redone a very careful comparison of my setup compared to the second stock evolve board I have and I realized they used a 14awg wire for b- and I used a 16awg for my setup...can this minor difference in awg be shunting more current through b0 as a result? 

3) I am using a 10awg for my b+ wire, and as just mentioned my b- is 16awg, Is there a problem caused by having an awg mismatach between b+ and b-? Do you need both wires to have matching awg?

THANK YOU !
```

---
## \#22 Posted by: HGsystem Posted at: 2018-02-23T12:41:16.210Z Reads: 168

```
My BMS closeup pics as requested:
![IMG_1914|690x282](upload://3huizqkHmwHlxf4MHxfdYlUAuhj.jpeg)![IMG_1915|616x500](upload://ueAlEEp5acovfyTps9rVUU0zvzd.jpeg)
```

---
## \#23 Posted by: krloz Posted at: 2018-02-23T14:01:29.763Z Reads: 155

```
[quote="HGsystem, post:21, topic:47142"]
”. Can you explain your reasoning
[/quote]

In AWG big value number means small wire thickness.  And low number means thick wire. 
So with decrease the awg I meant increase the wire thickness.  Sorry for the confusion
```

---
## \#24 Posted by: krloz Posted at: 2018-02-23T14:06:47.108Z Reads: 156

```
[quote="HGsystem, post:21, topic:47142"]
balancing of pack #1 is already accomplished with b1.
[/quote]

Balancing of cell 1 is accomplished between b0 and b1. Balance of cell 2 is between b1 Ann's b2.
The thing is some bms  dont carry a connecting for the first balance wire because it's the same than battery negative, so they just measure there instead.
```

---
## \#25 Posted by: Jumpman Posted at: 2018-02-23T15:33:23.692Z Reads: 154

```
16awg sounds way too thin.  If it was 14awg to start with, definitely dont go thinner than 12awg with your new battery.  I’d probably just use 10awg like the positive wire.
```

---
## \#26 Posted by: Fiori Posted at: 2018-02-23T16:57:56.489Z Reads: 153

```
16 AWG can handle 10amps or even more according to some sources... These wires should have 4 amps MAX flowing through them. Most of the time it's less than 2 amps. I'm sure this is not a wire thickness issue.
```

---
## \#27 Posted by: Jumpman Posted at: 2018-02-23T17:39:25.438Z Reads: 148

```
Even if it can handle 30A that might not be enough for the main negative wire.  I’m not talking about the balance wire.
```

---
## \#28 Posted by: Lambjr088 Posted at: 2018-02-24T01:11:05.192Z Reads: 144

```
I have talk to evolve about the b0 wire because my board came without it. They said that the negative lead that is for the management and not for the straight power is not needed my bms has 11 pins but only 10 wires coming out of it. They said the negative isn't needed when I get a chance I will take pics of my upgraded battery and the bms
```

---
## \#29 Posted by: longhairedboy Posted at: 2018-02-25T01:18:30.969Z Reads: 140

```
[quote="HGsystem, post:21, topic:47142"]
Here are my BMS leads volt meter readings: b0-0v, b1-3.68v, b2-7.35v, b3-11.03v, b4-14.7v, b5-18.38v, b6-22v, b7-25.7v, b8-29.4v, b9-33.1v, b10-36.7v, battery pack voltage-36.7v. Since you have done so many of these evolve packs now, have you noticed like I have that some of the evolve BMS units do not have b0 wired and some do?
[/quote]

That looks right. And yes, the black wire is hit or miss, as is the heat sink and fishpaper on the BMS. 

you just never know what you'll get in there. Expect nothing, be prepared for anything.
```

---
## \#30 Posted by: HGsystem Posted at: 2018-02-25T14:26:07.707Z Reads: 133

```
@krloz
Thanks for fixing my sloppy awg/wire thickness terminology. 

LOOKS LIKE THE PROBLEM IS FIXED!

Thanks to everyones input I changed the b- wire from 16awg to 12awg and i tested with some big hills pulling the max amps (60a total, 30a per motor), the b0 wire is not melting anymore!

As stated previusly the stock b- wire is 14awg and i accidently initially rewired with 16 awg, i am surprised evolve chose the stock 14awg setup...it so close to the margin of safety!

Question:
Can somebody explain why the 16awg resulted in b0 melting? It seems to me if the b- wire was too thin the b- should have been the wire to melt???

@longhairedboy and @Lambjr088
Thank you for confirming that there is a mix of BMS units that use all 11 balance wire and some have use 10 with the b0 clipped. @Lambjr088 please let me know if you can get more info from evolve about this. At first I thought that maybe the older BMS units were 10 leads with b0 clipped and the newer ones used all 11 but I made a VERY INTERSTEING discovery when I compared the 4 evolve gt BMS units that I have: If you look closely there are minor differences on chips/diodes/resisistors on the BMS units depending on the manufacture date/serial number:
The oldest is serial SP-M10-020-A05 date 2016-07-29 —> it uses all 11 leads
The next is serial SP-M10-020-A07 date 2016-10-09 —> it used 10 leads with b0 clipped
Newest (I have 2 from this batch) is serial SP-M10-020-A09 date 2016-12-08—> it uses all 11 leads

If you will notice it is not the newest or oldest BMS units that run 10 leads but the one from the middle date production. Like I said all three of these serials have subtle differences that I can see on the board. I am so curious if there is something we can do so that b0 wire does not have to be used on any of the BMS units (one less thing to break), and I am very curious why it is the MIDDLE production BMS that seems to be configured this way.

Thanks everybody :)
```

---
## \#31 Posted by: krloz Posted at: 2018-02-25T15:22:46.829Z Reads: 127

```
[quote="HGsystem, post:30, topic:47142"]
:

Can somebody explain why the 16awg resulted in b0 melting? It seems to me if the b- wire was too thin the b- should have been the wire to melt???
[/quote]
To small of a b- wire caused a resistance when power was taken through it that caused some of the power to travel through another path. That path being the parallel b0 wire which as we know is not good for any power usage

Simply put.  They were forced to share the power input to the bms And the b0 melted faster than the b- had time to heat up and melt
```

---
## \#32 Posted by: hotzy Posted at: 2018-08-26T21:21:48.939Z Reads: 87

```
Hi, my Evolve Bamboo has the same issue. Can I ask what Focboxes and 6374s, BMS and a Mini remote you went with? I'm think of doing the same. Thanks, Wayne.
```

---
## \#33 Posted by: Zama Posted at: 2019-04-16T00:26:55.338Z Reads: 45

```
Hy guys!

Does anyone know to tell me that effectively serving these cables here that are connected to ESC Evolve?

![05|494x246](upload://5UzGw1MkWMqFiOuQTex8AMRdZd3.jpeg)
![02|348x190](upload://4tB8JOeLW55ylsMJ1Gy0rmaBhov.png)
```

---
## \#34 Posted by: b264 Posted at: 2019-04-16T00:36:46.321Z Reads: 42

```
What is the question?
```

---
## \#37 Posted by: Zama Posted at: 2019-04-16T00:48:41.401Z Reads: 39

```
What’s the function of these cables in ESC
```

---
## \#38 Posted by: b264 Posted at: 2019-04-16T00:52:13.688Z Reads: 38

```
The 4 wires, or the 2 wires?

The two wires I think go to a power switch -- and the 4 wires carry the encryption codes to make the ESC only function from an actual Evolve BMS.
```

---
## \#39 Posted by: Zama Posted at: 2019-04-16T00:57:57.835Z Reads: 36

```
Actually, they all. I thought I was supposed to power switch, too, but there's a way out of the other side that connects the power button, so I m confused. And what would those duties be?![39|420x274](upload://e3mghmlKeaKSchZ73eJqEgqtp3X.jpeg)
```

---
## \#40 Posted by: Zama Posted at: 2019-04-16T01:01:29.919Z Reads: 37

```
[quote="b264, post:38, topic:47142"]
the encryption codes
[/quote]

What do you mean?
```

---
## \#41 Posted by: b264 Posted at: 2019-04-16T01:18:52.988Z Reads: 33

```
The ESC is programmed to only work with an Evolve BMS.
```

---
## \#42 Posted by: Zama Posted at: 2019-04-16T01:24:25.247Z Reads: 34

```
So, just that, it's make sense... I thought UART was some security protocol from coming to BMS. ...and the other switch power on the ESC?
```

---
## \#43 Posted by: b264 Posted at: 2019-04-16T01:25:54.752Z Reads: 35

```
UART is only the protocol it's using to transmit the information.
```

---
## \#44 Posted by: Zama Posted at: 2019-04-25T17:04:33.499Z Reads: 29

```
![4c9543e6-515a-47a9-ac1c-8a3493ad434f|281x500](upload://tSnPoyKbSOFZjQWOzsNvAj78KdK.jpeg) Does anyone know what this function is coming from BMS (BATSW)? What's the use for? Tks!
```

---
## \#45 Posted by: Zama Posted at: 2019-04-25T17:05:50.385Z Reads: 28

```
Thank Yous B
```

---
## \#46 Posted by: b264 Posted at: 2019-04-25T17:14:40.624Z Reads: 26

```
I think that's the power switch.
```

---
## \#47 Posted by: Zama Posted at: 2019-04-25T17:21:11.681Z Reads: 27

```
![790b996d-b157-4201-903e-255f1551b825|690x388](upload://aSLiaRTcel54uXOszAdQq5zSNfQ.jpeg) But... why two connections from the battery?
```

---
## \#48 Posted by: b264 Posted at: 2019-04-25T17:22:44.174Z Reads: 26

```
The two connections are from the BMS inside the battery.

https://www.electric-skateboard.builders/t/help-why-is-my-bms-balance-wire-melting-on-custom-evolve-gt-battery-build/47142/41?u=b264

[quote="b264, post:43, topic:47142, full:true"]
UART is only the protocol it’s using to transmit the information.
[/quote]
```

---
## \#49 Posted by: Zama Posted at: 2019-04-25T17:30:44.320Z Reads: 27

```
Interesting, a tension just for this protocol so :thinking:
```

---
