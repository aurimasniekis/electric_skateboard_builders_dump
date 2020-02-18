# Winter is coming - First build - The Norwegian

### Replies: 35 Views: 2054

## \#1 Posted by: 3dman Posted at: 2017-11-22T12:55:06.895Z Reads: 353

```
Hi!
I have pretty much never used a skateboard before but it looks really fun. I see myself cruising to work on a eskate! Since winter is coming, I will have time to tinker with this indoor while I dream of icefree roads :-)
I am 65kg, there are some mid steep roads around, I am more interested in good torque than high speed. 1 motor to save some cash for now.

I think I will buy most part at hobbyking to save some on shipping to Norway.

Please help me with choosing some parts:

**Motor:**
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html

**Battery:** 
3 off 3s1P: 25C, 30C Pea
https://hobbyking.com/en_us/turnigy-battery-5000mah-3s-25c-lipo-pack-xt-90.html

**ESC**:
Vesc: Turnigy SK8-ESC
https://hobbyking.com/en_us/turnigy-sk8-esc-for-electric-skateboard-conversion.html

The motor, is it a good choise? I see that it is rated for "Voltage: 10~12S Lipoly". Can it still be used with 9S, which I plan? 
Or should I go with this, or anything else:
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-149kv-brushless-outrunner-motor.html
```

---
## \#2 Posted by: PEX Posted at: 2017-11-22T13:43:50.842Z Reads: 309

```
Hello @3dman

What wheel are you planning to use?

I have a similar project (90% done) and here the [forum thread](http://www.electric-skateboard.builders/t/electric-mountainboard-winter-build-trampa-holypro-dual-sk3-245kv-max6-esc/37683) if you want to take a look 

Check also these batteries they are very flat and currently on sale! https://hobbyking.com/en_us/zippy-flightmax-8000mah-3s1p-30c-lipo-pack.html?gclid=Cj0KCQiA3dTQBRDnARIsAGKSflmiEghmlwS-QTr6KD4IHcpdAUytaAnVbsvfCR0vIJ1iagC6e3x_k3IaAkfXEALw_wcB&gclsrc=aw.ds
```

---
## \#3 Posted by: 3dman Posted at: 2017-11-22T16:49:10.187Z Reads: 275

```
Thanks for the reply Pex and what an awesome build you have there!

I am aiming for an asphalt build but it would have been cool with a proper winter build as well. That might be for the future.

Thanks for the battery link, I have missed that one. But will be sufficient for me to run two of these in series, 22v, any voltage sag? 6S on the 192Kv which is rated 10-12S is that OK?
```

---
## \#4 Posted by: FredrikHems Posted at: 2017-11-22T17:07:39.588Z Reads: 246

```
If going 6s you may wanna get a higher kv motor. something like 230-250. Av ren interesse, hvor i norge er du fra?
```

---
## \#5 Posted by: Youssless Posted at: 2017-11-22T17:14:19.517Z Reads: 225

```
I've that same 192KV SK3 motor and use a 9S battery (with the batteries @PEX recommended. Works fine, on 97mm ABEC11s and 15/36T I get good torque for 95kg load and top out at just under 35mph.

I've made a build with the same batteries for my wife, she's 55kg and I got her a 6355 260KV motor, need an enclosure to get it running long distances but it has quite the kick too. 

I've tried to run 6374KV with 6S but she didn't want to budge even with a kick start.

I'd recommend a smaller, higher KV motor or grab three or four of the batteries PEX recommended.
```

---
## \#6 Posted by: 3dman Posted at: 2017-11-22T17:27:37.864Z Reads: 205

```
@Youssless! 
@FredrikHems! 
Thanks for your answers. That was exactly what I needed :-) 

Hei Fredrik 
Jeg er egentlig fra Bærum, men flytta nettopp til Trondheim. Er du i nærheten :-)? Do you know any good Norwegian sites with parts, or a place where I can buy a deck with usable trucks?
```

---
## \#7 Posted by: NickTheDude Posted at: 2017-11-22T17:43:23.939Z Reads: 195

```
You can definitely use lower voltage than what it's rated for if you want to. However usually it's reccomended to use the highest voltage your VESC can handle since you will need to draw less amps for a given power output though 9S is pretty much perfect for that VESC. Use [this calculator](http://calc.esk8.it/) to figure out how you're going to gear it to get the speed you want.
```

---
## \#8 Posted by: FredrikHems Posted at: 2017-11-22T18:08:24.211Z Reads: 194

```
Nei, er vell ikke så veldig nærme akkurat.. Skedsmo, Akershus. If you want longboard parts in norway you can check out www.boardshop.com However it would be a lot easier to get caliber trucks from eBay.
```

---
## \#9 Posted by: Fatos Posted at: 2017-11-22T20:34:59.925Z Reads: 185

```
Why not go for a 18650 cells, instead of lipo?

Hilsen Fatos
```

---
## \#10 Posted by: FredrikHems Posted at: 2017-11-22T21:21:00.695Z Reads: 173

```
Because li-ion is alot more expensive, as well as it cant be compared to the amperage lipos can put out
```

---
## \#11 Posted by: pennyboard Posted at: 2017-11-23T06:44:02.691Z Reads: 164

```
Everything looks good to me. A few things to think about, I wouldn't go higher than 9s battery with that ESC, and when you program it, don't push it to its limits, choose safe values particularly for motor and battery amps. Those ESCs have been known to break when they are pushed to hard, but as long as you keep the values conservative, you should be fine. 
A lower gear ratio (13/16 instead of say 16/36) will help not put too much stress on the ESC and batteries and get more torque, just at the expense of top speed. 
A few things to think about: you'll need a motor mount and gearing. Hobby king sells a motor mount but I'd try to find something better if you can. Look for a mount with idlers as that will make the board coast better and keep the belt from slipping. Also, you're going to need a controller. There's lots of options if you search the forums.
```

---
## \#12 Posted by: 3dman Posted at: 2017-11-23T10:22:41.919Z Reads: 139

```
Thanks for input @pennyboard.

But a gear ratio of 13/16 will give higher speed than 16/36 and so give less torque..?

For the motor mount, yes I was planning to buy from Hobbyking but after seeing some reviews I will not. I will look for a drawing so I can make one myself.
```

---
## \#13 Posted by: pennyboard Posted at: 2017-11-23T10:43:00.226Z Reads: 131

```
[quote="3dman, post:12, topic:38997"]
But a gear ratio of 13/16 will give higher speed than 16/36 and so give less torque..?
[/quote]

Yeah i meant 13/36 not 13/16 haha. It was a typo. 13/16 is practically 1:1. No torque :joy:
```

---
## \#14 Posted by: OskarCastrone Posted at: 2017-11-23T11:04:54.511Z Reads: 129

```
Hey man! Nice to see some more folkes from Scandinavia! 
Jeg er fra Danmark! 
If you need any help with the electronics, please hit me up. If you are interested, I can also build you a battery pack, or solder some wires together for you. 
I suggest you do it yourself though, since I believe it is part of the experience to make it yourself. Its a very good feeling! :)
```

---
## \#15 Posted by: 3dman Posted at: 2017-11-23T15:54:12.309Z Reads: 123

```
Thanks @OskarCastrone :-) I'll keep you in my mind when I struggle with electronics! Denmark must be a perfect place for a longboard. Flat and nice. Will definitely bring mine on my next trip there. 

It's a really active community here.  Thank you all for your help.
```

---
## \#16 Posted by: 3dman Posted at: 2018-08-28T13:55:50.094Z Reads: 116

```
It took some time and but my dream of an electric longboard is finally taking shape. With help from the forum I 2D printed out a templated for the Amsterdam Oak deck. 
So went to the local woodshop in Trondheim (Nilssons Trelast) and got a piece of 1x 0,2 m and almost 1in thick. American white oak. I like the look of a solid piece of wood longboard. The piece of wood that I got has a natural concave. I was actually thinking of planning it flat before I noticed the beautiful shape :-P
I could have gone for a wider piece of wood for my 218mm trucks.. But the board kind of looks cool.
The board is a bit heavy. I plan to shave it down to maybe 1,5cm thickness.
The finishing touches with sand paper and coating is not done yet. (clear coat, lack maybe or hard wax? Hard wax beneath grip tape might not work..).
Next is to get it ready enough so I can test drive. Grip-tape, sanding, coating, edge routing etc. must wait! 

![image|374x500](upload://kQ46PZiZj3ztqfv7vZlYprGjCJH.jpg)
![image|666x500](upload://pLlCmFcfgETix6tDtSTnc8GejXm.jpg)
![image|374x500](upload://eFVZtUcWRTAfnKsMAZoYnzpM0NT.jpg)
![image|374x500](upload://5XplsoevDIqMDjXWo6ANr6DSpU0.jpg)
![image|374x500](upload://rCoteIzpN705BphmYoZRMXXLA6u.jpg)

Yes, forgot to mention that I bought/made the following hardware:
-Torqueboards wheels 83mm, 218mm trucks
-4x Turnigy 400mAh 3S lipos
-TOrqueboards 4.12 ESC (VESC)
-Famous SK6374 194  motor
-motor pulley with various teeth count
-3D printed wheel pulley
-3D printed motor support (the one I currently have printed seems a bit flimsy)

Upcoming work:
Solder series connectors, make preliminary enclosure, 3D print new wheel pulley, hook up vesc to motors and config, mount and test run!
```

---
## \#17 Posted by: 3dman Posted at: 2018-08-31T06:30:25.798Z Reads: 106

```
31.08.18:
So I 3D printed a motor pulley for 15mm belt with 40 teeth. Own design based on pulley from 
http://shop.sdp-si.com/catalog/product/?id=A%206A25M040NF1510 and information from https://www.electric-skateboard.builders/t/tooth-profile-for-htd-5m-pulley-need-help/11565/14.
Printed in PETG, 0,1 resolution. Together with the motor mount, it took 24h..
Will use it together with the 15 or 16T alu motor pulley. 


![IMG_1400|375x500](upload://gIQuMSxeVo8rDIQVCEoUhOeCJxX.JPG)![IMG_1398|375x500](upload://zwJUwvc1fnUxe9KrumZjUZtbAml.JPG)![IMG_1397|375x500](upload://n6TAE5Q3Z8iLTduxzicbj8JQSMe.JPG)
```

---
## \#18 Posted by: lennarn Posted at: 2018-08-31T06:51:15.461Z Reads: 99

```
Nice to see more Norwegians on here! I'd really recommend you buy a longboard deck, because the one you made from a single piece of wood looks like it would break under stress.
(Oslo her, holder på med min egen single motor build)
```

---
## \#19 Posted by: Mikaelj Posted at: 2018-08-31T07:21:56.606Z Reads: 99

```
Tromsø her :) Har kjøpt en del deler fra skatepro.no. De har caliber trucks om jeg ikke tar feil. Og kitenorge.no og boardranch.no har mye til ok pris.

Ellers produserer jeg egne mounts i 7075 alu, sort anodisert, har ett liggende om du trenger. Har også en 10s3p pakke med 60A bms med e-switch til overs, men det er ikke så enkelt med frakt av batterier.
```

---
## \#20 Posted by: 3dman Posted at: 2018-08-31T07:39:22.072Z Reads: 98

```
Så hyggelig at det er flere her inne!
I could be interested in a motor mount do you have any pictures of it? Currently plan is to test with a printed version, but will switch to something solid. Thanks for tips regards shops.

I have already bought batteries, four packs of 3s1p Hobbyking type (turnigy). I think I will go for a 9s setup. I am a bit worried about too much power :joy:
```

---
## \#21 Posted by: 3dman Posted at: 2018-08-31T07:44:54.212Z Reads: 90

```
Thanks for input regards your concerns about using solid wood. This is oak, heavy, and durable. I believe laminated decks are strong in terms of weight/strenght ratio. But I compensate having a thicker slab of wood. But Im new to this so I rellay dont know what stress I can expect!
```

---
## \#22 Posted by: slick Posted at: 2018-08-31T07:56:09.655Z Reads: 89

```
HEADS UP!

you need do design a "lip"  on the side where the pulley is mounted to the wheel to prevent the belt from rubbing against the wheel in case of misalignment. 

also, think of LiPos with a higher constant discharge rate to have some headroom and avoid voltage sags. 
speaking of LiPo - how are you planning to charge a 9S LiPo pack?
```

---
## \#23 Posted by: Mikaelj Posted at: 2018-08-31T08:13:48.533Z Reads: 92

```
Here is the thread for the mounts: https://www.electric-skateboard.builders/t/do-it-all-mount-caliber-tb-63xx-50xx/52943/82

Since its the last one and I am making a updated version now, I can give you a good price on it.
```

---
## \#24 Posted by: 3dman Posted at: 2018-08-31T08:19:53.200Z Reads: 95

```
Hmm.. won't the motor pulley lips prevent rubbing of belt against wheel?
I bought the https://hobbyking.com/en_us/turnigy-4000mah-3s-30c-lipo-pack-xt-60.html
30C packs. Hope it does not give too much sag.

The plan is to wire the two series connectors (if using 4 batteries) and a 6s jxt connector out of the battery enclosure. Then connect the last series connector between vesc enclosure and battery enclosure. So when it needs recharing i unconnect the series connector connect two induvidual chargers.![IMG_1403|375x500](upload://rRB6OVurL70AJqL33xK0LuX31Sm.JPG)
```

---
## \#25 Posted by: slick Posted at: 2018-08-31T09:55:07.626Z Reads: 80

```
your motor mount may loosen up a bit while riding and you may end up with such a situation or your motor pulley gets loose and slip around your motor shaft and cause belt misalignment.

this is how i did it on my pulleys - just enough to prevent it from rubbing agains the wheel incase it does drift out of alignment.

https://www.electric-skateboard.builders/uploads/db1493/original/3X/9/2/92954dd89a823b851f6d2db9ca1be88dd091b2c7.jpg
```

---
## \#26 Posted by: oyta Posted at: 2018-08-31T20:23:41.045Z Reads: 71

```
Yes! Good to see Norwegians on here. Bergen her :slight_smile:
```

---
## \#27 Posted by: Minim Posted at: 2018-08-31T23:42:34.959Z Reads: 68

```
Hey! Osterøy here :) What do you ride?
```

---
## \#28 Posted by: oyta Posted at: 2018-09-01T04:52:52.276Z Reads: 68

```
Hey! You’re from Osterøy, that’s nice! I have seen some of your posts around here. Had no idea.  What are you riding?  I have done one build with a single motor: https://www.electric-skateboard.builders/t/portable-custom-birch-fiber-glass-enertion-trucks-6355-190-kv-enertion-motor-mount-10s3p-lg-hg2-vesc-6-beta/26397/20?u=oyta
```

---
## \#29 Posted by: Minim Posted at: 2018-09-01T09:58:12.602Z Reads: 66

```
I'm riding a evoraptor. Some info in the post below. Not really using it a lotto :p

https://www.electric-skateboard.builders/t/landyachtz-evo-36-falcon-2018/51745/170
```

---
## \#30 Posted by: lennarn Posted at: 2018-09-03T19:35:04.438Z Reads: 59

```
I'd love to buy a few of your next generation mounts once they are available! How much to ship them within Norway? Also interested in belt covers, if it fits on my tb218, 107mm wheels, tb pulleys. Do your mounts come with mounting hardware?
```

---
## \#31 Posted by: Mikaelj Posted at: 2018-09-03T21:23:40.810Z Reads: 57

```
Sweet :) Tracked shipping is 145NOK. They will fit your setup in both forward (short) and rearward (long) versions. They will come with all the stainless hardware needed, and optional idler pulleys.
```

---
## \#32 Posted by: lennarn Posted at: 2018-09-04T07:42:05.672Z Reads: 52

```
Have you set a price yet?
```

---
## \#33 Posted by: Mikaelj Posted at: 2018-09-04T09:06:03.101Z Reads: 50

```
No, not yet
```

---
## \#34 Posted by: lennarn Posted at: 2018-11-07T11:29:07.668Z Reads: 33

```
What is your release date?
```

---
## \#35 Posted by: Mikaelj Posted at: 2018-11-07T11:56:54.247Z Reads: 32

```
Hi, the mounts are in and undergoing testing.
```

---
