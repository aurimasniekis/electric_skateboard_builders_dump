# Portable &#124; Custom birch Fiber glass &#124; Enertion trucks &#124; 6355 190 kv &#124; Enertion motor mount &#124; 10s3p LG HG2 &#124; VESC 6 beta

### Replies: 20 Views: 3073

## \#1 Posted by: oyta Posted at: 2017-06-29T17:27:35.267Z Reads: 364

```
After I found this site last summer I got a lot of inspiration to try to build my own :slight_smile: Yes, I read _a lot_ like I read most people do - but what I learned the most of is actually doing the build, trying the parts and failing. I would have done things differently if starting now. I will try to mention some of the things I would have done differently. So let's get to the build :slight_smile:

## Motor, trucks and wheels
<img src="/uploads/db1493/original/3X/0/2/02fe55a03c21a3d31199a9b40ba9361bab8629fa.JPG" width="666" height="500">
First I bought trucks, motor mount and a 6355 190 kv motor from Enertion. I don't like the colors much so I may repaint them someday. Or not :slight_smile: This was november last year. You may notice that I changed the wheels to some original flywheels :sunglasses:

<img src="/uploads/db1493/original/3X/5/0/508423dfef7d19cc58599bbb005b25295513ce37.JPG" width="375" height="500">
Mounting those circlips without a proper tool demanded good stamina and a good mood :smile:

##Battery
The battery was not that easy to get like I wanted for a reasonable price in Norway. I tried some options in Europe for a 10s3p pack - I wanted a small one for my small board I had in mind. In ended up getting really expensive. Luckily I found a guy nearby with a spot welder that he had used for some eBike and similar projects.

<img src="/uploads/db1493/original/3X/b/2/b295f0747ef669e38bb9f5e13d6303fd678a554d.JPG" width="375" height="500">
LG HG2 times 30. Should probably have bought a few extras, but it turned out ok. Unfortunately nkon.nl was not willing to ship to Norway so I found a local webshop selling batteries for ecigarettes. More expensive, but only option I found reasonable.
<img src="/uploads/db1493/original/3X/8/a/8ac9f6ab08b57db0f0a8217efc5fee019e27b54d.JPG" width="375" height="500">
Specs written on the box.
<img src="/uploads/db1493/original/3X/2/b/2bc54c86dd7969d2b4e98124717000868b2d179e.JPG" width="375" height="500">
Glued them with a hot glue gun.
<img src="/uploads/db1493/original/3X/6/c/6ce1a4e3cb1c4a5d00f8eb389ada72d9d40c6fec.JPG" width="375" height="500">
Spot welding
<img src="/uploads/db1493/original/3X/0/f/0feb4db7f54e5c9c79e455f6edd7a6ef900cc4b8.JPG" width="375" height="500">
Finished welding the nickel strips. **Note** This is not the best design as I see it:

1. I should have soldered on 10 AWG cables for the plus and minus end point on the nickel strip ahead of spot welding. Not smart to solder directly on the nickel strip afterwards and it also builds in volume.

1. I would have used a different wiring setup. Me and the guy helping me discussed it a bit and the reason for doing it like this is to have short battery cables. However then I need to isolate between the two rows of battery, and it the battery pack also increases in volume.

1. As you will see further down the balance wire chaos :weary: was a bad design decision. It was just done like this with too little thought.

Look at how @whitepony did it with his 10s3p here https://www.electric-skateboard.builders/t/carbon-jet-spud-freebord-bindings-single-vesc-10s3p-lg-hg2/5805/76?u=oyta That is a nice battery pack.

<img src="/uploads/db1493/original/3X/c/a/cadf6b4876373a1f23ebbb612f448d6a62691fc6.JPG" width="375" height="500">
Adding balancing wires times 2 - necessary? I wanted it to be able to measure the voltage of each pack in the series.

<img src="/uploads/db1493/original/3X/1/b/1b4c1a9b747b023b9242a1e64ea06eda2a1ee06d.JPG" width="375" height="500">
Messy! I've definitely improved my soldering skills during this build. A lot of connectors, cables and joints have been solder. Some quite bad - some redone - some good. The photo shows the batteryback on the board with BMS, VESC6 and other stuff.

I have more coming, but need to go now. Next up is making the plate and more. I will post some more later.
```

---
## \#2 Posted by: Jinra Posted at: 2017-06-29T18:00:31.353Z Reads: 326

```
Wow that BMS is HUGE! I did cell level fusing on my pack in which I soldered fuses to each cell terminal (160 joints!) and my pack works fine. You should be fine soldering reinforcement wire to the tabs, especially since you won't be directly contacting the cell with the iron.
```

---
## \#3 Posted by: oyta Posted at: 2017-06-29T20:48:27.732Z Reads: 318

```
Good to hear! I hope it works fine. The BMS is huge! I do consider a smaller one :) But it has some features that is nice to have. Next post coming up with more info.
```

---
## \#4 Posted by: oyta Posted at: 2017-06-29T21:58:32.915Z Reads: 325

```
## BMS
I ordered a BestTech BMS like this: http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html

The nice thing about it is that it has a switch function implemented. Easy to put together - just solder on a switch. To be sure I also have a XT90s to break the loop.

When ordering this BestTech BMS you set the parameters yourself. **Note again** I wish I'd set the over charge detection voltage to lower than I did - I chose 4.25V. I would rather like to charge to 4.1V and balance it at that voltage. However - for BestTech that was not an option. They only went down to 4.2V - I should at least have chosen that voltage. The reason is, as often stated, that the battery lasts longer if not charging it all the way to max - 4.25v.

Can anyone recommend a balance board for charging that either is 4.1V or is easy to change voltage?

## Wiring
<img src="/uploads/db1493/original/3X/1/3/13be9b080f93cf1ea396bd9f4375f5414254f31b.png" width="690" height="233">
Mostly the wiring. What is missing is the second balance wire I added. I have no fuse :fearful: I guess best practice is including a fuse - how large do you guys use for this kind of power - 60A?

I used 10 AWG for all battery wires between battery (-- BMS --) and VESC. Smaller wires for balancing (I think it was 22 AWG), charging (a bit thicker but my charger do 2 A - not much), switch and voltmeter.

## Making the board
<img src="/uploads/db1493/original/3X/d/d/ddea2b2a964b69c778fa704f72fa18f35661357f.JPG" width="375" height="500">
First - making a vacuum bag. This was not tight - bad tape. Made a second with better tape. Not sure about the English word but it has something to do with Butyl at least.
<img src="/uploads/db1493/original/3X/9/2/922541f716db65cead6077882c3cf09aa9b6ce04.JPG" width="666" height="500">
Sucking out the air to create under pressure. I cut out a shape in "Jackofoam" which is a high density isopor. Unfortunately I did not find any suppliers selling single ply veneers - so I had to use a 4 mm  x-veneer made out of 3 layers of birch ply. As that is already stiff I cannot create the forms I want :frowning:
<img src="/uploads/db1493/original/3X/9/a/9add9e361835b2af32a5acd6baaf89d3006c747e.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/a/4/a4e60a5d6b4c5e191331cebb675d6e755c64434d.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/7/4/747bf1c04201f91f70eabd50afa21d17a5fdbf79.JPG" width="375" height="500">
Cut to the shape.
<img src="/uploads/db1493/original/3X/d/4/d4959fd7730028130a97b86cb38b39bc31f39be8.JPG" width="375" height="500">
Time for some routing. Create a template around to make it a bit easier. Had to screw both the board and the template together with the table.
<img src="/uploads/db1493/original/3X/b/a/ba202f2f07cbfcb55bbe3d984402b00f281a8bfa.JPG" width="375" height="500">
Another perspective.
<img src="/uploads/db1493/original/3X/3/0/307024645404e7daac2371d33346d83c419ea977.JPG" width="375" height="500">
Almost done.
<img src="/uploads/db1493/original/3X/3/e/3ea2081e396e3ea8f452745875034dd0c9a35f98.JPG" width="375" height="500">
Not easy to keep the correct depth as the board has a bit of concave.
<img src="/uploads/db1493/original/3X/1/e/1edbb6bc287a340761cb85fdf2f93cc0119f1435.JPG" width="690" height="388">
Not a good photo - I did get some concave. Approx the amount I wanted.
<img src="/uploads/db1493/original/3X/a/9/a9aa3b9f368c3bda43ab3add92f4e68498a6d329.JPG" width="375" height="500">
Had to reinforce it with epoxy + glass fiber. Never done anything with glass fiber.
<img src="/uploads/db1493/original/3X/2/3/2381147cd9a3f649b4f147e7f2e67e6ce0b4057a.JPG" width="375" height="500">
The photo is taken after it has hardened - I think I used a bit too much epoxy :flushed:
<img src="/uploads/db1493/original/3X/d/5/d5595437a2557d9d3d78bf8ebb30e0f1e9181b94.JPG" width="375" height="500">
It also ran through the mounting holes for the trucks. Drilled the holes again and it was fine.

That is how far I got with the board for now. I was so eager trying it out - so I had to mount everything before making a proper enclosure, painting and grip taping it. So the prototype is up in the next post!  :slight_smile: :grin:
```

---
## \#5 Posted by: oyta Posted at: 2017-07-02T17:47:38.931Z Reads: 275

```
## Setting up the VESC 6

Setting up the VESC 6 was quite easy. The new wizards for motor detection and input control were fine with help texts to most of the buttons. General electrical knowledge is recommended doing this stuff (both building and VESC set up), and it makes it possible to understand the basic stuff. FOC tuning I'd say is a bit more demanding :smirk:

## Temporay fix to test the ride!

<img src="/uploads/db1493/original/3X/1/0/10fb3207d01bf54df80b02174a8b2adef4ac40c9.JPG" width="375" height="500">
Screwed together a temporary frame out of some wood. I had to test it! :slight_smile: 

<img src="/uploads/db1493/original/3X/9/3/93af30aa6212de3acfe659a8b5d3d26720b99949.JPG" width="375" height="500">
Used some velcro to attach the batteries and  BMS to the box. Look at the balance wire spaghetti. Next time I will make a better plan for those!

<img src="/uploads/db1493/original/3X/8/1/812f582b41b2de4db94c33a3f3cb7e9c56dd0528.JPG" width="375" height="500">
Some of all the wiring. The VESC Six has M5 threads made ready for attachment in the alu. casing. So I screwed it down with two screws.

How to you fix/attach stuff to the board or enclosure? Glue? Velcro? Screws and a band?

<img src="/uploads/db1493/original/3X/0/b/0bd7b55828b6f36c357a3f6bf30d92d45dca1f26.JPG" width="666" height="500">
Strapped the box to the board - ready :grinning::grinning: But yes -- it was to close and I could not turn much due to wheel bite :expressionless: 

<img src="/uploads/db1493/original/3X/a/5/a5dc4517003f682705079a2e6b92ff23970432e6.JPG" width="666" height="500">
From below. The motor wires was taped to the board. Not sure how to have those wires fixed permanently. Maybe I should have done like @longhairedboy routing a gate for the wires. But it would have been better doing that ahead of the fiber glass layers. 

And - oh no - it just work a bit and very unstable :frowning: I thought it was the Winning remote I am using after reading so much bad reviews about it.

Luckily it was just that I had broke the connector to the transceiver for the remote. I soldered on a new one to the wire - and yippii! It works!! I have just bearly tested it - looking forward to do som kms to gain some experience and see if it works ok.

So what to do now?

* Fix wheel bite on the temporary box.
* Order new bushings (the original on the Enertion does not fit me and my use)
* After the vacation: Create a proper enclosure in fiber glass and maybe a finish in glass fiber. Never done that - so excited to get on to it.
* Figure out the final attachment of the components. To the enclosure or to the board? If to the board - how shall I do it? I have some velcro, glue and I am trying to think of better ways with some bands/straps and screws or something.
* Painting both sides
* Grip taping
* Drill and glue inserts for enclosure. 
* Ride!
* Buy metr dongle thing for logging?
* Buy new BMS for lower over discharge threshold?
* Probably a lot more :slight_smile:

..and not in that order. I hope I can get going again in august. Excited!
```

---
## \#6 Posted by: oyta Posted at: 2017-07-07T20:13:26.061Z Reads: 248

```
## Testing
<img src="/uploads/db1493/original/3X/7/a/7a2ed3a231cf8b63a32bfecbaaf56ac77df697a5.GIF" width="180" height="320">
So I got to test it a few days - **and it so much fun**!! :smiley: At least as long as the remote is functioning. I bought two Winning remotes from a group buy last year - bad decision! :wink: My short experience is that it drops out in some areas and quite often.

However I bought a new one, some grip tape and some new bushings! Received it today.
<img src="/uploads/db1493/original/3X/c/c/cc1a2289449c6bc8cfd6bc53191df30eb77f753e.JPG" width="375" height="500">
"Unfortunately" I am leaving for the summer vacation tomorrow and it will be a while before I can continue the esk8 project :grin:
```

---
## \#7 Posted by: L3chef Posted at: 2017-07-07T22:08:01.560Z Reads: 230

```
Sweet build. What are those 3 cylindes on the wall? Is it a part of the vacuum pump?
```

---
## \#8 Posted by: NickTheDude Posted at: 2017-07-07T23:09:10.984Z Reads: 223

```
Nice build, when you get the chance could you let me know how the Venom Eliminators feel? I was considering getting some but couldn't find too much on what they actually feel like.
```

---
## \#9 Posted by: oyta Posted at: 2017-07-08T03:13:10.681Z Reads: 219

```
The three sylinders are a vacuum reservoir. When the pump has sucked enough air out of the system and the under pressure is large enought I flip a switch/valve. The the system is closed and I can turn the pump while keeping the vacuum.

As my system is not sealed properly (old and bad sealings) I still need my pump on :wink:
```

---
## \#10 Posted by: oyta Posted at: 2017-07-08T03:14:55.298Z Reads: 220

```
I will! 👍 Ask me again in august if you haven't heard from me.
```

---
## \#11 Posted by: oyta Posted at: 2017-07-27T21:32:35.345Z Reads: 220

```
Returned from vacation and slowly moving forward. Next up is creating an enclosure in fiberglass with polyester. New stuff for me.

<img src="/uploads/db1493/original/3X/3/c/3c33a01dc3aa3f8a1bf64334f862933d218dd3dd.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/c/2/c28f667d05c000a548c3a48c7ef88df2ae3334ca.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/0/4/04ae70263ebbc4010d419ea0256f438ff68eaea2.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/7/8/7875f8334d9569e6bd27bce39681bb30b2089de6.JPG" width="375" height="500">
Used Jackfoam as a mold. This was as long as I got today.
<img src="/uploads/db1493/original/3X/a/b/ab225908665660b11a8f77a0fc20569d350a6f53.jpg" width="274" height="499">
Testing how to do the polyester and fiberglass vacuuming. Messy stuff and smells quite bad. It killed the Jackofoam but using plastic in between seems to work. Tried to use a fluid that would make it slip easier, but  it seems as the polyester did not harden good enough using it.

Not decided yet but I guess I need to have the mold on top of the board, then a sheet of plastic, fiberglass and polyester and put everything in the vacuum bag.
```

---
## \#12 Posted by: oyta Posted at: 2017-08-29T19:20:03.407Z Reads: 201

```
<img src="/uploads/db1493/original/3X/7/f/7f3b7b4bc0a7596d623d29e6bbb1d26a7cd507e9.jpg" width="500" height="281">

<img src="/uploads/db1493/original/3X/b/b/bbbfdbb83283defbd91f81abad8a1f8915ce9676.jpg" width="500" height="281">


<img src="/uploads/db1493/original/3X/e/9/e96c0096a2606b6c246d73d738ee65b68663aa63.jpg" width="500" height="281">
M5 insets

<img src="/uploads/db1493/original/3X/3/c/3cb409fcde0cce7f4585a659744708d7b7822b6b.jpg" width="500" height="281">
Not exactly MasterCho finish :wink:
 
<img src="/uploads/db1493/original/3X/6/5/65fa679286be9b161934fea8be71f77d2647f50c.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/9/0/90f3ed25645e08f25573bf937e0cff8ae6805431.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/a/5/a5eae6c2e9524fc6980d874c671ba72f64c4d6b1.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/e/f/efe0eab16ebb6a66031239007624c12fdec39ecb.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/5/6/5653f803d7b46a47e7e14e205b5c63b68cfdde41.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/a/8/a82eea1fd6d020cb4ca7f25073fa2b4ca23aec86.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/0/2/02e921cec2eb0e86140e02c86a08c20bf6554702.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/a/5/a58a1d22a8637716e4eb579ea7eeafae32bd43c2.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/8/1/81e547e511e9356ce5ca5b8032196f5673b5d520.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/5/f/5f4c3a3e67ba1a885e666b4fc05fb1a31dc918ce.jpg" width="690" height="388">
:smiley:
```

---
## \#13 Posted by: oyta Posted at: 2017-09-01T19:18:24.311Z Reads: 178

```
Now I've had a few runs with the Venom using 91A SHR Eliminator board side and Downhill 88A SHR road side.

The Venom bushings are waaaaay better than the original Enerition bushings. I am really satisfied with how the board performs considering the size and parts. With the 90mm Flywheels and these bushings it quite fun carving while throttling a bit. It cannot be compared to carving a Dervish - but hey - this is a small practical board for commuting and transport.
```

---
## \#14 Posted by: Lionpuncher Posted at: 2017-09-03T02:50:09.822Z Reads: 174

```
 Really cool build thread. Thoroughly enjoyed seeing your process. In the middle of my first build. 
Your finished product looks great!
```

---
## \#15 Posted by: oyta Posted at: 2017-09-03T07:52:48.590Z Reads: 167

```
Thanks for the good words! Good luck with your build!
```

---
## \#16 Posted by: TunaTee Posted at: 2017-09-26T16:05:00.815Z Reads: 153

```
awesome build thumbs up.
```

---
## \#17 Posted by: nmagz3 Posted at: 2017-10-12T21:30:21.035Z Reads: 145

```
Great build thread!  I love how you made your own enclosure.  I've read and watched a lot of tutorials on vacuum forming fiberglass & carbon fiber.  I have everything I need except the mold.  I've been debating one what I should use.  I noticed you used a material called Jackfoam.  It looks very moldable!  

3 questions for you if you don't mind.  Would you recommend it?  If so where can I get it (I'm in the states).  If not, what other material would you recommend?

Thanks in advance!
```

---
## \#18 Posted by: oyta Posted at: 2017-10-16T21:35:01.236Z Reads: 129

```
@nmagz3 

* If I would recommend "Jackofoam". Yes - it is very easy to shape. However you should do a better job than I did. It is important that the surface is as even as possible. If the foam mold is uneven - the enclosure (fibreglass or carbon) will also be. So just be thorough and you will be fine. Secondly - no resin must leak into and come in contact with the foam. The resin (at least Polyester as I used) will destroy the foam and the result will not be good. You can see an example of shaping of XPS foam here:

http://www.thinairpress.com/skateboard-building/2015/1/23/how-to-shape-a-foam-mold-for-a-custom-skateboard

* Where I come from there is a similar product named Styroforam. It is high density foam of type XPS (extruded polystyrene). I am not quite sure what density rating I had, but it is quite hard. This is what I used: https://www.jackon.no/bygg/jackon-xps/jackofoam/ (in norwegian). I guess something like this is similar: 

http://www.homedepot.com/p/Owens-Corning-FOAMULAR-250-2-in-x-48-in-x-8-ft-R-10-Scored-Squared-Edge-Insulation-Sheathing-52DD/202085962

* Another way to it is using wood or similar. Like whole wood, MDF or plys of some sort. It will be solid and reusable a lot of times. If done nice - the result will be nice. However - it takes a lot more time creating the mold.

Good luck!
```

---
## \#19 Posted by: nmagz3 Posted at: 2017-10-18T17:12:58.973Z Reads: 112

```
Hey Brotha, thanks so much for the advice!  I was thinking would too but thought it might get complicated as I'm not a experienced woodsman.  Then I saw your build (beautiful by the way) and admired how your enclosure came out.  With your advice I'll now take a look at both the Styroforam and the Wood.  Thanks again, I really appreciate it!

- Neil
```

---
## \#20 Posted by: oyta Posted at: 2018-04-16T20:24:52.464Z Reads: 74

```
Last year I joined the DieBieMS group buy. So the **2018 upgrade** includes installing the BMS and making the whole board with installations more robust. 

 ![IMG_5588|666x500](upload://xliPkk3TyCIgkr2dZGThgiH1djl.JPG)
![IMG_6548|375x500](upload://qKoJrrk4EIM3VvO7Hm2A5ZgeERj.JPG)
Redid the motor wires! Sugru makes life easier :slight_smile: 

![IMG_1186 2|666x500](upload://85nkaRzWGDgUISHJeg7nZ8xCtF8.JPG)
Implementing and testing the new DieBie MS! Nice one!

![IMG_9714|666x500](upload://38rhaODm4HAdgGAZCKnWJqhojkg.JPG)
Redid almost all the wires.

![IMG_0392|666x500](upload://z3EYepZ1fzlgt2CAGCuvpFes8sM.JPG)
Complete :smiley: 

![IMG_2153|666x500](upload://8OEM9QyPyr4pIT3Tg0TPmQ6YeIA.JPG)
Up and running :) (and "perfectly" space cut for the OLED :flushed:)

![Copy of esk8 wiring with DieBieMS Large|690x259](upload://8wuZPJnlsYy2EUGOEmZmSik6Yrk.png)
The power wires. In addition to this I have a momentary switch wired to the "Power"-port and an OLED to the "Display"-port. And to the VESC I also have a receiver and a metr.at BT-module.

You'll find info about @JTAG's  DieBie MS at http://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639?u=oyta. Fedestanco has set up a new group by for this one: http://www.electric-skateboard.builders/t/new-batch-6-12s-open-source-diebiems/52240?u=oyta. Had my first 6 km ride today - esk8 :heart_eyes:
```

---
