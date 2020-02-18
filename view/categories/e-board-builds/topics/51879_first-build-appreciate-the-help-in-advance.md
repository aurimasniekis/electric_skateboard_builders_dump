# First Build&hellip;.appreciate the help in advance!

### Replies: 15 Views: 788

## \#1 Posted by: Jps224psu Posted at: 2018-04-10T21:37:31.527Z Reads: 171

```
Trying to keep it all in one topic but realize there are a lot of questions here.  I did the best I could to research as many posts as possible before deciding to put this up....

Quick background:  I bought a Carbon GT last year before i really knew much about E-boards.  At the time it looked pretty sick.  I have since got an upgraded battery from @longhairedboy (Damon is awesome) which was also awesome, buuuuuut after months of reading posts on Esk8 and looking at how sick some of the boards are (@duffman, @longhairedboy, @Nowind, and others) have built are, I think I am ready to try my hand building a mountain board.  I have never built a board before but I am a pretty bright dude who can figure much of it out. (but will definitely need help!)  I have done quite a bit research and have a skeleton of what i want to build but admittedly having no experience building I am certainly up for as much advice as folks will offer or debate on parts.  Here is what I am thinking: 

Rider: 6ft  220lbs/100kg in Long Island (NY) USA
Deck: Trampa Holypro (17ply)
Bindings: Ratchet Bindings Trampa
Trucks: Vertigo
Hubs: Superstar
Tires: Primo Striker
Battery: 12s (suggestions? Was thinking li-ion Samsung 30Q but curious about graphene want to try to make as light as possible)
ESC: was thinking Vesc 6 VS. Enertion FOCBOX VS. hobbyking Max6?
Motor: Leopard 8072 - 175kv (are all of the leopard unsensored?) or APS 8072S 165kv 6000w (leaning toward sensored)
Drive: E-toxx Chain Drive @nowind

Here are some wide open questions maybe folks can point me in right direction:
Remote/Receiver: Enertion nano-x  but wanted something w battery/speed display if possible either in remote or on vesc case any suggestions?
ESC box? If no speed/battery in remote what do I need for esc box to display?
Battery box? Pelican?
Lights (front and rear)? What brands? On a separate battery? 4s 2650?
Fuse?  Not sure exactly what is best for this set up
Cutoff? Not sure exactly what is best for this set up
BMS 12S  XXA?
Power switch? Not sure exactly what is best for this set up
Solenoids? (need one for + switch + battery)

For wiring I have this: 
male to male servo connector
10awg wire
Vesc can bus connector
vesc xt90s
dual xt90 connector
im sure im missing a ton of stuff

Any tools you highly recommended that aren’t obvious?
```

---
## \#2 Posted by: pat.speed Posted at: 2018-04-10T23:02:24.747Z Reads: 137

```
You will need some sort of antispark switch, I would not recommend a Vedder style switch as it probably won’t handle the current of a mtb. Instead I would go with an xt90s loop key or as150 bullet. 

As for the remote there are some that have been designed by forum members that have displays showing data, photon remote is one
```

---
## \#3 Posted by: moon Posted at: 2018-04-10T23:03:30.018Z Reads: 137

```
[quote="Jps224psu, post:1, topic:51879"]
For wiring I have this:

male to male servo connector

10awg wire

Vesc can bus connector

vesc xt90s

dual xt90 connector

im sure im missing a ton of stuff
[/quote]

Loctite red and blue
```

---
## \#4 Posted by: Grozniy Posted at: 2018-04-11T12:52:31.687Z Reads: 100

```
You could go with focboxes. Cheaper then vesc6, better then esc.
Liion last longer and are safer. Take less space. 30q are perfect. But you need a spot welder service. 
Bestech bms around 80amp
Enclosure: is it for off road or urban? For urban get something like @Eboosted sells for enclosure. For off road, get a top mounted box with the batteries.
Sensored motors are always better but not necessary.
Like @pat.speed said, make xt90s anti spark loop key.
Get a hm10 Bluetooth module and connect to @Ackmaniac app. It will show 🔋, speed, load, etc.
Get crash protection gear: helmet, pads, gloves,etc
```

---
## \#5 Posted by: Jps224psu Posted at: 2018-04-11T13:19:10.838Z Reads: 89

```
thanks will look into the xt90s loop key and wiring I know i have seen plenty of posts w some schematics.  thanks!
```

---
## \#6 Posted by: Jps224psu Posted at: 2018-04-11T13:21:21.284Z Reads: 86

```
thanks! @nowind loves loctite 603 and 243 (as portrayed in many posts :slight_smile) so was going with that
```

---
## \#7 Posted by: Jps224psu Posted at: 2018-04-11T13:28:12.871Z Reads: 90

```
any performance diff or downfall to using the focbox?  Im not really trying to spend a ton but also not trying to save if a product is superior.  I have been reading all about the batteries i think i will go for a spot welder and other equipment needed and see how big of a fire i can start :joy: 

Good to know on the Bestech BMS.

This board will primarily be used offroad...any onroad will just to be to get to offroad.  What top mounted boxes to people recommend? I keep reading pelican's rule.

thanks for advice on @ackmaniac app 

As for crash protection i already "exploded" my shoulder and had total reconstructive surgery due to a major wipe out on Carbon GT.:open_mouth:  As they say, "safety is no joke!" :flushed:

appreciate all the feedback will continue to adjust my list accordingly

as for the battery i was thinking 12s4p or 6p what do folks think?  In that range higher/lower?  I want to bea able to jump at a standstill so dont want cement on my feet.
```

---
## \#8 Posted by: DeathCookies Posted at: 2018-04-11T13:48:27.135Z Reads: 83

```
(assuming Samsung 30Q)
12S4P = 532,8WH ~ 25km ~ 2,4kg 
12S6P = 799,2Wh ~ 35km ~ 3,6kg

Most People use a 12S4P for lighter weight but some People Need more range. It depends ob what you want
```

---
## \#9 Posted by: Jps224psu Posted at: 2018-04-11T16:30:54.530Z Reads: 77

```
Thanks @DeathCookies i think i prefer some range over weight. Im in good shape so a couple pounds shouldnt kill me for the extra 10km. Good trade off.
```

---
## \#10 Posted by: Jps224psu Posted at: 2018-04-13T20:02:07.846Z Reads: 72

```
started ordering the parts see below...to be honest i am a bit overwhelmed with the battery design and what is needed.  I have read through many battery posts looking to build a 12s6p does anyone have detailed instructions or parts needed I cant seem to find it all in one place?

1 x VERTIGO Mountainboard Deck with CNC lite 12mm HOLLOW Axle Trucks 
     - 35º HOLYPRO Deck Shape 
     - 17ply 35º HOLY PRO Deck - Stiffest 
     - GUNMETAL Anodised with Black logo 
     - GREEN DAMPA's - 75a Firm Steering
     - Powder Coated RED Springs
     - Please fit 5 Spoke SUPERSTAR Hubs 
     - Matt Black Rim 
     - GUNMETAL Anodised Spokes 
     - 8 Inch BLACK Primo STRIKER Tyres 
     - RED ATB Bearings - 12mm Axles 
     - RATCHET Style Bindings please 
     - Black Strap with Red Foam Footstraps 
     - BLACK with SILVER logo L-Brackets 
     - GUNMETAL Anodised Ratchet Buckles 

1 x Heel Straps with RED Ratchets
     - Red Camlocks

1 x 16mm Carbon Fibre Multi tool for TRAMPA 12mm Axle Decks 

1 x 2x VESC 6 In CNC T6 Silicone Sealed Aluminum Box with Genuine XT90 Connectors - Vedder Electronic Speed Controller TRAMPA Special
     - Yes please add 2 x External Silicone Seals 
     - Yes please supply me with 2x Single VESC mounting plate 
     - Yes please supply me with 1x 10cm CANBUS Cable
```

---
## \#11 Posted by: Jps224psu Posted at: 2018-04-13T20:03:03.548Z Reads: 66

```
I really dont want to punk out and buy the assembled battery! :confounded:
```

---
## \#12 Posted by: Jps224psu Posted at: 2018-05-23T13:38:10.807Z Reads: 54

```
![image|666x500](upload://9D1UUK1HeXxW8yLq1UaVpkONfJ1.jpeg)![image|375x500](upload://o3nzWy5xbPgtPLhbjdu3NtYjqC1.jpeg)![image|375x500](upload://xNSu2cPJLcDv5vA39y1iG69L6w3.jpeg)![image|375x500](upload://1q9tCf9hYnVwgnjmTkiZdjjW8y5.jpeg)![image|375x500](upload://uzys6FGWGMDPueMHkQ58GMRhd8H.jpeg)![image|666x500](upload://qttbjLCu9RXa08P67sjKW0fjII6.jpeg)![image|666x500](upload://fvSHYWGra6eQhras8kaq5TDktE2.jpeg)![image|375x500](upload://4utt3CRvd9GCaP5RkZxIrzZi4tQ.jpeg)![image|375x500](upload://2JeD1x0nQtNoSae2XrcnzhNFR6n.jpeg)![image|375x500](upload://22yM4qIL6CFZQqyXzd0P3VOUX7l.jpeg)![image|375x500](upload://xNARh3BAX5IKaXSv2baJRZhFOKf.jpeg)![image|666x500](upload://AvkHb4S4B0wz7bXYsGdhECaQmE3.jpeg)![image|375x500](upload://XkKILldxw4G4mgHzQMRhHUeh8k.jpeg)![image|666x500](upload://ltlQ0bA0Vf14EddiLbqo3G6bRin.jpeg)![image|375x500](upload://tOpkQTKvdwQAv21otpJFj7jeDf0.jpeg)![image|281x500](upload://egpQKCwqB8Lhu7Wm7Wi71KIDuRn.jpg)
```

---
## \#13 Posted by: NoWindCH Posted at: 2019-06-23T13:14:50.661Z Reads: 29

```
Hallo can you help me yout how the pins are from the APS to the Vesc (yes on the Vesc it is written)

Do i have to change the order of the pins of my APS 8085?

How did you the connections of the Hall sensore?
```

---
## \#14 Posted by: Jps224psu Posted at: 2019-06-29T15:31:39.875Z Reads: 24

```
Hey should be marked up in drawings with the connectors you need and color coded. But yeah you usually have to play around w vesc to motor wires depending on how you plug them in they may spin diff ways or not at all. Let me know if u figure out combo if not i can take pics of how i have them and send.
```

---
## \#15 Posted by: NoWindCH Posted at: 2019-07-04T18:26:59.862Z Reads: 18

```
i have it done itr workes good!
but sad the 8085 have no temp..

i found the solution in the forom by surching

thenks
```

---
