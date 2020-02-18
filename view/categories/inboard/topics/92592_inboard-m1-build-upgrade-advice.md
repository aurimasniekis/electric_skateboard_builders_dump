# Inboard M1 build/upgrade advice

### Replies: 46 Views: 1762

## \#1 Posted by: maddec Posted at: 2019-05-02T20:12:19.408Z Reads: 217

```
Hello everyone, I bought the M1 almost 1 year ago, when I was a total noob about everything regarding electric skateboards. I use it almost everyday to commute to work but I almost regret buying it now that I've spend some time reading this forum and learned more about other brands and custom builds, also the huge price drop!

Some background:

After one month the first board died with water damage and that's when I realized it wasn't at all waterproof. Luckily I got it from a local store and they sold me as waterproof so they gave me a new one.
Then I started googling because I was pretty sure the Inboard was waterproof, that's when I found out this forum and this post:
https://www.inboardtechnology.com/blogs/behind-the-design/2017-1-20-water-resistance-battery-safety-update

> Blockquote Inboard cannot 100% guarantee weight shifting won’t briefly break the seal of the battery lid while the battery lid flexes. 

The lid isn't the only problem but, in their defense, I only got the first gen.. they made small updates after that so I can't tell if that's improved.

Finding this forum was the only good outcome of that episode, so I thrown my warranty away, opened it and with your help I made it waterproof myself. That worked for almost a year but last week I opened for maintenance.. was lazy to make it water tight again and well... a puddle fried the ESC almost instantaneously.. my bad I know.

I was mad at first that I just lost 1.2k euro.. but I started reading more and more here and figured out it not so hard to fix the board and probably make it even better than it was before.

Rebuild:

Ofc I need a VESC so I'm thinking Flipsky Dual FSESC4.20 Plus that seems compatible with 12s1p (can anyone confirm that? I get mixed opinions and confusions btw the normal and plus version).I'm also open to other VESC suggestions.

I want to have telemetry in the remote and some way to control/play with the M1 lights like flashing when breaking, on/off etc. The Advanced Electric Skateboard Remote seems to be a great option, what to you think?

I started doing some clean up:

![20190428_183458|666x500](upload://wF2JttGdmOUR1DriHpM7W9UkSDo.jpeg) 
![20190428_183526|375x500](upload://2wxeBKtNZzvnbIGDMARSRDgc7zq.jpeg)

They look good know but one of them had a bit of corrosion and dirt in the magnets.

This is the fried ESC:

![20190502_200045|374x500](upload://2iFZqeNZ1QYtrWApAgnDzL9YHnv.jpeg)
![20190502_200128|375x500](upload://kWs8HW50BdcbG4pQjc6H6jmIPOm.jpeg) 
![20190502_200123|375x500](upload://8Hiw85ng6REekSnzMsTemWPH3sU.jpeg)

As you can see the connectors for the sensors are standard and the pcb even has the order of the wires printed. I think I should have no problem connecting the motors to a VESC. So the plan here is just to get a VESC, remote, receiver and have the light controlled with the remote and telemetry

![20190502_195851|374x500](upload://u7X409jnb8HZu16sng7zUjtU348.jpeg)

Questions:

- Is Flipsky Dual FSESC4.20 Plus + Advanced Electric Skateboard Remote + receiver a good combo?
- I plan to upgrade the battery in the future but for now I'll just use this 12s1p, I think it already as BMS? Would it be fine connecting directly to the VESC?
- What parameters (mins/max's) should I use for the inboard motors?
- Will there be enough current in the receiver to power the lights? How can I test that before hand?
- The board as two connectors for heat dissipation plate underneath (they say it's used for regenbrakes when battery is full) can I somehow take advantage of that? See pic bellow:

![20190502_200209|374x500](upload://dQODYLcA0kv34UJ9BSKb5X5bR.jpeg) 

Overall I still love to ride this board and I hope with your help I can make it better than before. I don't need range and insane top speeds, I need to be able to travel with it and get to work everyday even if it's dripping a bit.

Sorry for the long post hehe.. any feedback would be greatly appreciated. Thanks!
```

---
## \#2 Posted by: Popeye2719 Posted at: 2019-07-07T22:06:59.830Z Reads: 165

```
I have a broken M1, something happened to the ESC, so I bought a VESC to replace the old one.

Unfortunately I can’t manage to complete the motor calibration, I have a problem with the resistance reading 0. 

Did you found a way to make it work?
```

---
## \#3 Posted by: maddec Posted at: 2019-07-08T12:44:02.987Z Reads: 160

```
@Popeye2719 Yes I was able to change to Flipsky Dual FSESC4.20 Plus. I did not have any issues with the calibration.

You should try to calibrate one motor at the time and see if that happens on both. What VESC do you have?

Btw, you will notice a difference with the new vesc hehe. I put mine in FOC mode so I lost a but of top speed but it's buttery smooth and makes no noise.

I'm also trying to figure out a way to connect the original lights to the VESC, I will try to update this thread when that happens.
```

---
## \#4 Posted by: Popeye2719 Posted at: 2019-07-08T19:37:33.126Z Reads: 151

```
I have the exact same setup, I’m using the Flipsky 4.2 plus with the power shift battery and the manta drive motors. So everything but the ESC is original from Inboard.

I have 3 motors (all from inboard) and one of those is brand new and I have the same problem. I think it might have something to do with the VESC, or maybe (probably) I did something wrong.

What where the specs you used for the battery? Can you show me how/where you conectes the motor sensors to the ESC?

The problem is that the hall sensor setup always fails. So I’m only able to finish the setup as a FOC sensorless. And I’m not sure if that could damage the motors.

How did you did the setup?
```

---
## \#5 Posted by: maddec Posted at: 2019-07-09T08:15:42.822Z Reads: 136

```
@Popeye2719 Fun to see someone going through the same as me and having the same idea.
I'm at work at the moment, when I get home I'll post some pictures and information about my configuration and the tutorial I'v followed to setup VESC. Hold tight :slight_smile:
```

---
## \#6 Posted by: MysticalDork Posted at: 2019-07-09T08:51:35.172Z Reads: 132

```
If you have the extra cash and room, I'd recommend spending the extra $70 for a FSESC6.6, instead of the 4.2. The 4.x hardware had some flaws that caused issues for me (Blew DRVs at 10s on the maiden ride of both my original vesc 4.12s) and a lot of other people, especially at 12s. I know Flipsky and others have made improvements to the 4.x design over time so I can't say outright that it'll be problematic, but the 6.x design is just better IMO.
```

---
## \#7 Posted by: maddec Posted at: 2019-07-09T10:33:58.273Z Reads: 126

```
You are right, the 6.6 is superior in every aspect, but are you talking about regular 4.2 or the PLUS?
I have the plus and run in with the original Inboard 12s and never had any issues, I run it on low amps tho, maybe that's why :stuck_out_tongue:
```

---
## \#8 Posted by: MysticalDork Posted at: 2019-07-09T18:59:31.765Z Reads: 113

```
I have no direct experience with the plus, but I have a bias against anything 4.x in general from my own problems, and seeing lots of others. The 4.2 plus may be perfectly capable and have no issues, but if I were in the position to choose, I'd most likely spend the extra money just for peace of mind. :P
```

---
## \#9 Posted by: AlanZhou Posted at: 2019-07-09T19:29:20.958Z Reads: 111

```
I'm surprised imboard's esc runs on DRV8302.
```

---
## \#10 Posted by: Notbig Posted at: 2019-07-10T17:51:09.985Z Reads: 116

```
Just finished my setup with Vesc 4.20, there was some issues that I encountered, like some here I got incorrect readings and noticed that the Hall Sensors from the Manta Drive were not the same as it should be on the Vesc, after changing 4 of the cables stuff started to work like it should!
Also running this as FOC  since that gave the best results maybe lost some at maximum speed but think it is enough 🤔
Still got some issues for the remote that I bought VX1 from Flipsky, don't get the different speed settings to work as they should so if anyone got a clue about this that would be great to get that info!
```

---
## \#11 Posted by: Notbig Posted at: 2019-07-10T18:02:36.927Z Reads: 114

```
Can you tell me your setup, think that I have done something wrong but sure, far from a pro builder?
```

---
## \#12 Posted by: maddec Posted at: 2019-07-11T17:01:24.783Z Reads: 113

```
I'm also not a pro builder, but I'll share my setup with you guys as soon as I can. Very busy with work atm.

With FOC is normal to loose top speed but you get less noise, if you go for BLDC mode you will get the top speed but more noise. It's way more complex than that but you get the point :wink:
Also add the same issue with the Flipsky VX1 remote, but it's not an issue at all. The speed modes of that remote don't change the topspeed, they only change the acceleration curve. If you go full throttle in the lowest setting you will fell way less acceleration. It works, just not as you expected :stuck_out_tongue:

In my board I only switched one wire, I think the temperature one but not sure. The order of the sensor wires don't matter. I'll show more details when I share my setup. Hopefully this weekend.
```

---
## \#13 Posted by: Notbig Posted at: 2019-07-12T22:09:13.919Z Reads: 107

```
Might help me getting the correct break settings, probably set the Amps to low but really not sure about anything 🙄
```

---
## \#14 Posted by: maddec Posted at: 2019-07-14T10:19:57.004Z Reads: 111

```
@Popeye2719 @Notbig

Here is my setup. First the order of the sensor wires:

![2019-07-14|666x500,50%](upload://qcowf0qHnd3T6VLFIsPRVcevCT6.jpeg)

I think I only switched the temperature wire with one of the sensor wires. You can use a nail to do that.

This is the configuration per VESC (same for both):

![09|690x231,50%](upload://iFs3rO69hbwfcFjlnLeH2rUcI0I.png) 

I think I'll increase the brake to -30A, I hope it will be the sweet spot.

And the battery (for original powershift):

![21|690x231,50%](upload://lCBYXsHSGXjSFyiDm56iXT1DQTM.png) 

Let me know if you need anything else. Hope it helps :slight_smile:
```

---
## \#15 Posted by: Notbig Posted at: 2019-07-16T09:26:17.995Z Reads: 97

```
Thank you very much, I think that I have set the Battery Current a lot lower not sure it is good or not so thinking about set it up like you! 
Happy rides 😃
```

---
## \#16 Posted by: maddec Posted at: 2019-07-17T12:14:22.194Z Reads: 96

```
I've been using this setup for 3 months daily with no issues. But I only ride in flat surfaces, there are no inclines in the Netherlands :stuck_out_tongue:

I think is much better than the original, the only thing I lost is a bit of topspeed. And that is actually a pro for me because I want to attract the less attention possible hehe
```

---
## \#17 Posted by: Notbig Posted at: 2019-07-17T15:50:52.663Z Reads: 90

```
Got a bit more hills to go over here in Sweden then 😂
```

---
## \#18 Posted by: linkus Posted at: 2019-08-31T12:07:08.127Z Reads: 87

```
Hey, how have you managed to open up the manta drives? I've been going over my head trying to figure that out. Mine don't want to open up. Got them off the truck, managed to remove the outer bearing, but the inner side I just can't figure out...
```

---
## \#19 Posted by: maddec Posted at: 2019-09-02T20:30:09.136Z Reads: 91

```
You don't need or even should take the bearings before opening it.. hehe

If you take a look at the side covers of the motor you will notice that one of them as bigger lip (the one facing the inside of the motor). That's where you need to open it. One of mine got loose easily but the other didn't. You should use a rubber hammer or something not too hard and hit it a little until you see a gap, then use some pliers to open a little bit more and it will get loose. It will not look like it because the magnets inside are very strong but just pull it out firmly and carefully to avoid scratching the magnets. 
No brute force needed at all :stuck_out_tongue:
```

---
## \#20 Posted by: Hansdieter Posted at: 2019-09-02T23:04:23.055Z Reads: 85

```
 @maddec so i have nearly the same problem, need a new Mainboard. 
So with the  Flipsky Dual FSESC4.20 Plus i still can use the og inboard battery ? is that right ? Could you aktivate the regenerative brake ability ?
And :D
(In my board I only switched one wire, I think the temperature one but not sure. I Ithink I only switched the temperature wire with one of the sensor wires. You can use a nail to do that.) what ya mean with that.
Please help me to keep ma board riding ;)
```

---
## \#21 Posted by: linkus Posted at: 2019-09-07T18:49:14.256Z Reads: 70

```
Thanks a lot! Finally took them apart!
```

---
## \#22 Posted by: Bingo Posted at: 2019-09-16T01:28:35.207Z Reads: 61

```
So I am new to the forum and new to e-skate in general and just got a used m1. I want to make it water proof so that it won't die on me in the occasional drizzle or rain. Any ideas as to how I can carry that out? Thanks
```

---
## \#23 Posted by: maddec Posted at: 2019-09-20T18:26:20.246Z Reads: 60

```
Yes you can do all that :slight_smile:

Check your motor sensor wire and compare the order of the colors with my picture above, you will see the difference :P
```

---
## \#24 Posted by: maddec Posted at: 2019-09-20T18:36:02.678Z Reads: 62

```
Water only come from the top and sometimes from the bottom where the wires enter the board.

The bottom one is easy just use silicone or similar. The top part is hard to make sure it wont leak inside.. To be honest the only thing I would kinda trust would be something like this (IF its waterproof):

https://www.evolveskateboards.co.uk/collections/accessories-1/products/bamboo-board-cover
```

---
## \#25 Posted by: siftingsands Posted at: 2019-09-23T05:01:16.342Z Reads: 59

```
Hey guys!

I'm new to the to the forum and have owned a m1 for a while. Recently I fell and broke my remote. I was looking through the forums and it seemed like you are able to use different remotes to pair with various ESCs. I wanted to see if it was possible to pair a different remote to the stock ESC.

I apologize if this isn't the right place to put it. 

Thanks!
```

---
## \#26 Posted by: maddec Posted at: 2019-10-01T09:56:38.971Z Reads: 56

```
@siftingsands you can pair different remotes on a VESC, not on a ESC usually. I replaced the original ESC with a VESC that is why I'm able to use a different remote.

You will need to buy a new one from Inboard and follow the instructions to pair.

Btw, I hope you didn't get much hurt :slight_smile:
```

---
## \#27 Posted by: Thumbs Posted at: 2019-10-01T13:23:00.183Z Reads: 55

```
Thanks for all the information!!! 
My M1 fried itself the other day- plugged in the battery and heard a sizzle followed by smoke. The circuit board compartment was covered in soot and the board was fried at least around one of the mounting screws.

In any case, since Inboard has gone out of business we are on our own to fix these things. That's why this page may become very popular!

In reading, the Flipsky 4.20 is not recommended for 12s batteries which I think is what the M1 uses. People are making it work but who knows for how long and how hard they push their motors. If you never go beyond 3/4 throttle and never go up hills you aren't pushing a lot of current through the ESC and the 4.20 Plus may work fine. 

The recommended ESC is something equivalent or better than the Flipsky 6.6. That one has the ability to use newer/more powerful batteries. If the rest of the board lasts long enough to need a new battery you will be able to upgrade to whatever the best tech is at the time rather than being limited to old battery chemistry/tech. 
Note that the compartment for the circuit board is ~112mm x 96mm (roughly- measure to be sure!).The regular FSESC 6.6 does not fit. I had to order the FSESC 6.6 MINI or you could order the FSESC 6.6 Plus as it will fit as well. The Plus gives you the option of running a 4 wheel drive (4 motor) board but is otherwise (I think) about the same as the MINI. 

Here is what I ordered:

Dual FSESC6.6 Based upon VESC6 with Aluminum Heatsink Mini Size
$183.20

Anti Spark Switch Pro 280A for Electric Skateboard /EBike /Scooter/Robots
$31.19

2.4Ghz Remote VX1 for DIY electric skateboard For VESC6  
$39.19

Bluetooth Module 2.4G Wireless Based upon the nrf51_vesc project For V4 (Diagram shows it with FSESC 6.6 too)
$7.93

XT60 Male & Female Connectors Plugs 10 Pairs
$4.01

|Subtotal|$265.52|
|Shipping|$27.50|
|Total|USD $293.02|

I don't know if I needed the new remote and probably didn't need the bluetooth but I think that will make setup easier.

Hopefully the battery and motors will last long enough to make this a good purchase. Worst case scenario, I have a good start on a DIY board build.
```

---
## \#28 Posted by: Thumbs Posted at: 2019-10-01T13:33:17.707Z Reads: 53

```
You won't be able to make it waterproof by adding silicon or anything like that- the water will seep in to the motors and cause problems. If you ride in the wet you will always be taking a risk with these boards. A light splash may not be a problem but a long ride on wet pavement is probably going to cause motor problems at some point. 

The battery is well sealed and the circuit board is.... well.... They sealed it up pretty well. I don't know if mine failed because of moisture, poor circuit board quality, or poor circuit design (not able to handle the power long-term). I think it was a poorly built circuit board AND not robust enough to handle the power. 

There was no indication of water ever getting in to the battery box nor the circuit board compartment despite some wet adventures. I haven't disassembled the motors yet but will try to update this forum when I do so.
```

---
## \#29 Posted by: Thumbs Posted at: 2019-10-01T13:35:14.781Z Reads: 48

```
I wonder if it is possible to plug a new receiver in to the existing circuit board. If so, a new $49 remote with included receiver would be an easy installation/solution.
```

---
## \#30 Posted by: maddec Posted at: 2019-10-01T18:46:57.928Z Reads: 46

```
@Thumbs welcome to the forum :slight_smile:
 
The battery compartment is very small too so I don't see a way to put something in there that my 4.20 Plus cannot handle. It has no issues with 12Ss.
But your setup is better and almost the same price I got my stuff so it's a better choice now. And like you said it's a good start for another build if you decide to do that later.

I think the motors are fine with water.. it's the dirt that comes with it that will cause problems.  I try to avoid it but I use mine on wet conditions quite often. I have the version with holes so I covered them and I open and clean the motors sometimes. I clean the bearings more often and also replaced them once.

> I wonder if it is possible to plug a new receiver in to the existing circuit board. If so, a new $49 remote with included receiver would be an easy installation/solution.

I think if that is possible it will be anything but easy to do hehe
```

---
## \#31 Posted by: BD0G Posted at: 2019-11-09T00:18:28.764Z Reads: 41

```
Thumbs ,

I am in a similar situation with a mainboard / ESC on my M1 that has a fried diode. Purchased it that way so that I could come up with a solution to fix the board and make it useable. Any way you could document the links to the parts you are going to be using and a step by step as you work on this solution? It would serve as a great roadmap to others that need to come up with a way to solve a fried ESC/ mainboard issue on the Inboard M1.
```

---
## \#32 Posted by: Thumbs Posted at: 2019-11-09T01:21:44.321Z Reads: 40

```
I will do my best. Stuck right now because I got superglue in the holes of the little white connectors and now I need to figure out what size it is to get a replacement.

The parts look like they will fit with some modification of the layout. The circuit board is larger than the factory one so it fills that space. I think pushing the wires outside of the black box will let everything fit.

Out of town right now but will try to get moving on it next week.

Message me to remind me if I don't update soon!
```

---
## \#33 Posted by: BD0G Posted at: 2019-11-12T00:10:16.560Z Reads: 39

```
I am interested in any and all updates as I may be forced to travel down a similar path. I have a board with a bad mainboard so I want to find a good reliable working solution to replace the electronics / remote , etc.

I can learn from any pitfalls you may encounter along the way. First one I learned is to not get super glue in any of the connectors . :) LOL
```

---
## \#34 Posted by: Thumbs Posted at: 2019-11-12T02:03:04.862Z Reads: 38

```
Hehe. Yeah, so when you switch those wires on the little white connector coming from the wheel motor, be really careful pushing the pins out of the connector. If they are loose I'd use hot glue to secure them instead of super glue! Maybe the thick gel super glue, just not the watery stuff.
```

---
## \#35 Posted by: BD0G Posted at: 2019-11-14T05:46:28.891Z Reads: 39

```
If you have to just strip the wires and solder them. Heat shrink tubing over the solder joints.
```

---
## \#36 Posted by: Thumbs Posted at: 2019-11-14T12:52:22.055Z Reads: 37

```
I was hoping to keep it easily reversible since it is my first build. I guess getting it finished would be better!

Not sure my soldering skills are up to the task on those little pins. I drilled it out, need to check the continuity. Some sort of conductive glue/putty/filler that could go in the holes, tiny drop in each, would be great.
```

---
## \#37 Posted by: BD0G Posted at: 2019-11-14T21:50:16.187Z Reads: 37

```
I could do it if you were close by.
```

---
## \#38 Posted by: Leggera Posted at: 2019-11-17T15:12:33.966Z Reads: 31

```
 

I just bought an ownboard kt mini for a bit of fun recently and its pretty good so far but my brother found an m1 in the trash. What would you do with it? Are the motors better than the ownboard?

Or does anyone know a cheap esc that will work with it as hes on a budget. I can build the battery ok 12x40t 21700 maybe. There is some arcing on the phase wires but once unplugged the motors turn fine. Thanks if anyone can help.
```

---
## \#39 Posted by: BD0G Posted at: 2019-11-18T17:18:12.250Z Reads: 31

```
You will probably want to follow this thread and see how @Thumbs makes out with his modifications.
```

---
## \#40 Posted by: Thumbs Posted at: 2019-11-18T18:17:57.172Z Reads: 30

```
The Flipsky 6.6 Dual is about $220 and does fit in the board with some minor modification to the board. Definitely not cheap. The up-side is that the Flipsky can be used on high-power systems so it can pulled out of this board and put to use in something else two years from now. Heck, they even use it for electric surfboards, etc.
```

---
## \#41 Posted by: Thumbs Posted at: 2019-11-18T18:18:53.214Z Reads: 28

```
I think you can make a 4+ series VESC work if you don't go full throttle with it. Definitely a lot cheaper, and easier, route.
```

---
## \#42 Posted by: Leggera Posted at: 2019-11-19T02:00:01.468Z Reads: 26

```
Ok thanks i did think it would be cool to buy an focbox or something to spend a few months on the m1 till its toast and pop the esc in my kt mini. At least then its not a one use purchase. He will only use it for flat beach rides so i should just go for cheap and cheerful like the 4 wotsit mentioned. I do prefer plug and play

My brand new ownboard motor has stripped thread bolts so guess ill be upgrading that piece of poop too haha. The bolts only engages 3 threads. 

The M1 has magic smoke possibly from arcing at the phase terminals. Motor had resistance but is fine once disconnected

Anyway will watch what goes on here thanks :)
```

---
## \#43 Posted by: Leggera Posted at: 2019-11-21T02:18:26.947Z Reads: 25

```
As im just looking at beach front cruising would something like this do?

https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.co.uk%2Fulk%2Fitm%2F113975660167
```

---
## \#44 Posted by: ripinboard Posted at: 2019-11-27T23:45:20.970Z Reads: 24

```
what did you use to clean your motors? I was thinking of using isopropyl alcohol and qtips but just want to make sure I am not going to mess up anything lol.
```

---
## \#45 Posted by: v01t Posted at: 2020-01-25T13:10:56.244Z Reads: 13

```
thanks a lot guys for information, it help me a lot.
I'm on the beginning of my journey to replace original ESC and battery in my m1 and will be glad if someone can help me with the following questions:
- As my battery already dead, I need to replace it, I read several topics here and got impression that I need to invest some more time in that field in order to find the best alternative, someone post link with [esk8 Calculator](https://calc.3dservisas.eu/) that I found quite useful, but in order to use it in full I need to know motor specs (kV, poles, W, Wh/km) I would greatly appreciate if someone would share at least average values for it. So far I cant decide between 12s1p of Samsung 30Q or Samsung 30/40t.

- Second step is to replace original ESC with [Flipsky Dual FSESC4.20 Plus](https://flipsky.net/collections/electronic-products/products/dual-fsesc4-20-100a-plus-based-on-vesc-with-anodized-aluminum-heatsink) and I'm curious about two things: (a) can I switch 4.20 Plus to CAN bus single mode (4.20 has external switch for that) to have a [traction control](https://www.youtube.com/watch?v=PL0TPdrhMuI&t=558s); (b) possibility to turn off/on motors (1wd/2wd switch) on the go is there any way for that? as this would help to save some battery and increase distance.

Will greatly appreciate any comments, doubts, ideas.
```

---
## \#46 Posted by: tflynn Posted at: 2020-02-06T18:47:05.933Z Reads: 7

```
Battery died during an update. Now it’s stuck in pairing mode. Killed batteries and fully recharged. Lights on board and remote just blink slowly. Not pairing or responsive. Any advice is greatly appreciated!
```

---
