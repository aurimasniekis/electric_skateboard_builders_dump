# First Build - Trampa HolyPro - Etoxx direct drive - 12s7p - Dual Vesc 6

### Replies: 21 Views: 2265

## \#1 Posted by: danggilmore Posted at: 2017-12-06T04:47:53.370Z Reads: 347

```
Hi all,

First build and its game time.

I've ordered many parts and they're all on the way! Can't wait to start building!

Trampa deck - Holypro
Veritigo Trucks
Superstar Hubs
Dual Vesc 6
APS Motors 6384S - 170kv - 4000w
E-toxx Direct Drive
12S7P battery by Chiboards
Benchwheel remote from Miami electric boards

What else do I need?

I need a vesc enclosure. Any recommendations?

I need a canbus to connect my vescs. Any recommendations?

I need heat shrinks and wraps and figure out the wiring. I've been searching and reading and have somewhat understanding but am a little intimidated.

I'll upload pics as I build!

Open to any and all suggestions. Thanks to all!
```

---
## \#2 Posted by: BigBoyToys Posted at: 2017-12-06T07:57:25.803Z Reads: 307

```
I think your remote is less than ideal for such a torquey build but give it a try maybe it will be ok bu your standards. Try the GT2B in mastercho mod if you decide youd like to spread the power delivery over longer trigger distance.

3/4" Braided wire loom for your  battery to vesc wires

XT90S connector to dual XT90 connector harness to split power from your battery to both vescs (or an antispark switch from @goldenHusky ).

Ive been using the CF dual vesc6 mount from Trampa with no enclousure but @Nowind has a nice box he'll be releasing for sale soon I believe.

Sensor wire adaptors. JST ZH to PH
```

---
## \#3 Posted by: E1Allen Posted at: 2017-12-06T08:02:36.356Z Reads: 277

```
Any reason for that specific battery pack? Have any experience with electronics or consider lipo?  $850😢
```

---
## \#4 Posted by: danggilmore Posted at: 2017-12-06T15:14:07.919Z Reads: 266

```
@BigBoyToys

Thanks for your input!

I didn't go with a gt2b because of how big it is. I hope i like the benchwheel or I'll switch over to the gt2b. Surprised how minimal quality options for remotes there are.

@goldenHusky So if I buy that antispark switch, I won't have to make my own wiring sequence? Just vescs to antispark and antispark to battery? Whats the difference between 6way, 3 way and dual? is that the amount of inputs? so a dual will work?

Thanks for details on braided wire loom and sensor wire adaptors

@E1Allen
I've already spent hella money and I figured if I was going to spend 200-300 on lipos and charging equipment, I might as well drop the extra 500 and have a quality battery I can just plug in and only stress a little bit about stuff blowing up. 

I've got decent amount of electronic experience and am an avid DIYer my whole life but never messed with 18650's before. I figure after recieving my battery pack, I'll be able to asses baja's build and be able to gain some knowledge for myself to assemble cheaper packs in the future. and i hate spotwelders. :D
```

---
## \#5 Posted by: BigBoyToys Posted at: 2017-12-06T17:23:00.839Z Reads: 236

```
You would still l need to split the power coming off the the AS switch to connect to each VESC so some sort of Y adaptor is required. You can just solder one up. The difference between the AS switch models are how much current they are rated for. I have the 6 fet model and its working well on a build of mine thats 4wd that pulls over 100A.
```

---
## \#6 Posted by: Cobber Posted at: 2017-12-06T20:05:21.832Z Reads: 225

```
[quote="BigBoyToys, post:5, topic:40261"]
I have the 6 fet model and its working well on a build of mine thats 4wd that pulls over 100A.
[/quote]

so you are just using one BBT?
```

---
## \#7 Posted by: BigBoyToys Posted at: 2017-12-06T20:27:11.703Z Reads: 216

```
I am  using one 6 fet switch on the carvon V3 4wd atm. I only used one 2 fet version on the Carvon V2 top speed board as well but I blew 3 of them up, pretty much anytime I pushed more than 4000 watts threw them for more than a few seconds.
```

---
## \#8 Posted by: Cobber Posted at: 2017-12-06T20:34:01.582Z Reads: 217

```
@BigBoyToys are you running a 6awg backbone on your carvon v3 4wd, do you you think 6awg will fit on the solder pads?

sorry for the highjack danggily ;)
looks like a cool build bro
```

---
## \#9 Posted by: BigBoyToys Posted at: 2017-12-07T00:54:57.456Z Reads: 216

```
Naw, no 6awg required as each motor is only supplied with 30A max since the pack has only a 120A ccr
```

---
## \#10 Posted by: danggilmore Posted at: 2017-12-15T21:32:24.271Z Reads: 215

```
<img src="/uploads/db1493/original/3X/e/9/e95907f04fcf41a0231a1116d00a21eec93e4e7b.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/c/e/ce54bb8c2355daaa2a48e289dc051ccf4d0dbf03.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/6/b/6ba10110eb42d1c40d1193be82822c3bf553d847.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/2/2/22f546da87017db1512fe530fa8360ec9b755a2c.JPG" width="666" height="500">

it has begun! 
 
still can't decide on a vesc enclosure.
```

---
## \#11 Posted by: Cobber Posted at: 2017-12-16T01:20:00.706Z Reads: 187

```
get one from @Nowind with your direct drive?
```

---
## \#12 Posted by: danggilmore Posted at: 2018-01-23T22:20:38.309Z Reads: 167

```
![53838081695__AF20F7F2-71AD-4F93-A032-0BB008EF837D|375x500](upload://7XXzadvophnK1C06AxcD7urYVQd.JPG)
```

---
## \#13 Posted by: FredrikHems Posted at: 2018-01-23T22:23:02.752Z Reads: 159

```
Got any updates? :slight_smile:
```

---
## \#14 Posted by: danggilmore Posted at: 2018-01-23T22:24:15.479Z Reads: 164

```
everythings done except for exposed wires from electronics box to wires. goes HELLLLA fast. pops wheelies and errrrrything! :D

check out pic i just posted couple minutes ago.
```

---
## \#15 Posted by: FredrikHems Posted at: 2018-01-23T22:25:14.088Z Reads: 153

```
Share som pics and even better vids, then!!
```

---
## \#16 Posted by: danggilmore Posted at: 2018-01-23T22:27:46.483Z Reads: 160

```
i just finished last night. i'll get some way better pics and vids up soon! ;]
```

---
## \#17 Posted by: danggilmore Posted at: 2018-02-01T02:03:42.409Z Reads: 157

```
![IMG_0082|666x500](upload://7IEgT7xjXsH6FdE3iSppYFrWdnX.JPG)![IMG_0083|666x500](upload://yjs2FqjemAdeZwsdDDsNz2l6T2c.JPG)![IMG_0084|666x500](upload://nBxn82w7OMZva6HCOJWln0e05LM.JPG)![IMG_0086|666x500](upload://kRTL3yoeGBXTPR7kwQAeiWKcdBc.JPG)![IMG_0085|666x500](upload://9KY3WOyrzcyZZNWqdWHBZvCsUl8.JPG)![IMG_0087|666x500](upload://xDz9lejjk4DtnF7uPrTTyRejA4c.JPG)![IMG_0088|666x500](upload://yUtUZlgmEqMDqL11yonFrfOSBMU.JPG)

love it so far. feels so good finishing a build and jumping on it and starting to shred. 

range roughly 18-20 miles. i can get it up to 30 and then get too scared to go faster. :smiley: 

i'm aware the charging port probably shouldn't be where it is but i'm too lazy to put it in my electronics box. the box i used is pretty flimsy so i'll probably replace in it in due time. 

apppreciate anyone's input! good luck to everyone with their builds!
```

---
## \#18 Posted by: benjammin Posted at: 2018-02-01T03:00:04.437Z Reads: 143

```
Nice build 👍
```

---
## \#19 Posted by: sydeskater Posted at: 2018-04-28T14:38:23.923Z Reads: 120

```
Very nice build.  How has it been running?  Also if you don't mind sharing, what was the rough cost of the build?  Thank you in advance.
```

---
## \#20 Posted by: danggilmore Posted at: 2018-10-23T22:15:14.349Z Reads: 79

```
been running great! and cost was prolly in between 2-3k. i dont like to keep track cuz it makes me sad.
```

---
## \#21 Posted by: danggilmore Posted at: 2018-12-04T20:11:06.351Z Reads: 59

```
@Sn4pz

You can see it here. I ran Velcro to keep my battery stable and drilled holes in my electronic box and only use the standard truck hardware to keep it set. I've since added some foam to protect the electronics
```

---
