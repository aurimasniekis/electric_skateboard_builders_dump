# Battery Build 10s4p / 12s5p or any better?

### Replies: 10 Views: 310

## \#1 Posted by: viraj.invents Posted at: 2019-09-24T12:47:19.300Z Reads: 114

```
Hi All

I am starting this new topic for people who are newbie to this world but very enthusiastic to build the one. 

I am keen on making a new board, I have figured out everything but the only thing where I am stuck is the battery. 

I need to make a battery for long-range which can touch 50Kms in one charge and plug and play so can connect other battery immediately for another 50kms ride, hence kindly suggest

a) which battery to take 18650? or something else 

b) neat diagram for the for 10s4p / 12s5p or better (keep it simple as I am not from electric/electronic background)

c) BMS - will this work,  https://www.amazon.in/Lithium-Battery-Protection-Electric-Equalization/dp/B07MDWP4CP/ref=sr_1_7?crid=2XHTB48SEC51A&keywords=bms+10s&qid=1569328192&s=gateway&sprefix=bms+10s%2Caps%2C261&sr=8-7)

d) I have Flipsky Dual FSESC4.20 Plus, will this work with battery we are planning ?? 

kindly suggest guys 

thanks 

Viraj S
```

---
## \#2 Posted by: accrobrandon Posted at: 2019-09-24T13:29:19.729Z Reads: 104

```
So u want.to build 2 batteries or 1? 100km roundtrip? Thats a lot of riding. Without knowing yur setup or your weight probably a 5p possibly 6p will be good for one way.
```

---
## \#3 Posted by: pjotr47 Posted at: 2019-09-24T13:47:43.307Z Reads: 98

```
Start first with reading! You can find all you questions on topics here on the forum. 

If you don’t put your time into searching, I am not willing to help you out.
```

---
## \#4 Posted by: viraj.invents Posted at: 2019-09-24T13:47:54.627Z Reads: 94

```
[quote="accrobrandon, post:2, topic:102170"]
out knowing yur
[/quote]


I want to build 2 batteries, each battery to touch 40-50kms per charge

I will use evolve 7" all terrain tyres
I weigh 76 Kgs 

I need to know will Flipsky Dual FSESC4.20 Plus support the 5p ? and can you send me the diagram to how to connect batteries together and then to BMS. 

which batteries should I use, will this work??

3800 mAh Battery Capacity. 
Voltage: 3.7 Volts Battery Size: 
Diameter- 18mm x Length- 65mm. 
(Standard- 18650)
```

---
## \#5 Posted by: Ben.Nexus Posted at: 2019-09-24T14:29:05.092Z Reads: 83

```
Any ESC supports any number of parallel groups, its about the series groups which is important, the max reliable setup is 12S for most VESC/ESCs. Your power will get bottlenecked at a certain number of P groups because your battery will be able to output more than your ESC can take, but usually you'll have enough power especially at 4P+

If you ride at around 15mph on pumped tires you can expect about 13wh/km so at 10S you're looking for about 1300wh, so if you went for 10S10P Samsung 35E you'd get to 100km range on 1 charge. You could build 2 10S5P, but I'd actually urge you to do 2 10S6P if you need to because of the sag in the last few km you may not get to 100km if you just split the pack in 2.
```

---
## \#6 Posted by: accrobrandon Posted at: 2019-09-24T16:21:15.448Z Reads: 76

```
[quote="viraj.invents, post:4, topic:102170"]
and can you send me the diagram to how to connect batteries together and then to BMS.
[/quote]
i was kinda thinking @pjotr47 was being a little bit of a dick BUT he is right. there is soooooo much info here already on what you seek that we cannot spoon feed you when its already here. And I dont feel like pulling teeth asking every question about every part of your proposed build 

[quote="viraj.invents, post:4, topic:102170"]
which batteries should I use, will this work??

3800 mAh Battery Capacity. Voltage: 3.7 Volts Battery Size: Diameter- 18mm x Length- 65mm. (Standard- 18650)
[/quote]

tons covered on batteries. Specs about a cell with out the actual brand doesnt help, as not all batteries are created equal.

So are you not stopping before you turn around? no time to charge or are you trying set a long distance ride record?

Id do some research cuz it doesnt sound like you know exactly what you want yet, beside range and tires. top mount? bottom mount? which size deck? motors? esc probably can handle what your building as mentioned...
```

---
## \#7 Posted by: Elera Posted at: 2019-09-25T06:59:50.366Z Reads: 53

```
Most of people replacing 18650 lion-ion battery with Lipo battery that [high C rate discharge](https://www.grepow.com/page/high-discharge-battery.html) for Electric skateboard. Most people like lipo battery because of support charge quickly, safety and lightweight itself.
```

---
## \#8 Posted by: pjotr47 Posted at: 2019-09-25T15:16:00.673Z Reads: 36

```
Lol. Everybody goes to li ion.....
```

---
## \#9 Posted by: Acido Posted at: 2019-09-25T17:18:39.529Z Reads: 34

```
Ahh the silly new guys :sweat_smile:
```

---
## \#10 Posted by: BillGordon Posted at: 2019-09-27T00:29:49.401Z Reads: 29

```
This is wrong. BTW, the two names above mine? Two of the most experienced and respected battery builders in the game.
```

---
