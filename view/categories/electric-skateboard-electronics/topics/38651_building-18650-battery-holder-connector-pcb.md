# Building 18650 battery holder/connector pcb

### Replies: 146 Views: 7881

## \#1 Posted by: Kug3lis Posted at: 2017-11-17T21:26:24.427Z Reads: 624

```
As I saw many have interest in "Blasto" created 18650 holder PCB I went did my own similar design. Just wanted to have some thoughts from other before sending PCB's to manufacture.

<img src="/uploads/db1493/original/3X/0/2/0274b0b1c0680cf1b4a78dadf9c74c1e9aa89e30.jpg" width="667" height="500">
```

---
## \#2 Posted by: Kug3lis Posted at: 2017-11-17T21:28:51.003Z Reads: 559

```
Dimensions are 60mm x 65mm
```

---
## \#3 Posted by: Maxid Posted at: 2017-11-17T21:35:55.330Z Reads: 556

```
Why not make the balance leads through hole? Should make it even even easier to solder them while not using up additional space
```

---
## \#5 Posted by: Kug3lis Posted at: 2017-11-17T21:37:08.304Z Reads: 531

```
I do not really want have any contacts on bottom side because of posibility of shorting something.
```

---
## \#6 Posted by: scepterr Posted at: 2017-11-17T21:45:59.884Z Reads: 519

```
Using matching ribbon cable, it's really simple
```

---
## \#7 Posted by: Maxid Posted at: 2017-11-17T21:50:21.849Z Reads: 515

```
You don't need contacts on the bottom - push the cable from bottom to top and solder on top - done.
You could position the holes so that the cables sit between cells so they won't even touch them.
Just a thought...
```

---
## \#8 Posted by: scepterr Posted at: 2017-11-17T22:11:20.159Z Reads: 499

```
The idea is no wires, just ribbon cable with matching S count
```

---
## \#9 Posted by: gogomrrobot Posted at: 2017-11-17T22:13:45.266Z Reads: 499

```
I really like it... one question -- this is limited to 8S ?
```

---
## \#10 Posted by: Kug3lis Posted at: 2017-11-17T22:15:35.445Z Reads: 503

```
No, its just to save space, for bigger S than 7S you need to connect wires like this:

<img src="/uploads/db1493/original/3X/b/4/b42fcb03cdfd89ea55eb55105ea13290e62243fd.PNG" width="690" height="164">
```

---
## \#11 Posted by: Maxid Posted at: 2017-11-17T22:16:11.616Z Reads: 490

```
You can't bend a ribbon cable that easily and flexy decks need a bend in the balance leads
```

---
## \#12 Posted by: gogomrrobot Posted at: 2017-11-17T22:16:36.593Z Reads: 483

```
Got it... that's actually how I have my 12S right now... two split 6s.
```

---
## \#13 Posted by: scepterr Posted at: 2017-11-17T22:16:39.487Z Reads: 478

```
You didn't see what this is based on ?
```

---
## \#14 Posted by: Maxid Posted at: 2017-11-17T22:17:04.266Z Reads: 477

```
What do you mean?
```

---
## \#15 Posted by: scepterr Posted at: 2017-11-17T22:17:48.579Z Reads: 478

```
This is where it originates from
https://www.electric-skateboard.builders/t/arch-s-build-log-kaly-nyc-build-dual-6374-focbox-12s4p/25995
```

---
## \#16 Posted by: Kug3lis Posted at: 2017-11-17T22:18:09.451Z Reads: 447

```
and it's not only 7s you can also do 2s if you want
```

---
## \#17 Posted by: Maxid Posted at: 2017-11-17T22:20:10.898Z Reads: 449

```
Looks cool - how many of us will have the right ribbon cable at home though? Having through holes would make the design more flexible and allow both methods - so win win I guess? I am just trying to improve the design
```

---
## \#18 Posted by: scepterr Posted at: 2017-11-17T22:20:43.405Z Reads: 427

```
@Kug3lis will the ribbon be included ?
```

---
## \#19 Posted by: Kug3lis Posted at: 2017-11-17T22:21:58.970Z Reads: 422

```
If I will be able to find where to buy then yes
```

---
## \#20 Posted by: scepterr Posted at: 2017-11-17T22:22:22.746Z Reads: 420

```
Mouser has it, I think
```

---
## \#21 Posted by: b264 Posted at: 2017-11-17T23:01:22.490Z Reads: 431

```
[quote="Maxid, post:3, topic:38651"]
Why not make the balance leads through hole?
[/quote]

Through-hole is much worse for ruggedness.  Sharp pokey things can wear through insulation, and inside a lithium battery pack, that's the worst possible thing
```

---
## \#22 Posted by: Maxid Posted at: 2017-11-17T23:02:28.429Z Reads: 390

```
As I said: have the solder spots on top and nothing can wear through any insulation
```

---
## \#23 Posted by: b264 Posted at: 2017-11-17T23:13:28.555Z Reads: 383

```
Whatever would go "through the hole" could
```

---
## \#24 Posted by: Maxid Posted at: 2017-11-17T23:15:39.476Z Reads: 383

```
Why use the PCB then - it could also wear through the insulation :confused:
```

---
## \#25 Posted by: scepterr Posted at: 2017-11-17T23:20:19.845Z Reads: 377

```
In my view the purpose of this is to eliminate any loose wires, otherwise just do it the regular way
```

---
## \#26 Posted by: Sender Posted at: 2017-11-19T13:21:06.568Z Reads: 356

```
This is cool, I really like this idea for flexi decks. It really seems to clean up some design elements!
```

---
## \#27 Posted by: gogomrrobot Posted at: 2017-11-22T04:19:58.191Z Reads: 340

```
When @Kug3lis will you have these? Just experienced (3) 30Q cells go bad tonight... after a ride. I need the PCB's.
```

---
## \#28 Posted by: Ronny_CTS Posted at: 2017-11-22T07:41:05.512Z Reads: 342

```
These PCB's along side some cell level fuses would make an awesome battery pack! I'll buy a few PCB's if they are made.

One question though, where do you solder the BMS balancing wire that comes from each individual pack up to the PCB? Do you just solder it with the ribbon cable?
```

---
## \#29 Posted by: Kug3lis Posted at: 2017-11-22T10:38:54.377Z Reads: 354

```
[quote="gogomrrobot, post:27, topic:38651, full:true"]
When @Kug3lis will you have these? Just experienced (3) 30Q cells go bad tonight... after a ride. I need the PCB's.
[/quote]

I will be ordering soon the PCB's so it would take around 2 weeks to get them.

[quote="Ronny_CTS, post:28, topic:38651"]
One question though, where do you solder the BMS balancing wire that comes from each individual pack up to the PCB? Do you just solder it with the ribbon cable?
[/quote]

The idea is you solder ribbon cable through all pcb's and on each pcb you solder jumper which cell number it will be. One line of board can have up to 8 cells then you need another cable and then you join them together like Y adapter
```

---
## \#30 Posted by: gogomrrobot Posted at: 2017-11-22T11:41:03.122Z Reads: 331

```
I don't know the price... but I will take 50 units...well it will be 24 if the price is insane but otherwise 50 ;) I want the ribbon cable too.

Soldering series connections onto nickel just sucks.
```

---
## \#31 Posted by: Kug3lis Posted at: 2017-11-22T11:59:09.704Z Reads: 328

```
It should be around 2$ each, depending on quantity the price maybe be lower. I don't know yet about ribbon cable.
```

---
## \#32 Posted by: gogomrrobot Posted at: 2017-11-22T12:01:51.550Z Reads: 326

```
That's a good price -- yeah I am good for 50 then.  If you can't supply the ribbon cable... why don't you link it at least.  I am not a fan of flat braided copper wire either... it just starts separating it's weave as you try to work with it.
```

---
## \#33 Posted by: Kug3lis Posted at: 2017-11-22T12:03:13.628Z Reads: 345

```
I mean what way of connection you will use is up to you, if you want you can solder copper bars :D
```

---
## \#34 Posted by: gogomrrobot Posted at: 2017-11-22T12:18:24.411Z Reads: 354

```
Hue hue... ok smarty pants... I get it now... so you do have to use something... maybe 10AWG wire or braided or copper bar for the series connection.  I tried searching for that ribbon cable for the sense wires... that's the one I think I will have to ask around for.  Because if you don't use something like the ribbon cable you will have to run each sense wire back around to JST plug which makes for wire messes...

<img src="/uploads/db1493/original/3X/f/6/f69e08ccdac04a818902452a6fd3a1543d3b78e0.jpg" width="690" height="361">
```

---
## \#35 Posted by: Kug3lis Posted at: 2017-11-22T12:20:13.846Z Reads: 349

```
My friend is just gonna use simple single wires to join the sense as you see in your picture on the right side. He said way cheaper and simpler but bit more work
```

---
## \#36 Posted by: Kug3lis Posted at: 2017-11-22T12:21:34.915Z Reads: 338

```
@scepter said will use RGB led wire but its only 5wire so will need to use 5 + 3
```

---
## \#37 Posted by: gogomrrobot Posted at: 2017-11-22T12:38:41.552Z Reads: 335

```
Ok... so for a 12S... you will essentially make this like (2) 6S packs.... will need 7 wires for that.

Lastly and this maybe a retarded question and why I don't 100% understand this PCB thing but believe the magic... how does it know if you run 7 or 8 sense wires down the PCB's which cell is which cell number?
```

---
## \#38 Posted by: Kug3lis Posted at: 2017-11-22T12:42:03.461Z Reads: 338

```
There are solder jumpers which you solder to connect this cell to that specific channel, it does not much matter how much you will connect 2, 3 or 7 its just wire basically. Then you connect to balancer 1 pin on the first series pack is minus and for e.g. 8 pin is cell 7 on next series pack pin 1 will be cell 7 from the last pack or pin 8 from the first pack and pin 2 will be cell 8 and so on. I will draw a circuit then I will be at home don't have tools at work to draw this.
```

---
## \#39 Posted by: Ronny_CTS Posted at: 2017-11-22T15:15:19.488Z Reads: 341

```
Thanks you very much for your reply. I fully understand now. Looking forward to buy a bunch of these. Is the distance between the BMS tracks (pitch) the same as regular ribbon cable?

@gogomrrobot You can buy ribbon cable at any place that sell electrical stuff. Just by searching on digi-key there are so many different options to choose. I don't know what specs the ribbon cable has to have because i haven't done any research on the subject yet however, for example here you have an [8 way flat ribbon cable](https://www.digikey.com/product-detail/en/assmann-wsw-components/AWG28-08-G-1-300-R/AE08A-5-ND/2391672)  that would fit perfect on @Kug3lis PCB's.
```

---
## \#40 Posted by: Kug3lis Posted at: 2017-11-22T15:53:06.729Z Reads: 335

```
The pitch's 2mm so you would need to bit expand this ribbon cable. I never tried so I don't know which ribbon is better :)
```

---
## \#41 Posted by: Ronny_CTS Posted at: 2017-11-22T18:41:15.261Z Reads: 333

```
I found a [2.54 mm pitch cable](https://www.digikey.com/product-detail/en/3m/8125-08-100/ML08G-10-ND/2658735) which would go along well with your PCB. To bad they only sell 3 meters at a time. But i bet it can be bought cheaper and in less quantity elsewhere.
```

---
## \#42 Posted by: Kug3lis Posted at: 2017-11-22T18:44:57.480Z Reads: 303

```
You don't really need ribbon cable. I suggest to buy silicon wire and it will be better
```

---
## \#43 Posted by: Ronny_CTS Posted at: 2017-11-22T19:09:10.068Z Reads: 306

```
I was contemplating that option as well because silicone will behave better under flex for longer. The PVC material that shields the ribbon cable might start to crack after a while.
```

---
## \#44 Posted by: Kug3lis Posted at: 2017-11-22T19:10:07.340Z Reads: 300

```
Exactly :)
```

---
## \#45 Posted by: JohnnyMeduse Posted at: 2017-11-22T19:43:15.022Z Reads: 303

```
If your not using ribbon cable... what will happen if a solder broke ? My educated guess is a big f***king 💥💥💥 and 🔥.
```

---
## \#46 Posted by: Kug3lis Posted at: 2017-11-22T19:47:31.573Z Reads: 298

```
??? What do you mean solder broke? The same broke could happen and for ribbon. Plus you can always glue together leads
```

---
## \#47 Posted by: JohnnyMeduse Posted at: 2017-11-22T19:57:07.032Z Reads: 288

```
Can’t really happen with ribbon cable. Flexing will bring alot of stress over the solder, specially with silicone wire since they are too flexible.
```

---
## \#48 Posted by: Kug3lis Posted at: 2017-11-22T19:58:25.703Z Reads: 288

```
Ok, I can make some holes if you need, but it's not really save because it can touch bottom side like battery case or etc
```

---
## \#49 Posted by: JohnnyMeduse Posted at: 2017-11-22T20:01:24.322Z Reads: 291

```
Doesn’t really matter ribbon cable are in one pieces and distance between each cable won’t change even if one is disconnect. In other word they are one unique piece and won’t gigleling around and risque to short if only one solder broke off
```

---
## \#50 Posted by: scepterr Posted at: 2017-11-22T20:14:21.534Z Reads: 286

```
There are 4pin led ribbons too if you wanna use all 8 just double up
```

---
## \#51 Posted by: gogomrrobot Posted at: 2017-11-22T20:46:57.453Z Reads: 322

```
[quote="Kug3lis, post:38, topic:38651, full:true"]
There are solder jumpers which you solder to connect this cell to that specific channel, it does not much matter how much you will connect 2, 3 or 7 its just wire basically. Then you connect to balancer 1 pin on the first series pack is minus and for e.g. 8 pin is cell 7 on next series pack pin 1 will be cell 7 from the last pack or pin 8 from the first pack and pin 2 will be cell 8 and so on. I will draw a circuit then I will be at home don't have tools at work to draw this.
[/quote]

I know you were going to produce circuit drawing... but about the solder jumper.  Does it go like this (in the below example I am thinking this is the cell #3 jumper?)

<img src="/uploads/db1493/original/3X/f/9/f90cb9274eeff90272a4483a0a361a6135f5685e.jpg" width="667" height="500">
```

---
## \#52 Posted by: Kug3lis Posted at: 2017-11-22T20:53:14.675Z Reads: 309

```
basically, yes
```

---
## \#53 Posted by: scepterr Posted at: 2017-11-22T21:18:23.122Z Reads: 308

```
Just found a box of my old IDE cables...ribbon problem solved 🤣

Also this, 22awg 10 conductor
https://www.mouser.com/ProductDetail/Amphenol-Spectra-Strip/111-2214-010/?qs=sGAEpiMZZMsJiFh04Lj2rlWgz3ZT9ViBgvU%252bHaYzQPg%3d
```

---
## \#54 Posted by: Kug3lis Posted at: 2017-11-22T21:23:44.417Z Reads: 308

```
Now the question: Pads are 2mm pitch (basically you can solder JST header on it) do you guys prefer smaller for 1.26mm? IMO I think bigger gap is better plus you can expand gap on ribbon cable
```

---
## \#55 Posted by: scepterr Posted at: 2017-11-22T21:27:09.230Z Reads: 311

```
I'm fine with the way it is, bigger gap, better
```

---
## \#56 Posted by: gogomrrobot Posted at: 2017-11-22T22:07:16.305Z Reads: 311

```
Yes please bigger is easier... many of us aren't master solderers (if that's a noun... you know what I mean)
```

---
## \#57 Posted by: Kug3lis Posted at: 2017-11-24T21:59:23.547Z Reads: 319

```
The last changes of design, will be ordering pcbs soon so it will be available through our online store

<img src="/uploads/db1493/original/3X/d/b/dba69ca399d704e6e9ea21a7b142d7aec69ce6d9.jpg" width="564" height="500">
```

---
## \#58 Posted by: rene Posted at: 2017-11-26T15:49:33.603Z Reads: 323

```
<img src="/uploads/db1493/original/3X/1/f/1fc80eb6b250064aec11c181b7001e97a4827433.jpeg" width="666" height="500">

Could you scale your awesome design up for Sanyo 20700B cells?

I would take the extra costs and take 50pcs.
```

---
## \#59 Posted by: Kug3lis Posted at: 2017-11-26T15:51:09.317Z Reads: 319

```
I think I could, what kind of width are you looking for? Because 60 does not cover whole batteries in 18650 design?
```

---
## \#60 Posted by: Vanarian Posted at: 2017-11-26T15:54:47.780Z Reads: 313

```
Looks neat but I fail to understand how it works and what it does. Is it like a cleaner wiring "node" for balancers / BMS ?
```

---
## \#61 Posted by: Kug3lis Posted at: 2017-11-26T15:55:33.172Z Reads: 324

```
Basically no wires touching cleaner setup and etc.
```

---
## \#62 Posted by: Vanarian Posted at: 2017-11-26T15:57:02.878Z Reads: 318

```
ok those are directly connections between batteries ! Thanks for explanation
```

---
## \#63 Posted by: rene Posted at: 2017-11-26T16:05:22.938Z Reads: 323

```
I think 75mm width should work.

<img src="/uploads/db1493/original/3X/8/2/8201ba48cd1bb46542b9be00f8d609040bb6b705.png" width="653" height="500">
```

---
## \#64 Posted by: banjaxxed Posted at: 2017-11-28T01:32:08.415Z Reads: 317

```
A 3d file for a case for these boards would really be killer, I'm in for a few good job ☘️
```

---
## \#65 Posted by: Kug3lis Posted at: 2017-11-28T01:38:38.202Z Reads: 314

```
You mean a case for 4 cells and this pcb? For 3d printing?
```

---
## \#66 Posted by: banjaxxed Posted at: 2017-11-28T01:39:22.643Z Reads: 319

```
Yep dats what I mean, if the pub had holes you could even mount it in the case, the case would be open on the topside and you could seal it against the underside. Would work nicely for segmented build

Single channel to route both power and balance ribbon through to the next cell 'box'.

Actually edit that dual exit channels to keep power away from balance, don't want another fireball!
```

---
## \#67 Posted by: Kug3lis Posted at: 2017-11-29T16:35:04.886Z Reads: 310

```
Just to make sure, if you still interested in this I would require you to preorder before I could make them.
```

---
## \#68 Posted by: rene Posted at: 2017-11-29T17:16:58.357Z Reads: 308

```
you got a PM.
```

---
## \#69 Posted by: akhlut Posted at: 2017-11-29T18:00:00.074Z Reads: 317

```
Maybe you should look at what @kaly is doing now.  

https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/3037

The latest iteration of PCB's omit the balance lead ports entirely, with each balance lead being a home run to the BMS.  Got a bad P group?  Yank it and replace it by breaking only 3 connections (in, out, balance@bms) twice.  6 joints are fast and easy.

These PCB's are a good idea, but how would you go about replacing a bad P group?  Desolder up to 12 balance leads and not short them out (6 in, 6 out) and remove the series connections, twice.  That's a ton more work - potentially 28 joints.

Also, how many flex duty cycles are those ribbon cables rated for?  Every time you step on the board, not to mention every bump you go over is a flex.  Got a bad balance lead connection somewhere?  It's gonna take time to identify and fix it, especially if you goop up the balance leads with hot glue to protect them.

Not trying to be a downer here, just pointing out some potential flaws.
```

---
## \#70 Posted by: Kug3lis Posted at: 2017-11-29T18:21:52.820Z Reads: 301

```
There is a reason why balancing tracks are on PCB so that it would not run through the whole pack. Most fires started because wire isolation got damaged and got shorted. Flex cable is the same as your normal cable just joined together.
```

---
## \#71 Posted by: scepterr Posted at: 2017-11-29T18:35:15.571Z Reads: 297

```
The option is still there to run the balance leads independently, choose what you prefer. I wouldn't use these for just flexpacks but regular flatpacks too. So you can use it however you feel will work best for the pack youre making.
```

---
## \#72 Posted by: akhlut Posted at: 2017-11-29T18:56:36.128Z Reads: 307

```
> Most fires started because wire isolation got damaged and got shorted.

Wait, what?  How many fires are we talking about, and how many have had as their root cause a shorted balance lead?

I've only seen two eskate fires on this forum, and only one was due to a spontaneous battery pack issue that is unresolved.  The other an eskate got run over by a trolley.  Are there any other instances to back up this claim?

Also, these PCB's are introducing needless complexity.  Each solder joint between PCB's is a potential point of failure.

Let's think about a 12S pack structured like you suggest above

(10) PCB's with (12) balance connections and (2) series connections
and 
(2) PCB's with (6) balance connections and (2) series connections

That's 156 solder joints. 

Compare that to the home run packs - 36 solder joints.

That's over 4x as many connections!

@scepterr Yeah, totally.  But 4+oz copper PCB's aren't cheap to produce and real estate in an enclosure is valuable, so why waste that space on part of a PCB that does essentially nothing?  You could fit another whole cell or two where those balance leads are.
```

---
## \#73 Posted by: Kug3lis Posted at: 2017-11-29T18:59:05.363Z Reads: 272

```
If you don't see a point of it then just ignore it. There are people who understand it and wants it.
```

---
## \#74 Posted by: akhlut Posted at: 2017-11-29T19:09:10.421Z Reads: 275

```
Just trying to help you think this through before you plunk down cash.  What weight copper are you using, and what's the trace width on your busses?
```

---
## \#75 Posted by: Idle Posted at: 2017-11-29T19:11:36.615Z Reads: 283

```
Let it go 
Let it go
```

---
## \#76 Posted by: Kug3lis Posted at: 2017-11-30T02:09:33.235Z Reads: 305

```
20700 design for @rene

<img src="/uploads/db1493/original/3X/3/1/31a995b08a7b26e4afb88ff3b97df3dbecce78f5.jpg" width="553" height="500">

If you interested you have time to join the order until tomorrow 12 PM GMT
```

---
## \#77 Posted by: rene Posted at: 2017-11-30T07:22:06.512Z Reads: 299

```
On 20700B PCB the future is bright with possible 16S :-)
```

---
## \#78 Posted by: Kug3lis Posted at: 2017-12-13T13:08:02.910Z Reads: 313

```
Today, received the PCB's. It should be available to buy by the end of the week.

<img src="/uploads/db1493/original/3X/4/1/4112eb784368109775c10b33e6565d272ca35172.jpg" width="375" height="500">
```

---
## \#79 Posted by: banjaxxed Posted at: 2017-12-13T17:35:37.517Z Reads: 312

```
Here we (almost) go
https://shop.3dservisas.eu/products/18650-4-cell-pcb-holder?variant=5142975217691
```

---
## \#80 Posted by: Kug3lis Posted at: 2017-12-13T19:39:51.858Z Reads: 304

```
Will be bit different links the minimum quantity will be 10 pcs
```

---
## \#81 Posted by: Kug3lis Posted at: 2017-12-13T21:49:32.629Z Reads: 311

```
Here are the links to the items. If anyone is interested in more than 50 pcs. Give a message we can make a deal then ;)

https://shop.3dservisas.eu/collections/pcb
```

---
## \#82 Posted by: DeathCookies Posted at: 2017-12-14T13:41:03.475Z Reads: 304

```
Well, i missed the Explanation of this PCB... what does it do?
```

---
## \#83 Posted by: Rob69de Posted at: 2017-12-27T16:54:18.471Z Reads: 311

```
My thoughts on  these PCB’s
If building a 4p the fourth battery has to stick out from PCB 
In order to catch the bus bar fully.and only two points of contact 
Even a 3p only two points on contact 
I wish the bus bars on pos/neg were longer so I can catch each individual battery, instead of 2 <img src="/uploads/db1493/original/3X/8/9/89437e88700e88c1999390afcc75dbdfb43f74ed.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/a/1/a16db24bc15c954e8163737629f7738e5cf42bff.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/b/a/ba2399eae97e5f34992064221b6fc4140037503d.jpeg" width="375" height="500">
```

---
## \#84 Posted by: Kug3lis Posted at: 2017-12-27T18:43:12.427Z Reads: 291

```
That pad wasn't supposed to be used as bus bar it just solder point for connecting pad and wire together
```

---
## \#85 Posted by: Rob69de Posted at: 2017-12-28T19:03:13.317Z Reads: 290

```
<img src="/uploads/db1493/original/3X/e/1/e108a3b7d1e0d75d0ab0b1dd3d0b01f0dc91eaaf.jpeg" width="637" height="500">I’m happy with the results
```

---
## \#86 Posted by: Kug3lis Posted at: 2017-12-28T19:08:40.364Z Reads: 288

```
You better solder those leads to copper because I don't think it will hold because I don't believe they welded correctly.
```

---
## \#87 Posted by: Rob69de Posted at: 2017-12-28T19:10:29.984Z Reads: 290

```
Thought about that but when I tried to peel the nickel strip off couldn’t get it of easily
```

---
## \#88 Posted by: Kug3lis Posted at: 2017-12-28T19:14:53.247Z Reads: 288

```
But still I would recommend to solder it ;)
```

---
## \#89 Posted by: Rob69de Posted at: 2017-12-28T19:30:22.143Z Reads: 288

```
Ok I took your advice and put a dab of soldier on connecting nickel on tops of pcb
```

---
## \#90 Posted by: gogomrrobot Posted at: 2018-01-07T00:55:09.393Z Reads: 293

```
@Kug3lis can you explain the balance lead jumper again on your PCB's. I ordered some and well I think I may have asked this question when you were still designing but now that the units are out I need to ask again.

I did look at the front and back of your PCB.

See below picture... do I just fill in those two holes with solder to say for example complete the balance jumper for Cell #7? Without both those holes have a dab of solder balance cell #7 wouldn't be indicated.

<img src="/uploads/db1493/original/3X/7/3/73fa4be034d64ce00779ed05db1f7d41f4599bdb.jpg" width="375" height="500">
```

---
## \#91 Posted by: PXSS Posted at: 2018-01-07T04:25:28.792Z Reads: 279

```
You only need to jump where the positive comes out to the bunch of pads to the corresponding one right next to it. 

He has traces going on the bottom layer of the board. The holes you see are called vias and they are essentially vertical traces that connect layers on the pcb. 

For the first group you need to jump cell 1 on the neg and cell 2 for the pos, for every subsequent group, you only have to jump the pos to the correct number, eg for group 2, you connect pads labeled cell 3 on the pos, for group 3, you connect pads labeled cell 4 on the pos and so on.
```

---
## \#92 Posted by: gogomrrobot Posted at: 2018-01-07T09:14:01.371Z Reads: 265

```
Ok still confused.... what does jump mean. Can u put in a diagram
```

---
## \#93 Posted by: gogomrrobot Posted at: 2018-01-07T09:20:41.878Z Reads: 274

```
[quote="PXSS, post:91, topic:38651"]
For the first group you need to jump cell 1 on the neg and cell 2 for the pos,
[/quote]

So place a wire on neg solder it... run it to box that says cell #1. Additionally... place a wire on positive solder it and then solder other end to the box that says Cell #2?
```

---
## \#94 Posted by: scepterr Posted at: 2018-01-07T09:33:02.419Z Reads: 261

```
Just solder the 2 pads next to Cell # together corresponding to the series of that pack
```

---
## \#95 Posted by: gogomrrobot Posted at: 2018-01-07T09:40:33.195Z Reads: 260

```
I think that makes sense... so literally there are two boxes next to each cell #... so all I have to do is place some solder that covers both 'boxes'... the solid one and the one with a hole next to it?
```

---
## \#96 Posted by: PXSS Posted at: 2018-01-07T13:41:09.462Z Reads: 260

```
Yes. I'd use a wire or 0 ohm resistor
```

---
## \#97 Posted by: Kug3lis Posted at: 2018-01-07T13:46:57.879Z Reads: 259

```
There is no space for 0R I used 1.5mm spacing If I remember just enough to make it easy solder together.
```

---
## \#98 Posted by: Kug3lis Posted at: 2018-01-10T10:27:42.400Z Reads: 255

```
Up Up

10char
```

---
## \#99 Posted by: DeathCookies Posted at: 2018-01-10T13:13:21.967Z Reads: 255

```
I am still curious whats about this PCB? what does it do? what is the benefit?
```

---
## \#100 Posted by: Martinsp Posted at: 2018-01-10T13:48:27.405Z Reads: 262

```
I am currently editing videos about the benefits and also some tutorials for these and my version of pretty much the same concept. I will post them in my thread or maybe create a dedicated one.
http://www.electric-skateboard.builders/t/18650-battery-pcb-shop-launch-repairs-products-and-more-to-come/42870
```

---
## \#101 Posted by: evoheyax Posted at: 2018-01-10T16:30:10.391Z Reads: 259

```
Are you planning a 12s version. It's an interesting idea to say the least, good work.
```

---
## \#102 Posted by: Martinsp Posted at: 2018-01-10T16:33:23.445Z Reads: 244

```
It is designed for up to 13S because a couple of people run it surprisingly without issues with VESC.
```

---
## \#103 Posted by: evoheyax Posted at: 2018-01-10T16:38:48.633Z Reads: 241

```
How can it do 13s when theres only 8 balance lines?
```

---
## \#104 Posted by: JohnnyMeduse Posted at: 2018-01-10T16:40:37.908Z Reads: 260

```
By running them in parallel, like this

http://www.electric-skateboard.builders/t/arch-s-build-log-kaly-nyc-build-dual-6374-focbox-12s4p/25995
```

---
## \#105 Posted by: Kug3lis Posted at: 2018-01-10T16:49:32.753Z Reads: 251

```
The idea was that you not going to run 12s cells in one line, max cases you will run 2 x 7S which in the end will be 14S setup that's why I only have 8 balance leads (- and 7 cells)
```

---
## \#106 Posted by: Kug3lis Posted at: 2018-02-28T20:21:50.028Z Reads: 255

```
The last batch clearance on half price :)

https://shop.3dservisas.eu/collections/pcb
```

---
## \#107 Posted by: elaser Posted at: 2018-05-04T11:18:21.776Z Reads: 248

```
Thanks for making them available, I've just ordered 12  (even if the shipping was more expensive then the pcb how is that???) 
I want to make a 12s4p and it will be my first pack! Can you explain me better this image ![image|690x164](upload://ixQbWiwErbInYCnOikhhDbWlN13.png)  you published earlier where you made that balanced lead connection, what is it and where it goes to? Can you point me to a picture that shows in detail the connections?
![image|216x233](upload://1ma7ARJFaUyqe5TnabJjwlLMr39.jpg) taking this schematics as a reference the balanced lead you are referring goes where? 

Some buying advice of where to source that nice flat cable to connect the pcb +/- (not the flat one for balancing)
Also anyone knows a place where I can buy good Li-ion pre-welded in a 4P pack? (shipping in EU)

thank you!
```

---
## \#108 Posted by: Kug3lis Posted at: 2018-05-04T11:27:05.078Z Reads: 234

```
We are selling them out as not many is left.

There is plenty of information how to connect in this topic has been answered multiple times 🧐

P.S. Your BMS schematic doesn't have balance leads...
```

---
## \#109 Posted by: elaser Posted at: 2018-05-04T11:42:29.180Z Reads: 227

```
Ok I think I understood the connections sorry somehow that schematic made up more confusion now I understand what you were referring to.
```

---
## \#110 Posted by: jadatmag Posted at: 2018-05-29T20:01:11.228Z Reads: 231

```
![im120803031_1|500x500](upload://je7bLDw43QJuIKy4DUhizh9n7RM.jpg)

Can you make something like this for us? With balancy thingies and suchs? A little tape wrapped arround that and the batteries would stay in place rock solid and no spotwelding is needed.

Edit:

Found this: http://www.dx.com/nl/p/diy-4-slot-series-18650-battery-holder-w-2-leads-black-367045#.Ww2yQUiFOUk
Just need the balancy thingies :D

Or someone just sell us some premade 10-12S1P packs with balancy thingies, we're lazy as fuck.
```

---
## \#111 Posted by: Hummie Posted at: 2018-05-29T20:10:24.884Z Reads: 214

```
wires look very thin, also in the one you linked.  the tabs on the one you linked look better..i wonder how many amps either of them could do or what the resistance of the holder is.  if you find a holder with FAT wire and platted copper tabs please post it
```

---
## \#112 Posted by: Martinsp Posted at: 2018-05-29T20:16:55.150Z Reads: 222

```
I would suggest finding someone local because shipping batteries (at least the legal way, disclosing the contents properly :D ) is very expensive.

As far as batteries, they look thin but if you are going to be using new cells and a BMS it may be enough since there is a couple of mA for balancing. If you are using a hobby charger that can balance with higher current you may need to change the wires for some thicker ones.

Also the current on the springs is probably not enough for an esk-8 unless you are going for some high P groups and high voltage
```

---
## \#113 Posted by: moon Posted at: 2018-08-03T13:29:35.256Z Reads: 200

```
Hey @Kug3lis do you have any of these in stock, in the UK?

If not I will just order my own in China
```

---
## \#114 Posted by: Kug3lis Posted at: 2018-08-03T13:37:02.725Z Reads: 193

```
What is left in store https://shop.3dservisas.eu/collections/PCB but the store is not in the UK
```

---
## \#115 Posted by: moon Posted at: 2018-08-06T20:10:30.437Z Reads: 188

```
Did you finish this pack??

I want to do the exact same with a few changes
```

---
## \#116 Posted by: Rob69de Posted at: 2018-08-07T01:38:44.174Z Reads: 183

```
Yes the pack was complete, and used in my Trampa carve.. along with eboosted enclosure..
```

---
## \#117 Posted by: moon Posted at: 2018-08-07T10:16:13.107Z Reads: 182

```
Have you got any build pics?
```

---
## \#118 Posted by: Rob69de Posted at: 2018-08-07T12:15:12.822Z Reads: 182

```
Pictures on old phone, but I built my battery exactly like @Eboosted build, because I used his Carve Enclosure, even 10 gauge wires connecting each battery, only difference was I ran my BMS wires on the side left side and right side, I also shrink wrapped the batteries first and ran bms wires over to the side, on top of srink wrap. Also, I tried using the solder bms spots that were on the Kug3lis  PCB but the bms wires kept breaking. So I just soldered the bms wires on top of positive bus bar and it worked out good
```

---
## \#119 Posted by: moon Posted at: 2018-08-07T12:19:09.320Z Reads: 187

```
[quote="Rob69de, post:118, topic:38651"]
PCB but the bms wires kept breaking. So I just soldered the bms wires on top of positive bus bar and it worked out good
[/quote]

Yeah i would have done this too

Ok thanks. I have looked at his battery builds before, I really didn't know what to think of it.
```

---
## \#120 Posted by: Reelop19 Posted at: 2018-08-07T15:57:16.052Z Reads: 182

```
I’m starting my 12s4p build in the same enclosure. I wouldn’t mind seeing your setup. Thanks
```

---
## \#121 Posted by: moon Posted at: 2018-08-07T15:58:18.282Z Reads: 199

```
![image|375x500](upload://qV5tD7KxM0u22LEl8ZyfViUtF6s.jpg)
![image|375x500](upload://hXCbJ1UDa1PEsTvfaPSES9cm3MQ.jpg)
![image|637x500](upload://xrY2FGOeqTZ1t2eGVUFt5wvkoeP.jpg)
```

---
## \#122 Posted by: cryo Posted at: 2018-08-12T04:56:21.085Z Reads: 181

```
Just curious, how much current can the positive/negative traces carry?
```

---
## \#123 Posted by: Nordle Posted at: 2018-08-12T08:39:39.821Z Reads: 186

```
that are just terminals they don't have to carry much current....
```

---
## \#124 Posted by: cryo Posted at: 2018-08-12T12:17:10.156Z Reads: 180

```
Can u explain? If I draw 60a from those 30q cells they still pass through those terminals to whatever people use to connect them in series. 60a is 60a... I don't understand what you mean when you say they don't have to carry much current
```

---
## \#125 Posted by: Nordle Posted at: 2018-08-12T12:29:14.554Z Reads: 190

```
solder wire from batterys to terminal, and then a second wire right next to that point on the terminal (or in the picture above you could solder ontop of the spotweld)
```

---
## \#126 Posted by: jadatmag Posted at: 2018-10-20T23:29:02.468Z Reads: 179

```
Combine that green thing with this $$$

https://youtu.be/X-L88hga3Mo?t=144

My next board has to be easier than IKEA furniture and Lego.
```

---
## \#127 Posted by: Acido Posted at: 2019-03-17T17:21:56.120Z Reads: 149

```
Im planning to switch to these pcbs to make my batteries faster, and I plan to use JLCPCB to make them, I still need to figure out what settings to use 
I do not have any experience with this so any help would be nice
I guess these are okay to carry 80A from a 4p pack?
And to carry 120A I would need a 6 layer pcb?
I removed the bms traces from the design btw

If you have any interest in buying a few for your pack just send me a pm, maybe even a small GB could happen.
![Screenshot_3|639x500](upload://uzPqWhfjGLweyMUQmcA97HWpJNy.png)
```

---
## \#128 Posted by: Hummie Posted at: 2019-05-23T04:45:13.662Z Reads: 122

```
anyone sell these already connected to cells?
```

---
## \#129 Posted by: deucesdown Posted at: 2019-05-23T07:21:45.365Z Reads: 122

```
https://www.electric-skateboard.builders/t/4-20-a-cell-samsung-30q-cells-and-battery-build-service/74504?u=deucesdown
```

---
## \#130 Posted by: Hummie Posted at: 2019-05-23T16:56:46.764Z Reads: 112

```
@thisguyhere are you selling pcbs connected to cells?
```

---
## \#131 Posted by: thisguyhere Posted at: 2019-05-23T17:12:55.176Z Reads: 117

```
yessir, just select the P count in the options:

![image|690x285](upload://du7JMbkH92JPODEJjZDMd4UWxvl.png)
```

---
## \#132 Posted by: Hummie Posted at: 2019-05-24T01:16:07.572Z Reads: 109

```
Can u rivet a board or get some terminals put on so you could screw down connections.  Any solderless ways.  A through hole you could wind through maybe would be good.  Could do some resistance test.  Hope to get some soon.

OR MAYBE JUST RUN THE WIRE OVER THE TOP AND HOT GLUE IT!  im definitely doing resistance tests doing that.
```

---
## \#133 Posted by: Hummie Posted at: 2019-05-28T22:45:39.822Z Reads: 105

```
r![28%20%20%20no%20through%20holes|690x136](upload://lkJuc1ImhxZ2moMFy1A9h3h9SuH.jpeg) 


this is it.   These have wide copper two ounce strips, double-decided,  with a solder cover on the bottom.  meant to be welded to and soldered at the ends to the other pcb and escs.  

if you want to get some of this first test batch im ordering its 20$ for the two and you do the spot welding yourself.
```

---
## \#134 Posted by: Hummie Posted at: 2019-06-06T18:19:15.488Z Reads: 94

```
I have to try this conductive copper tape. The supposedly conductive sticky part is amazingly sticky.  Ironically it seems safer without the positive side donut attached and it holds better bare. All in all all though this may look flimsy it’s very solid.   This pcb was a mistake at 67mm wide instead of 65 so the tape isn’t as secure here as will be when the 65mm pcbs show that are coming. 
How to test the conductive addhesive?  I want to do a conductivity test somehow.   If it takes twenty amps for five min straight and I can still touch it I’m sold. Doubt it will.    I only have a ten amp supply and can split the copper strip or would that be too low a resistance or something for the supply and break itt?  ![image|375x500](upload://yJoiqMpZKP5AamSAdwsMQnORnX.jpeg) ![image|375x500](upload://dWh35R92oomBxdl3yeiu9kweIgB.jpeg) ![image|375x500](upload://cp0bRJmrCFxO7PWZ3tVNVoSk0Pm.jpeg) ![image|375x500](upload://qo9rdQACll98zON8EOtjS5OndpO.jpeg) ![image|375x500](upload://gMQEFWBEwfvsyvlCtCJ8Sjpkvk4.jpeg) ![image|375x500](upload://mf08JWzS3nNHoVXMbWnjPKFaIE9.jpeg) ![image|375x500](upload://7wjvNf4u2oxLe3gm2aQT6c2j21k.jpeg)
I’ll tear it down to bare cells after riding it and look for wear.  If the solder mask on the pcb can take some rubbing from the cell, which I expect it should and not rub through to the copper but other than that...having been playing with this tape and now on the board I think physically it could be reliable and at worst if it did break, with the tape stuck so well it is unlikely to short through the pack.  But you could maybe push the tape into the positive tab down to the negative.  Unlikely.  assuming it shows good enough with conductivity and continuous heat put on the glue I’ll put them to the real test.    I think a glue connection maybe isn’t possible with cycling of heat and hoping for way too much
```

---
## \#135 Posted by: Vykku Posted at: 2019-06-09T10:31:59.783Z Reads: 84

```
I had a look at a datasheet for one of the best copper foil tapes I could find, 3M 1182: https://www.tedpella.com/technote_html/16074%20TN.pdf

The resistance through a 1 inch square adhesive is 0.01 Ohm according to them. On the cell you have roughly a 15mm circlular contact area, and in that case there is 3.65 times less contact, or 3.65 times higher resistance, so about 0.036 Ohm. At a conservative 10 A per cell, there would be 3.6 W of heat lost in the adhesive, which is a huge amount for that small area and it will definitely heat up instantly to over the spec.

It is a nice idea but it doesn't seem like it will work. These foil tapes are mainly meant for shielding, not power transmission.
```

---
## \#136 Posted by: Vykku Posted at: 2019-06-09T14:24:40.754Z Reads: 82

```
[quote="Hummie, post:132, topic:38651"]
Can u rivet a board or get some terminals put on so you could screw down connections. Any solderless ways
[/quote]

I was thinking to build parallel PCB battery modules with XT30 connectors to handle the current from one to another in the near future. Basically something like this:

![IMG_20190609_151511|375x500](upload://7BAovZ29tS23qt2QDjDkJq26WYK.jpeg) 

In this case the end user would not have to solder at all. Also don't have that in the diagram, but the balancing would be done with a JST 1 pin connector to each module going to a balancing connector. Also would need an XT30 extension for the middle of the pack, and an 2x XT30 to XT90 adapter for the positive and negative terminals of the battery.

There would be some length lost due to the protruding tabs, but that drawing is not to scale and they should be easy to make pretty small, about 8-9 mm of space between each module.
```

---
## \#137 Posted by: Vykku Posted at: 2019-06-09T14:49:05.833Z Reads: 83

```
Here is a very quick rough CAD model of my idea, with accurate scale. The wires would have more slack than in these pics:

![image|690x485](upload://uuzuvoYoejeCKTeOsZ67nForTV9.jpeg) 
![image|685x500](upload://mhZwDy4qI1lfo1vflTixT5hvhb2.jpeg) 
![image|690x221](upload://bwofReOos6vn4aiJFkHCwtF9f0L.png)
```

---
## \#138 Posted by: Hummie Posted at: 2019-06-09T15:58:32.267Z Reads: 83

```
Xt30 are pretty small but there’s thousands of connectors out there even smaller.  It’s appealing to take them apart to be plane legal with just the four cell groups but I broke from that goal with using the two long pcbs 

With the tape it could’ve been broken down easily but the adhesive in this tape is hugely resistant and not usable for any substantial current. The copper strip width and thickness is good enough and I’ll try spot welding this tape.   .06mm I think it is.
```

---
## \#139 Posted by: Hummie Posted at: 2019-06-11T06:54:52.162Z Reads: 79

```
![image|375x500](upload://s1L5Jr0iWfOLiaCZDrdpNB1L5rh.jpeg) ![image|666x500](upload://9AP3hlIfq4DHyT1SHeL97YN3rQE.jpeg) 

The nickel is .2mm and 8mm wide. the cell is solidly connected to the pcb.  The copper in background was too finicky to weld probably because of the adhesive and when it does work it doesn’t make the strong structure the nickel does

And a cell with a hole from doing the copper with adhesive.  And my keys maybe I’ll crank up the settings and make the monokey

I ordered the correct 65mm pcbs and with a chamfered edge but otherwise the same.  If u want these 67mm ones take them for 5$ each plus shipping
```

---
## \#140 Posted by: mishrasubhransu Posted at: 2019-06-11T07:15:54.908Z Reads: 77

```
This looks amazing! You should definitely take it forward. Post it on the no words thread.
```

---
## \#141 Posted by: mishrasubhransu Posted at: 2019-06-11T07:16:51.417Z Reads: 79

```
Hummie, please consider  soldering the tab to the pcb. If you have a high wattage soldering iron that will work the best.
```

---
## \#142 Posted by: Hummie Posted at: 2019-06-11T14:40:55.279Z Reads: 73

```
The welder seems better for making it reliable and fast
```

---
## \#143 Posted by: Hummie Posted at: 2019-07-04T21:51:55.402Z Reads: 48

```
![image|666x500](upload://AvWEvcOM14B8ED2oXexFgHR5bcS.jpeg) ![image|666x500](upload://1ieMqtwE19RY48GExb5gWSVEGWQ.jpeg) if youre in the bay area and want to pick up some of these completed batteries one pair is all new cells and that other with some used cells.    new for 240$ or a pair I have with some used but good cells for 180$.


   includes 48 cells welded on a pcb and wrapped up.  Flexible and equivalent of over 12awg wire series connections.  Tabs are .2mm nickel and all positive terminals have added protector donuts
```

---
## \#144 Posted by: Schulerbible Posted at: 2019-07-05T00:40:29.778Z Reads: 43

```
How much OZ copper were used?
```

---
## \#145 Posted by: Hummie Posted at: 2019-07-05T01:41:18.169Z Reads: 42

```
2oz and double-sided fat traces.
```

---
## \#146 Posted by: Schulerbible Posted at: 2019-07-05T01:43:14.520Z Reads: 43

```
Thank you. I assume those holes are all vias?
```

---
## \#147 Posted by: Hummie Posted at: 2019-07-05T02:07:56.904Z Reads: 45

```
![image|375x500](upload://aZRlUpZGPHLTGJJGZ0g2CoMuZ95.jpeg) ![image|375x500](upload://fTaYhGemjHnWU9XimtfqX0lTvh8.jpeg) ![image|375x500](upload://8kvmXxMcxVyNLbezoq34pRB07Kj.jpeg) ![image|375x500](upload://xAT77MOOjaH5offXbrtjHKshpyC.jpeg) ![image|666x500](upload://wEx7SJGrU10toghFDmxI7zivkDn.jpeg) ![image|375x500](upload://bXuypa8UblHaP0oRpCAskZLnBKw.jpeg) ![image|666x500](upload://rynNk3L8lVvOz0vqPlWYUCGqnUl.jpeg) If that's what the name for through holes is yes.

I like them velcroed to the bottom of the enclosure held by the cells and all needed
```

---
