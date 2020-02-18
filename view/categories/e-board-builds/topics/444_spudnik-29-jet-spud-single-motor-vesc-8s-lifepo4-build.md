# &ldquo;Spudnik&rdquo; &#124; 29&rdquo; Jet Spud / Single Motor / VESC / 8s LifePo4 Build

### Replies: 49 Views: 7821

## \#1 Posted by: siggs3000 Posted at: 2015-11-11T07:35:39.618Z Reads: 464

```
I'm sure it'll be worth the wait but my VESC has finally arrived from down under and I think that was the last part I needed to finally put it all together. 

I started tonight by soldering some connectors onto the three wires from my VESC which will be connecting to my Enertion motor. So far so good. (save for a few "practice" solders)

Anyway, my first **question** is already upon us. With three black wires coming off the VESC and three black wires coming out of the Enertion motor, what gets connected to what here? I have a few good diagrams of the wires on the VESC but it's hard to tell what's what on the motor. 

From there, I'll be on my way! 

- Jet "Spud" 29" board with extra long wheelbase 
- Enertion R-Spec Motor
- VESC
- Enertion motor mount
- Caliber Trucks
- Generic flywheels
- 2 4s 8400 LifePo4 batteries by Zippy (will wire in series) 
- Kama Nunchuck 
- DIY Skateboards power switch
- Alien carbon-look housings for ESC and Batteries 

Wish me luck!
<img src="/uploads/db1493/original/1X/e6915dd50a3b2c17a0963b211a91e285f0123861.JPG" width="666" height="500">
```

---
## \#2 Posted by: trbt555 Posted at: 2015-11-11T08:37:57.399Z Reads: 431

```
Looking good !
 Will probably be a FUN board to ride. I do wonder about risk of speed wobble with the short wheelbase though.

Regarding the 3 wires to the motor: it doesn't matter which goes where. If the motor runs in the wrong direction, just switch any two wires and you're good.
```

---
## \#3 Posted by: treenutter Posted at: 2015-11-11T14:40:37.942Z Reads: 420

```
Ya! @siggs3000 great to see that you've made so much progress! @trbt555 is right that you can swap a motor wire if your board is going the wrong direction. However, since you're using VESC and the nunchuck, you can also use the reverse button to swap directions more easily. In BLDC tool choose "Current with Reverse."

Another tip from my recent build experience; use VESC to limit RPM on your first few rides. Much better to start slow and increase the speed once you are confident that everything is glued/screwed/connected well. 

RE: you motor wires, I suggested taping them once they are connected to the leads to the ESC, this is one point where vibration can easily separate the connection and if that happens while you're riding you'll have no brakes!

You're gonna have so much fun! What charging solution did you end up choosing?
```

---
## \#4 Posted by: psychotiller Posted at: 2015-11-11T15:44:31.178Z Reads: 371

```
That looks like it's going to be a super fun setup
```

---
## \#5 Posted by: torqueboards Posted at: 2015-11-11T16:55:46.786Z Reads: 372

```
Awesome deck! I've been wanting a 29" deck lately!
```

---
## \#6 Posted by: siggs3000 Posted at: 2015-11-11T17:50:07.185Z Reads: 386

```
Thanks everyone! I'm pumped to finally be getting started. 

This is a pretty cool deck for this because the trucks are pushed all the way to the edges of the board. So it's wheelbase is longer than a normal board of it's size. It's also super wide. My goal is to have a very compact board that's easy to carry around and doesn't draw too much attention to itself and has some space in the center between the batteries and esc to I can carry it like a regular board. I'm 145 lbs so didn't need that much power so a single motor seems fine enough and since it's an r-spec and with 8s, I think it should be able to handle the hills here in San Diego. (Not too steep) 

https://www.muirskate.com/longboard/decks/70513/jet-2015-spud-29-longboard-skateboard-deck-w-grip

@treenutter I ended up exchanging the weird 8s 4000mAh lipo's I originally had, for a pair of 4s 8400 LifePo4's that I'll wire in series. The nice thing about these is that charging 4s is infinitely easier and the LifePo4 chemistry alleviates some of my explosion concerns. The downside is that these batteries are a little bulkier than the lipo's but I think it's a good tradeoff. 

Thanks @trbt555 for the wiring tip! I'm going to try to bring it to life tonight without any big sparks or smoke...
```

---
## \#7 Posted by: onloop Posted at: 2015-11-11T22:00:45.848Z Reads: 346

```
LOOKS SICK!

also, just so you know the VESC is already pre-programmed to work with that motor. 

just setup the controller and go!
```

---
## \#8 Posted by: onloop Posted at: 2015-11-11T22:02:14.176Z Reads: 346

```
Also, i suggest changing the Build thread title to better represent your build & make it easy for people to find when searching.
```

---
## \#9 Posted by: siggs3000 Posted at: 2015-11-11T22:31:52.770Z Reads: 349

```
Thanks @onloop! Good to know about the VESC too! (I also updated the thread to be a little more descriptive)
```

---
## \#10 Posted by: onloop Posted at: 2015-11-11T23:12:46.160Z Reads: 346

```
much better title.... i know i am being picky... but feel free to also give your build a name too (not compulsory). Also i would write "jet spud" because people who already own this deck might want to convert it to an eboard one day. They might search the name of their deck.
```

---
## \#11 Posted by: longhairedboy Posted at: 2015-11-12T14:27:57.417Z Reads: 326

```
Spudnik! 

I love that deck. That's going to be a sweet ride.
```

---
## \#12 Posted by: torqueboards Posted at: 2015-11-12T18:56:24.142Z Reads: 314

```
I need to make me one of those :smile:

Update - I just ordered one :smiley:
```

---
## \#13 Posted by: siggs3000 Posted at: 2015-11-12T23:39:19.475Z Reads: 310

```
@torqueboards nice! It's a spud invasion!
```

---
## \#14 Posted by: torqueboards Posted at: 2015-11-13T01:22:53.510Z Reads: 306

```
@siggs3000 Nice choice :smile:
```

---
## \#15 Posted by: siggs3000 Posted at: 2015-11-13T02:20:22.224Z Reads: 330

```
Build day #2 update:

- All soldering is done but some of my earlier solders will probably be re-done for piece of mind. I was getting exponentially better at it each time. 

- Worked out an issue I was having with the BLDC on my Macbook Pro, finding the proper USB port address but got some excellent help in the thread for OSX BLDC and made contact with the VESC. 

- Once in the VESC, I configured the Kama Nunchuck and rebooted the VESC. I held my breath and while connected to just one 4S pack, eased the nunchuck trigger upward and WE HAVE CONTACT! The motor purred to life and spun the drive wheel with smooth ease. I even apparently nailed the belt alignment on my first try. (Beginners luck) 

- I upped the ante by pulling in the other battery pack and put it into series to see what it sounded like at 8S. Big spark on connection but I powered though and hit the trigger and now it sounds more like a mini F1 car. This is going to be awesome... 

- Messing around for a little bit longer and inspecting the alignment of the drive gear and stuff, my voltage alarms sounded going off. Should've discharged and charged earlier this week when I got the VESC shipping notification :frowning:

- Running my first charge now. 

- Will go to Home Depot tomorrow to get the screws and wire conduits needed to lace it all together and if all goes well and time allows... the maiden voyage!
```

---
## \#16 Posted by: siggs3000 Posted at: 2015-11-13T02:21:22.123Z Reads: 302

```
[quote="longhairedboy, post:11, topic:444"]
Spudnik
[/quote]

And the build has an official name now! "Spudnik!" Nice one!
```

---
## \#17 Posted by: treenutter Posted at: 2015-11-13T03:30:07.660Z Reads: 302

```
Congrats @siggs3000 it sounds awesome! Looking forward to seeing some pics and\or footage! Have a fun and safe first ride!
```

---
## \#18 Posted by: siggs3000 Posted at: 2015-11-13T05:11:05.357Z Reads: 336

```
Nothing I'm most excited about the way the switch looks. It's the small things...

<img src="/uploads/db1493/original/1X/1ee009b6f388e7b32cb05944e12af3301ccf77a2.jpeg" width="375" height="500">
```

---
## \#19 Posted by: siggs3000 Posted at: 2015-11-13T05:54:01.801Z Reads: 344

```
Space is tight on a 29"board. But it's running perfectly so far. Tomorrow will be assembly. 

<img src="/uploads/db1493/original/1X/8d0979b680728d14266a7714d3cc22781974a7cf.jpeg" width="666" height="500">
```

---
## \#20 Posted by: siggs3000 Posted at: 2015-11-13T06:27:34.269Z Reads: 352

```
Well, it was jubilation followed by some serious fireworks and then sadness abounds. 

I put my board on its wheels to watch it inch forward. To do so, I mounted my vesc temporarily and it moved slightly during the first few inches travelled. The back of the capacitor board made contact with the PPM input prongs and it was a fairly epic light show and then silence. 

For those using this model of the vesc, I recommend putting some e-tape on the cap board and/or the PPM prongs... The vesc seems fried and the build has hit a speed bump but it will not be stopped!

<img src="/uploads/db1493/original/1X/20163b4c7ebb40a81842db5aaa89241981a5b142.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/1X/831e5f930d605031d648a78f15c4aa56a5204973.jpeg" width="375" height="500">
```

---
## \#21 Posted by: elkick Posted at: 2015-11-13T13:22:54.919Z Reads: 328

```
Thanks for mentioning, I'll insulate that connector immediately. For those using the connector with ppm it might be no issue though, but for everybody else it will cause a shortcircuit even with heatshrink.
```

---
## \#22 Posted by: psychotiller Posted at: 2015-11-13T14:16:24.356Z Reads: 318

```
Dammit! That's sucks man..
```

---
## \#23 Posted by: treenutter Posted at: 2015-11-13T15:46:05.630Z Reads: 311

```
@siggs3000 No! Oh what terrible luck! Sorry to hear it man! Ye olde version of VESC that I use doesn't  have those prongs, I had to solder PPM/servo extension directly to the port on the pcb. Now I feel lucky because I never would have thought of that potential for a short! So does it seem like you'll need a new VESC?
```

---
## \#24 Posted by: siggs3000 Posted at: 2015-11-13T16:52:39.402Z Reads: 306

```
Bad luck for sure but in a way, I'm glad it happened early so I know what avoid in the future. 

I think that probably fried it pretty well indeed. It was 8S and that's a lot of voltage to put into that servo port! It was a pretty epic sight when it went off. Three massive sparks came off the board and actually landed on the floor, staying hot and bright for a split second or two!
```

---
## \#25 Posted by: kai Posted at: 2015-11-13T16:58:09.738Z Reads: 295

```
Sorry bro. Do you think you can fix it? Or do you need to get a new one?
```

---
## \#26 Posted by: siggs3000 Posted at: 2015-11-13T17:01:30.141Z Reads: 292

```
I'm going to order a new one this morning. I think it's toast. 

Everyone with this model should insulate those prongs or even trim them down.
```

---
## \#27 Posted by: longhairedboy Posted at: 2015-11-13T20:23:25.167Z Reads: 286

```
There's also the option of casting it in potting epoxy. If the whole thing's encapsulated in plastic  (except the bus ports) it would be very difficult to short anything out, and probably make the VESC hella easier to work with since it would then be a plastic brick instead of a series of shorts waiting to happen. 

it would, however, make repairs to the components impossible, so i suppose that's a downside if you're used to fixing things and not replacing them.
```

---
## \#28 Posted by: siggs3000 Posted at: 2015-11-13T21:12:05.067Z Reads: 278

```
@chaka I just placed an order for a new one from you. I'm going to mount it permanently before wiring it up this time...
```

---
## \#29 Posted by: siggs3000 Posted at: 2015-11-13T21:15:53.901Z Reads: 283

```
That's a pretty good idea. Someone should also make a minimalist housing for it that utilizes it's mounting holes on raised threaded posts like the ones for arduino boards. The only thing we would have to add is a way to lash the caps in place to keep them separated from that servo port. It would be a cool 3D printing project for those that know how to design them.
```

---
## \#30 Posted by: onloop Posted at: 2015-11-13T22:05:08.144Z Reads: 293

```
Hey @siggs3000 I got your email about this i just didn't get a chance to reply yet.

It sux man....  I have personally destroyed 3 vesc so far from shorting accidentally.

I don't think it's a design flaw per se, the problem is the product is just not a finished product. It's a bare pcb! which is just asking for trouble...

Its worth nothing that a short can pretty much occur anywhere on the vesc when it's powered. I destroyed two vesc because the usb port touched a pcb mounted cap on the other vesc it was connected to. Boom.

@jacobbloy and i have been working on a design for  a lid and base made from pcb that will screw onto the vesc to help prevent this from happening.... it all adds to the cost though. Might have something by end of month.

The other option is some shrink tube. Or i saw one guy use liquid tape. 

You can send the vesc back and I'll try to get it repaired for you. Submit an RA through the user account page at enertion.
```

---
## \#31 Posted by: siggs3000 Posted at: 2015-11-13T22:19:58.606Z Reads: 276

```
Thanks @onloop - I wasn't asking for a warranty or anything. I definitely blew it up. 

I just wanted to provide some feedback about having the contacts of the caps in such close proximity to those servo pins that are pointed right at it! With the cap board able to move freely, it's just something to keep in mind for future iterations. 

I ordered a new one already so I can move forward without much delay. I appreciate the offer to RA it though.
```

---
## \#32 Posted by: jacobbloy Posted at: 2015-11-13T22:47:34.260Z Reads: 285

```
Maybe Jan order we will add 3 16mm X 25mm caps to the pcb, already designed the board, still have wires going from the power pads to the cap part but it won't move and will be small enough to still fit in a case, you have them at 90deg or standing up!
```

---
## \#33 Posted by: siggs3000 Posted at: 2015-11-13T22:58:42.302Z Reads: 285

```
I think that would be sweet!
```

---
## \#34 Posted by: chaka Posted at: 2015-11-14T06:41:54.885Z Reads: 293

```
I hope you don't mind it in white. 

<img src="/uploads/db1493/original/1X/433d154bc9e78d6876b7ce767db020b25118d58b.jpg" width="690" height="388">
```

---
## \#35 Posted by: siggs3000 Posted at: 2015-11-14T07:21:28.039Z Reads: 290

```
Oh sweet! Looks a little more designer-edition in white
```

---
## \#36 Posted by: cmatson Posted at: 2015-11-14T15:11:54.939Z Reads: 288

```
first thing that came to mind was storm trooper VESC, lol.

Hopefully one of those is mine too
```

---
## \#37 Posted by: siggs3000 Posted at: 2015-11-20T04:41:12.818Z Reads: 308

```
As I await my new vesc, I found myself with a little free time tonight so I decided to mount the enclosure. The spud has a lot of concave and on top of that, my LifePo batteries are pretty thick. (8400 mah each) that combination means that things are going to be tricky. I had this carbon-look enclosure measured for my original batteries but I decided to try to make this work. 

I got some extra long screws and some super thick, cushy, rubbery weatherstripping. The batteries fit into the enclosure perfectly side-by-side without a mm to spare. And though I planned to have a second smaller enclosure for the vesc and power switch, I think there might just be enough space to squeeze it into the one bigger enclosure with the batteries. 

It came out looking a lot cleaner than I thought it might. 

Tight fit but there might just be enough space for the VESC in here too...
<img src="/uploads/db1493/original/2X/d/d00c2f5ac75dd4a94883d827d3c7effb0085acfe.JPG" width="666" height="500">



On first mounting, we may have some fit and finish issues.... Thick batteries and a lot of concave.... 
<img src="/uploads/db1493/original/2X/9/978a5d1f2782af00c0da71af2b0807372088e328.JPG" width="666" height="500">



Weatherstripping to the rescue! Luckily it doesn't rain in San Diego so I'm not worried about weatherproofing for real but we do need to look good...
<img src="/uploads/db1493/original/2X/4/4c752d942d1084ff57060af7d2d1a97f9453823e.JPG" width="666" height="500">




Can't see the cool lips design anymore but it's a good tradeoff. 
<img src="/uploads/db1493/original/2X/6/6933994a73cff5443ca3df08ef4d6690949c8d4a.JPG" width="666" height="500">




Just an ESC away from a first ride now
<img src="/uploads/db1493/original/2X/e/e65d3cf53fd07fe359b54c11cb122722eceb72f2.JPG" width="666" height="500">

<img src="/uploads/db1493/original/2X/f/fb473f39ec8e61754327c8d099cff6448c2d0e09.JPG" width="666" height="500">
```

---
## \#38 Posted by: cmatson Posted at: 2015-11-20T04:45:38.363Z Reads: 293

```
nice job on taking something that most people would just discard for not fitting, and making it work!
```

---
## \#39 Posted by: torqueboards Posted at: 2015-11-20T04:55:57.795Z Reads: 290

```
Looks great. I just bought one of those decks too :smile:
```

---
## \#40 Posted by: kai Posted at: 2015-11-20T12:38:12.881Z Reads: 291

```
Wow. That board really does have a lot on concave. It is like a hole you can't get out of lol
```

---
## \#41 Posted by: longhairedboy Posted at: 2015-11-20T13:52:18.049Z Reads: 271

```
Spudnik is my new favorite electric potato. This thing is going to be quick too!
```

---
## \#42 Posted by: treenutter Posted at: 2015-11-20T17:05:14.531Z Reads: 273

```
@siggs3000 I hope that VESC fits because that looks great! Nice workaround dealing with all the concave!
```

---
## \#43 Posted by: siggs3000 Posted at: 2015-12-16T19:08:57.380Z Reads: 281

```
The Spudnik is officially back on track with the arrival of my shiny new @chaka VESC yesterday. 

<img src="/uploads/db1493/original/2X/1/1132e2a48c868116c3e738a8535e26ae5e32bb1e.jpeg" width="375" height="500"> 

It's super nice with ultra heavy 10 gauge wire and big XT90 connectors. I soldered the supplied female half of the xt90 to my battery connector and spliced a new battery gauge in there while I was at it. I uploaded @onloop's xml settings for the Enertion R-Spec motor onto it via the newest version of the Mac BLDC and hit the trigger on my kama nunchuck and everything was looking good!

I crammed everything into the enclose (tight fit but good to go!) and drove it a couple of feet in my living room. Then it hesitated and then stopped responding to the kama input. I opened it all up and saw that the vesc was still lit up and and I emailed @chaka to ask about troubleshooting. He responded even though it was about midnight in our time zone! And I was able to use motor detection to see that both the vesc and motor were still working properly. It was a dud kama! 

Screw that thing, I decided and ordered a pre-built badwolf version of the gt2b from Chaka's site and he shipped it out today. Life is too short to depend on bluetooth! I should finally ride this baby this weekend if all goes well!

<img src="/uploads/db1493/original/2X/c/c9daa64dfd5b4bb9d2eb5ff9404cbe779768c426.jpeg" width="666" height="500">
```

---
## \#44 Posted by: longhairedboy Posted at: 2015-12-16T20:40:04.237Z Reads: 270

```
Mmm mmm mmmm. That's the good stuff right there, son.
```

---
## \#45 Posted by: torqueboards Posted at: 2015-12-18T05:51:38.231Z Reads: 264

```
Bluetooth connection is unreliable :frowning:

Looks great! I got my 29" Jet Spud too! I just need to finish it :smile: 

 <img src="/uploads/db1493/original/2X/3/3332844ecf2b07dab47ebfea00d88c200e35e198.png" width="690" height="400">
```

---
## \#46 Posted by: siggs3000 Posted at: 2015-12-18T07:17:45.421Z Reads: 260

```
Looks good with two motors!
```

---
## \#47 Posted by: lox897 Posted at: 2015-12-18T10:47:21.796Z Reads: 256

```
Build thread please! Looks cool!
```

---
## \#48 Posted by: siggs3000 Posted at: 2016-01-26T00:08:25.545Z Reads: 248

```
Well it's taken a village and has been a journey but I took the madden voyage today on the Spudnik! I had a few issues in getting my BLDC settings right so @chaka took the time to hop on the phone to walk me through it today. Amazingly this was also after helping me in countless email questions and even a reflashing of my firmware and installation of custom 11" motor wires. I can't say enough about that kind of customer service. 

After dialing it in and screwing it shut, I put my helmet on and hit the road for the first time to scuff up those shiny wheels. I squeezed the trigger and almost went flying off the back of this little board but held on and tapped the brake, promptly almost sending me over the handlebars. Holy Shinto, this thing is fast and responsive! I'm going to dial back the amps before my next ride until I get the handle on it. 

Thanks to everyone who has helped along the way. It was worth the trip! 

Here's a pic of the enclosure before I closed it up. Tight fit! The last things I need to work out are:

 1. A power switch of some sort
 2. Flush mount that voltage gauge 

<img src="/uploads/db1493/original/2X/f/f9f3a49205e80955f6efa79a34aa5132563ff5b2.JPG" width="375" height="500">
```

---
## \#49 Posted by: RunPlayBack Posted at: 2016-01-26T02:46:55.430Z Reads: 244

```
Yes! The original E-Spud! I got a lot of love for this thread because once you posted pics of that deck, I decided not to get an Evolve and go DIY. The Spud is super challenging as a first build but totally worth it. Congrats getting it up and running! PS - if you ever decide to upgrade to a 10s Space Cell, the enclosure I made for this thing fits like a glove, especially over those large wheel wells.
```

---
