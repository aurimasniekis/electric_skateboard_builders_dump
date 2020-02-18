# Custom Evolve Carbon GT(10S5p 30Q)(Dual FocBox)(Bluetooth BMS)

### Replies: 180 Views: 14218

## \#1 Posted by: Fiori Posted at: 2017-09-27T02:02:57.880Z Reads: 866

```
Hey everyone. This will be my first "build log" here. I figured this would probably be the best place to introduce myself. My name is Dylan, I'm 25 years old and currently reside in Northern California. I'm a Mercedes Benz mechanic by trade(going on 6 years now). I'm certified to work on multiple Hyrbid/full electric models that we sell(pretty recently, MB is just dipping their toe in the electrical game at this point).I am by no means an electrical engineer, but I like to think that my experience gives me a small leg up in this hobby I have taken on.    Iv'e been lurking around here for the better part of the last year posting in other sections, and just soaking up info. Anyway, enough about me and onto the battery build. 

I have estimated that I have over 6,000 miles on this CGT battery, and at almost 400 charge cycles this battery has seen its better days. It was a junker battery to begin with, and the range was diminishing with every ride. I decided it was time to build a new pack, and I wanted more range than before for sure. I really want to keep the remote/esc setup because I don't wanna just throw it away and have to buy two vescs(I'll save that for my custom build). To do this, all I have to do is keep the evolve bms and wire it up to my new pack.

When all is said and done I should have a 10s5p 15AH pack :smiley: 

I started by ordering 60 of these Samsung 30Q batteries(50 for the build, and 10 extra for when I inevitably mess something up):

<img src="/uploads/db1493/original/3X/a/f/afecba49e65a2bddcface5ae13c961d3d3ede2f4.jpg" width="374" height="500">

And then I ordered the Sunkko 709a(fyi i wish i bought the arduino kit instead, but this did the job fine):
https://joyfay.s3.amazonaws.com/media/catalog/product/cache/1/image/1000x1240/e9c3970ab036de70892d86c6d221abfe/j/f/jfhsw05-2.jpg

Next I opened up the evolve and took out the old junker battery:
<img src="/uploads/db1493/original/3X/0/5/059df5fcd1a3a64eb9307f220761e79c1a019ae6.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/f/3/f3be5781f4b081486dacf5b873ce6d6863328e31.jpg" width="666" height="500">

Then It was time to inspect this bad boy(evolve bms), and trace down each and every BMS wire. It actually wasn't too hard at all. 
<img src="/uploads/db1493/original/3X/8/0/808af3c4d4a4baa21b28585ef74b4dd3325e80ca.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/e/c/ecf3b5e2ab4fea94678b263807014a1bbf306a39.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/0/b/0bcd17cfe48fb8c7ed742ac2f5085f4864a90934.jpg" width="374" height="500">

The balance lead closest to the RED wire(the blue one closest to the red wire on the balanace lead connector) is 1S, then just go down the line from there all the way up to 9s. 
<img src="/uploads/db1493/original/3X/d/c/dc429fc2e21056d64a4f48568e73e492a424698e.jpg" width="374" height="500">.

Test fitting the cells:
<img src="/uploads/db1493/original/3X/0/c/0c212bc6c9c384ebf2d94cc1ff690520206afa0e.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/9/1/9184cf8a9782724c521b728756abdcf8b4311842.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/c/4/c4f67c12b4a57047d7f677b359b29eaeec0babac.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/5/b/5bb2009bcf01e2735fa558e5a014f8993fe869c0.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/4/0/40b3a18e909768dd4b2bba64489dc283bbd9be0d.jpg" width="374" height="500">

At this point, I found out that 50 cells and the evolve bms just wont fit very well in this compartment. I didn't want to smash it all in there and risk damage. So I made the decision to relocate the Evolve BMS to the top of the rear truck area. I figured I never use that area on the drop through deck anyway. I even though about putting in an extra 10 cells there too... but I just feel like it will be too bulky. That led me to create this BMS case with my 3d printer. I still might make some revisions to this bms case, when I'm all done I'll upload the files.  Printr: printrbot simple metal with DIY heat bed installed. More on this later....
<img src="/uploads/db1493/original/3X/8/1/817aa79be709574890f07b2eceebb89ec622cb5b.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/1/4/143c56526bcb899aff06b0a3a7a060f5cc149c7c.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/9/f/9f798443e5caf3a3f9a6ba6f0871c1cfabf34a4f.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/5/0/507648e890e0bda3fe75270a93dec837be7bd89a.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/7/5/757bdc9ba8d586c7a8fea58c5d113ae310b6e719.jpg" width="666" height="500">

Time to start spot welding some cells! I made 10 packs of 5 parallel cells.  My plan is to essentially make two 18v packs and connect them in series. 

<img src="/uploads/db1493/original/3X/1/b/1bbd7187e172f88c219673c8aeb1ed19d0083350.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/4/1/41f4599dc39d866b59199d6aa21df195e4b6d949.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/7/9/796a3a0ad94d28ee0baa21a750455196a8dae831.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/f/0/f000ec16ec266efd3d14186425a4af6b183ae049.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/4/f/4f6dcb50131952f011e0090be129ff2be112db13.jpg" width="666" height="500">

After spot welding it all together I decided I would carefully try to see if it would all fit into the compartment. This is where I ran into some issues. The first thing I want to talk about: BEWARE, THE DECK HAS CONTINUITY! I set down half the pack in there and smelled something burning. My pack was shorting...... I quickly got it out of the deck, and only a small burn mark remains inside of the enclosure area, no serious damage. 

At first, I thought that some of the nickel strip had shorted out something out on the positive end of some of the cells. I had some issues early on with some of the strips bending due to mis alignment and then shorting(which is why I will ALWAYS recommend using those cardboard protector ring caps[ill post a link]). 

[![](https://youtu.be/4evbTQgTtX0)](https://youtu.be/4evbTQgTtX0)Long story short after some investigating I had a thought: "they make motor brushes out of carbon..... maybe the deck combined with my non insulated pack caused it to short". Grabbed my multi meter, and sure enough there is continuity in multiple places(not everywhere). So... anyway, for anyone doing this beware of that. I instantly thought of the board that lit on fire on the evolve forums. tldr: be carful. 

Luckily, the extent of the damage was only about 3-4 cells due to the nickel strip acting like a fuse. I used my 10 extra cells to swap out any that were even near the short.  Here's the damage(looks worse than it really was):

<img src="/uploads/db1493/original/3X/2/1/216709a6b4441ba4a2fc0defd83d10f8682569f0.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/1/2/125dfef9b74f925c9120775aabc0bcf72bb44a2b.jpg" width="374" height="500">

After that turn of events , I got everything cleaned up and carried on. I double insulated EVERYTHING. I soldered in all my balance leads, and labeled them accordingly, connected the two in series at the back end. Then, It was time for a test run!:
https://youtu.be/4evbTQgTtX0

ALL GOOD :) Then it was shrink wrap time(back ones are exposed because I had to make the series connection). 
<img src="/uploads/db1493/original/3X/2/d/2d1e0f890c376e8895854c54a75a6a75536f8b2a.jpg" width="666" height="500">

Then I added some duct tape for support. 
<img src="/uploads/db1493/original/3X/f/e/fe87c200551bb8f3c1670c5e380f0a3f95f5cbaa.jpg" width="666" height="500">



AAAANDDDDDD  after all the shrink wrap and tape: NO FIT :( . I'll have to relocate the balacing wires to the middle and hopefully that's all the clearance I need. It's super close, but I dont want to force it. 

that's pretty much as far as i've gotten thus far. I except to finish some time in the next few days or so. I still have to:

Extend the battery switch, and UART cables to reach my new BMS location and clean up some of the wiring and such. If you've made it this far THANKS FOR READING. I'll update this post as often as I can.
```

---
## \#2 Posted by: caustin Posted at: 2017-09-27T02:09:41.052Z Reads: 661

```
Awesome, I am probably 75% down the CGT battery degrade scale from you so interested to see how this goes!
```

---
## \#3 Posted by: Fiori Posted at: 2017-09-27T02:13:31.256Z Reads: 655

```
Thanks man! Check back here in about 30 minutes I'll have a lot more pics up
```

---
## \#4 Posted by: Fiori Posted at: 2017-09-27T02:57:41.304Z Reads: 641

```
As of now I finally got all the pics uploaded! Woop woop! I'll keep everyone updated as i go along here.
```

---
## \#5 Posted by: Okami Posted at: 2017-09-27T08:21:49.748Z Reads: 616

```
U should get some insane range with this pack. Nice work, clever way of relocating bms, i think some other people just extended enclosure but that requires work with plastic
```

---
## \#6 Posted by: Fiori Posted at: 2017-09-29T07:15:21.569Z Reads: 623

```
Took off the blue shrink wrap and all the tape. Cleaned everything up. rerouted the bms leads to the top. And got everything wrapped in clear shrink wrap(satisfying :D)  and it FINALLY FITS! WOOO. Man it's tight in there.... 

Also 3d printed these spacers to go in between the deck and the battery on the sides, and in between both packs. Printed them in 1mm first, and had to go down to 0.50 and even 0.35mm in some places to make them fit. The extra insulation makes me feel a lot better though. 

<img src="/uploads/db1493/original/3X/d/8/d8ea6742b7f064f241bfa77df2b5cf06caa1d77f.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/0/d/0d7bffb5131a38b95f919da00a6012264e2f2873.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/6/7/67a67e7fb7063a78f60584eb164f0cae6bc2285f.jpg" width="666" height="500">
```

---
## \#7 Posted by: Jebe Posted at: 2017-09-29T09:47:42.878Z Reads: 574

```
nice job. killer range now. does the lid fit smoothly ?
```

---
## \#8 Posted by: Fiori Posted at: 2017-10-01T11:40:04.099Z Reads: 580

```
Took it for a test ride just now! Finished at 3am tonight and couldn't resist going out. 

I put on the 200kv racerstar motors. WOW. It's like a whole new board. The range is insane. Voltage sag is almost non existent. I am running the "AT" wheels and still getting awesome range. I am hitting 28 mph with the AT setup. Rode 10 miles and was still at 38V after the ride. 

I have to say, fitting everything in the deck was a HUGE task. Even after moving the BMS its a tight fit. 

Will report back tomorrow with extended ride info, and some more pictures.
```

---
## \#9 Posted by: Fiori Posted at: 2017-10-01T11:41:09.090Z Reads: 564

```
It's super tight but its fits without crushing anything! I only have 1 test ride to compare with, but the range is GREATLY improved.
```

---
## \#10 Posted by: tex Posted at: 2017-10-01T19:47:45.515Z Reads: 559

```
cool work man

with this new battery pack, the total weight of the skate is changed?
```

---
## \#11 Posted by: Fiori Posted at: 2017-10-01T19:50:38.537Z Reads: 547

```
Thanks brotha. 

Yea. I haven't weighed the whole deck yet. But I would say it feels about a pound or two heavier. Not much.
```

---
## \#12 Posted by: Fiori Posted at: 2017-10-02T00:49:03.638Z Reads: 579

```
about 35 miles on the new battery and it feels GREAT!

<img src="/uploads/db1493/original/3X/c/b/cbdb7289332f6ab612b9e8b5acd7df01d2f2ef68.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/2/c/2c32145a79a7ce44591ced27efe46d58947580a3.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/4/4/44614a32045a4af6d852dd4bdf6d89ad0e1a196f.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/9/8/988b0767eb84ba8ad5e25fed9f388339964ab7df.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/5/8/580fc50ff4af2f5fe634f1a55f567f8e9195d828.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/6/d/6df16048ace18896e13814a1a326250966f6807d.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/c/f/cf2efb75ff86df7c5c7a42c6247c864eb33a86e2.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/0/b/0bbac03370c2253f5b1433ed714e8d111a31eaf5.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/a/c/ac7f991b044236df380cd3f91cc2aa2b17eca7e6.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/8/7/87f5e00df13b32b57807a0edf750690d2b093350.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/d/f/df68b8ed7563ea320663cfeb559356b923f381ba.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/a/0/a02bf6152ee867a4575d10d23c812513c08b07a7.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/a/5/a56dddbb50df20ecdad069112c8d7d17e5fd3d5b.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/9/5/952ce0d95266c08849c957c17af9872d8b40988c.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/b/8/b80fd36b87589aeee3a2346e7632c844802cc4c2.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/7/0/70607080a0b27690c75921fa171f467fa0073380.jpg" width="374" height="500"></uploads/db1493/original/3X/4/1/4136844d64092a25f1004370668228ee682268d4.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/4/1/4136844d64092a25f1004370668228ee682268d4.jpg" width="374" height="500">
```

---
## \#13 Posted by: MysticalDork Posted at: 2017-10-02T01:20:37.228Z Reads: 516

```
Where in NorCal are you? I live in Quincy.
```

---
## \#14 Posted by: Fiori Posted at: 2017-10-02T02:43:01.242Z Reads: 518

```
About 60 miles north of San Francisco. Sonoma County, Quincy is a tiny little town! A friend of mine went to school down there. He said there's 1 stop light there haha.
```

---
## \#15 Posted by: Fiori Posted at: 2017-10-02T03:55:27.301Z Reads: 521

```
Wires wrapped. <img src="/uploads/db1493/original/3X/0/a/0af7281eb4eccf6a5408a4474e172b5d0cac45e7.jpg" width="666" height="500">
```

---
## \#16 Posted by: MysticalDork Posted at: 2017-10-02T04:30:38.080Z Reads: 497

```
We've grown! there are two stop lights now lol :P
```

---
## \#17 Posted by: Okami Posted at: 2017-10-02T05:21:15.449Z Reads: 494

```
35miles with AT wheels sounds incredible :heart_eyes:
```

---
## \#18 Posted by: Fiori Posted at: 2017-10-02T05:22:24.906Z Reads: 501

```
Not in 1 ride lol. I am getting about 20 miles per ride so far. I hammer the throttle MOST of the time :p. But I am getting up to 29-30 MPH(according to the evolve remote) with the new 200kv motors :D
```

---
## \#19 Posted by: Fiori Posted at: 2017-10-02T16:37:44.425Z Reads: 500

```
Battery today after my ride in to work :slight_smile: 

https://i.imgur.com/7jwTAVh.jpg
```

---
## \#20 Posted by: b264 Posted at: 2017-10-02T17:27:35.091Z Reads: 493

```
Putting the power switch on top of the back trucks could help somewhat mitigate the evolve remote disconnection issues.  If it disconnected, you could step on the switch twice to get it to reconnect ... instead of having to reach under the board which basically you have to already be stopped to do
```

---
## \#21 Posted by: BigBoyToys Posted at: 2017-10-04T23:10:26.589Z Reads: 463

```
Cant you just put the board in pairing mode by holding down the buttokm for a few seconds?
```

---
## \#22 Posted by: b264 Posted at: 2017-10-05T00:31:29.726Z Reads: 461

```
Yeah, but the board won't accept a pair request until it power cycles.  I have since learned I think my power switch may actually have an issue where it disconnects sometimes on bumps
```

---
## \#23 Posted by: Fiori Posted at: 2017-10-05T02:53:17.899Z Reads: 462

```
Is your switch actually physically pushed in still when the board dies and you need to cycle it? You may have a different issue separate from the switch.
```

---
## \#24 Posted by: b264 Posted at: 2017-10-05T03:05:15.839Z Reads: 448

```
Yes
10 char
```

---
## \#25 Posted by: Fiori Posted at: 2017-10-05T03:09:10.178Z Reads: 456

```
I would check all the cells on the hidden menu of your remote and make sure they are all draining equally. Hit up evolve if you are having trouble finding the switch and just order from them. 

I feel like something else is shutting your board down. I have only had the board shutdown with the switch in like that when I crashed and hit something really hard

EDIT: Open up the deck lid and ensure that all you're connections are good and not being smashed. When my deck cracked initially, I found evolve had pinched my motor wires(ESC side) in between the heat sync and the deck....
```

---
## \#26 Posted by: Fiori Posted at: 2017-10-08T23:00:59.306Z Reads: 460

```
Longest ride yet. Mostly on GT mode. Riding on the 7 inch evolve AT wheels/tires. Quite a few steep climbs. The last few miles were on eco. I could have squeezed out that extra .9 miles but didn't wanna walk back :stuck_out_tongue:<img src="/uploads/db1493/original/3X/b/a/ba05197824c67bc4ffa43f0e070982b1410738e1.jpg" width="281" height="500">

Sadly I have to wait for it to charge before I can go back out :(
```

---
## \#27 Posted by: b264 Posted at: 2017-10-09T04:57:31.296Z Reads: 424

```
[quote="Fiori, post:26, topic:34045"]
Sadly I have to wait for it to charge before I can go back out
[/quote]

Yeah, that's exactly why more boards is moar better.
```

---
## \#28 Posted by: BigBoyToys Posted at: 2017-10-16T20:47:42.192Z Reads: 406

```
Ive solved a few of my evolve problems by disconnecting things and reconnecting them, lol. I had a "batt drain" error  that mept coming back randomly. Unplugged the bms and a few other connectors thrn reassembled and itnhasnt been back since. Basic, but mayne worth a try?
```

---
## \#29 Posted by: b264 Posted at: 2017-10-16T21:04:56.711Z Reads: 416

```
@BigBoyToys Actually, this is going to sound funny, but all of my Evolve disconnection problems have completely gone away by FIRMLY and in one continuous motion pressing the power button to turn it on.  Yeah, you read that right.  When you turn it on, press the power switch firmly and in one fluid motion.  It seems it was rattling and momentarily disconnecting whilst riding I guess...  Maybe something inside wasn't seating correctly?  I don't know

I mean the disconnection problems that cause you to lose brakes/throttle until a power-cycle, not when the displayed battery level goes away shortly.  That seems harmless as the throttle and brake still work
```

---
## \#30 Posted by: Fiori Posted at: 2017-10-17T03:36:49.678Z Reads: 409

```
I have had that same battery error issue, and fixed it the same way LOL. Once it was due to the remote randomly switching to V1 speed controller mode in the settings.
```

---
## \#31 Posted by: Fiori Posted at: 2017-10-17T03:38:30.060Z Reads: 435

```
Got the 107mm's on today :heart_eyes: . They look and ride amazing. Still not as smooth as pneumatics, but still a great inbetweener. They roll for days. They are HUGE. Look at them next to the AT wheels.

ps: yes I use my automotive lift to work on my esk8 :stuck_out_tongue: 

<img src="/uploads/db1493/original/3X/0/5/052b1f9f3fc4a6e99988586ce08e7610b3723cfb.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/5/b/5b49f6713ac4df48f9b45db473c760915017fcb8.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/5/2/52e18ebdca4ebf4c4afd29e9f8c827e8e7c51b0b.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/6/a/6aaf0117b48cc4cccc926dfb4c114560e8a8913b.jpg" width="374" height="500">
```

---
## \#32 Posted by: anorak234 Posted at: 2017-10-17T03:58:09.974Z Reads: 391

```
How are you doing with the fires? I live east of SF - the smoke is still pretty bad down here
```

---
## \#33 Posted by: Fiori Posted at: 2017-10-17T04:05:07.261Z Reads: 403

```
Dude I literally almost had my house burned down this last week. It's been really rough. Fire was less than a mile from my home. My parents entire neighborhood is burned down, except their house and two others. They were really lucky their house made it. 

My neighborhood was luckily not hit, but it was really close to me. They evacuated everywhere around me, and I had to stay up all night Monday-Thursday fending off looters/waiting to hear if the fire was blowing/heading towards me. Water here has been unsafe to drink until today(finally cleared) and I just finally got my power back this last Saturday, and my gas got turned back on today. 

It's been a wild ride man BUT, I am safe, and so is everyone in my family. My house, and my parents house remain unburned and that is all I can really ask for in a situation like this.  Thanks for asking, and I hope you've been safe during this whole crazy situation too.
```

---
## \#34 Posted by: sketchy Posted at: 2017-10-17T04:20:55.739Z Reads: 393

```
[quote="Fiori, post:33, topic:34045"]
I had to stay up all night Monday-Thursday fending off looters
[/quote]

That's really depressing :frowning: Glad to hear you made it out well.
```

---
## \#35 Posted by: Fiori Posted at: 2017-10-17T04:26:29.936Z Reads: 390

```
Thank you

People are definitely shitty. Luckily we are well armed here in my house, but we didn't have too many run ins. Only chased off a few people/cars.  A few cars and people on foot rolled through(past midnight) and I could just tell they were scouting for evacuated houses.. disgusting...

But for every shitty person during this catastrophe there's been 100 good people to offset it. The amount of help and assistance offered from people here,from people all over the country, people from everywhere,  has been awesome to see.
```

---
## \#36 Posted by: Kit Posted at: 2018-01-28T22:23:17.223Z Reads: 362

```
Nice build, looks great! I am going to try to follow this for my own Carbon GT - I gotta have that range with the AT tires. Do you think the build would be easier if I just made it a 10s4p battery build in order to not have to relocate the evolve bsm? Maybe that'd create enough space for it?
```

---
## \#37 Posted by: Fiori Posted at: 2018-01-28T22:35:58.227Z Reads: 348

```
Yea going 10s4p will be half the work(at the expense of 20% less range). 10s4p should fit with room to spare
```

---
## \#38 Posted by: Kit Posted at: 2018-01-28T22:53:13.993Z Reads: 344

```
_Awesome_ - I'll even attempt that motor upgrade. If I go the 10S4p route though do you think the 200kv motors would need a cooling upgrade for the bsm, if I don't relocate it?
```

---
## \#39 Posted by: Fiori Posted at: 2018-01-28T22:58:20.156Z Reads: 345

```
No the bms doesn't get hot at all. The esc gets hotter than before(because the old crappy battery couldn't maintain the amperage the the 30q's can). But it hasn't been a problem for me yet.The exposed heat sync does a pretty good job imo.
```

---
## \#40 Posted by: Eboosted Posted at: 2018-01-28T23:47:06.802Z Reads: 350

```
I had my Bamboo GT through the same process, I went with a 10s4p with Samsung 25r, I thought I was going to get far more acceleration and power but at the end it was exactly the same as a brand new bamboo GT. 

The restriction wasn't on the battery but in the ESCs
```

---
## \#41 Posted by: Kit Posted at: 2018-02-01T02:57:32.083Z Reads: 320

```
Alright, I've pulled the trigger - got myself 50 batteries. I just realized I need to spot weld on some nickel plates too - would you mind telling me what size you used?
```

---
## \#42 Posted by: Fiori Posted at: 2018-02-01T03:07:20.255Z Reads: 321

```
I used 0.15 for this battery, and I doubled it up.
```

---
## \#43 Posted by: Kit Posted at: 2018-02-01T04:07:44.080Z Reads: 334

```
So about 100 [of these](https://smile.amazon.com/gp/product/B004DDH9IG/ref=oh_aui_detailpage_o04_s00?ie=UTF8&psc=1) should do, right? Is it really necessary to double up though? I'd imagine that a single strip would have sufficient current capacity. 

Also, did you run out of Kapton tape? Why the blue painters tape?
```

---
## \#44 Posted by: Aleks Posted at: 2018-02-01T04:13:31.770Z Reads: 338

```
those are 6mmx0.15 -- those are tiny. I think generally reccomended is 10-12mm wide x0.15.  your pack in parallel will put out almost 100 amps, no way these can handle it.
```

---
## \#45 Posted by: Fiori Posted at: 2018-02-01T06:19:24.292Z Reads: 337

```
Those are garbage don't buy them. They are fake, and made of steel. 

Evolve BMS will only pull 65 amps, however I still think you should double up. 

These are better:

https://ru.nkon.nl/accessories/welding-material/nikkel-battijersoldeerstrip-10mm.html
```

---
## \#47 Posted by: Kit Posted at: 2018-02-02T17:15:30.482Z Reads: 326

```
Ok, so something like [this](https://www.ebay.ca/itm/10mm-X0-15mm-99-7-Pure-Nickel-strip-1m-for-26650-18650-21700-battery-spot-weld/271794492996?hash=item3f4836d644:g:gRsAAOSwjL5ZDsIo) would be far better to get then? One meter of  a 0.15T*10W mm Pure Nickel Strip.
```

---
## \#48 Posted by: Fiori Posted at: 2018-02-02T19:06:54.019Z Reads: 333

```
That seems fine, however there is no way to know you if you will get pure nickel or not from that seller until it arrives and you can rust test it.
```

---
## \#49 Posted by: Fiori Posted at: 2018-02-03T02:35:24.148Z Reads: 362

```
Well everyone, I'm sad to report that I was hit by a car today on my CGT. He ran a red light trying to turn right (cali stop):/ I'm ok and am not hurt luckily  (as far as I can tell). I was able to dive off my board and onto the sidewalk. I believe if I didn't I would be seriously injured or killed. Luckily I was wearing my helmet

My CGT on the other hand was not so lucky. He completely ran over it. I will do an updated assessment on the damage after legal actions are worked out. ![20180202_180723|374x500](upload://jk1B1XzcRd4f2yAlayLL4gGvaeG.jpg)![20180202_180723|374x500](upload://jk1B1XzcRd4f2yAlayLL4gGvaeG.jpg)![20180202_183557|666x500](upload://2ZKv8CBUybOz40teKKyWZMz2gCX.jpg)![20180202_183606|666x500](upload://8ih2us5vcTifU31xf3AxnFufTry.jpg)![20180202_183603|666x500](upload://zWkCM9LYFVDjMeHwivY4JVwoHFV.jpg)
```

---
## \#50 Posted by: mmaner Posted at: 2018-02-03T03:39:39.506Z Reads: 324

```
That sucks dude, glad your unhurt though.
```

---
## \#51 Posted by: Kit Posted at: 2018-02-03T03:48:24.705Z Reads: 323

```
Nooooo, the CGT!! Good thing you didnt get hit :+1:

Any chance you got insurance info from the driver?
```

---
## \#52 Posted by: Fiori Posted at: 2018-02-03T04:28:49.019Z Reads: 320

```
Thank You. It really makes you think about what's important that's for sure.
```

---
## \#53 Posted by: Fiori Posted at: 2018-02-03T04:30:16.929Z Reads: 324

```
Yes I got all his info and a photo of his license. I had the police come and file a report as well. I was lucky that he did not try to run away. I actually had to dislodge my board from under his car.
```

---
## \#54 Posted by: mccloed Posted at: 2018-02-03T18:48:16.015Z Reads: 316

```
Glad to see you were unhurt. Too bad about your board.
```

---
## \#55 Posted by: ninja Posted at: 2018-02-03T19:06:02.956Z Reads: 319

```
Hi!
Looks like your wheels are attached wrong way, the tire pattern is like you should ride backwards! :wink:  But maybe its just me..:laughing: too much beer.:rofl:
```

---
## \#56 Posted by: Kit Posted at: 2018-03-02T15:28:16.700Z Reads: 311

```
Hey Fiori, my spot welder arduino arrived finally - I'm going to get my own project going soon, hopefully I will have a thread like yours here. I was wondering - would kapton tape be sufficient to insulate the battery? I was thinking of also using some foam as insulation in-between the board and the battery since I can not print spacers. 

Also, it looks like you welded each cell of 5 batteries together with a single strip of Pure Ni., and then connected 2 sets of one positive cell and one negative cell with a second Pure Ni. strip, while leaving a final positive (?) cell for the series BMS connection unless I am mistaken.
```

---
## \#57 Posted by: Fiori Posted at: 2018-03-02T15:35:54.624Z Reads: 311

```
Awesome, it's a nice little machine. 

I think the kapton tape is fine, most people here are using it. I just think that you should have something extra and thicker underneath or on top of it to insulate the terminals better(fish paper, or even blue tape if you can't find the fish paper). The kapton is really thin. Then just get some of the really wide heat shrink to finish it off. 

I think the 3d printed spacers are a must, if you can't print those you can just use cardboard, playing cards, or even old credit cards if you wanted. 

Yea I did 10 sets of 5 cells each. My configuration is very simple. I havne't done it yet, but I plan to use those drawer liner sheets to use as extra padding(like these: https://goo.gl/ZM5JDb)
```

---
## \#58 Posted by: Kit Posted at: 2018-03-02T15:52:13.572Z Reads: 298

```
For sure, is a 2x50mm wrap from [here](https://www.aliexpress.com/snapshot/0.html?orderId=89898418767090&productId=32794376528) suitable to wrap each cell? I was going to wrap each cell individually, but It looks like you went with a larger sized wrap for the entire series/both series.
```

---
## \#59 Posted by: Fiori Posted at: 2018-03-02T15:54:08.327Z Reads: 304

```
I wrapped each series pack in its own layer of shrink wrap. The 50mm stuff wasn't wide(tall?) enough for me especially with all the soldering and nickel strip. 

Keep in mind I used two layers of 10mmx0.15 nickel.
```

---
## \#61 Posted by: kyle985 Posted at: 2018-03-06T11:04:28.273Z Reads: 319

```
Hi guys, I'm new here and would like your opinion on a similar topic, I have an evolve GTX and am planning on doing some overseas travel. I would like to convert my boards standard battery to 2-3 smaller batteries that are allowed to be taken on board a flight

I am thinking after i have the correct cells set up, I will get a custom housing made for the underneath of the board so the batteries can be easily removed and replaced, eventually i would like it set up to have swappable batteries on the go

Any suggestions are appreciated
```

---
## \#62 Posted by: Schulerbible Posted at: 2018-03-06T11:16:56.776Z Reads: 328

```
What nickel strips/belts are you guys using for the middle connections? I really would like to use belt-type strips but unsure whether they hold up the load (see below). I'm in the make of a 10s4p VTC6 pack. 

If there are belt-type strips suitable for higher currents, do you guys know a reliable source?

![image|690x441](upload://dOyA5yByUv1feTlh99P1YdUQT6x.jpg)
(credit whitepony)
```

---
## \#63 Posted by: Fiori Posted at: 2018-03-06T16:32:11.678Z Reads: 314

```
I wouldn't suggest flying at all with a home made battery back, regardless of size. Highly doubtful they would let it through. But, I would suggest you start your own topic for that.

Here is a top I made for nickel strip discussion as well:

http://www.electric-skateboard.builders/t/10mm-pure-nickel-strip-wtb-usa-battery-spot-welding-discussion/32543
```

---
## \#64 Posted by: b264 Posted at: 2018-03-06T16:34:43.001Z Reads: 288

```
Ship the board to your destination and then fly there to pick it up
```

---
## \#65 Posted by: pixelsilva Posted at: 2018-03-06T20:15:43.122Z Reads: 283

```
...or ship the battery ....and fly with the board, no?
```

---
## \#66 Posted by: b264 Posted at: 2018-03-06T20:21:40.887Z Reads: 285

```
I'd just prefer to ride out of where you pick it up rather than having to assemble it first
```

---
## \#67 Posted by: pixelsilva Posted at: 2018-03-06T20:22:17.560Z Reads: 295

```
I was thinking the other day....what if there was an esk8 App that you just use every time you arrive into another country and you'll get access to this universal battery pack that every Eskater ln the world could use?? Like a standarized battery size, and that all DIY projects will consider this size into their builds. It will be like an Airbnb or Scoot renting kind of service for the Esk8 community around the world.
```

---
## \#68 Posted by: ATLesk8 Posted at: 2018-03-06T20:47:37.367Z Reads: 288

```
There was a forum member in NYC looking to rent batteries on here a whilr back.
```

---
## \#69 Posted by: Sebike Posted at: 2018-03-06T21:52:51.796Z Reads: 281

```
@scepterr ?
```

---
## \#70 Posted by: scepterr Posted at: 2018-03-06T21:57:25.721Z Reads: 292

```
Yep was me 😋
Didn't get much traction so I dropped the idea
https://www.electric-skateboard.builders/t/nyc-battery-loan-service/42676/
```

---
## \#71 Posted by: kyle985 Posted at: 2018-03-06T22:38:50.281Z Reads: 293

```
Thanks for the responses guys! I had thought of removing the battery for air travel and purchasing a second one when I land in Cali, but I will likely be taking multiple flights within the country, this makes it a big hassle.

I also want the cells reduced in size so that I can easily swap the batteries on the go when riding in my home city, that way I can keep an extra couple of batteries in my backpack and extend my range

The other alternative is to splash out and buy a boosted board, but they emailed me and said their extended range batteries are not safe for air travel, and they do not sell their standard batteries separately - they should consider doing this as I would think they would sell out!!
```

---
## \#73 Posted by: Fiori Posted at: 2018-03-17T22:45:36.320Z Reads: 311

```
I'm back on the road boys.![20180317_154421|666x500](upload://vkHLtQFyx7p4QMXLu1dRh9BDTLE.jpg)![20180317_154410|374x500](upload://xwVEuwYFNpL91tRhQwwZYdJRhnZ.jpg)![20180317_154402|666x500](upload://wd2F9B4udYiis1R6feQrtJtpVWk.jpg)![20180317_154405|666x500](upload://dkvJW5n1jMiYzWMLTDwfBpwJ9bX.jpg)![20180317_154418|666x500](upload://bYWDhWqmE1epaY3fbgWcSZahBTZ.jpg)
```

---
## \#74 Posted by: Fiori Posted at: 2018-04-26T02:13:05.379Z Reads: 289

```
Well the Evolve ESC finally took a dump a couple of weeks ago. One of the motors stopped working on my ride home, and considering it was the one i beat the pulley onto with a hammer(well supported the shaft but still...) I figured the motor was gone: new motor = still no go. BAD ESC. I must say it did ALOT of miles for me(thousands), and was solid up until now. 

So....... I did a thing :hugs::sunglasses:

EDIT: Don't worry I'm printing a nice cover to go over that mess of wiring underneath and secure my loop key. :stuck_out_tongue: 

Oh, and I must say the throttle curve on the Focbox with mini remote is a big improvement. With the extra 15 amps I can now put to the motors its a bit quicker too(80A vs 65A on old evolve ESC). 

I also noticed that the motors are MUCH MUCH cooler after long rides, and the FOCBOX's are barely warm to the touch, they don't even break a sweat. After my rides to work on the old ESC the motors would be almost too hot to touch(as was the ESC heat sync).

![thumbnail2|375x500](upload://vr8MudFaiHNLljyoCTfdZSJgqd9.jpg)![drtuijj|375x500](upload://2O91r7SSl6CEDQWUz4RZXe2go8k.jpg)
![image|690x373](upload://aYBA86Av5kjn1nbUUhPPZub9Txo.png)![image|690x373](upload://3GpEslXrwys81Km2gdH1bRrQYWG.png)![20180425_191617|666x500](upload://fZIQe6EAx1h0qQyb7hPKeU1vrUQ.jpg)![20180425_191651|666x500](upload://ipXYBSIxQRNqIf5YyKx6QAYBj6q.jpg)
```

---
## \#75 Posted by: mikenyc Posted at: 2018-04-26T11:47:57.804Z Reads: 275

```
Why did you get rid of the stock power switch?
```

---
## \#76 Posted by: Fiori Posted at: 2018-04-26T18:03:55.501Z Reads: 274

```
Stock switch has 4 wires that plug directly into the old motor controller. It's like an electronic switch that sends an open/closed signal to the ESC(which probably uses a mosfet as a switch or something). 

 It's definitely not rated to have 80 amps running  directly through it.
```

---
## \#77 Posted by: mikenyc Posted at: 2018-04-26T19:19:51.404Z Reads: 265

```
oh interesting. I thought it was a standard latching switch (button) that could be connected to an anti spark switch.
```

---
## \#78 Posted by: b264 Posted at: 2018-04-26T19:30:53.229Z Reads: 266

```
It is that.  I'm not sure how trustworthy the latching part is.  Replacing it is a good move.
```

---
## \#79 Posted by: Fiori Posted at: 2018-04-26T19:37:42.300Z Reads: 263

```
You are correct it can be connected to an anti-spark PCB, but I didn't want to get one of those. I feel they are unreliable(iv'e read through a ton of threads). 

I feel like the loop key is unmatched in reliability and trustworthiness.
```

---
## \#80 Posted by: b264 Posted at: 2018-04-26T19:40:25.868Z Reads: 258

```
Whenever the [fatboy antispark](https://www.electric-skateboard.builders/t/fatboy-sparky-switch-300a-60v-anti-spark-switch/51532/38?u=b264) comes out I might give it a try, but until now I don't trust them either.  Loopkey for the win
```

---
## \#81 Posted by: Battosaii Posted at: 2018-04-26T19:42:53.685Z Reads: 253

```
BMS with built in switch have been the most reliable for me.
```

---
## \#82 Posted by: Fiori Posted at: 2018-04-26T19:58:13.864Z Reads: 262

```
@b264 I have been keeping an eye on that. 


@Battosaii That's nice too because it will save you some build space as well. When I install a BMS i'll try to look for one with a switch.   

What I am really waiting for is an all in one esk8 solution to come out. BMS/ESC all built into 1 easy to use PCB unit.
```

---
## \#83 Posted by: mikenyc Posted at: 2018-04-26T20:16:52.825Z Reads: 265

```
that would be great, but what about the software to run it?
```

---
## \#84 Posted by: mikenyc Posted at: 2018-04-27T12:28:27.996Z Reads: 252

```
Besttech? Don't you have to have the board turned on to charge?
```

---
## \#85 Posted by: Fiori Posted at: 2018-04-28T15:02:28.073Z Reads: 266

```
Files for my bracket if anyone wanted to use it:

https://www.thingiverse.com/thing:2883308
```

---
## \#86 Posted by: Fiori Posted at: 2018-04-28T23:58:25.729Z Reads: 279

```
Just finished a cover for the bottom wires. Thicker than I wanted so I may print a lower profile version later(maybe with some vents in it too) This is a much better improvement for now though  :) ![20180428_165425|374x500](upload://rPq2pq9NvG6As8SkQGBJmA7jWWw.jpg)![20180428_165414|666x500](upload://zMU4vnGOxY67itOPwkCJopXVsVI.jpg)![20180428_165428|666x500](upload://v5wuftVj8Bqmmv2GAofarLKTtfZ.jpg)![20180428_165444|374x500](upload://9X0XzGjIhdpxDDenWEBBzQqvApo.jpg)
```

---
## \#87 Posted by: KiwiDelta Posted at: 2018-05-17T05:50:46.354Z Reads: 253

```
Love the setup with the FOCBOX's, what kind of top speed are you getting? I'm a little late, but noticed the run you posted in October came right by my place in Windsor :slightly_smiling_face:
```

---
## \#88 Posted by: Fiori Posted at: 2018-05-17T06:14:23.301Z Reads: 249

```
Grew up in Windsor! Crazy small world. 

I am getting about 34 mph with the new setup on AT wheels. Probably much faster on 107's but i never tried
```

---
## \#89 Posted by: Janosh Posted at: 2018-05-17T21:57:18.768Z Reads: 241

```
Hi,

I 'll do the same upgrade to focboxes next week.
Maybe I missed it, what BMS do you use for charging?
```

---
## \#90 Posted by: Fiori Posted at: 2018-05-18T02:17:07.240Z Reads: 242

```
You didn't miss anything. I have been bulk charging since I did the swap. I have the balance leads hanging there in case I want to use them later.  I have checked the cells manually a couple times, they haven't even drifted a tenth of a volt over the last month or so of charging(I would say 60 cycles at least). 

I cut the ends off both my evolve chargers and soldered a bullet connector to one wire(+) and the other wire to a single port of the xt-90 connector(the end with the resistor marked in green) and just charge straight to the battery.

I never charge when I am not around to monitor it. If you do this just please be aware that YOU are the BMS for your battery.
```

---
## \#91 Posted by: Janosh Posted at: 2018-05-18T11:37:54.943Z Reads: 232

```
Ah. Ok.

My first plan was to use a charger with balancer, but I want to use an external battery pack in addition to my 10S5P to increase the range if needed. So I will intsall a BMS just for charging and use the external balancer from time to time to double check the function of the BMS.
```

---
## \#92 Posted by: Fiori Posted at: 2018-05-18T16:17:47.575Z Reads: 224

```
i thought about doing this too, like some sort of extra 10s2p pack I could mount on the back for extra range. 

But i decided not to because I don't think it's good to be connecting two separate made packs in parallel unless they are going to be permanently connected and charged together. 

The cells in the main pack could be more or less degraded than the smaller pack and cause some issues.  I could be totally wrong.
```

---
## \#93 Posted by: Janosh Posted at: 2018-05-18T16:48:42.600Z Reads: 218

```
The packs won't be connected in parallel ;-)
I will charge my main pack while riding.
```

---
## \#94 Posted by: Fiori Posted at: 2018-05-18T17:08:22.673Z Reads: 213

```
Oh so just building a spare battery pack?
```

---
## \#95 Posted by: Janosh Posted at: 2018-05-18T18:59:45.419Z Reads: 206

```
Using a 6s Lipo with 16 Ah connected to a DC boost converter connected to the charging port and charging with 5 amps while riding.  :slight_smile:
```

---
## \#96 Posted by: b264 Posted at: 2018-05-18T19:02:00.985Z Reads: 212

```
In that scenario, if you hit the brakes from high speed, you could spike the charge current pretty high
```

---
## \#97 Posted by: Janosh Posted at: 2018-05-18T19:10:01.490Z Reads: 214

```
We have a few people here using this setup, no issues so far. Even with the original Evolve electronics.

You can also use this setup as a mobile charger.
```

---
## \#98 Posted by: Fiori Posted at: 2018-05-18T20:04:01.200Z Reads: 209

```
I'm confused..... why would you want to use your board to charge another battery? Seems really in efficient...
```

---
## \#99 Posted by: Janosh Posted at: 2018-05-18T20:17:13.168Z Reads: 219

```
Hä? The Lipo pack can be used while riding or as a mobile charger while takeing a break.
If you don't want to use it while riding.
```

---
## \#100 Posted by: Fiori Posted at: 2018-09-06T15:28:10.693Z Reads: 203

```
Quick update: Yesterday I went to ride the board back from dropping off my girlfriends car at the dealer and it wouldn't go. Check voltage at the loop key and port i placed underneath: found the board had no voltage. 

Took the board home and took the battery out for diagnosis. After checking the balance leads I quickly found out I had a bad parallel pack. When I made the pack, I made 10 separate packs of 5 cells in parallel, and then welded them together in series. 

I'm thinking that 1 cell in the parallel pack went bad, and then the other 5 slowly killed themselves. I am not sure if this is from bulk charging(I bulk charged for over 100 cycles im sure). I'm just glad this wasn't a fire. 

I plan to get a bluetooth BMS and install it this time around so I can monitor everything more closely. More pictures to come.
```

---
## \#101 Posted by: b264 Posted at: 2018-09-06T15:39:39.611Z Reads: 193

```
What exactly do you mean "bulk charging"?
```

---
## \#102 Posted by: Fiori Posted at: 2018-09-06T15:53:27.043Z Reads: 194

```
No bms, charging using a brick straight to the leads.
```

---
## \#103 Posted by: b264 Posted at: 2018-09-06T15:55:22.467Z Reads: 197

```
:open_mouth:&nbsp;&nbsp;
```

---
## \#104 Posted by: Fiori Posted at: 2018-09-06T15:57:24.190Z Reads: 201

```
Shouldn't be much of a problem in a pack this small. But, here we are... lol. I am not sure if that was even the issue. I'll never know, but i suspect it. 

I didn't find any burn marks, or any signs of damage. Just 5 cells with 0volts(an entire P pack). 

Luckily, due to the way i wired my pack(by luck not design), the P pack acted as a fuse almost, and rendered the pack unuseable(so this didnt spread) after this happened.
```

---
## \#105 Posted by: b264 Posted at: 2018-09-06T16:22:56.764Z Reads: 193

```
Did you ever bulk-charge consecutively?  Or did you always alternate with a balanced charge?  Because alternating shouldn't really be harmful at all -- but trusting end-users or self to do that every other time is a recipe for a dead battery
```

---
## \#106 Posted by: Fiori Posted at: 2018-09-06T16:55:40.950Z Reads: 190

```
I hadn't balance charged in over 100 cycles. I had just checked all the cells about two weeks ago, all within 0.1v
```

---
## \#107 Posted by: Fiori Posted at: 2018-11-07T17:57:30.509Z Reads: 206

```
Built a fresh new 10s5p for this beauty this last weekend. Much cleaner battery build this time around, more insulation and a better fit. Now complete with bluetooth bms, and no more box on top. 

![Screenshot_20181106-070031_xiaoxiang|243x500](upload://5Z3WhFg2hPceST2o5FrkNnEPSq2.jpeg)
![Screenshot_20181106-070051_xiaoxiang|243x500](upload://bTCPEDRtDA1JY5lyGtAefHf6DGR.jpeg) 

![Screenshot_20181106-070022_xiaoxiang|243x500](upload://qVMl1117nR9N458ylbGkeNRleTJ.jpeg) 

![20181107_092417|666x500](upload://f6kBOo1Bt7GZVBy60vHBDFv2TQp.jpeg) ![20181107_092452|666x500](upload://yCKsFI8sKxWZm4w7aSDNsbmPsmj.jpeg) ![20181107_092423|375x500](upload://4SKbq7P18oRY8sUkTagYmxiR1Oa.jpeg) ![20181107_092427|666x500](upload://rAxvRVk5oS4DGgG7LgrgPTcmmqh.jpeg)![20181103_224553|375x500](upload://zSyFYdpfnCbLNSzd2oA7VvN8Ku9.jpeg) ![20181103_224546|666x500](upload://12CQMq8TtVpXSKGxfCwAGqs5OP6.jpeg) ![20181103_224544|666x500](upload://5sLCKvpaoOnhGRuHJ6ebnReefvm.jpeg) ![20181106_164545|375x500](upload://aVECZuf7zQoZYw2PFUGeIFyrlaG.jpeg) ![20181104_130415|666x500](upload://v2W6xTIH3yYkVGdtnHzpL49m6dJ.jpeg)
```

---
## \#108 Posted by: Fiori Posted at: 2018-12-02T20:38:51.485Z Reads: 200

```
![20181118_131022|375x500](upload://y3rPJZBZ0LtukuCB2bqKCdji9CE.jpeg) ![20181118_130959|374x500](upload://s3Z7uyQgClxD5CkxtmBLrFzU63P.jpeg) ![20181118_115222|375x500](upload://e9F9J9WfJCPfrPFPUITmJYEQlsN.jpeg) ![20181118_130951|374x500](upload://n0vNOon4AudygkmuQ7M7stk6Ygb.jpeg)  ![20181118_131006|666x500](upload://hETFjRMHoGnhT2pcfjM1OhNDgfM.jpeg) ![20181118_130946|666x500](upload://nMsNXMbWkhqp6fHaYesCk2gPNL5.jpeg) ![20181118_130914|375x500](upload://sdu4NJu4ZL8ozcaPWm4ROdq9Kir.jpeg) ![20181118_130850|374x500](upload://3m6TGZSV8B1K7mPtMoLzKyXNGm9.jpeg)![20181118_115227|666x500](upload://zxol9XeKSvzHafYWfqiyK8fa6Ah.jpeg)
```

---
## \#109 Posted by: PickSix24 Posted at: 2018-12-02T21:19:42.623Z Reads: 184

```
Nice upgrade, can I ask what your vesc settings are ? I’m
Running same setup.
```

---
## \#110 Posted by: Fiori Posted at: 2018-12-02T21:23:07.680Z Reads: 187

```
I setup my focboxs awhile go and haven't changed them since. I am running 40 battery amps per foc box. I think I have motor max turned up to 80A. BLDC MODE. Sensorless. Vescs connected over CAN. 

When I take a ride later today I'll upload a pic from the BT app of my settings.
```

---
## \#111 Posted by: PickSix24 Posted at: 2018-12-03T04:42:16.807Z Reads: 181

```

I’ve got a similar setup , trying to figure out how you got 34mph. I’m topping out at 25mph on 8” AT
I’ve got dual Focboxes, 5065 200kv , 15T / 66T, 10s4p 30Q.  Maybe my vesc settings aren’t up to snuff.
```

---
## \#112 Posted by: Fiori Posted at: 2018-12-03T05:10:11.119Z Reads: 182

```
Full charge, air up tires to max. I got 34 when I was set to 50A per foc box (100 Battery Amp total). But Im on 10s5p i wouldnt go 100A on 4p
```

---
## \#113 Posted by: PickSix24 Posted at: 2018-12-03T05:18:17.364Z Reads: 181

```
I may have to build a larger battery. I’m at 40a batt amp with 10s4p
```

---
## \#114 Posted by: Fiori Posted at: 2018-12-03T05:21:40.606Z Reads: 179

```
I keep mine at 40A, I felt like it was too much strain on everything to go 20A per cell.
```

---
## \#115 Posted by: Fiori Posted at: 2018-12-30T22:34:04.184Z Reads: 179

```
Almost two months since the new pack has been in. Still nice and balanced :) 

![Screenshot_20181230-143357_xiaoxiang|243x500](upload://wiYTPQvKPJUolb1jcWMMn13F923.jpeg)
```

---
## \#116 Posted by: pjotr47 Posted at: 2018-12-30T22:41:12.055Z Reads: 165

```
What BMS are you using?
```

---
## \#117 Posted by: Fiori Posted at: 2018-12-30T22:43:33.809Z Reads: 174

```
This is the BMS i ordered: https://www.aliexpress.com/item/10S-36V-Lithium-Battery-PCB-and-smart-BMS-with-Bluetooth-Function-APP-software-42V-electric-bike/32879447246.html?spm=a2g0s.9042311.0.0.10a14c4drSrOgP

Surprisingly not many people here use it. I also found a huge thread related to this bms(and a few others like it) on endless-sphere: https://endless-sphere.com/forums/viewtopic.php?t=88676

EDIT: I bought the lowest amp one they had, as i am running it bypassed(charge/balance only).
```

---
## \#118 Posted by: legend27 Posted at: 2018-12-30T23:10:25.199Z Reads: 165

```
next level stuff you got going on
```

---
## \#119 Posted by: legend27 Posted at: 2018-12-30T23:12:43.782Z Reads: 164

```
Can you also limit how many volts the battery charges to?
```

---
## \#120 Posted by: Fiori Posted at: 2018-12-30T23:26:58.707Z Reads: 166

```
Yea you can set it to whatever you want. Almost everything is adjustable.
```

---
## \#121 Posted by: pjotr47 Posted at: 2018-12-30T23:33:11.949Z Reads: 168

```
Thnx for the link. I see it is the same I have ordered 5 days ago :slight_smile: I have ordered the 12s 60A BMS. I hope it will work
```

---
## \#122 Posted by: b264 Posted at: 2018-12-31T04:14:59.100Z Reads: 176

```
https://endless-sphere.com/forums/viewtopic.php?t=88676#p1293475
[quote]
The BMS must have on board memory because it saves the number of cycles the battery has seen
[/quote]
 This right here is badass.
```

---
## \#123 Posted by: Fiori Posted at: 2018-12-31T05:42:30.125Z Reads: 182

```
Only if you have it setup for discharge too though.
```

---
## \#124 Posted by: b264 Posted at: 2018-12-31T05:46:40.406Z Reads: 180

```
Welp, there goes that idea. LoL
```

---
## \#125 Posted by: Fiori Posted at: 2018-12-31T15:54:21.330Z Reads: 190

```
I was a little bummed about it too. I thought it could get a rough value from just the voltage....but I guess it makes sense.
```

---
## \#126 Posted by: hyperIon1 Posted at: 2019-01-05T02:46:07.630Z Reads: 189

```
throw a unity in and all kinds of room will appear 

![E1474D32-97F1-4095-9C73-7C3F48ABBAA8|690x488](upload://1RGwrnK9g8Kv20RGD60kP6LuaaT.jpeg) ![10AFB660-BB80-485D-B0BA-4F48551D41E8|690x345](upload://yE4rd7OWxwNQv6xCoxY2eK0dH1.jpeg)
```

---
## \#127 Posted by: Marsen Posted at: 2019-01-05T05:54:26.061Z Reads: 182

```
I use these BMS's and haven't had any issues with them. I have just ordered a load of Infineon MOSFETS ( IRFS4115) to upgrade the power switch side of the BMS. They are rated 375W each a big improvement on the ones fitted. I got them for a 160 Amp upgrade for a golf cart battery I am building.
```

---
## \#128 Posted by: Marsen Posted at: 2019-01-05T06:01:21.377Z Reads: 178

```
I think you will need the PC module to change the voltage settings on these, I only use the PC module for setup so have never tried the App for changing settings just for checking. Yes there is an EPROM on the BMS and microprocessor.
```

---
## \#129 Posted by: Eboostin Posted at: 2019-01-05T06:01:36.551Z Reads: 178

```
How does it perform with the 10S4P 30q?
```

---
## \#130 Posted by: hyperIon1 Posted at: 2019-01-05T06:07:43.247Z Reads: 183

```
In comparison, I would say it as if its a new board.  with all new evolves you get the best at the beginning and start to decline from there. 
I have room for a 10s5p but wanted to see what a 10s4p would do.
its direct discharge and on 63mm motors (carbon) with the unity
the GTX enclosure is on a nomad (bustin board) with duel focbox
we just did an upgrade to a GTX with a 3d printed riser
```

---
## \#131 Posted by: hyperIon1 Posted at: 2019-01-05T06:09:56.410Z Reads: 188

```
![image|217x500](upload://9ES5Fp8QzpjQQu39eY9U0v4vokx.jpeg) ![image|375x500](upload://eESVJmv89K4qiguX7GZOFQ1LS8e.jpeg) ![image|198x500](upload://5SAy38TmCTSopPTq2lhM5c03LrS.jpeg) ![image|272x500](upload://88H8I55zDOufdAYPnx13lwCn13n.jpeg) ![image|281x499](upload://rYJWG8XNHwHcwbKf7fsNpRi77m7.jpeg)
```

---
## \#132 Posted by: Marsen Posted at: 2019-01-05T06:10:00.445Z Reads: 174

```
Wow stacks of room. You could carry a sandwich in there for long rides.
```

---
## \#133 Posted by: hyperIon1 Posted at: 2019-01-05T06:10:51.444Z Reads: 177

```
This is a 10s5p. With tons of room.
With only a 1/2 inch increase in enclosure depth or drop.
```

---
## \#134 Posted by: hyperIon1 Posted at: 2019-01-05T06:14:34.709Z Reads: 184

```
The gtx 
![image|690x336](upload://ywn4PHac5NwcG6MPTepxs5U0k9l.jpeg) ![image|690x458](upload://lXfhjsCV1qq0TzNfyoxQh9TPuGB.jpeg)
```

---
## \#135 Posted by: hyperIon1 Posted at: 2019-01-05T06:18:20.467Z Reads: 185

```
![image|375x500](upload://7tfQtrfFsaVtkU8khotqzcZT2HU.jpeg)
```

---
## \#136 Posted by: hyperIon1 Posted at: 2019-01-05T06:21:27.409Z Reads: 184

```
for this one, the battery was so new I just converted it to direct discharge put it on a mini bms, results so far are great
```

---
## \#137 Posted by: Jaydawg56 Posted at: 2019-01-05T13:46:40.232Z Reads: 187

```
Forgot to ask, how’s the spacer holding with the flex and weight of the bamboo/double stack batt combo?
```

---
## \#138 Posted by: hyperIon1 Posted at: 2019-01-05T20:53:42.930Z Reads: 188

```
great, we had it printed with a material that flexes a bit and it is 4 pc so plenty of flex
```

---
## \#139 Posted by: ducnuken Posted at: 2019-02-20T15:23:59.384Z Reads: 177

```
hi i would like to ask if it is possible to get that 3d-printed riser shipped from you?
i really want that 10s5p in my gtx and its hard to fins that kind of riser =(

btw i live in sweden.
```

---
## \#140 Posted by: hyperIon1 Posted at: 2019-02-21T00:00:04.272Z Reads: 170

```
I will see what shipping will be and get back to you.
```

---
## \#141 Posted by: ducnuken Posted at: 2019-02-25T01:58:55.909Z Reads: 169

```
Pls can you add me on messenger?
```

---
## \#142 Posted by: hyperIon1 Posted at: 2019-02-25T15:14:01.721Z Reads: 168

```
Sorry for the delay in responding. I checked shipping and if you not in a big hurry I can send you one for $50 shipped
```

---
## \#143 Posted by: M.Hboards Posted at: 2019-02-26T01:50:54.156Z Reads: 159

```
@Fiori i know you used the bms for charge only but do you know if the 2 wires that come off the bms are for a switch? If yes does that switch need to be on while chargeing or only dischargeing?
```

---
## \#144 Posted by: Fiori Posted at: 2019-02-26T05:25:18.237Z Reads: 149

```
Do you mean the bluetooth bms or the evolve one? The two wires on the bluetooth bms is actually a temperature sensor.
```

---
## \#145 Posted by: M.Hboards Posted at: 2019-02-26T12:24:42.671Z Reads: 141

```
On the bluetooth one i thought mabe there was a built in eswitch useing the 2 black wires comeing out
```

---
## \#146 Posted by: Fiori Posted at: 2019-02-26T19:22:58.226Z Reads: 132

```
I know there are pads on the circuit board for a switch though if you wanted to use one.
```

---
## \#148 Posted by: ducnuken Posted at: 2019-02-27T01:23:06.845Z Reads: 130

```
Yes pls, How do We process This?
```

---
## \#149 Posted by: Fiori Posted at: 2019-02-27T05:13:47.631Z Reads: 124

```
@hyperIon1 and @ducnuken you fellas mind taking this to PM?
```

---
## \#150 Posted by: ducnuken Posted at: 2019-02-27T10:19:17.839Z Reads: 131

```
Sorry Im new in This  forum and i did try to PM but it didnt worked :/
```

---
## \#151 Posted by: Fiori Posted at: 2019-02-27T18:21:53.092Z Reads: 138

```
It's ok. New members actually do not have access to private messaging until they reach a certain rank.
```

---
## \#152 Posted by: ajplant96 Posted at: 2019-04-24T01:24:36.691Z Reads: 127

```
Did you have to lower the heatsink to fit the unity in your CGT? I’m finding it’s too tight a fit for the sensor cables and it’s stuffing up the board’s performance when rider weight is applied
```

---
## \#153 Posted by: hyperIon1 Posted at: 2019-04-24T01:41:48.513Z Reads: 131

```
No, you just have to strip it down

![IMG_1159|666x500](upload://hb2c8abUDLip5TToXKr969Zt5iC.jpeg)
```

---
## \#154 Posted by: Rithblu Posted at: 2019-04-24T02:00:31.791Z Reads: 130

```
Dud's those mods looks great.
```

---
## \#155 Posted by: hyperIon1 Posted at: 2019-04-24T02:02:28.918Z Reads: 131

```
I need to talk with you about some stuff........
https://www.electric-skateboard.builders/t/mbs-emtb-kits-and-prebuilt-affordable-options/90814
```

---
## \#156 Posted by: Rithblu Posted at: 2019-04-24T02:03:13.967Z Reads: 131

```
This is what i did with mine, swapping out different wheels just to see which one i like better.
![20190404_213407|375x500](upload://6jzpmyqCGkzaXse2DfkoBVi8KFp.jpeg) ![20190411_122455|666x500](upload://eSUvXdUs6uTQddQ2Tplg3LgtSDx.jpeg) ![IMG_20190411_230920_155|500x500](upload://5NWz7wejqwpUDd4mIyC8ZBIhq9t.jpeg) ![thumbnail%20(2)|375x500](upload://1RBs2g5uBQTg0hPc0YPC9SbUNhs.jpeg) ![thumbnail%20(3)|375x500](upload://eMS1LXW3ftizrLyryO7dfPW63UY.jpeg) ![thumbnail%20(4)|666x500](upload://bEIovtfbICur9JSLp56pEVbKg7U.jpeg) ![thumbnail|666x500](upload://eh1vmY31m2D9IkHkwuku0sFd8Si.jpeg)
```

---
## \#157 Posted by: hyperIon1 Posted at: 2019-04-24T02:06:09.247Z Reads: 122

```
OMG those gears are as big as the tires WOW that's a hell of a MOD
```

---
## \#158 Posted by: hyperIon1 Posted at: 2019-04-24T02:07:23.549Z Reads: 127

```
unity?

![image|421x500](upload://iCqENSA5XxmLgPo5fdJ3Nwt2OVT.jpeg)
```

---
## \#159 Posted by: Rithblu Posted at: 2019-04-24T02:08:31.540Z Reads: 123

```
No dual Foc.
```

---
## \#160 Posted by: hyperIon1 Posted at: 2019-04-24T02:10:19.295Z Reads: 122

```
whats the battery size, some people have been looking for a mod like this
```

---
## \#161 Posted by: Rithblu Posted at: 2019-04-24T02:25:32.948Z Reads: 127

```
12s 4p Samsung 30Q
```

---
## \#162 Posted by: ajplant96 Posted at: 2019-04-24T03:05:07.331Z Reads: 126

```
Strip it down? Do you mean remove the heatsink built in to the bottom of the unity?
```

---
## \#163 Posted by: hyperIon1 Posted at: 2019-04-24T04:26:30.676Z Reads: 124

```
no, just remove the silicone cover. and I used the OG evolve heatsink.
And because space is so tight I used double sided heat transfer tape only. It should fit
```

---
## \#164 Posted by: ajplant96 Posted at: 2019-04-24T06:41:44.063Z Reads: 123

```
Hmm that’s strange, in my enclosure it’s still too high doing that as the sensor cables are being compressed to the point of causing the motors not to run properly
```

---
## \#165 Posted by: hyperIon1 Posted at: 2019-04-24T18:03:34.221Z Reads: 121

```
You can try to add a few washers to the heatsink to lower it a little. you have some room but not much. Maybe enough, the CF decks are inconsistent because a lot of the process is still by hand.
```

---
## \#166 Posted by: ajplant96 Posted at: 2019-04-25T10:37:17.869Z Reads: 115

```
I just installed a 8mm spacer and it’s still problematic, even after removing the foam from underneath the lid for even more clearance... gonna try adding rubber to the edges of the lid next for some extra lift and water resistance simultaneously.
```

---
## \#167 Posted by: hyperIon1 Posted at: 2019-04-25T20:46:23.090Z Reads: 111

```
that's wild, I have only done this upgrade to the one CGT I had n idea they were so inconsistent.
```

---
## \#168 Posted by: ajplant96 Posted at: 2019-04-30T03:22:51.007Z Reads: 110

```
Evolve should be announcing their gen 4 lineup tomorrow so hopefully the carbons are sorted for being made identical from now on
```

---
## \#169 Posted by: Jaydawg56 Posted at: 2019-04-30T04:30:19.143Z Reads: 107

```
Tomorrow? That right?
```

---
## \#170 Posted by: drone001 Posted at: 2019-04-30T23:53:28.183Z Reads: 107

```
ok its tmr....lets see em.....
```

---
## \#171 Posted by: Jaydawg56 Posted at: 2019-05-01T01:06:33.199Z Reads: 108

```
Just a teaser pic blasted out on FB so far
```

---
## \#172 Posted by: pixelsilva Posted at: 2019-05-01T15:12:00.393Z Reads: 107

```
With this teaser smells like Metroboard rained much sooner over the party with less fanfare.
```

---
## \#173 Posted by: Jaydawg56 Posted at: 2019-05-02T00:54:06.100Z Reads: 103

```
Yea that metroboardX is the answer to every complaint that was voiced to evovle, haha. Batteries are good, display and button placement are nice and comes with 107s and 190s right out the gate.
```

---
## \#174 Posted by: pixelsilva Posted at: 2019-05-02T01:21:35.827Z Reads: 106

```
Totally. Metroboard is a dark horse. Is about time Esk8 collective gives them the credit they deserve.
```

---
## \#175 Posted by: b264 Posted at: 2019-05-02T02:12:49.798Z Reads: 104

```
They do deserve credit, they are definitely the best prebuilts.
```

---
## \#176 Posted by: ajplant96 Posted at: 2019-05-23T10:55:13.829Z Reads: 96

```
Hey forgot to ask last time I visited this thread but what remote are you using and where did you get that BMS? I'm switching to a 10s5p and the current components I'm using in those categories aren't super space friendly
```

---
## \#177 Posted by: hyperIon1 Posted at: 2019-05-23T15:28:05.574Z Reads: 97

```
im using the maytech remote and the bms is a d124 from litech/bestech.

I have both 


https://maytech.cn/products/maytech-2-4ghz-waterproof-remote-controller-mtskr1805wf
```

---
## \#178 Posted by: b264 Posted at: 2019-05-24T03:59:20.166Z Reads: 88

```
[quote="hyperIon1, post:177, topic:34045"]
d124 from litech/bestech.
[/quote]

http://www.litechpower.com/product-detail/HCX-D124LI10S.html
```

---
## \#179 Posted by: hyperIon1 Posted at: 2019-05-24T22:44:33.866Z Reads: 84

```
yep that's the one, smallest we could find with a decent charge rate and foot print
```

---
## \#180 Posted by: b264 Posted at: 2019-05-25T06:05:08.771Z Reads: 85

```
The double-PCB ones are more difficult to waterproof, but I like that one also.
```

---
## \#181 Posted by: PixelatedPolyeurthan Posted at: 2019-08-18T06:40:19.793Z Reads: 65

```
is the d124 BMS good? I have a stock evolve battery with a focbox needing to with it and I am looking for BMS's. here is a photo of evolve bms.![IMG_20190817_214106|666x500](upload://2LEznkClYaeMFVecrHUXZwCxmOB.jpeg)
```

---
## \#182 Posted by: hyperIon1 Posted at: 2019-08-18T17:02:55.221Z Reads: 61

```
So to clarify, you are looking for a bms to replace the bms on an evolve battery pack? So you can use a focbox esc instead of the evolve esc?

the d124 is smaller

![IMG_1129|375x500](upload://ebbHVbcV7OiLr2WYdwe2rYZ36EI.jpeg)
```

---
## \#183 Posted by: hyperIon1 Posted at: 2019-08-18T17:03:31.164Z Reads: 61

```
the d124 bms on a evolve battery pack

![image|322x500](upload://tfoATYqzkt6WrCflPPgKLY0ZIsh.jpeg)
```

---
## \#184 Posted by: PixelatedPolyeurthan Posted at: 2019-08-18T19:35:34.576Z Reads: 55

```
yep, that's what I wanted to know, thanks :smile: !
```

---
