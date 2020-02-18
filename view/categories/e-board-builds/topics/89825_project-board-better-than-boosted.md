# Project Board - Better than boosted

### Replies: 18 Views: 930

## \#1 Posted by: Winkelmann Posted at: 2019-04-08T17:54:48.657Z Reads: 260

```
Hey People!

So now I'm turning to this community to gather your thoughts and fill in the gaps I have

As the title says I'm currently planning my board, but before I'll get into that I really need to give a shoutout to these people for getting my inspirations

Pryside for his monster board [here](https://www.electric-skateboard.builders/t/3d-printed-boosted-board-killer/88803)

the foosted board: [here](http://skatemetric.com/index.php/2018/07/03/ultimate-accessible-foosted-build-tutorial/)

and for controllers:
[Simple 3D](https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543), 
[nano](https://www.electric-skateboard.builders/t/firefly-nano-remote/72916), 
[Smart Remote](https://www.electric-skateboard.builders/t/featherremote-and-smartremote-files-in-post-577/74084)

So for the project, this is my plan:

Body:

* Vanguard deck (same as boosted)
* caliber II trucks
* wheels
* Enclosures and stuff is still under planning stage

I want to try to 3D print as much as possible so the motor mounts and gearing STL files are something I'm looking for (I might CNC out the motor mounts in aluminum) - would love if you have any good links or models

So I'm planning to do a single motor set up to keep the price down and I can always add another one later!

But now for the part where I need help!!

I'm planning to build my own controller as you've seen earlier but I'm not a hundred percent when it comes to certain things:
I've fallen for the smart remote because of the bigger screen, layout, and features like ESTOP, but I'm having a hard time accepting that it talks over 433Mhz instead of 2,4 GHz, what are your thoughts here?
Should I try to modify the Simple 3D remote instead and get a bigger screen and try to use the same firmware as the smart remote?
Does anyone have knowledge of the battery in them?
Maybe to try to build one with the [esp8266](https://www.banggood.com/search/esp8266.html) instead?

And now for the receiver, is there any specific VESC I should look for and maybe stay away from?
I've been looking at [this one](https:///collections/esc-speed-controller/products/torque-esc-bldc-electronic-speed-controller) and [this](https://www.mboards.co/collections/all/products/bldc-esc-4-12)
Both of these shouldn't have a problem with me building my own remote right?

I'm planning to build a 10s2p battery since I'm happy with 10km range, but the question is if that's a safe setup since if I build the battery with [samsung 25r](https://eu.nkon.nl/samsung-18650-inr18650-25r.html) batteries I have a safe max continuous discharge rate of 40 amps but the [motor](https://www.mboards.co/collections/electric-skateboard-motors/products/mboards-6355-180kv-motor) ([alternative](https:///products/electric-skateboard-motor-6355-190kv)) has a max amp of 80 amps. 

Should I aim for a 10s3p battery to be on the safe side? I don't live in the hilliest area and in Sweden, so it's not boiling hot in the summers. I'm also considering too fit it with a smart BMS as Pryside did in his.

For the motor, I've been looking at the ones linked above but I've also looked at [this one](https:///collections/electric-skateboard-motors/products/electric-skateboard-motor-6355-260kv). Thoughts? are there any advantages with higher KV other than speed? I'm not looking for a board that goes over 40km/h, 35-40 is a sweet spot I think.

So my biggest concerns right now are with the electronics. I want to make sure I'm building a reliable and good setup, that my VESC and remote, battery ESC, gives me the best riding experience!

I can always go more into detail how I'm going to design the board if there is interest!

What are your thoughts? everything is appreciated! :slight_smile:
```

---
## \#2 Posted by: brenternet Posted at: 2019-04-08T18:26:01.964Z Reads: 211

```
I would suggest getting an inexpensive mini remote and using it to set your board up, tune and get going. After that worry about remote modding and fancy business. The mini remote is flawless.

Stay away from mboards. A proven inexpensive alternative to the tb vesc is a single 4.12 flipsky esc. Search ebay for them.

If you're set on 18650 cells I would suggest Samsung 30q's for a 10s2p pack to avoid discharge sag. 

Motor wise get the lower kv tb 6355 or a maytech 6355. Both proven and shouldn't let you down.
```

---
## \#3 Posted by: Winkelmann Posted at: 2019-04-08T18:48:26.365Z Reads: 197

```
Hey!

Thanks for the feedback really appreciate it!

That might be a good idea and that VESC will also be compatible with setting up my own remote after?

okay ill stay away from mboard, any specific reason?

You got me curious now when you say if im set on 18650 cells, is there other good options?
the reason ive planned that i should go with those is partly the convienient charging and maintenace after you've set them up!
but the 30q only have a 15 amps safe discharge rate? wont that be a problem with a 2p setup? i want to be able to have torque but obviously not killing my batteries along the way.
2p would only give me a safe discharge of 30 amps?
```

---
## \#4 Posted by: Jinra Posted at: 2019-04-08T18:55:49.068Z Reads: 168

```
on paper 30q's can discharge at 15 amps, but Mooch has done a bit of testing on the cells and rate them at 20a given adequate cooling. You'll likely never be pulling the 20a continuous on the cells anyway. I use a 12s2p 30q config on my travel board
```

---
## \#5 Posted by: venom121212 Posted at: 2019-04-08T19:07:50.293Z Reads: 160

```
I would strongly suggest not 3d printing motor transmission parts. There are a **few** users here that report success and **many** that report failure.

Do not skimp on battery or controller first and foremost. There are lots of good motors, many go for sale used here. 

Good job using proper formatting and linking :+1:
```

---
## \#6 Posted by: brenternet Posted at: 2019-04-08T19:16:40.648Z Reads: 156

```
Yes the flipsky can do anything the others can do. Essentially Ben's hard work in setting the code up is what drives them, they are just a hardware bom to support the flexibility of his work.

https://www.electric-skateboard.builders/t/is-mboards-legit/47112?u=brenternet

Mike/Mboards has a history of shipping late, if at all. Lots of silly excuses over time. He's a young guy who swears he's turning over a new leaf but honestly.. just use a reputable seller, why mess around with a 50/50?

For a smaller pack but a slightly larger cell you'd be better off with the discharge of a 21700 or 20700 pack perhaps. 

Samsung 40T 4000mAh - 35A as an example. Have a good read here on the forum, there's far more capable people building than me. Use their experience.

Justin also hit the nail on the head there. It's almost not worth making mounts with dickyho and boardynamics knocking out such inexpensive and trustworthy mounts. I would consider e-caliber though for the back truck. That extra axle space really opens up your pulley options and makes your motor fit really easy.
```

---
## \#7 Posted by: Winkelmann Posted at: 2019-04-09T08:17:10.436Z Reads: 128

```
So maybe I've understood this a bit wrong?
if I standstill on a hill and then push full throttle, will that not draw a high amp for a short period?

what motor setup are you using and what is your average amp?

venom:
Hmm i will look more into that since i have access to high-quality 3d printers at my university and for the mounts, i can laser cut it with CNC in aluminum.

im probably going with the tb 6355 180KV motor

brenternet:

Thanks, ill def look into the flipsky instead!

i looked into i guess that doing a 10s1p setup with [these](https://eu.nkon.nl/rechargeable/21700-20700-size/samsung-inr21700-40t-4000mah-30a.html) could work?
otherwise, ill prob be doing a 10s2p pack of [these](https://eu.nkon.nl/rechargeable/18650-size/samsung-inr-18650-30q-3000mah.html) as long as its not to low of a discharge rate

**Updated:**

So apperantly im not allowed to do more posts for another 4 hours haha...

 @venom121212 well good to know! haha

Do you have any stats on your average discharge? are you happy with your setup? what range do you get and what setup do you have?

as @brenternet said, what are your thoughts about going with a 10s1p setup of [these](https://eu.nkon.nl/rechargeable/21700-20700-size/samsung-inr21700-40t-4000mah-30a.html)

**update 2**

@venom121212 and whats your motor setup?
```

---
## \#8 Posted by: venom121212 Posted at: 2019-04-09T12:08:02.126Z Reads: 103

```
Can't go wrong with the Samsung 30q cells. They are trusted by a ton of users here, myself included.

Also just a pro tip, if you put an @ before the usernames, it will notify them specifically (like you replied to them as well)

Example: I love @brenternet :kissing_heart:
```

---
## \#9 Posted by: Sender Posted at: 2019-04-09T12:19:03.991Z Reads: 104

```
[quote="venom121212, post:8, topic:89825"]
Example: I love @brenternet and want to take him in my mouth :kissing_heart:
[/quote]


Let's keep it PG here Justin.  And, everyone has tasted Brent anyway.
```

---
## \#10 Posted by: lrdesigns Posted at: 2019-04-09T12:39:35.019Z Reads: 100

```
[quote="Sender, post:9, topic:89825"]
everyone has tasted Brent anyway.
[/quote]

Eww. :nauseated_face:
```

---
## \#11 Posted by: Sender Posted at: 2019-04-09T13:08:07.955Z Reads: 96

```
Nah, he always drinks a bunch of pineapple juice before...
```

---
## \#12 Posted by: venom121212 Posted at: 2019-04-09T13:13:05.792Z Reads: 92

```
I'm not the battery master here... yet. I've only just sorted out lipo vs lithium ion and even then there is a rabbit hole of math and discharge curves that I haven't explored yet.

I run 10s5p on a pneumatic board (8" wheels). I can say I'm extremely happy with my setup. I rode aggressively, through hilly terrain, for roughly an hour and a half the other day and was still over 50% battery. I also ride semi conservatively, coasting when appropriate and not hitting top speed on small stretches... Only long awesome ones. I really ought to make a darn build thread one of these days.
```

---
## \#13 Posted by: Winkelmann Posted at: 2019-04-09T18:40:04.061Z Reads: 80

```
What motor setup are you running?
```

---
## \#14 Posted by: venom121212 Posted at: 2019-04-09T19:32:54.264Z Reads: 77

```
Dual belt driven 6369s by @psychotiller, couldn't be happier with them
```

---
## \#15 Posted by: TSJ Posted at: 2019-04-10T19:34:53.385Z Reads: 79

```
I just built my first board this winter, single TB6374 motor, TB Vesc and 10s3p 30Q custom battery from @thisguyhere.  I wish I had gone with a 10s4p for a couple of reasons.  1) any decent hill >6% grade I have to walk up.  When I built the board I was more worried about running a single motor setup uphill and it overheating.  Turns out the 10s3p battery limits that concern.  2) Regenerative braking has to be limited by the charge rate of the batteries, which is about 4amps per p cell if I remember right.  I get decent braking with the 3p, but down a steep hill it will run away a bit.  With a 2p, it may be marginal.  These are two things I didn't understand when I built my board, so hopefully this will help you.  I also started with a mini remote and am in the process of building a smart remote.  I echo the comment above, get a mini remote to dial in the board before you start messing with a less mature remote.
```

---
## \#16 Posted by: thisguyhere Posted at: 2019-04-10T19:55:56.221Z Reads: 74

```
are you a big guy?  6% grade on a single 6374 shouldn't be problem...

there's a host of variables, but to start, what's your motor / batt amps?  gearing?
```

---
## \#17 Posted by: Winkelmann Posted at: 2019-04-12T09:07:12.064Z Reads: 52

```
hmm, that sounds a bit wierd, thats the first case ive heard that that should be a problem! My plans are at the moment to go with 10s2p (prob 30Q). i've never encountred a case where hills that small and breaking should be a prob! maybe your VESC settings are a bit off?
```

---
## \#18 Posted by: bartroosen12 Posted at: 2019-04-12T10:03:56.467Z Reads: 57

```
I got a 10S2P with samsung 40T cells.
I really like it, small and powerfull pack which gives me 15-20km range.

Btw Samsung 30T cells are pretty affortable these days:
https://www.nkon.nl/rechargeable/21700-20700-size/samsung-inr21700-30t-3000mah-35a.html

Only 1€/cell more than 30Q, and these 30T cells can deliver twice the current so they will be MUCH better for the same 10S2P.
```

---
