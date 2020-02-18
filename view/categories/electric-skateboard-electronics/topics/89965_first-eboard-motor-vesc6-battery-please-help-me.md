# First eboard, motor, Vesc6, battery please help me :)

### Replies: 32 Views: 601

## \#1 Posted by: zed Posted at: 2019-04-09T19:22:25.554Z Reads: 105

```
Hello everyone,

I am in process of building my first board.
And I need help with some thing like every new empty head like me. :) 

I have already:
Trampa street carver deck HolyPro,
Trampa ultimate truck, 
Superstar hubs,
Urban street tire 
Mini direct with Helical 

And now I dont know what next.. 
I would like to use
Turnigy sk3 6374 149kv with sensor: 
https://hobbyking.com/cz_cz/turnigy-sk8-6374-149kv-sensored-brushless-motor-14p.html
but I dont know if It is good idea with Vesc6 
And also I dont know what type of battery I should to buy

Please help 
Thank everybody
```

---
## \#2 Posted by: Andy87 Posted at: 2019-04-09T20:20:45.774Z Reads: 93

```
You speak about sk3 but linked sk8 motor. What you want? Both will work with a vesc6. Why you think it wouldn’t?
Battery is up to your preference. Depending on your range, discharge and top mount or below the deck.
```

---
## \#3 Posted by: zed Posted at: 2019-04-09T21:22:41.119Z Reads: 80

```
Sorry, I made a mistake. 
I would like own sensored motors. 
And Sorry but I really don’t know nothing about it. 
Can You help me with this settings, please? 
I live in city and Let’s say I would like to drive about 20-30km,30-50 km/h 
Is It possible?
Iam Sorry for my english
```

---
## \#4 Posted by: rich Posted at: 2019-04-09T23:44:01.779Z Reads: 78

```
I would do more research before you buy more things otherwise you'll buy twice.

[quote="zed, post:1, topic:89965"]
Trampa street carver deck HolyPro, Trampa ultimate truck, Superstar hubs, Urban street tire Mini direct with Helical
[/quote]

That's a sick first build :ok_hand:

Do you ride with bindings?

The easiest way would be to topmount 2x6s Lipos in series for 12s.

If you want an enclosure under the deck you need a flexible or segmented enclosure and flexible Li-ion battery which is quite tricky if you do it yourself.

Regarding the motor, the SK8 works but the shaft is too long so you have to cut it. With helicals you must have washers between motor bearing and motor gear on the shaft. The SK8 has a 6mm deep hole with 10mm diameter between the bearing and the motor plate. You need special brass tubes with 9mm outer diameter. You can order them at Trampa (with 6.5mm length or you cut the original ones which are included) and close the gap with washers (best is to also order 8mm washers in different thickness like  0.2mm 0.5mm and 1mm).

With 1:4 gearing your top speed is about 50km/h

![PNG|648x500](upload://aHRWvDhqexM6vTpaOHvRCvPVl5c.jpeg)
```

---
## \#5 Posted by: seaborder Posted at: 2019-04-10T00:05:29.163Z Reads: 65

```
Hey man! 

Yeah sure get "sensored motors" when you can get them. Its not hard to set it up in the "vesc tool" or "bldc tool". From 0 you acceleration will be much smoother. Sometimes the "motor detection" wont work 3 times and the next try it works but dont worry. Do you want to go single or "dual drive"? For a mountainboard only for street it should be alright with single drive but to ride into some terrain and to climb some steeper hills I wouldnt go single drive. You can go 40-50km/h even with single drive but brakes with single drive arent that good. But thats all a thing of how much you want to drain your battery/range and of course the config in the vesc. 

Next you need a battery you can go for "Lipo" or "Li-ion 18650 packs". For your first board I would recommend lipo 2x 5s Lipo in series or 2x 6s Lipo in series.  But you dont have to there are many other ways! Just read or watch some videos about "cells, volts, c ratings and lipos or Li-ion" there are much quick videos!:) 

Get an "enclosure" and think about where and how you want to add it! There are ways to put it under the board but the trampa decks flex and you will slam it to the ground when you want to jump and land hard or not paying attention to it. So I put stuff at the top.

There are still some things like "Bms or Balance Charger, Remote and Reciever" any many small things left.
You will find out! 

Just search the words in the apostrophes it in the forum or google it. You will find much info!:)
```

---
## \#6 Posted by: zed Posted at: 2019-04-10T09:24:02.515Z Reads: 49

```
Thank you for your answer.. 

Yes I have Ratchet binding for this setup..
And I don't need to have batteries under the deck.

And thanks for washers and special brass tubes informations, I take note of it!
But for now I exactly don't know what's going on until I see it.

I'm not going to be a professional builder which will build new e-boar every 6 months.
I just want to own one good board and that's all. if any part will destroyed I will buy exactly the same thing.
So I don't want to learn the things too much,  because it is so many things to know.


About Battery:
So if I understand it well, for 1motor - sk8 6374 149kv I need battery 6s2p 
And for 2 motors - 12s4p ?? 

Can you send me just a link to buy a battery? it doesn't matter how much it will cost.
I would like to use sk8 6374 149kv  and  Vesc6+  and battery.
I will use "dual drive"

Thank you
```

---
## \#7 Posted by: zed Posted at: 2019-04-10T09:48:50.627Z Reads: 46

```
Hi,

 thank you so much for your answer.

Ok I will take sensored.For sure :) And I want to go with "dual drive"  
2x sk8 6374 149kv sensored, 2x Vesc6+
Could you help me with the recommendation for the battery to buy exactly? by the link? 
I don't need have to batteries under the board..

Thank you for everything
```

---
## \#8 Posted by: seaborder Posted at: 2019-04-10T10:00:23.981Z Reads: 45

```
sure, where are you US or EU?
```

---
## \#9 Posted by: zed Posted at: 2019-04-10T10:59:59.813Z Reads: 39

```
I live in Prague - Czech Republic.( EU )
```

---
## \#10 Posted by: zed Posted at: 2019-04-10T11:14:39.642Z Reads: 39

```
it doesn’t matter how much it will cost. I want just the best :) 
I read that Jens use SONY VTC6, 12s4p on this turnigy 6374 149kv..


thank you
```

---
## \#11 Posted by: moon Posted at: 2019-04-10T11:15:36.634Z Reads: 40

```
SK3 Motors are good :)

So are Sony VTC6 and 30q
```

---
## \#12 Posted by: meesie Posted at: 2019-04-10T13:46:35.340Z Reads: 39

```
take a look at www.electricboardsolutions.com

he's based in Belgium and has good shipping rates in EU. also sells good quality parts
```

---
## \#13 Posted by: zed Posted at: 2019-04-10T16:00:56.217Z Reads: 38

```
Thank you, I will check it..
```

---
## \#14 Posted by: zed Posted at: 2019-04-11T06:25:20.301Z Reads: 35

```
Hello, I am still waiting on Your link to battery pack. 
Can I buy already connected 12s4p battery pack? Thank You
```

---
## \#15 Posted by: seaborder Posted at: 2019-04-11T20:45:17.412Z Reads: 30

```
hey man, sorry I was a bit busy.

First you need to tell me how far you want to ride. You want to take Lipos? 

You can take bigger 8-10Ah lipo or for a board not that heavy about 5Ah (5000 mAh). You have to think about getting a bms or a balance charger for the batteries of your well. 

Just search for  Lipo lets say for a 12s Lipo you need 2x 6s or you also can 6x 2s if you want and the capacity you need and dont take the cheapest ones. You will buy twice. Watch for the c rating.  Also you need to connect them in series.

In addition, I would recommend you to find out a bit about the "basics" and things yourself in the forum or videos. Otherwise things will go wrong really quickly and you'll be annoyed twice afterward, believe me :slight_smile:
```

---
## \#16 Posted by: trampa Posted at: 2019-04-11T21:20:29.479Z Reads: 29

```
The carver will not take dual 6374. The truck is not wide enough. There is a new best box for sale in the next days. Takes twin VESC 6 and 16000 mAh batteries, hidden wires, very clean, plenty of range, simple wiring. It does look very sexy in combo with a 35 Short deck and only fits in combo with the wider MTB trucks.
```

---
## \#17 Posted by: sebaszz Posted at: 2019-04-11T21:26:08.522Z Reads: 27

```
pictures? :smiley:
```

---
## \#18 Posted by: trampa Posted at: 2019-04-11T21:35:02.925Z Reads: 25

```
They just arrived. We will post something on instagram soon.
```

---
## \#19 Posted by: sebaszz Posted at: 2019-04-11T21:48:22.521Z Reads: 23

```
thanks

10char
```

---
## \#20 Posted by: zed Posted at: 2019-04-11T21:59:00.691Z Reads: 27

```
I want to use ultimate 16 inch for that. 
And urban treads wheels.. 
and Twin Vesc6 also.. I have this everything in basket now. 
I saw video on YouTube: 
https://youtu.be/V1oMTsW8_Vg
And there is this deck and trucks I think..
```

---
## \#21 Posted by: zed Posted at: 2019-04-11T21:59:50.232Z Reads: 26

```
Hi, 

of course I would like to go as far as I can and as quickly is possible. 

I just want to buy the best battery.. 

I was searching a little today and I’m thinking about 

Sony Vtc6 3000mAh, 3,6V-4,35V(full)

in 12s4p pack for one motor.

So if I connect 12 batteries into a series, I will get 43,2 - 51V and still have 3000mAh. Right? And then connect 4 into parallel and I will get still 

43,2 - 51V but now 12000mAh 

That’s It?  Is It good idea with Sk8 6374 149kv and Vesc6+ 

I would like to buy everything twice for dual helical drive. 

I also know I will need BMS for 12s for one battery pack and charger.. 

but I dont know which BMS is best and where to buy.
```

---
## \#22 Posted by: seaborder Posted at: 2019-04-11T22:03:28.701Z Reads: 28

```
I dont know that much about the sony cells, but yeah if you have a spot welder you can build you own battery. Bms you can get on several shops like ebay unikboards, batterybest, bestech or china ones, I think eskating.eu has also some. Just watch out for the correct size for amp you need. For the motors and the vesc its alright.
```

---
## \#23 Posted by: trampa Posted at: 2019-04-12T03:26:51.357Z Reads: 24

```
12S4P is not enough for twin 6374. You want 12S 6P really. Otherwise voltage sag becomes your issue.
```

---
## \#24 Posted by: Andy87 Posted at: 2019-04-12T04:59:40.150Z Reads: 21

```
[quote="zed, post:21, topic:89965"]
Sony Vtc6 3000mAh, 3,6V-4,35V(full)
[/quote]
I don’t know where you found this information but end voltage is 4.2V not 4.35V.
I would also rather go with the vtc5a and add up to 6p. That will give you less voltage sag and the cells are way cheaper and similar performing.

Bms you can have a look at the bestech website. Just use google 😉 D140 for charge only and D596 for discharge are a good option.
```

---
## \#25 Posted by: zed Posted at: 2019-04-12T05:11:18.993Z Reads: 18

```
I wrote 12s4p for One motor.
Dual drive = 2x pack 12s4p
```

---
## \#26 Posted by: zed Posted at: 2019-04-12T05:13:26.113Z Reads: 21

```
sorry i made a mistake in the number. but the calculation is correct 51V ( 12s )
```

---
## \#27 Posted by: pat.speed Posted at: 2019-04-12T05:16:17.845Z Reads: 23

```
Please don’t make your purchase yet. There is still a lot you need to take into account. @trampa has said you can’t fit two motors onto the trucks so that is an issue you need to solve. 

You also shouldn’t have two separate batteries. You need 1 large battery to power both vescs and motors. I would got for a 12s6p battery made of 30q cells. I wouldn’t recommend building it yourself unless you will use nese or a similar no-weld kit. Speak to @pjotr47 about the battery and he will be able to make one for you. He’s in eu. 

For the motors sk3 are good but don’t have sensors and apparently won’t fit onto the trucks so you will need to get wider trucks or small motors. I would talk with @trampa about this

Also lithium batteries are only charged to 4.2v any higher and they can catch fire. The max voltage for 12s is 50.4v and minimum with li-ion is 33.6v
```

---
## \#28 Posted by: trampa Posted at: 2019-04-12T05:29:28.974Z Reads: 22

```
I would go full MTB, Monterbox, 12S8P. The carver deck is too small for such a battery and dual 6374. I would also go for Vertigo trucks, not Ultimate. 
We know what we are talking about. 25 different boards are in our fleet and riding them one after another gets you to the right conclusion pretty fast. This is a very powerful board and the Holy Pro MTB deck is well proportioned for what you want to achieve.
```

---
## \#29 Posted by: zed Posted at: 2019-04-12T05:33:24.612Z Reads: 21

```
When @trampa send me this information, I answered with link to video. https://youtu.be/V1oMTsW8_Vg

And I think Jens got in this video: ultimate trucks 16inch
Dual drive with helical 

Look at his comment of sestup for this video: 
 
![image|281x499](upload://lPj51nDdWK2osUsMq4yF1o74WrG.jpeg) 

So is possible have 2 motor on 16inch truck? 

And for information: I worte in top I want 
Sk8 6374 149kv sensored - check It 

Simply, I want the same set JUST upgraded with sensored motors. Thats It.
```

---
## \#30 Posted by: Andy87 Posted at: 2019-04-12T05:43:19.370Z Reads: 21

```
You can get sensored sk3 here at the moment 

https://www.electric-skateboard.builders/t/6374-sk3-sensored-motors-for-group-buy-150-170-and-190-kv/89393?u=andy87

6374 will fit on mini trucks @trampa maybe not with a gear drive and maybe not the sk3 but sealed maytechs fit for sure. From where I know? 
![image|375x500](upload://p3OJX8NtWqkINTUgjeguBGS97j8.jpeg) 

@pat.speed i think there is a bit a confusion. The OP first wanted mini trucks but than decided to go 16“ which will fit the motors without problems
```

---
## \#31 Posted by: zed Posted at: 2019-04-12T05:49:43.777Z Reads: 20

```
Thank You.. :) 

I am looking for sensored 149kv At hobbyking. But I will look at It.
```

---
## \#32 Posted by: Andy87 Posted at: 2019-04-12T06:02:56.046Z Reads: 18

```
he is ordering 149kV as well.
they are from the sk3 factory directly and with custom wires and added sensors. 
Better deal you will probably not get on this motors with this configuration.
```

---
