# Electric SHORTBOARD Proyect - needed advise - complete proyect

### Replies: 33 Views: 3729

## \#1 Posted by: raulgda36 Posted at: 2016-01-08T14:02:20.307Z Reads: 208

```
Hi everybody. This is my first time here, so I want to tell you about a proyect I have in mind. 
You know about this new trend, the shortboards, also called Penny boards? I find them very usefull for moving arround yo I want to have one electrified.
I have never seen a similar proyect, everything I've seen is about longboards, but not this kind of boards, so is like I have no model to follow.
First of all I have to say that I haven't bought anything of the necesarry stuff for the conversion to e-board, so any advise or change offered will be taken in count.
My budget, with the stuff I have in mind is about 150€. If the changes you suggest me make it far more expensive than that, I won't take the proyect into reality. Sorry for that, guys.

This is the board I want to electrify:
MODEL: Oxelo Yamba
SHOP: Decathlon
PRICE: 50€
IMPORTANT SPECS: Wheels diameter is 59mm
It uses ABEC 7 (I don't know the name of the piece in english but you know what I am talking about).

Probably is not the best board ever, but it is what I can easily adquire.


As this board is much smaller than the ones you usually electrify, I haven't enough space for the drive-chain method you use. To solve that, I think I'll do something like this:
http://muted.com/kickr-an-electric-motor-for-longboards/
The motor body will be directly in contact with the wheel, instead of using a drive chain which I have no space for.
In my case, to hold the motor, y was thinking to add a wood piece to the front os the board axis. As this part is completly flat, the wood part will fit well and I can fit at the sides of this wood piece the motors, and they will end over the wheel in the same way the link guy does. Instead of putting the metalic piece at the outside of the wheel, mine will be in wood and at the inside. I'm sorry but all this is in my mind only so I cannot uoload any pic.

I will use 2 motors, one for each front wheel. The motors I've chosen are these:
MODEL: NTM_Prop_Drive_28_36_750KV_265W
MAX AMPERS: 18A
BATTERIES NEEDED: 3S-4S
POWER: 165W
RPM/V: 750kv

I know it is not the kind of motor used habitually, so I must explain why I choose them:
1. They are CHEAP, really cheap
2. They are small, only 28mm diameter, thats great for me, as the motors I've seen in other proyects are as big as my wheel here (59mm diameter)
3. It is 750kv, I know it is too much, but with this size this is the lowest kv I've found. I'll run it at 11.1V so that makes it run with lower rpm.
HERE IS MY PRINCIPAL DOUBT WITH THE PROYECT: Despite I'm running two motors, what doubles the torque, will I have enough torque?
I don't want it to be the most powerfull board in the world, just enough to keep me moving at flat routes and to up little hills (maybe with some help).
I've done the calcs and it can reach 86km/h at full throthle. (I won't definetly push it so hard, it scares) but I know its torque will be rubbish. Will it be enough rubbish? That is the question. I repeat, I don't mind hepling it to start moving or at some hills. Please if anyone knows, solve me this.

I continue with the rest of the parts
The ESC chosen os this one:
MODEL: HobbyKing 20A ESC 3A UBEC
PRICE: 9,67 €
CONSTANT CURRENT: 20A
MAX CURRENT: 25A
BEC: Yes
Obviously I will be using two, one for each motor. It gives 20A constantly and a max. of 25A. My motor is suppossed to have a max of 18A so this ESC will be enough I think. It cames also with BEC, which I find usefull to use with the rc receiver, so I won't need a different battery for it. This one has wide programming options so I am hapoy with it

The batteries. Here I need also a little bit of help.
I've chosen these ones:
MODEL: Turnigy 5000mAh 3S 30C LipoPack 5000mAh
PRICE: 23,18€
CONSTANT DISCHARGE: 30C
MAX DISCHARGE: 35C
CAPACITY: 5000mAh
VOLTAGE: 11.1V (3S1P)
It has 5000mAh, 30C of constant discharge and a max of 35C discharge (only for 10 seconds).
What I doubt is if the following calc is correct:
It is 5000mAh, so in 1 hour it gives me 5A. But the specs say that it has 30C CONSTANT discharge, so I suppose it will work at 30C during the complete hour. So that gives me 150A for 1 hour. My motor has a max of 18A, but I will run it behind that almost all the time. DOES ANYONE KNOWS how many time will my battery last if I choose this one?

About the battery charger, I have no idea, any advise will be welcome

About the rc transmiter and receiver, I only need one channel. I was thinking to conect both ESCs to the same channel with an Y wire, as long as they must run both at the same speed always.
The rc transmiter and receiver I was thinking to use is this one:
MODEL: Hobbyking GT2E AFHDS 2A 2.4ghz 2 Channel Radio System
PRICE: 14,00€
SHAPE: Gun Type
The only question I have about this is the following:
The release point of the trigger is at the middle. Will I be able to set the ESC to recognise the 0 speed when the trigger is completly pulled, and the max speed when it is completly pushed? It will be great because it will run at medium speed whitout having the finger on it, I will only need to touch it to brake or to enter the "turbo mode" as I call it. (remember my calcs set a max speed of 80km/h, so it is important not to use this "turbo mode" lol)

That is all my proyect, with this stuff I keep behind my budget
Please feel free to advise me, opine or whatever you want. All the help is welcome. Thanks.

PS: My weigth is about 58kg, if it concerns for the torque issue.
```

---
## \#2 Posted by: Jack Posted at: 2016-01-08T17:13:06.464Z Reads: 164

```
Not sure that setup will have anywhere near the torque to start, I'm using a NTM propdrive 5060 270kv motor which I'm using with 6s and I still need to kick for it to start and a 120a ESC (soon to be VESC).

Also I'm not sure the friction drive off the motor case will work, even with duel drive. Sorry to be so negative but I don't want you to waste your money by buying parts that won't work! 

Have a look at some of the build threads on here for recommended setups. In terms of electrifying the board there isn't much difference between a longboard and a penny board it will just reduce the space to strap batteries too!

Good luck with the project, it would be really cool to see if you get it working. :)
```

---
## \#3 Posted by: raulgda36 Posted at: 2016-01-08T17:49:52.658Z Reads: 148

```
Thank you @Jack
Is not being negative, I wanted to know if it was viable or not, so you're not being negative. I will search again looking for a stronger motor this time, and I might change to single drive. Thanks for your answer
```

---
## \#4 Posted by: cmatson Posted at: 2016-01-08T17:56:59.482Z Reads: 146

```
Welcome!

I think you could pull off the friciton drive, but I agree with jack's assessment that the motors are probably too weak to do anything. As it is, 50mm motors are pretty underpowered for anything more than flat groud, and their acceleration isn't great either. You are dropping to 3s and 28mm... I just don't even see it being able to maintain speed without burning them out. 

Haha I know you are going for a cheap setup, but if it doesn't work, that it's actually just an expensive mess..
```

---
## \#5 Posted by: raulgda36 Posted at: 2016-01-08T18:23:13.879Z Reads: 145

```
I've looked again and found this motor, is the one @Jack mencioned before

Specs:
Model: NTM Prop Drive Series 50-60 270kv
Kv: 270rpm/v
Max current: 90A
Max Power: 2400W @ 29.6v (8S) 
Shaft: 8mm
Weight: 454g
ESC: 100A
Cell count: 6s~8s Lipoly
Bolt holes: 30mm
Bolt thread: M4
Connection: 4mm Bullet-connector

It cost 30€ so I might be able to aford it if I increase my budget up to 200€

Could you recomend me an ESC for it?

Running two of this as I was thinking I won't have any torque problem, is it?
```

---
## \#6 Posted by: longhairedboy Posted at: 2016-01-08T19:39:33.006Z Reads: 129

```
got the same setup on one of mine and i have to kick start it too. But once its running.. damn its fast.
```

---
## \#7 Posted by: raulgda36 Posted at: 2016-01-08T20:06:58.207Z Reads: 129

```
That sounds cool @longhairedboy
```

---
## \#8 Posted by: Jack Posted at: 2016-01-08T20:09:01.418Z Reads: 130

```
Yeah haha the NTM is a beat for the price, It's pretty funny at traffic lights, I'm at the front of the traffic give a couple of kicks then take off! The look on the drivers faces is priceless.
```

---
## \#9 Posted by: Jack Posted at: 2016-01-08T20:10:13.826Z Reads: 132

```
Oh only problem is they seam to be out of stock everywhere. I wanted to get a second for duel but no luck so I'm looking at getting a new pair.
```

---
## \#10 Posted by: psychotiller Posted at: 2016-01-08T20:28:59.922Z Reads: 138

```
The tacon big foot 110 is a great deal and would be pretty powerful
```

---
## \#11 Posted by: longhairedboy Posted at: 2016-01-08T20:32:18.576Z Reads: 139

```
yeah that's a nice find. 6354 296kv with ringclip groove. all it needs is a few flat spots for the grubs.
```

---
## \#12 Posted by: raulgda36 Posted at: 2016-01-11T21:12:18.716Z Reads: 129

```
Oookey, new update guys. With all the answers and some more research I've made, I came up with the following setup

I'll start with single drive and might upgrade to dual drive in the future

The motor choosed is NTM 5060 270kv
Max. A: 90A
Power: 2500W
Lipo: 6S-8S

I've chosen 16-30 gear, that makes a 1.88 to 1 ratio
I know it is really low, but my trucks are 59mm diameter only, which increases my torque.
I downloaded RcCalc and for 22,2V (6S), this gear and this motor gives me 33 km/h. It is not a really high speed so I suppose it should have an aceotable torque.

For the ESC, I'm scared with VESC, so I just choose a normal multicopter ESC
Cont. Current: 100A
Max. Current: 120A (10 sec)
Lipo: 2s-7s

I've read that comercial ESCs like this one usually got hot and stop working, but I'm not riding it neither at its max current nor its max voltage, it is suppose to survive.
I will take an old computer fan and add it I don't know how, just for prevention. 
Will this ESC resists?

For the batteries I've chosen Lipo over Li-ion, just because they are cheaper and easier to find.
I'll take two 6S 2650mAh batteries and connect it in parallel, so that gives me a 6S 5300mAh battery pack. I think it is enough for this built and gives me a decent range does it?
(no calcs here, just using intuition)

An Imax charger complete my setup

About the pulleys, where can I order them online? (cheap please) Or are they easy to find on local typical town shop?

Again, thanks you all, everything is a great help now
```

---
## \#13 Posted by: lox897 Posted at: 2016-01-11T21:49:12.603Z Reads: 112

```
You said "multicopter esc"

I don't think the brakes will work that well on that ESC. Usually everyone here advises car esc's unless you are making custom firmware.
```

---
## \#14 Posted by: raulgda36 Posted at: 2016-01-11T21:58:19.146Z Reads: 112

```
@lox897 I've read its manual and has a braking option. It's set off by default but I can easily turn it on. Now that I think I'm not sure if it is multicopter or what the hell it is for. But I'm sure it has that braking option yes.
It's this one
http://www.hobbyking.com/hobbyking/store/__64849__HobbyKing_Red_Brick_100A_ESC_Opto_.html
```

---
## \#15 Posted by: lox897 Posted at: 2016-01-11T22:08:32.228Z Reads: 111

```
Okay. I would strongly advise that you use a trusted car esc like the hobbyking 150amp or a hobbywing car esc. Also, that esc is opto so you will need a ubec/sbec to power your receiver.
```

---
## \#16 Posted by: raulgda36 Posted at: 2016-01-11T22:19:12.199Z Reads: 110

```
@lox897 Pfff that ones are 4 times the price of the one I said... I've found another one, the same product but upgraded to 125A. Also in the descripcion says that is has better dissipation than the aluminium ones...
```

---
## \#17 Posted by: lox897 Posted at: 2016-01-11T22:28:15.488Z Reads: 115

```
They also won't blow up. Most people on this forum will tell you to get a quality car esc. You'll spend the money on that inexpensive esc and you will have to buy a new one again and again and again. Get the VESC, HK 150, Good hobbywing or torqueboards 12s esc.
```

---
## \#18 Posted by: cmatson Posted at: 2016-01-12T03:31:35.737Z Reads: 123

```
[quote="raulgda36, post:16, topic:944"]
Pfff that ones are 4 times the price of the one I said...
[/quote]

and for very good reason:

Your multicopter esc was made to spin 1 out of the 4 motors on a 2-pound quad-copter... Pulling a human is asking WAYY to much of it, and you will just be wasting your money.

Sometimes the cheapest route isn't the way to go.. especially when you are asking your electronics to push a human rider.
```

---
## \#19 Posted by: psychotiller Posted at: 2016-01-12T04:02:05.157Z Reads: 117

```
Get a car esc. @lox897 and @cmatson are right. You may as well just send me your cash otherwise. I'll put it to good use I promise!
```

---
## \#20 Posted by: raulgda36 Posted at: 2016-01-12T15:00:28.315Z Reads: 114

```
May this one work? http://www.hobbyking.com/hobbyking/store/__17983__Turnigy_dlux_80A_HV_Brushless_Speed_Controller_OPTO_.html
It's for rc cars as you advised
```

---
## \#21 Posted by: psychotiller Posted at: 2016-01-12T16:10:30.616Z Reads: 102

```
You'll need to purchase an sbec/ubec so that is an added expense and I'm not sure anyone has tried this one out yet so it's not a proven choice, but you may as well be the first. If it performs at 8 to 12s like it says you'll be set. Just know, that you are going to occasionally pull more amps than it is rated for. 
Give it a shot!
```

---
## \#22 Posted by: trbt555 Posted at: 2016-01-12T18:42:52.668Z Reads: 95

```
I remember seeing reports of those DLux Esc's catching fire.
Why not get a VESC ?
```

---
## \#23 Posted by: raulgda36 Posted at: 2016-01-12T20:46:14.961Z Reads: 99

```
I'm not english (you probably have realised that) and I'm not sure to be able to understand all about VESC, to be able to build and program it.
I've looked on the VESC web and it seemed just madness for me.
```

---
## \#24 Posted by: raulgda36 Posted at: 2016-01-12T21:27:29.864Z Reads: 98

```
I've found this one
http://www.hobbyking.com/hobbyking/store/__38782__TURNIGY_K_Force_120A_HV_OPTO_V2_5_12S_Brushless_ESC.html
It seems quite similar to the one that torqueboard sells. I'm not able to buy torqueboard's one because shipping to spain will double its cost, bust this one can be easily delivered.
120A, max of 180
5-12s cells
Even the pic seems similar to it!
Has someone tried this?
```

---
## \#25 Posted by: raulgda36 Posted at: 2016-01-12T21:30:24.673Z Reads: 94

```
@psychotiller If I push more ampers than the ones it is rated for (100A), won't it blow up the motor, which is rated for 80A?
```

---
## \#26 Posted by: lowGuido Posted at: 2016-01-12T21:54:34.810Z Reads: 91

```
those red brick ESC's are CRAP. Avoid at all costs.
get the car ESC 
http://www.hobbyking.com/hobbyking/store/__77145__HobbyKing_174_8482_X_Car_Beast_Series_ESC_1_8_Scale_150A.html
```

---
## \#27 Posted by: psychotiller Posted at: 2016-01-12T22:06:46.187Z Reads: 91

```
You'd probably burn up the esc first
```

---
## \#28 Posted by: cmatson Posted at: 2016-01-13T03:12:49.764Z Reads: 92

```
[quote="raulgda36, post:24, topic:944"]
It seems quite similar to the one that torqueboard sells.
[/quote]

he loads rc car firmware onto it because the stock firmware is for airplanes or helicopters; it just doesn't work well for eboards.
```

---
## \#29 Posted by: raulgda36 Posted at: 2016-01-13T15:56:42.243Z Reads: 92

```
@lowGuido Have you (or anyone else) tried this esc? The webpage says it only work with 4 poles motors. Will it run the NTM 5060 motor, or the sk3?
```

---
## \#30 Posted by: lowGuido Posted at: 2016-01-13T20:59:54.875Z Reads: 103

```
I have it running an SK3.
I cant see why it wouldn't work with the NTM 

I *think* that because it is a car ESC it is assumed that you would be using an inrunner motor. and that is what they are referring to when they say 4 pole only, meaning that it is not compatible with 2 pole inrunners.
getting useful information out of hobbyking can be futlie sometimes.
```

---
## \#31 Posted by: raulgda36 Posted at: 2016-01-13T21:40:08.337Z Reads: 102

```
I may (not sure yet) change to sk3, because to keep inside the budget I will make it single drive, so that motor gives me higher torque running alone than the NTM.
So if I have your word that it works probably I will run this one
```

---
## \#33 Posted by: linsus Posted at: 2018-09-06T09:33:16.512Z Reads: 31

```
Sneaky advertisements are sneaky...
```

---
## \#34 Posted by: J0ker3366 Posted at: 2018-09-06T09:34:19.387Z Reads: 31

```
You have got to be kidding me..... If we wanted prebuilts, we wouldn't be building our own. This makes the third time I've seen this tonight. And no less on threads where they're building their own board.
```

---
