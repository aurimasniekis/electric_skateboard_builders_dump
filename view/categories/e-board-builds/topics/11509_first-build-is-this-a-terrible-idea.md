# \[First Build\] Is this a terrible idea?

### Replies: 14 Views: 1296

## \#1 Posted by: Aborn Posted at: 2016-10-20T01:30:26.212Z Reads: 141

```
**Hello**
I am a 17 year danish student who thinks electric skateboards are cool!
also i like building stuff, soldering electronics etc.

I've been looking around on prebuild board, and they alle seem to be very expensive, which i belive is fair, since it's a lot of work to design and manufacturer. What i've also noticed is that they all have quite small batteries. Boostedboard for and example has about 12 km(8 miles) of range, with a what 4800 mah battery? 

Why not just strap a huge battery underneath the deck?, i mean the space is there, and the weight of 18650's is not a problem

**What i want**

I have a 15 km comute to and from my school, that's at least 30 km a day, and i dont want to go slow either, i have some very long and safe streatches where i want to be able to achive some speed;


*Tell me if this build is a terrible idea or what:*

**Battery**
I want 96     18650's in a batterypack strapped under my board; 12S8P
i did the math, and a battery like that would be 43 cm ( 17' ) long, 13 cm ( 5' ) wide and a bit under 4 cm ( 1.5' ) high(tall whatver);
dont know if that's too long?, could also cut down to 10S8P as 36V would probably be enough, and that would cut the length down to 36 cm ( 14' );
that''s give me 44V and about 22 Ah
Also i will be able to purchase cheap cells, as a bit more than 2C discharge rate will be enought to get about 60-80 amps;

for the casing i would possible go with some aluminium and creating a housing for the battery, and the electronics with some sheets;

I've played around with 18650's earlier and have the soldering skill to make a pack like this;

**The Drive system**
I want to create the drive system for the board my self, with truck's that i will purchase, and a metal plate mounted to the truck, and the motor will mount on that; i'll asume you know how a basic one motor drive system works;
Also i will fire some nuts through a wheel and mount the pulleys and stuff there, you know how it goes;

I have access to a metal workshop through my school, so i have access to welding and to make the very simple parts for the drive system (Not the pulleys)

**The Electronics**
I have a remote from an old RC car (Not the little toy ones, the ones that you custom build that goes 80km/h)
from that i will harvest my controller and receiver;

The motor i will get from hobbyking or something, it will be around 190kv and be on 2500-3000 watts;
I'll get one of those fance VESC and figure out to program it to run nicely with my controller, that shouldnt be a problem:

Also i will need some kind of battery protection circuit, which i am unsure of is build into the VESC;

**The Deck**
This is where i am kindof on bare ground; I will need some very stiff wood, because if the deck is too flexy, the huge battery pack mounted underneath will not have a good time;

I'd like to know which kind of wood would be good to use, i'd like to know how long the board should be, and what shape; Also i would like to know where you can purchase thin boards of wood;

I am about 182 cm tall, and weigh around 70 Kg,
Also i would like to build the deck my self, and preferably not purchase one; 

**Thank you**
For reading this, please give me some feedback and some helpful ideas, critics or anything else you can think of

*sorry about all the semicolons, im a programmer;*
```

---
## \#2 Posted by: susplus Posted at: 2016-10-20T18:56:41.297Z Reads: 87

```
u can use this calculator to have some info about top speed:

http://calc.esk8.it/
```

---
## \#3 Posted by: susplus Posted at: 2016-10-20T19:07:14.319Z Reads: 83

```
here\s a shop for boards :D 
 www.sickboards.nl
i have recently bought a Xtension Boards..Maverick which has a good wheelbase ( the longer the more stable at higher speeds) thickness is about 16 mm and seems to be sturdy enough for more than 100 kg. Also it is very stiff. 
Some people may prefer more elastic boards which are good for carving and such but i sincerely prefer a stiffer board as electric skateboards and carving ( in my opinion ) don't really go together that well unless you are extremely good at it;)
```

---
## \#4 Posted by: susplus Posted at: 2016-10-20T19:09:15.157Z Reads: 77

```
[quote="Aborn, post:1, topic:11509"]
Also i will need some kind of battery protection circuit, which i am unsure of is build into the VESC;
[/quote]

look for the vedder anti spark Switch ;)  here's a link 
http://www.electric-skateboard.builders/t/vedder-anti-spark-switch-v1-3-kit/9949/31
```

---
## \#5 Posted by: Aborn Posted at: 2016-10-20T21:13:13.632Z Reads: 60

```
Thanks it seems like 12S will let me go about 48 km/h which is plenty, do you know how well you can break on those boards?, i know the motors can break quite hard, but how fast can you stop without flying off the board?
```

---
## \#6 Posted by: Aborn Posted at: 2016-10-20T21:16:02.318Z Reads: 56

```
I deffinitely prefer a stiff board, as the batterypack will be strapped underneath. As for the site, that is a lot of options, do you know what width / length of board i should get?
```

---
## \#7 Posted by: susplus Posted at: 2016-10-20T21:19:02.539Z Reads: 50

```
can't really say as each and everyone has different VEsc settings that will allow for faster braking or slower depending on riding style, weight and so on....You just have to experiment as much as possible to find the most suitable settings for your style....it is not rocket science. A day of researching will reveal quite a lot of info o Vesc settings that you can use after to experiment
```

---
## \#8 Posted by: NickTheDude Posted at: 2016-10-20T21:34:16.854Z Reads: 46

```
Yeah, it is a pretty terrible idea...

Just kidding, but realistically I think 22 Ah at 12S is absurd. That gives you almost a thousand watt hours, which translates to a range of roughly 100km... From what you said that doesn't seem necessary, and would just be more expensive and heavier than it needs to be.
```

---
## \#9 Posted by: Aborn Posted at: 2016-10-20T21:49:00.575Z Reads: 44

```
That is a very good point, maybe cut it down to 10S and about 6P ?

That'll give me 16Ah and a bit less speed to kill my self with.

a 10S6P battery would be a round 2.8 Kg
```

---
## \#10 Posted by: NickTheDude Posted at: 2016-10-20T21:57:46.739Z Reads: 41

```
Still around a 60km range. Generally I've heard that 10 watt hours translates to 1 kilometer of range. Wh = Ah * V. Pretty common configurations are 10S3P, 12S2P, 12S3P, 8S4P, 6S4P. Just make sure your pack will have a high enough discharge rate.

Also keep in mind top speed isn't just dependant on voltage. kV, wheel size and gearing are huge factors.
```

---
## \#11 Posted by: Aborn Posted at: 2016-10-20T22:00:15.764Z Reads: 40

```
Kv = RPM per Volt so topspeed is quite dependend on voltage.

I have a 30 km commute every day and i would like to travel more than that everyday. i dont think a 60 km range is such a bad idea.

Also i can use cells with a lower discharge rate when i have more of them in paralel.
```

---
## \#12 Posted by: NickTheDude Posted at: 2016-10-20T22:02:02.156Z Reads: 36

```
The VESC has an ERPM limit of 60,000. So generally I choose my voltage/kV setup accordingly and then pick gearing/wheels to match whatever top speed im going for.
```

---
## \#13 Posted by: Aborn Posted at: 2016-10-20T22:04:17.089Z Reads: 36

```
Do you have any suggestions as for the deck size and shape or the drive system?
```

---
## \#14 Posted by: NickTheDude Posted at: 2016-10-20T22:07:47.067Z Reads: 35

```
I think generally people use 7-9 1/16 inch veneers of Canadian maple, birch or bamboo. You're going to want to add some concave to the board to make turning easier. The overall shape/length just comes down to the type of board you like to ride, and how much space you need for components.
```

---
