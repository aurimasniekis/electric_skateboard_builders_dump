# Benchwheel pairing issues

### Replies: 69 Views: 4065

## \#1 Posted by: kptheinventor Posted at: 2017-02-28T03:57:06.745Z Reads: 177

```
Hi there. I have recently ordered a Benchwheel remote and are having issues connecting it to the receiver it came with. I have followed the instructions they came with and have tried many variations on the wires. When I plug the wires from the vesc into the receiver and turn on and hold the power on button on the remote for 7secs, I'll get the beeping on the remote however it will not work. I have tried plugging in the vesc into my and checked on the BLDC tool which on the ppm tab, looking at the display section goes from 50% to 49% and the pulse width number flickers.

Does anyone have any ideas?

https://www.youtube.com/watch?v=ysDfeabX730&feature=youtu.be

<img src="/uploads/db1493/original/3X/d/7/d721cf542ed3c2ccea6de4ed6f17347bdb98381e.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/9/d/9d4ee60e8ec806a95753301acbda4f5daecd1610.JPG" width="690" height="388"><img src="/uploads/db1493/original/3X/b/d/bd1dfdb15533fb876b21f9285195be4774589dc7.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/c/d/cda78600152fe1705b2fd061997202ce2a47df02.JPG" width="690" height="388"><img src="/uploads/db1493/original/3X/4/e/4e062bb5902d59caf5a1cb0e00bd4d2caa53e94c.JPG" width="690" height="388">
```

---
## \#2 Posted by: Namasaki Posted at: 2017-02-28T04:09:10.552Z Reads: 153

```

Try connecting the vesc to the receiver before connecting the power.
Then press and hold the red button on the remote
Then while holding the remote red button, connect the power to the vesc.
The receiver should beep 3 times and you should see a green light on the remote.

Here are the instructions for pairing with a benchwheel board. Make sure remote and board are fully charged.
Make sure remote and board has been turned off (off status)
1, press and hold the red buttons on both remote and board at the same time. 
2, keep holding both red buttons and wait around 3 sec. 
3, release both red buttons when you hear 3 beeps. 
4, the pairing process is done. You can now turn off the board and remote, restart and have fun.
```

---
## \#3 Posted by: mmaner Posted at: 2017-02-28T04:12:25.272Z Reads: 145

```
Make sure you're turning the remote in before the VESC.  I have 3, they all work flawlessly but it won't bind if the VESC is in first.
```

---
## \#4 Posted by: kptheinventor Posted at: 2017-02-28T04:20:25.046Z Reads: 137

```
Okay will use those troubleshoots thanks. Do you have to turn off and on the board and remote before testing the throttle?
```

---
## \#5 Posted by: kptheinventor Posted at: 2017-02-28T04:21:48.873Z Reads: 137

```
Thanks will give it a go once I fully charge the remote. Should the wires connecting the receivers be connected to the vesc during those steps?
```

---
## \#6 Posted by: Namasaki Posted at: 2017-02-28T04:32:51.570Z Reads: 130

```
you will need to connect the vesc to the receiver in order to supply power to the receiver
```

---
## \#7 Posted by: kptheinventor Posted at: 2017-02-28T05:43:40.496Z Reads: 130

```
When you say "press and hold the red buttons on both the remote and the board at the same time" assume the red button on the remote is the first which is the second red button?
```

---
## \#8 Posted by: kptheinventor Posted at: 2017-02-28T05:58:31.556Z Reads: 134

```
@Namasaki @mmaner

https://www.youtube.com/watch?v=YiWvo9sogto&feature=youtu.be

Tried starting the remote before the vesc. Only got two beeps
```

---
## \#9 Posted by: Namasaki Posted at: 2017-02-28T06:51:34.398Z Reads: 128

```
those instructions where actually for the benchwheel board and remote
```

---
## \#10 Posted by: kptheinventor Posted at: 2017-02-28T10:19:08.150Z Reads: 125

```
Yeah I see. I'm thinking it is a faulty remote, do you know any about that?
```

---
## \#11 Posted by: darkkevind Posted at: 2017-02-28T11:17:09.203Z Reads: 124

```
You connected the battery to the VESC before you turned the remote on!?

You're supposed to turn the remote on first...
```

---
## \#12 Posted by: yaca Posted at: 2017-02-28T19:47:36.106Z Reads: 119

```
You have to press the white button on the receiver for 7 seconds as well.

http://www.electric-skateboard.builders/t/benchwheel-remote-receiver/14171/39
```

---
## \#13 Posted by: kptheinventor Posted at: 2017-02-28T20:28:30.225Z Reads: 112

```
I had tried the remote before the vesc before lots of times that was just a video to show, apparently not a good one haha. How long from turning on the remote would you say I should be turning on the vesc? I was leaving roughly 1 second in between.
```

---
## \#14 Posted by: darkkevind Posted at: 2017-02-28T20:29:09.784Z Reads: 110

```
Yeah that's about all you need...
```

---
## \#15 Posted by: kptheinventor Posted at: 2017-02-28T20:38:29.984Z Reads: 107

```
OMG YES. It was the white button of course hahah it should really say that on the instructions. Although now it seems to not want to change from High mode to Low mode.
```

---
## \#16 Posted by: yaca Posted at: 2017-02-28T20:46:15.204Z Reads: 108

```
Good to hear it works now. For to change the mode you have to press the power button on the remote, but only for a short time when the remote is already on.
```

---
## \#17 Posted by: yaca Posted at: 2017-02-28T20:48:31.497Z Reads: 108

```
Do you have a constant blue light on the receiver or is it a undefined blue flashing?
```

---
## \#18 Posted by: kptheinventor Posted at: 2017-02-28T21:13:56.059Z Reads: 105

```
Yeah I've tried that but doesn't do anything
```

---
## \#19 Posted by: kptheinventor Posted at: 2017-02-28T21:14:13.984Z Reads: 103

```
blue flashing
```

---
## \#20 Posted by: yaca Posted at: 2017-02-28T21:19:56.869Z Reads: 104

```
Strange, even without receiver the remote's LED will change from red to green when I press the button for a short time. The battery is full?
```

---
## \#21 Posted by: Norco Posted at: 2017-02-28T21:23:49.188Z Reads: 103

```
You can't change the mode once you have moved the trigger. You need to power off then on again to change the mode. The trigger locks the mode.
```

---
## \#22 Posted by: kptheinventor Posted at: 2017-02-28T23:21:19.235Z Reads: 102

```
@yaca @Norco Don't worry it just seems to take awhile how long the button should be pushed for
```

---
## \#23 Posted by: kptheinventor Posted at: 2017-02-28T23:23:12.762Z Reads: 100

```
Thanks everyone for helping out! I have been able to take out my board for the first time in over 2 weeks after waiting for a new remote and troubleshooting it :) This is why the DIY esk8 community is so good
```

---
## \#24 Posted by: darkkevind Posted at: 2017-03-13T12:38:33.406Z Reads: 97

```
Could someone just give me a little advice here please?

Which pins do i connect the ESC to on the receiver? Do i need a separate power source for it if my ESC has BEC?

<img src="/uploads/db1493/original/3X/3/5/3564336196f4171ddf46381a3fea62cb5fbeeb18.jpg" width="281" height="500">
```

---
## \#25 Posted by: mmaner Posted at: 2017-03-13T12:56:54.776Z Reads: 91

```
I don't know about the BEC but the 3 pins closest to the antenna connect to the ESC.
```

---
## \#26 Posted by: darkkevind Posted at: 2017-03-13T13:04:32.340Z Reads: 91

```
Yes, thank you. I tried that and it came on (blue led). Still can't pair it though :frowning:
```

---
## \#27 Posted by: mmaner Posted at: 2017-03-13T13:06:02.345Z Reads: 91

```
Turn on the ESC
Connect the RX and turn on the remote at the same time
  while holding the remote power button until you hear 2 or 3 beeps, depending on model
```

---
## \#28 Posted by: darkkevind Posted at: 2017-03-13T13:09:22.363Z Reads: 90

```
I got the two beeps, but no control from the remote...

Do you have to do anything after you get the two beeps? Thing is, holding down the power button on the remote, even when not trying to pair gives me two beeps after a few seconds.
```

---
## \#29 Posted by: mmaner Posted at: 2017-03-13T13:10:56.114Z Reads: 90

```
just turn everything off and then back on.  I have 3 benchwheel remotes and this has always worked for me.
```

---
## \#30 Posted by: darkkevind Posted at: 2017-03-13T13:13:53.464Z Reads: 88

```
OK, I'll give it another go, thanks :thumbsup:

I think I'll wait until my remote is fully charged.
```

---
## \#31 Posted by: mmaner Posted at: 2017-03-13T13:14:23.161Z Reads: 88

```
No worries, just slow down and maybe take a break.  Remotes can be frustrating as hell :)
```

---
## \#32 Posted by: kptheinventor Posted at: 2017-03-13T22:38:58.261Z Reads: 89

```
@darkkevind I think It depends on what board you are using. Whether it's Benchwheel board or a DIY board. If it is a benchwheel board then I think the instructions are up the page. I have DIY using a vesc and you plug the connects to the inside 3 plugs on the receiver. Remember you must order the remote and receiver together.

What I eventually did for DIY (through the help of this fourm):

-Charge you batteries for the board and the remote.
-Plug your receiver into the esc
-Turn off both the remote and the board
-Press and hold the small white button on the receiver
-Press and hold the remotes red power button
-Turn on the board still holding down both the white button and the red button until it pairs (should start flashing a blue light on the receiver quite fast at this point)
-Turn the board and the remote on and off

I'd try those a few times and if it doesn't work switch the order slightly and keep trying
```

---
## \#33 Posted by: darkkevind Posted at: 2017-03-13T23:44:53.803Z Reads: 81

```
Thanks, I'll try what you've suggested. It's a DIY board and i did get them together. I thought they'd already be paired to be honest. No such luck.

I'm still waiting for the remote to charge! I've only got one light still and it's been on charge for hours. It's charging with a Samsung phone charger, pretty sure it's 1.5mah... Is that enough?
```

---
## \#34 Posted by: mmaner Posted at: 2017-03-14T02:08:38.323Z Reads: 76

```
If it's 1 green light, the one on top, that means it's fully  charged.
```

---
## \#35 Posted by: kptheinventor Posted at: 2017-03-14T02:12:07.024Z Reads: 78

```
Those battery lights on the remote don't mean anything unless you have a Bench wheel board, just ignore them.
```

---
## \#36 Posted by: mmaner Posted at: 2017-03-14T02:13:40.549Z Reads: 79

```
When charging the remote they mean a lot.  The lights will light up 1 start time up to the battery level, each light being 20%. When the remote is fully charged you will have a single green light at the top.
```

---
## \#37 Posted by: kptheinventor Posted at: 2017-03-14T02:17:16.192Z Reads: 77

```
Are you sure? My remote only shows the very top blue light (the low mode light) while charging?
```

---
## \#38 Posted by: mmaner Posted at: 2017-03-14T02:19:51.902Z Reads: 76

```
I have 3...1 from Benchwheel, 1 from MEB and 1 from Alibaba.its the same on all of mine, not saying it couldn't be different, especially if from a different source or manufacturing run.
```

---
## \#39 Posted by: kptheinventor Posted at: 2017-03-14T02:37:09.772Z Reads: 79

```
Haha sorry that might have sounded like I was having a dig at you, I'm just curious how mine is not doing that as it would be nice to see when it's fully charged rather than just assuming it's charged after a certain period.
```

---
## \#40 Posted by: mmaner Posted at: 2017-03-14T02:53:24.830Z Reads: 83

```
No worries.  I don't know why it's different. I charge my 2 diy by plugging them into my computer, my kid uses a Samsung Android phone charger in his actual Benchwheel remote.  The funny this they all have different markings/labels but the same lights. Weird.
```

---
## \#41 Posted by: darkkevind Posted at: 2017-03-14T10:04:05.149Z Reads: 76

```
Same here, mine only shows the very top blue light during charging.
When i turn it on, only the lowest red light is illuminated.

Still can't get this bloody thing to pair though! :frowning:
```

---
## \#42 Posted by: darkkevind Posted at: 2017-03-14T11:17:23.991Z Reads: 78

```
This is what I'm trying...

* Power on remote (do i need to hold the button from this point?)
* Turn on the ESC
* Immediately hold down the white button on the receiver
* After a few seconds remote beeps twice (but nothing has happened)
* Leave for at least 7 seconds, holding down both red and white buttons (nothing happens)
* After a while RX stops flashing blue (nothing still)
* Blue light on TX is still flashing (top light for low speed)

What am I doing wrong? :frowning:
```

---
## \#43 Posted by: Norco Posted at: 2017-03-14T12:24:18.740Z Reads: 77

```
Mine only has the top and bottom lights too. I was under the impression that the middle 3 are for the power left in a benchwheel boards battery.
```

---
## \#44 Posted by: Norco Posted at: 2017-03-14T12:25:27.803Z Reads: 76

```
I would think you'll need to be holding down the button on the remote from the start to get it into bind mode. 

Have you grown 7 extra hands recently?
```

---
## \#45 Posted by: darkkevind Posted at: 2017-03-14T13:37:46.501Z Reads: 72

```
Haha! Exactly! My Dad was round just now so I got him to help with the extra hands, still no luck. I'll make a video to demonstrate...
```

---
## \#46 Posted by: mmaner Posted at: 2017-03-14T13:55:52.715Z Reads: 72

```
Just to be clear...
  1.  When pairing, the step where you turn on the remote means hold the remote button down & do not release until the remote is paired.  
  2.  When I talking about the light on the remotes lighting up from 1 to 5, I mean when the remote is charging.  Like here...  https://www.youtube.com/watch?v=nZlT0WzyyGQ&feature=youtu.be
```

---
## \#47 Posted by: darkkevind Posted at: 2017-03-14T14:09:09.742Z Reads: 74

```
This is how mine looks whilst charging...

[https://www.youtube.com/watch?v=xg2Kzo8M3rY](https://www.youtube.com/watch?v=xg2Kzo8M3rY)
```

---
## \#48 Posted by: mmaner Posted at: 2017-03-14T14:16:37.630Z Reads: 75

```
That is so weird, where did you buy yours?
```

---
## \#49 Posted by: darkkevind Posted at: 2017-03-14T14:17:49.004Z Reads: 76

```
From Benchwheel, AliExpress
```

---
## \#50 Posted by: mmaner Posted at: 2017-03-14T14:19:15.452Z Reads: 77

```
I got one from there & 1 from MEB, they both charge the same.  The one with my kids Benchwheel Dual 1800 does too.  So freekin weird.
```

---
## \#51 Posted by: darkkevind Posted at: 2017-03-14T14:21:42.404Z Reads: 75

```
Here's me trying to pair this thing! I wait for 7 seconds but nothing, although when I release the white button, the flashing light stays solid blue, indicating to me that it's paired, but then the remote keeps flashing...

[https://www.youtube.com/watch?v=tADtx97P-M8](https://www.youtube.com/watch?v=tADtx97P-M8)
```

---
## \#52 Posted by: mmaner Posted at: 2017-03-14T14:48:17.951Z Reads: 72

```
Try powering up the board 1st.  The connect the RX, hole the white button n the RX and power on the remote (while keeping the remote power button depressed, do not release) all within a second or so of each other.  I think I remember someone having that issue and powering on the ESC before hand, for a few seconds let it be fully running, seemed to solve the issue.
```

---
## \#53 Posted by: darkkevind Posted at: 2017-03-14T14:59:06.992Z Reads: 71

```
Thanks.

Still nothing. :frowning:

I've contacted them, one of them must be dud. I saw a video on YT where a guy pairs it to his actual BW board, he gets the first beep (on), then the two beeps that I get and then a third which actually looks like it's signifying the pairing. I don't get that third beep!
```

---
## \#54 Posted by: mmaner Posted at: 2017-03-14T15:07:35.877Z Reads: 71

```
I actually don't get the 3rd beep either, just 2.  But the RX is solid and the remote is solid, so I know its good.  Honestly, I don't think I've ever spent more than 60 seconds pairing one of these remotes.  I'm thinking your RX and remote are mismatched or something.
```

---
## \#55 Posted by: darkkevind Posted at: 2017-03-14T15:08:53.086Z Reads: 71

```
Yeah tell me about it, this is ridiculous!! :frowning:

Hopefully I'll get some joy with Benchwheel
```

---
## \#56 Posted by: darkkevind Posted at: 2017-03-15T11:28:15.824Z Reads: 77

```
Benchwheel have responded. They've seen my video, they agree it's a product fault and are arranging for a replacement...

Let's see if this happens!
```

---
## \#57 Posted by: mmaner Posted at: 2017-03-15T12:00:06.807Z Reads: 77

```
Great, good luck.
```

---
## \#58 Posted by: darkkevind Posted at: 2017-03-16T11:37:35.396Z Reads: 79

```
Turns out they sent me their scooter remote! Not the DIY one.

They're sending me a replacement remote FOC.

Hopefully it won't take forever to arrive...
```

---
## \#59 Posted by: mmaner Posted at: 2017-03-16T12:05:07.517Z Reads: 74

```
That's crazy, glad you got it worked out.
```

---
## \#60 Posted by: darkkevind Posted at: 2017-04-03T10:09:40.701Z Reads: 76

```
I **finally** received my replacement remote from Benchwheel a few days ago, pleased to say that it's now paired and working, just need to get me a new ESC now with decent brakes... Would love a VESC but they're so expensive :frowning:

What do you do about throttle trim for the Benchwheel remote?
```

---
## \#61 Posted by: kptheinventor Posted at: 2017-04-03T10:25:02.101Z Reads: 70

```
That's good to hear, that was sorted out faster than I thought. I haven't tried any esc other than vesc but I can say that the vesc does a very good job and is worth the investment. It gives you such a smooth ride. Although I can't personally compare it to any other esc since I haven't tried any other.
```

---
## \#62 Posted by: mmaner Posted at: 2017-04-03T14:37:35.772Z Reads: 70

```
[quote="darkkevind, post:60, topic:18360"]
What do you do about throttle trim for the Benchwheel remote?
[/quote]

I have never needed it, which is good as its not available on a benchwheel remote :slight_smile:.   If you get a VESC you can tweak the PPM setting in the BLDC tool.
```

---
## \#63 Posted by: darkkevind Posted at: 2017-04-03T14:54:59.848Z Reads: 69

```
Cheers! I hope I won't need it then...

Just ordered a second hand VESC off of a member on here, can't wait to get back on my board, especially now the summer is coming!! :slight_smile:
```

---
## \#64 Posted by: mmaner Posted at: 2017-04-03T14:56:41.202Z Reads: 70

```
I can dig that, I've been without one on occasions and it sucks :slight_smile:.  You can really tweak any remote to being really responsive or slow in th VESC PPM tab,  I usually keep mine pretty tight with very little dead range, but I'm really used to the benchwheel remote.
```

---
## \#65 Posted by: darkkevind Posted at: 2017-04-03T15:00:10.452Z Reads: 75

```
Nice! Looking forward to a really custom setup...
```

---
## \#66 Posted by: jackw Posted at: 2017-05-21T23:04:23.343Z Reads: 63

```
Hey guys. What's the behaviour like on your Benchwheel remotes? I have both the Winning V1 (which for me has been excellent with no problems!) and recently gotten my hands on the Benchwheel for my 2nd build.

I was wondering about yours, because if I compare the two, firstly the Benchwheel seems to have a much bigger dead-zone than the winning, regardless of my settings in the VESC (even down to 0.01MS). A good few millimetres travel from centre on the Benchwheel don't show up as changing the pulse-width in the VESC so I'm assuming thats some kind of slop in the potentiometer.

Secondly, and more annoyingly, the pairing is much worse in my experience. Not the initial pairing as that worked fine once I figured out the correct procedure, but the pairing when you power on the board and the remote. Now, the Winning V1 has been awesome on my first build (and the same if I bring it across to my second build) and super fast and non-fussy (?) when turning on. Doesn't matter which you turn on first or at what time, once they are both on they are connected within a second or two. The Benchwheel on the other hand is super unreliable, sometimes connecting, sometimes not, usually I have to have the board on first before turning on the remote, in which case it sometimes find the remote, and sometimes doesn't, even if i cycle the remote on or off after the board has been turned on, it just won't find it. Do you think I have a dodgy remote/receiver? Or is this normal behaviour with having  to make sure the board is on and then the remote (Quite inconvenient in day to day usage, especially if I'm not even sure if the remote has connected as when the receiver is in the enclosure I can't exactly check the see if the LEDs are blinking on the Rx!)

Sorry for the wall of text, I've become quite obsessed with getting my second build perfect and wanted the benchwheel remote to be a part of that! :P

@mmaner @darkkevind @Norco
```

---
## \#67 Posted by: mmaner Posted at: 2017-05-22T14:12:08.452Z Reads: 64

```
I have noticed a larger dead zone in Benchwheel remotes, as compared to the GT2B and Nano-X, but not significantly so.  If you are using the @Ackmaniac firmware you can use the PPM wizard to negate the dead zone, at least I have been able to.   

As far as binding is concerned, there are a couple of different version of the Benchwheel remote, some use a button on the RX and some don't.  

<img src="/uploads/db1493/original/3X/6/e/6e6ceb8a00916dd7df56a8fe5bbfba192eee9757.JPG" width="690" height="460">
<img src="/uploads/db1493/original/3X/a/a/aaed7eaa06cabee25fbc70b96499acd410959cd5.jpg" width="363" height="500">
```

---
## \#68 Posted by: Norco Posted at: 2017-05-22T14:44:16.556Z Reads: 58

```
Sounds like you might have a suspect unit. Mine has been pretty flawless to be honest. When I first set it up i had some brief sticking of the throttle at max which was weird but once it was properly set up in BLDC then its been spot on since. I have to say I have been impressed and glad I dont have the bulk of the GT2b or hassle of modding it.
```

---
## \#69 Posted by: rok Posted at: 2018-01-11T18:47:49.984Z Reads: 29

```
Hey, do you think that this is/was a reciever problem or remote itself?
```

---
