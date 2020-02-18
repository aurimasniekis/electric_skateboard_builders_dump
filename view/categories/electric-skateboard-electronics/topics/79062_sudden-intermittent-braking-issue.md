# :exclamation: Sudden Intermittent Braking Issue?

### Replies: 47 Views: 736

## \#1 Posted by: Sascha_stevenson Posted at: 2018-12-26T21:09:50.640Z Reads: 187

```
Hi,
My board sometimes has a sudden jolt from the brake at full. This is completely random and I don't really want to eat street any time soon. Also some times it won't brake at all. WTF IS HAPPENING!?

I am using:  
Mboards 7s2p
Streetwing - focbox 
Streetwing - mini trigger remote
Anything else you need to know about the build please ask as I really need help with this!
```

---
## \#2 Posted by: Andy87 Posted at: 2018-12-26T21:11:21.209Z Reads: 182

```
Do you use a bms for discharge?
If yes than the bms could cut out if you for example break with full charged battery or if you pull more amps than your bms can handle
```

---
## \#3 Posted by: Fiori Posted at: 2018-12-26T21:12:00.048Z Reads: 174

```
Most likely your phase wires(motor wires) are shorting: check them and make sure they are properly insulated and not touching each other.

EDIT: If it doesn't brake, accelerate or work at all sometimes then most likely your BMS is cutting power to your FOCBOXES.
```

---
## \#4 Posted by: Sascha_stevenson Posted at: 2018-12-26T21:14:41.193Z Reads: 154

```
@Andy87 & flori I will check with Mboards if the BMS is for discharge.
```

---
## \#5 Posted by: Andy87 Posted at: 2018-12-26T21:15:58.163Z Reads: 145

```
If yes, than also ask what’s the rating for the discharge. I mean how much amps the bms can handle.
```

---
## \#6 Posted by: Andy87 Posted at: 2018-12-26T21:17:12.071Z Reads: 142

```
Did you notice that you can’t break when you fully charged or is it totally random?
```

---
## \#7 Posted by: Sascha_stevenson Posted at: 2018-12-26T21:17:48.487Z Reads: 134

```
totally random, im in a waiting list of 36 people right now :frowning_face:
```

---
## \#8 Posted by: b264 Posted at: 2018-12-26T21:18:21.917Z Reads: 128

```
What are your motor kv and wheel size and motor/wheel pulley tooth counts?
```

---
## \#9 Posted by: b264 Posted at: 2018-12-26T21:19:03.585Z Reads: 125

```
You can connect to the VESC if it hasn't been powered-off yet and type "faults" on the terminal to see details
```

---
## \#10 Posted by: Sascha_stevenson Posted at: 2018-12-26T21:20:58.550Z Reads: 121

```
though you would show up soon, haha. 
motor KV 190
motor pulley 15 teeth
wheel pulley 60
wheel size 6" or 152mm

Post 2:
i will try that now, just opening up the board
```

---
## \#11 Posted by: Sascha_stevenson Posted at: 2018-12-26T21:31:41.404Z Reads: 109

```
@b264 
no faults
10 chars
```

---
## \#12 Posted by: thisguyhere Posted at: 2018-12-26T21:33:27.168Z Reads: 110

```
[quote="Sascha_stevenson, post:4, topic:79062"]
I will check with Mboards
[/quote]

well...there's your first problem.
```

---
## \#13 Posted by: Sascha_stevenson Posted at: 2018-12-26T21:33:50.823Z Reads: 108

```
@thisguyhere 
indeed
```

---
## \#14 Posted by: thisguyhere Posted at: 2018-12-26T21:36:26.570Z Reads: 107

```
7s is pretty low voltage, can you verify your vesc battery settings.

you could be hitting hard cutoff, that would instantly stop power draw.
```

---
## \#15 Posted by: thisguyhere Posted at: 2018-12-26T21:37:01.360Z Reads: 104

```
link the battery product page.
```

---
## \#16 Posted by: Sascha_stevenson Posted at: 2018-12-26T21:37:46.985Z Reads: 104

```
is there a way to connect to the vesc with the bt module?

https://www.mboards.co/collections/batteries-1/products/7s2p-battery-complete-battery-solution
```

---
## \#17 Posted by: Sascha_stevenson Posted at: 2018-12-26T21:39:50.646Z Reads: 95

```
talking to Mboards is like talking to a wall. they will never reply
```

---
## \#18 Posted by: Sn4pz Posted at: 2018-12-26T21:47:53.239Z Reads: 91

```
because its some dickhead* who just rebrands and resales, no knowledge of the inside of the product



just so you know most of his products come from diyeboard.... and.... well...............yep.

*sort of joking, take it as you see it :man_shrugging:
```

---
## \#19 Posted by: Sascha_stevenson Posted at: 2018-12-26T21:53:56.818Z Reads: 92

```
@Sn4pz 

honestly, when I bought the battery I wish I wasn't so blind to see what really happened behind "MBoards". I bought it with all postage fees paid option when it gets into the UK £60 fees. He just wanted to make extra £££. the cheeky bastard. so I couldn't agree with you more
```

---
## \#20 Posted by: Sn4pz Posted at: 2018-12-26T21:58:13.329Z Reads: 91

```
the best people to purchase things from are those who post on the forums, with only a few exceptions (I cant think of any, but im sure there are some xd ) 

For batteries I reccomend cory: @ hyperIon1

enclosures: @ Eboosted

everything else is generally made in a factory, electronics wise.... 

of course this changes bc youre in europe, unfortunately I dont have any exp. with vendors over there, but (for batteries ) @ pjotr47 seems like a standup *chap* :P 

stay local, it helps cut down on shipping and you can even make connections with them via group rides if thats your thing, better builders = more experience = a better product for you

e: unmentioned everyone as it seemed unnecessary to drag their attention
```

---
## \#21 Posted by: Sascha_stevenson Posted at: 2018-12-26T22:02:53.664Z Reads: 87

```
I will be changing out the battery to something like a 10s4/5p early 2019
```

---
## \#22 Posted by: dareno Posted at: 2018-12-26T22:14:26.060Z Reads: 89

```
[quote="Sascha_stevenson, post:21, topic:79062, full:true"]
I will be changing out the battery to something like a 10s4/5p early 2019
[/quote]

If you're in the uk then @bigben will make you a 10s of pure 30q loveliness.  Those mboard/diye batteries are just not very good at all.
Put it this way.  I have a 10s3p from the same source and the esc it was designed for is rated ffor 18 amps per motor (its a dual)  I upped the amps when I converted to focboxes to 20 amps per motors and the bms blew up.  Didn't cut anything out it just went pop.
They are very low rated for use with the generic chinese esc that is in all those boards so unless you have reprogrammed that focbox completely to allow for this you will have all sorts of problems.
```

---
## \#23 Posted by: Sn4pz Posted at: 2018-12-26T22:16:46.163Z Reads: 88

```
[quote="dareno, post:22, topic:79062"]
I upped the amps when I converted to focboxes to 20 amps per motors and the bms blew up
[/quote]

holy shit Ive never heard of this before. Did you happen to take pictures?
```

---
## \#24 Posted by: Sascha_stevenson Posted at: 2018-12-26T22:20:10.490Z Reads: 84

```
I think you are the one which gets to take home the solution check today my friend! :grin:
so you had an MBoards Battery?
any photos of the BMS :fire:?
i will talk to @bigben, is he in the UK?
```

---
## \#25 Posted by: Sn4pz Posted at: 2018-12-26T22:21:28.597Z Reads: 83

```
yep bigben is in the UK :)
```

---
## \#26 Posted by: thisguyhere Posted at: 2018-12-26T22:23:03.373Z Reads: 86

```
sorry about the bashing, but let's get back on track.

yes you can connect your bt module to the vesc, that's a whole thing you'll need to figure out because it differs based on type, what phone OS you're running, etc.

in terms of battery numbers, here's some conservative values you should be using:

![image|193x123](upload://cOzEYDVfInnwFgcuRoiooJEOHO1.png) 

the product page says "LG cells," which really means nothing.  i'm assuming they're some shit cells that sags a lot, hence the 0.7v sag figure.

basically if the cells sag and hit the hard cutoff voltage, vesc will cutout.  one way to prevent that is to set the soft cutoff pretty high so the vesc can limit current draw before it hits hard cutoff.
```

---
## \#27 Posted by: dareno Posted at: 2018-12-26T22:24:03.464Z Reads: 77

```
I use it now as a test rig for my bench.  Bought it way back when we all fell under the DIYE spell.  Its the exact same unit that mboards sells as his own.  Total bollocks.  Made a whole video about building these things and all the time he was just reselling generic chinese crap.
The point is the tolerances between what the battery can supply and what the bms is rated to are very small so be careful with the battery amps settings.
```

---
## \#28 Posted by: Sascha_stevenson Posted at: 2018-12-26T22:25:17.272Z Reads: 79

```
i am using IOS any good apps for config?
```

---
## \#29 Posted by: dareno Posted at: 2018-12-26T22:27:51.290Z Reads: 79

```
https://www.electric-skateboard.builders/t/vesc-ios-bluetooth-app/53479

This guy has an ios app for bluetooth but I'm not sure how far he got with it or if it was successful.  PM him and check it out.  I don't do bluetooth.
```

---
## \#30 Posted by: thisguyhere Posted at: 2018-12-26T22:27:54.021Z Reads: 74

```
??

i'm not aware of any ios apps where you can change the config.

you'll need to your computer via usb.
```

---
## \#31 Posted by: Sascha_stevenson Posted at: 2018-12-26T22:31:00.386Z Reads: 75

```
what about android?
```

---
## \#32 Posted by: thisguyhere Posted at: 2018-12-26T22:31:50.044Z Reads: 74

```
i dunno, no bluetooth for config, i only use bluetooth for monitoring.

only do config with physical connection via usb.
```

---
## \#33 Posted by: Sascha_stevenson Posted at: 2018-12-26T22:34:48.940Z Reads: 74

```
ok, its a bit of a pain to cut the silicone open up the board update the config and then seal it back up. once I upgrade the battery it is a must to put this on the enclosure. but what has to be done has to be done! :grin:

https://street-wing.com/product/micro-usb-panel-mount-extention/
```

---
## \#34 Posted by: pat.speed Posted at: 2018-12-26T22:47:22.800Z Reads: 74

```
I know the unity can be setup by phone, maybe it’s possible to load that firmware onto a focbox, probably not though
```

---
## \#35 Posted by: dareno Posted at: 2018-12-26T22:47:32.775Z Reads: 72

```
That is a really good idea.  I have 2 ip65 rs versions sticking out of mine.  Very handy indeed.

https://au.rs-online.com/web/p/usb-cables/1116750/

They have a little screw on cap that goes with them which keeps the crap out but are pretty big and not the most attractive of connectors.
```

---
## \#36 Posted by: Sascha_stevenson Posted at: 2018-12-26T22:53:51.765Z Reads: 68

```
@dareno 
is you're entire board ip65? here in london because the roads are crap water always sits in little holes and I really need to get places with my board. Maybe I could learn something from you!
I plan on every port I use to be rated at IP65 and the enclosure too. I think i will even end up making a custom cable to go through the deck into a IP65 pelican case with everything like the power switch, battery meter, etc.
To put it simple, water damage shouldn't even come to my mind :smile:
```

---
## \#37 Posted by: dareno Posted at: 2018-12-26T23:00:40.173Z Reads: 68

```
Alas no I have done my best for stopping ingress but here in the colonies when it rains you hide because otherwise you drown.  Don't ride if it even looks like rain because one minute you're fine next you're floating.  You need @b264 for the kind of protection you need in the uk.  Water ingress protection and waterproofing for when the  water inevitably gets in there.
```

---
## \#38 Posted by: b264 Posted at: 2018-12-26T23:56:58.641Z Reads: 64

```
I just got home from CVS, and it started raining on my way home.

I try to keep water out.  That being said, I always assume water will be in everything and make sure it will still work anyway.

This is usually manifests itself as a *bunch of coats* of "MG Chemicals silicone modified conformal coating" in the 55ml brush-on bottle -- with some "MG Chemicals acrylic conformal coating" in the 55ml brush-on bottle for a *single coat* on any heatsinks

But every thing is unique and if you pretend there is saltwater all over it, what needs to happen to make it still work and not corrode or short out?  Do that LoLz
```

---
## \#39 Posted by: Jc06505n Posted at: 2018-12-27T01:18:54.827Z Reads: 60

```
Metr can 

10 char
```

---
## \#40 Posted by: Andy87 Posted at: 2018-12-27T06:17:30.556Z Reads: 53

```
you can change the vesc/focbox settings with the Xmatic or eSkate VESC app on iOs.
but that´s only for the motor and batter max/min values
ERPM and Watt limit 
in xmatic you can set a max speed too.
the battery cut off and motor detection you would still need t make via your laptop, but usually you set this up only once when you make the first configuration anyhow.
```

---
## \#41 Posted by: Sascha_stevenson Posted at: 2018-12-27T11:17:23.471Z Reads: 41

```
so everyone, 
MBoards has said that the BMS is for discharge too
```

---
## \#42 Posted by: Andy87 Posted at: 2018-12-27T11:18:56.650Z Reads: 41

```
Did they say how much this bms can handle?
I could imagine that the bms is reason of your cut outs.
```

---
## \#43 Posted by: Sascha_stevenson Posted at: 2018-12-27T11:20:45.579Z Reads: 41

```
nope they haven't said how much it can handle. I do get a huge amount of sag tho when riding it goes from 100% charge to 47%
```

---
## \#44 Posted by: Andy87 Posted at: 2018-12-27T11:27:04.245Z Reads: 39

```
Thats very likely with a 7s2p battery.
I can’t say it 100% but I would guess it’s the bms.
If you have so much sag it means that you pull a good amount of amps, the same while breaking.
If you break hard enough the bms tries to protect your battery from getting hit by too much amps and just cut out.
Without battery you than also can’t break anymore.
```

---
## \#45 Posted by: Sascha_stevenson Posted at: 2018-12-27T11:29:10.884Z Reads: 39

```
I've had a chat to Ben and I think we will sort out something Soon.
```

---
## \#46 Posted by: Andy87 Posted at: 2018-12-27T11:30:57.165Z Reads: 42

```
That’s good to hear!
No breaks, no good ☝️😅
Especially if you drive on the road with cars and other people.
```

---
## \#47 Posted by: hyperIon1 Posted at: 2018-12-27T21:41:40.240Z Reads: 27

```
If you are discharging through the bms and it’s chocked at a certain amp like 30a or 50a you will experience this every time. 
The bms try’s to do its job in both situations. 
When you draw from the battery and when you regenerate during braking. 
A bypass to direct discharge will solve this problem. 
In doing so you eliminate the chock in both directions. 
Your esc can now regulate input ( power in ) taking the place of discharge ( bms )
While still having charge and balance function on bms. 
This opens your pack ( battery ) to full potential
```

---
