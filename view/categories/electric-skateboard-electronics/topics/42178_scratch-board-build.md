# Scratch board build

### Replies: 48 Views: 2172

## \#1 Posted by: Holyman92 Posted at: 2017-12-29T08:50:56.369Z Reads: 266

```
Okay so I'm gonna build a board from scratch to include the trucks, the board, etc... but here is my setup so far

200x 30q cells (already ordered)
2x 6374 149kv turning sk3 motors (already ordered)
2x VESC (own 1 ordering another soon)
1x 12S BMS (needing reliable recommendations please)
1x Custom motor mounts for my trucks

Now my question is this, my enclosure can house a 12s12p pack with room for the bms and 2 vesc with wiggle room left over... what I was thinking of doing is 2x 12s6p packs and incorporating a switch to flip between the 2 packs but even so... my pack at 12s6p is still outputting 90amps continuous 240a burst, can 2 vesc take that? Correct me if my math is wrong on that but again the cells are 30q's


Update:

Trucks need to be welded and threaded, and need to go find my square tubing...  but here are some pics,
 10" tires 33"x9" deck stencil (might make it longer still undecided)

<img src="/uploads/db1493/original/3X/6/8/68d6b1f65f8319abcf3cd03afe5002f28851fe5d.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/4/f/4f1cfeb660b42521e95b8bbaebbf7515d0e692be.jpg" width="666" height="500">


Buddy came through w/ the bulletproof glass today woot woot, and he got me an extra piece, which means 2 BOARDS!!! 
<img src="/uploads/db1493/original/3X/7/e/7e7f55bef3f8b70076b0a46f935809bf4773bc05.png" width="281" height="500">
```

---
## \#2 Posted by: b264 Posted at: 2017-12-29T08:55:05.416Z Reads: 253

```
200 Samsung 30Q cells is enough for 4 boards.  Also if you want a chance at running super-quiet motors you may want to run 10S voltage.  What brand are the VESC?

By build the trucks, do you mean machine the truck hangers?
```

---
## \#3 Posted by: Holyman92 Posted at: 2017-12-29T09:02:15.731Z Reads: 239

```
I mean im fabbing some suspension trucks that resemble trampa's for roughly 60$ in material (my time is where I guess it's a loss, but I can can them faster than they can ship from UK to the US)

Quiet is outta the question already lol, I'm going to be running a chain drive system it's an e-mtb 

The vesc are 4.12 from  (at least the one I have already is I was thinking of getting 2 vesc 6 but I'll upgrade to those a little later) 

And I bought 200 because 144 cells is such an arbitrary order plus if any cells are doa I dont have to wait for them to send more out

Also 200 cells put me in a cheaper price bracket per cell
```

---
## \#4 Posted by: b264 Posted at: 2017-12-29T09:12:30.416Z Reads: 222

```
[quote="Holyman92, post:3, topic:42178"]
it's an e-mtb
[/quote]

This is a big difference.

[quote][/quote]  

I'd be careful and try to work with only 150 cells because selling 50 brand new 30Q around here will be no problem.  You're going to have INSANE range with 144 cells.

The bestech D122, D140, D205V1 are good for 12S.  Will you run bypassed - or discharging via BMS?

The VESC4 circuit will not reach 90A continuous.  That's enough to run a pair of vesc4.  You don't want to run your cells at max current anyway because it eats up their lifespan.
```

---
## \#5 Posted by: Holyman92 Posted at: 2017-12-29T09:20:44.211Z Reads: 192

```
It will be 2x vesc and 2x 6374 sk3 149kv motors
Insane range is what I'm going for, have to commute 30miles one way for work everyday 6 days a week.

I'm not sure about the discharging idk the pros and cons vs bypassing the bus or going through it

I was curious if the vesc would limit the cells input current somehow without the 90a killing them, not really sure if that's a thing
```

---
## \#6 Posted by: Holyman92 Posted at: 2017-12-29T09:24:45.297Z Reads: 182

```
Do you think valve springs from a car would be too stiff or just right for use in the trucks lol... I have a bunch of valve springs laying around my garage most are new because I rebuild motors (more often than I like) in my free time for friends... they go to chevy 350 heads
```

---
## \#7 Posted by: b264 Posted at: 2017-12-29T09:27:59.520Z Reads: 182

```
VESC can limit the battery current in both directions; yes.  You can limit it to 50A/out and 20A/in if you want, or any other number.  I would hook up all the 12P and not disconnect half of it.  That will stress the cells less and minimise voltage sag.  Not that you'll have a problem with either, but might as well minimise it even more if the cells are there.

30 miles is going to take an hour or two each way depending on terrain, will you have time for that?  It'll be the most fun ever though and you'll want Monday to come sooner so you can ride again.  Also will the board be able to charge while you're at work?  Do you have electric skateboard experience?  What about longboard or trick board experience?
```

---
## \#8 Posted by: Holyman92 Posted at: 2017-12-29T09:33:30.742Z Reads: 181

```
I have 0 eboard exp. But I have ridden trampa's boards in Spain (non-motorized) I did down hill long boarding in Washington state with speeds around 50-60mph (w/ proper slide gear) and I used to skate vert in HS, ik my way around a board, oh yea I almost forgot, I built a gas board using an itallian logging chainsaw from the 80s topped it out at 45mph at the beach before I ate shit and went skipping across the sand like a flat stone on water haha
```

---
## \#9 Posted by: Holyman92 Posted at: 2017-12-29T09:35:21.994Z Reads: 188

```
<img src="/uploads/db1493/original/3X/1/3/13ff937c1a8f820cc54e3c1d96cbf7af163324f4.jpeg" width="690" height="388"><img src="/uploads/db1493/original/3X/0/a/0ac3e877a11e539ca14189bc60dbc0e0a0842e35.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/e/2/e240e0a8e116803f41e56c768960c25ecc1cbea2.jpg" width="666" height="500">

Stencil for the board with proper angles, modeled after trampas holypro 30°
```

---
## \#10 Posted by: PredatorBoards Posted at: 2017-12-29T09:49:59.201Z Reads: 181

```
30Q cells are good for 20A continuous discharge. Not that it matters with the sheer size of battery pack you're running, but just so you know...

I wouldn't run a trampa styled deck. They have zero concave meaning your feet slide off without straps. Even then,  turning is a bitch with a flat deck.
```

---
## \#11 Posted by: Holyman92 Posted at: 2017-12-29T09:53:56.975Z Reads: 172

```
It will have a concave, that was my biggest gripe about trampa as well, and it will have straps

Although it's unorthodox I will be making the deck out of bulletproof polycarbonate, as well as carbon fiber, and a Kevlar version as well... I want to test the durability of different materials...

The polycarbonate will be reinforced with metal flat bar, kind of like leaf springs to control the flex as well as help keep it from "snapping" like people keep saying will happen

The Kevlar, Carbon, and fiberglass will have the metal bars embedded in the middle of the board
```

---
## \#12 Posted by: b264 Posted at: 2017-12-29T10:30:51.710Z Reads: 168

```
[quote="Holyman92, post:6, topic:42178"]
Do you think valve springs from a car would be too stiff or just right for use in the trucks
[/quote]

I don't know.  I know how to find out though.  Take 2 pieces of wood and screw one to the other like a seesaw.  Make sure the one piece of wood sticks out just about 153mm from the pivot point on each side for a 305mm total length.  See if you can place 2 springs under the wood and position them so that by standing on the arm and shifting your weight, you can get the arm to travel up and down about 6cm on the end.  If you have to put the springs over halfway out towards the ends, they are too weak.  If you can't get the springs close enough to the pivot, then they are too strong.
```

---
## \#13 Posted by: Holyman92 Posted at: 2017-12-29T10:32:52.589Z Reads: 159

```
I would have not thought of that... that is a great Idea, I will try tomorrow after work :D and the best part is I have different tolerance springs
```

---
## \#14 Posted by: PredatorBoards Posted at: 2017-12-29T19:58:00.782Z Reads: 147

```
it's great that you want to test different materials... but wood is still probably the best candidate for a ride that dampens/absorbs vibrations.
```

---
## \#15 Posted by: wmj259 Posted at: 2017-12-29T20:01:18.615Z Reads: 138

```
Valve springs have a huge spring constant. They are really rigid, as for using them in this application, not sure if anyone has tried this.
```

---
## \#16 Posted by: Holyman92 Posted at: 2017-12-29T20:04:40.480Z Reads: 144

```
[quote="wmj259, post:15, topic:42178, full:true"]
Valve springs have a huge spring constant. They are really rigid, as for using them in this application, not sure if anyone has tried this.
[/quote]

yea, thats why i wanna try them... they are rigid and might allow for use w/o plastic/rubber dampers.. plus they are already just laying around lol.

I also like having a pretty tight low flex deck when i skate ramps and what not (just personal preference)
```

---
## \#17 Posted by: scepterr Posted at: 2017-12-29T20:09:42.531Z Reads: 134

```
Dibs on extra cells if/when you sell them 😉
```

---
## \#18 Posted by: Holyman92 Posted at: 2017-12-29T20:13:28.383Z Reads: 140

```
lol scepterr, i'll let you know if i decide to sell them or not... 30q's are 30q's after all... and extra 50 cells makes a nice 10s5p pack lol
```

---
## \#19 Posted by: faithfulpuppy Posted at: 2017-12-29T23:10:09.242Z Reads: 143

```
[quote="Holyman92, post:8, topic:42178"]
I built a gas board using an itallian logging chainsaw from the 80s topped it out at 45mph at the beach before I ate shit and went skipping across the sand like a flat stone on water haha
[/quote]

i need to see this
```

---
## \#20 Posted by: Holyman92 Posted at: 2017-12-30T00:45:04.827Z Reads: 147

```
@faithfulpuppy I ended up bedlining it and made the board from layers of maple veneers and a custom form/press (weights, rocks, and foam core)

I dont have many more pics lol, i was 18 when i made this back in 2011/2012

<img src="/uploads/db1493/original/3X/c/f/cf294ebaf4967c40519b407cac1dca86ebffbce9.jpg" width="640" height="480"><img src="/uploads/db1493/original/3X/b/4/b4d2b5725dfc36f945ad952db0b51a1776f8bc70.jpg" width="640" height="480"><img src="/uploads/db1493/original/3X/b/2/b2bfb824cf1b68b4d4c569d0758fcf77b2b992dd.jpg" width="640" height="480"><img src="/uploads/db1493/original/3X/6/5/658d78a7d5a1d39f64a70eacedd0c7ccca6c4e0b.jpg" width="375" height="500">
```

---
## \#21 Posted by: faithfulpuppy Posted at: 2017-12-30T16:17:49.981Z Reads: 127

```
ahahahah that's amazing!
```

---
## \#22 Posted by: Holyman92 Posted at: 2017-12-30T17:56:22.314Z Reads: 126

```
Isn't it tho
```

---
## \#23 Posted by: Holyman92 Posted at: 2018-01-03T10:49:22.376Z Reads: 121

```
About to cut the board shape, then heat and bend the 30° nose and tail :D... still can't believe I got this 33"(838mm)x9"(228.6mm)x1/2" (12.7mm) polycarbonate piece for free (upon further inspection one is poly, one is acrylic so... I guess I only have 1 viable board the other idk what ima do with)
 <img src="/uploads/db1493/original/3X/c/d/cd66503f8387ee0d35a41326558ba10246dfea05.jpg" width="666" height="500">
[Uploading...]()<img src="/uploads/db1493/original/3X/9/c/9c3325d6799525476951a05a3b21ec234681abc0.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/4/d/4dd15f567391deffc2997d7f7f258d6eb2bcfa7e.jpg" width="666" height="500">
```

---
## \#24 Posted by: Acido Posted at: 2018-01-03T12:18:42.902Z Reads: 112

```
Get a vesc 6 from trampa or that other guy who is selling them here for 130£
```

---
## \#25 Posted by: Holyman92 Posted at: 2018-01-03T12:35:33.866Z Reads: 112

```
I was thinking about getting an APS dual motor kit, would the vesc 6 be better in your opinion?

http://alienpowersystem.com/shop/e-board-kits/aps-150amp-6-4kw-twin-motors-e-board-diy-kit/
```

---
## \#26 Posted by: Acido Posted at: 2018-01-03T12:42:05.471Z Reads: 111

```
Well if you are going dual 2 vescs will be okay if you ask me since you will not be drawing as many amps with one motor

Take a look at the vesc 6 here for 130£ its definetly worth it, seller says he tested it for quite some time without problems
```

---
## \#27 Posted by: Holyman92 Posted at: 2018-01-03T13:05:43.356Z Reads: 111

```
I'm going dual motors
```

---
## \#28 Posted by: FredrikHems Posted at: 2018-01-03T13:44:29.545Z Reads: 105

```
Its not even a question If the Vesc 6 is better performance vise, but it is so fucking expensive and overkill for most setups
```

---
## \#29 Posted by: Holyman92 Posted at: 2018-01-03T13:46:22.813Z Reads: 105

```
Well I'm going to be running a 12s12p setup so... I'm already pretty over kill... and idk much about the vesc 6... I'm still learning and reading up on the vesc 4.12
```

---
## \#30 Posted by: FredrikHems Posted at: 2018-01-03T16:20:53.119Z Reads: 101

```
12s12p and Vesc 6's is not what most people see as scratch :wink:
```

---
## \#31 Posted by: Acido Posted at: 2018-01-03T16:49:25.942Z Reads: 101

```
A guy here sells them for 130£ about the price range of a focbox
```

---
## \#32 Posted by: Holyman92 Posted at: 2018-01-03T17:17:17.044Z Reads: 97

```
What do u mean? I was referring to the actual board not the whole setup, ima be making a fiberglass, carbon, and polycarbonate version
```

---
## \#33 Posted by: FredrikHems Posted at: 2018-01-03T17:22:50.685Z Reads: 100

```
Aha, then I understand :wink:

@Acido
They're fair bit more expensive, especially If you ordered focboxes from the cyber monday sale. 150£ vs 72£
```

---
## \#34 Posted by: Holyman92 Posted at: 2018-01-03T17:26:15.991Z Reads: 103

```
Yea, I listed the other specs just to get opinions and recommendations
```

---
## \#35 Posted by: Holyman92 Posted at: 2018-01-20T09:07:30.314Z Reads: 93

```
![20180117_221657|374x500](upload://36aBrTcw3tuvSgmCgBgyq7WmERa.jpg)![received_10215016776876986|281x500](upload://8XnFdfAVcZ0qgkaIXsK8NSYLJ3R.jpeg)![1516439287776993393241|374x500](upload://stwNw3qDM8ETnYEfPpn9Dgae8iT.jpg)
```

---
## \#36 Posted by: dragopepper Posted at: 2018-01-20T09:28:09.490Z Reads: 85

```
why i have the feeling, that i will see one day this build on Braille Skateboarding - you make it we skate it :joy:
```

---
## \#37 Posted by: Holyman92 Posted at: 2018-01-20T09:37:51.103Z Reads: 88

```
It's already been done on there which is why I have confidence in it lol... if those guys can abuse PC on ramps... the street cruising will be no issue lol
```

---
## \#38 Posted by: Holyman92 Posted at: 2018-01-20T09:39:29.020Z Reads: 89

```
I used Metal flat bar I had laying about to give the board less flex but still flex enough to be usable until I get the motor trucks made
```

---
## \#39 Posted by: Holyman92 Posted at: 2018-01-24T09:12:53.054Z Reads: 82

```
https://www.instagram.com/p/BeU5oAqlHg6/

Testing placement of led strips before committing them... I don't like the current placement but figur3d I would share how it looked
```

---
## \#40 Posted by: Holyman92 Posted at: 2018-02-01T01:27:09.950Z Reads: 82

```
![15174481687031965323419|374x500](upload://bDot4Gtnd4zFbI6kvsitLmu5vUV.jpg)![20180131_192442|666x500](upload://2o1W7gdAwmQOz7aeHhaZuOd4o7C.jpg)![20180131_192418|374x500](upload://w7jQwj94t6e6hHfXw7YrjjMG4Qe.jpg)![20180131_192426|666x500]
(upload://sxWlIO7wkAiLyk2jVBHXvESKEeB.jpg)

Tomorrow the 2nd motor arrives and then I have to order the 218mm truck kit
```

---
## \#41 Posted by: Holyman92 Posted at: 2018-02-01T04:44:33.911Z Reads: 74

```
![15174599894972049978660|666x500](upload://rNi8GYCiVon2B5XG4odDDG47Ct7.jpg)![1517460021838421854875|666x500](upload://mBxShBIaVTFJKBdvPfnWrMDdWae.jpg)![151746004311510325749|666x500](upload://zXKCEjjJWa2fxjUm5YGAluvQlx0.jpg)

10s10p, 100 cells in a nice little arrangement, electrical tape is just for holding them together while I figured out how I was gonna arrange them... I like this arrangement, now ima design a case and find a 10s bms... 

P.s.  the same arrangement can be used to make a 12s12p pack and still fit on this board with no added height
```

---
## \#42 Posted by: PXSS Posted at: 2018-02-23T23:09:31.415Z Reads: 68

```
Why do you have some cells lying down and some standing?
```

---
## \#43 Posted by: Holyman92 Posted at: 2018-02-23T23:27:24.108Z Reads: 67

```
@PXSS Minimize the max height
```

---
## \#44 Posted by: pixelsilva Posted at: 2018-02-23T23:28:29.436Z Reads: 66

```
@PXSS, because he is a happy camper and obviouly doesn't give a ...... !
```

---
## \#45 Posted by: Holyman92 Posted at: 2018-02-23T23:30:38.913Z Reads: 69

```
Lol its for the enclosure im using,
```

---
## \#46 Posted by: Holyman92 Posted at: 2018-05-31T07:29:03.538Z Reads: 47

```
![1527751624256191195833|375x500](upload://nCXnhmXP36VTPRBx7YlC2PEbtWF.jpg)

It has rgb led strips with a key fob and set up to "breathe" has other features too but I like this color and the breathing effect

Also, psychotiller 6 shooters will be here in the morning, and the only reason I finally had time to wire up the LED's and upload this pic is because this board decided to throw a piece of glass at me and cut my hand down to the bone cruising at 20mph hahaha... 5 stiches later...

![JPEG_20180531_003538|374x500](upload://hi5jLmLZh88DHLnYuIv34sb9sv0.jpg)
```

---
## \#48 Posted by: Holyman92 Posted at: 2018-05-31T21:16:37.796Z Reads: 37

```
Thanks blitz and why did u withdraw ur comment?

So wheels got here... and nearly killed me... my drive wheel split during the 1st test run belt is now janky... and another wheel lost 2 of its bolts... 

@psychotiller do you locktite the wheels before you ship? They seem sturdy but nothing should back it's way out before you hit the end of ur street 

That being said... I live the look and feel of them and the ride was smooth until it failed

![15278014082661787809696|374x500](upload://7PnNXaqKXPzcvKwPkTU5ZBYZlSu.jpg)
![15278014726841492129406|374x500](upload://rDzAL8VZnOD7qcDzGwI0svdHlaI.jpg)
![1527801499125514141228|374x500](upload://cVx0Uo1xfiIpfVnnxMSnqyG4Ixh.jpg)


P.S. what's the thread pitch and bolt size? I have to go buy some new ones so I can get back on the road
```

---
## \#49 Posted by: Holyman92 Posted at: 2018-06-04T17:10:14.347Z Reads: 28

```
Is it normal for trucks to warp after a couple months?

Torqueboard trucks, hard to see with wheels on but u can see the steady decline in thane on these 100mm wheels... My rear wheels look like I have a camber kit on my board -__- 

![20180604_120511|690x454](upload://eaIzJSFk0Vw6ZLCALeJ9dxDGWvd.jpg)
```

---
