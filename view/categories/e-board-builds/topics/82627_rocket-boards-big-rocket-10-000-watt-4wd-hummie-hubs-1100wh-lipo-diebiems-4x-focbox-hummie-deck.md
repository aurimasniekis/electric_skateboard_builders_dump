# Rocket Boards - Big Rocket - 10,000 watt 4wd hummie hubs, 1100wh lipo, DieBieMS, 4x focbox, hummie deck

### Replies: 49 Views: 1916

## \#1 Posted by: evoheyax Posted at: 2019-01-30T22:06:36.616Z Reads: 439

```
Finally taking the time to document this build. This build is a combination of everything I've been working towards for the past couple of years. This board came from my last build (deck and motors), but upgraded from chaka 4.12 vesc's to focbox's and from 8Ah to 25Ah and a DieBieMS instead of no bms. Please excuse the dirty grip tape and deck paint imperfections, as I didn't feel like putting another $100 and hours or work to do another fresh deck, just for a perfect look that will be dirty and banged up by rocks in a few days, lol.

![IMG_3315|666x500](upload://4GV73QDGNkGaAKVX7RYgtZxqZp8.jpeg)

![IMG_3597|666x500](upload://2a6LWixyOvy4keoCbkOs4Tsczc1.jpeg)

![IMG-3625|375x500](upload://bo6Ls9DvXZjPybA54QKvYEb7OTt.jpeg) 

**First off, the full specs:**
- 4wd hummie hub motors (all motors are between 80-90kv, 84mm wheels, poured by a&e)
- 12s25ah zippy lipo battery, 1110wh (2x 6s5p 5000 mAh packs, so 10 in total) 
- DieBieMS for the bms
- 4x focbox's (settings are 50 battery amps and 120 motor amps per focbox for a total of 200 battery amps, 480 motor amps)
- Modified hummie deck to create a larger pocket and decrease wheel bite
- @psychotiller enclosure (The Alter Wedge)
-  Metr Pro Bluetooth Module
- 2.4ghz mini trigger
 
**Now onto the story:**

After riding with many of you in Vegas, I realized I needed more range. 4wd hubs are not exactly efficient, especially if you ride the way I ride. I was getting best case 11 miles on 8ah. so at 25ah, I can expect more than 30 miles now. And at worst case, I'll i'm expecting 15 miles, since I was getting in the worst case 5 miles before.

This board is still young. Only about 10 miles put on it, most of which was the Barrett Junction Race. Partly because it started off with a drv issue with 1 of my 4 focbox's, and a canbus issue with my DieBieMS. @barajabali sent me a replacement focbox, which I just received, thank you very much for that btw. And @JTAG offered to fix my bms's. So thank you, again! 

So the goal was long range, charge and forget. But lipos can be very sketchy. I figure it was time to finally bring the DieBieMS into the mix. Thanks to @rpasichnyk's integration into the Metr pro app, I decided to pull the trigger and use one for this build. And to get the full experience, I needed the metr pro module.

I won't bore you with too many details but if you haven't heard of the DieBieMS, you should look it up here on the forum. It has an integrated backlit push button power switch, push to start (which is really nice), oled display for battery charge status, up to 12s, built on top of the vesc firmware (which means with canbus, it will play nice), and you can get individual cell voltages on your smart phone thanks to the metr pro app. You can also adjust a lot of settings, such as min and max voltages to protect the battery, and what voltage balance charging should kick in (very nice). Besides the other normal bms features such as balance charging. What a bms it is...

![IMG_3622|375x500](upload://4pwe8hDXfOo32YZxFGiwMJRQVyj.jpeg) 

![IMG_3623|375x500](upload://thltWr8enJT4fGhHquxBEtDHakJ.jpeg) 

**Back to the battery:**

I didn't want to waste space with the battery, so I looked at how I could maximize battery space not waste space in the enclosure. I did a lot of calculations with about a dozen or so different lipo cells. And this is the cell I came up with this cell sitting sideways as the best option:

https://hobbyking.com/en_us/zippy-compact-5000mah-6s-25c-lipo-pack-xt90.html

I got a steal of a deal as I picked them up as part of the black friday deals. That with an extra 10% off for signing up with hobbykings text messages, meant I only paid $47 per pack, for a total of $470 shipped to my door. That is $0.42 per wh. Not too bad.

With assembly, the idea was to have a neg and a pos in a straight line down the pack's length. Make 1x 6s5p pack, then flip to start putting together the next 6s5p pack in series for get to 12s. I just worked one pack a time, starting by connecting the pos and neg and then connecting the balance leads from one pack to the next.


![IMG_3058|375x500](upload://eWfsSTb4WZdkadOZE2JXRQfFCSa.jpeg) 

![camphoto_342241519|375x500](upload://9emokdBtvCpZfXqV95RihEOhpyw.jpeg)

![IMG_3061|375x500](upload://j9gMSfsLwKzgbWqtXIQ7XUAzP4B.jpeg)

![IMG_3065|375x500](upload://95fE4CJ6urmKkMO87b8t07M97DT.jpeg)

**Electronics plate:**

I wanted a plate I could screw my electronics into so it would be easy to replace things easily if needed. So 3d printed a plate with inserts for small nuts that everything can be screwed into. This plate is then fixed to the board with glue.

![IMG_3577(1)|375x500](upload://6JyiOnkpN3jOKOl7tQO5iirxW51.jpeg) ![IMG_3578|375x500](upload://pi7sbip0mtnfmcggh9U0p0404t6.jpeg) 

**The Ride:**

With a full acceleration, it is incredibly difficult to stay on this board. 0-20mph in under 2 seconds, No hill is too steep for this board. And range anxiety is a thing of the past.

Thanks for checking out my build and I hope this can inspire others to build big, over powered machines of death lol.
```

---
## \#2 Posted by: Sebike Posted at: 2019-01-30T22:09:57.602Z Reads: 351

```
looks like an amazing ride, congrats, man! :star_struck:
```

---
## \#3 Posted by: Mobutusan Posted at: 2019-01-30T22:24:06.337Z Reads: 354

```
Awesome build. Way to come back from your last board. Can't really say if the fate of your previous board was a blessing in disguise, but it did seem to pave the way toward something bigger and better. :+1:

What does that beast weigh in at? Are those new hub motors or were you able to salvage them from before?
```

---
## \#4 Posted by: mishrasubhransu Posted at: 2019-01-30T22:39:28.527Z Reads: 338

```
Looks fantastic and big rocket is the perfect name.

One thing I am concerned about is that the deck might break near the trucks. It's a drop through and you trimmed it further.
```

---
## \#5 Posted by: JTAG Posted at: 2019-01-30T22:41:04.673Z Reads: 324

```
No problem! I am sure we will get it to work with 4 esc's!
```

---
## \#6 Posted by: banjaxxed Posted at: 2019-01-30T23:30:27.546Z Reads: 311

```
Very very nice, must be monster torque
```

---
## \#7 Posted by: mynamesmatt Posted at: 2019-01-30T23:38:21.646Z Reads: 305

```
awesome build. very impressed how you managed to squeeze that many lipos under there along with all your electronics! Well done g, looks damn good
```

---
## \#8 Posted by: Pedrodemio Posted at: 2019-01-31T00:02:40.449Z Reads: 297

```
@evoheyax that’s crazy, the positive crazy

Nice that with the focboxes you can stack them up and still can use all connectors 

The cut on the nose, was it just aesthetically?
```

---
## \#9 Posted by: Riako Posted at: 2019-01-31T01:58:59.380Z Reads: 286

```
Wow, what a big toy !!
And it looks so slim at the same time, well done sir :clap:
```

---
## \#10 Posted by: evoheyax Posted at: 2019-01-31T18:08:37.840Z Reads: 264

```
These motors are the ones from the fire board. The firefighters where tyring to push them into the fire, and I was like "noooooooo!!!!" and saved them. Hummie hubs... fire tested! lol

It's approximately 32 lb. Not as bad as you would think for the power and range.

Battery - 14 lb ($470)
Motors - 12 lb ($800)
Board - 4 lb ($170)
Electronics - 2 lb (~$600)

All in all, just about $2k to build also.
```

---
## \#11 Posted by: evoheyax Posted at: 2019-01-31T18:11:06.287Z Reads: 260

```
[quote="mishrasubhransu, post:4, topic:82627"]
One thing I am concerned about is that the deck might break near the trucks. It’s a drop through and you trimmed it further.
[/quote]

Yes, I am a little bit worried also. My cnc machine didn't cut where I thought it was going to and I had to make the best of it after that lol. It does "roll" a little bit on sharp turns, but only 1 way to find out what will happen... But if it could survive the Barrett Junction road quality, it could survive anything, lol.
```

---
## \#12 Posted by: evoheyax Posted at: 2019-01-31T18:14:12.098Z Reads: 255

```
[quote="Pedrodemio, post:8, topic:82627"]
The cut on the nose, was it just aesthetically?
[/quote]

No, it was originally to eliminate wheel bite that comes from top mounting the trucks. But the battery would bottom out if I top mounted, so I switched to bottom mounted, and now I have the clearance, at the cost of high speed stability. I don't think it was necessary now, but it was with the original plans.
```

---
## \#13 Posted by: rusins Posted at: 2019-01-31T18:45:31.267Z Reads: 246

```
Wait a minute – if all your focboxes are stacked together like that, does that mean you have 6 super long motor phase wires going from one side of the board to the other? I've heard people on this forum advise against that many times due to desync issues, so am wondering how that's playing out for you. 

Awesome build nonetheless! :)
```

---
## \#14 Posted by: evoheyax Posted at: 2019-01-31T18:52:35.690Z Reads: 237

```
I have been riding like this for years with out any issues of de syncing I originally did this because I asked @chaka which was better, long phase wires or long battery wires, and he said long motor wires are better. The long battery wires require more caps inline or you could have the voltage drop out, which I had happen to me before in the past. But never had a motor sync issue with long motor wires.
```

---
## \#15 Posted by: chaka Posted at: 2019-01-31T21:01:29.632Z Reads: 231

```
How do you know you had a voltage issue and not some other fault?

Either way I have never had any issue with motor syncing. They all run independently anyway. Seems like a non issue.

Thanks for letting me ride that beast, if you come out to bakers we should do a small group ride on Saturday!
```

---
## \#16 Posted by: evoheyax Posted at: 2019-01-31T23:49:17.502Z Reads: 237

```
[quote="chaka, post:15, topic:82627"]
How do you know you had a voltage issue and not some other fault?
[/quote]

I was getting jerking at about 10 mph under a full throttle acceleration. I looked at my data log and could see the voltage bouncing around way more than a normal acceleration and triggering a low voltage cutout (I'm guessing that's why it jerked). I added 3 more big caps in line (the ones you used on the 4.12), and the jerking went away and the voltage smoothed out on the graph and no more voltage dips causing low voltage cutouts. So I'm assuming based on all of my observations that the voltage was the issue. I had long battery wires in that case, and that was when I first asked you about it.
```

---
## \#17 Posted by: evoheyax Posted at: 2019-02-20T03:33:39.997Z Reads: 210

```
Just did some acceleration testing. Going slightly up hill, 0-20mph in 1.5 seconds. 0-30mph in just under 3 seconds. I guess technically, starting at 2 mph because from 0, I would cog at full throttle on an uphill. But you get the point.

https://metr.at/r/Sldec
```

---
## \#18 Posted by: Pedrodemio Posted at: 2019-02-20T03:39:37.331Z Reads: 198

```
This is for all Focbox right?
```

---
## \#19 Posted by: mishrasubhransu Posted at: 2019-02-20T03:40:58.251Z Reads: 196

```
So is it for one motor? The ESC that's connected to metr pro? Could you also tell us your VESC config? Motor current, battery current?

So your max current is 93.4A, is that per motor? :open_mouth:
```

---
## \#20 Posted by: evoheyax Posted at: 2019-02-20T03:57:56.937Z Reads: 199

```
No, this is for 2 motors ;)

Can’t get the 4 vesc option to work in the metr pro.

Settings are 50a battery and 120a motor per vesc.

In this case, about 93.5/2 = 46.75a x 47.2 = 2206 watts per motor, so 8824 watts in this acceleration test.
```

---
## \#21 Posted by: Pedrodemio Posted at: 2019-02-20T04:07:48.281Z Reads: 187

```
Damn, please make some videos of that

Or go to a drag strip
```

---
## \#22 Posted by: mishrasubhransu Posted at: 2019-02-20T04:18:51.987Z Reads: 181

```
Very cool! How are the four vescs connected? Canbus?
```

---
## \#23 Posted by: evoheyax Posted at: 2019-02-20T04:33:59.065Z Reads: 179

```
Yes, canbus. 4wd focboxes.
```

---
## \#24 Posted by: pat.speed Posted at: 2019-02-20T05:33:01.330Z Reads: 169

```
I really wanna see a race between you and a car lol
```

---
## \#25 Posted by: evoheyax Posted at: 2019-02-20T05:42:53.730Z Reads: 167

```
Things can be arranged... lol

I’ll be sure to put it through some paces. Hill climbs for sure.
```

---
## \#26 Posted by: PatRocks Posted at: 2019-02-20T07:28:03.488Z Reads: 170

```
So at 187A battery Amps, you're pack is only sagging by 2 volts? Pretty freaking solid, dude 😎
```

---
## \#27 Posted by: sayekim Posted at: 2019-02-20T12:18:50.866Z Reads: 166

```
Which fw version are you using?
```

---
## \#28 Posted by: evoheyax Posted at: 2019-02-20T14:26:14.828Z Reads: 165

```
The new 2019 firmware just released. I can confirm the 3 mph to 0 mph braking is indeed fixed! Thank you @Deodand It’s fm version 3.48
```

---
## \#29 Posted by: evoheyax Posted at: 2019-02-20T14:57:14.683Z Reads: 162

```
Yea, it's pretty crazy. But if you look at the math, 25c rating and 25ah, you get 625 amps. So in theory, I could pull more than 3x that. And combine that with the fact it's a lipo. And voltage sag is a non issue, finally!

Bigger is defiantly better!
```

---
## \#30 Posted by: sayekim Posted at: 2019-02-20T15:13:13.799Z Reads: 155

```
What about before that?
```

---
## \#31 Posted by: evoheyax Posted at: 2019-02-20T15:14:11.583Z Reads: 155

```
I was using 3.39 before.
```

---
## \#32 Posted by: mishrasubhransu Posted at: 2019-02-21T01:33:19.888Z Reads: 154

```
So it's 8824 watts **peak**, because you can see the battery current is ramping up almost linearly as you increase the speed. Impressive numbers. Now, I want to check how well I fare with my dual flipsky 6374. 

@evoheyax, Can you also plot watts vs time. I can obviously calculate it from voltage and current, but would be nice to see it in the same plot.
```

---
## \#33 Posted by: evoheyax Posted at: 2019-02-21T03:08:31.640Z Reads: 161

```
Just went for my best test of the board yet. 6.2 miles uphill, down hill, with stop signs in the avenues, average speed of 19 mph, 31 mph top. Just plowing up hills, way faster than anything I've ever built before. It took me some time to full throttle it from stop, over week of riding tbh. Some cool video is going to be coming from this  board in the near future.


Again, data for only 2 motors:
https://metr.at/r/sSFIy
```

---
## \#34 Posted by: Pedrodemio Posted at: 2019-02-21T03:32:43.695Z Reads: 149

```
Will you add temperature sensors on the motors  at some point? really curious to see how the Hummie's compare to the Ghost
```

---
## \#35 Posted by: evoheyax Posted at: 2019-02-21T04:39:08.588Z Reads: 150

```
Yea I want to stick some in soon.
```

---
## \#36 Posted by: mishrasubhransu Posted at: 2019-02-21T05:09:41.869Z Reads: 147

```
can you plot watts too or is the plot not configurable in metr app?
```

---
## \#37 Posted by: evoheyax Posted at: 2019-02-21T05:28:58.729Z Reads: 149

```
I don’t see any way to adjust it. As far as I know, that is not part of the graph.
```

---
## \#38 Posted by: mishrasubhransu Posted at: 2019-02-21T05:54:53.230Z Reads: 153

```
@rpasichnyk, is there any way to configure the app to log the watts too? battery_volts*battery_current right?
```

---
## \#39 Posted by: Pedrodemio Posted at: 2019-02-21T13:18:43.568Z Reads: 150

```
If you export it to use it Virb to make a video overlay it will calculate watts and show on the video
```

---
## \#40 Posted by: evoheyax Posted at: 2019-03-31T03:00:53.142Z Reads: 136

```
So @MoeStooge and I finally got the hummie hubsnon 3’link turners. The turnablitity is insane.,I have to really fuck up to lose the up coming k1 speed race evolve is hosting.

![image|666x500](upload://4d7g8heOQP4jleU7dU5NQLGHvPf.jpeg) ![image|666x500](upload://lzeUiJHVru6pkRYmokn06Jup9mT.jpeg) ![image|374x500](upload://rSETgTSSoX1fWRP9qDAAe7luDJa.jpeg) ![image|374x500](upload://32wCzzjgIvuV3TIaIVXb3ErLpGj.jpeg) ![image|374x500](upload://ufa3zkCeHXD7Yy50Jy4wWsQfZjQ.jpeg) ![image|374x500](upload://dYjpn5z16he7OdzMxixKAs7X1TU.jpeg)
```

---
## \#41 Posted by: Vanarian Posted at: 2019-03-31T05:23:05.077Z Reads: 128

```
Looks sick. Now I have to ask : which one will be faster?

https://i.imgur.com/3tzqpF7.png

There's serious power in the builds lately.

Tagging @Blasto 🏁
```

---
## \#42 Posted by: topcloud Posted at: 2019-03-31T06:38:07.802Z Reads: 121

```
the one that maintains traction :)
```

---
## \#43 Posted by: topcloud Posted at: 2019-03-31T06:41:06.553Z Reads: 120

```
my favorite build ever posted on this forum; all business, do heart.  10/10
```

---
## \#44 Posted by: Vanarian Posted at: 2019-03-31T07:36:02.489Z Reads: 115

```
Well Hummie & Stooge's nitrile compounds are hard to beat then !
```

---
## \#45 Posted by: pat.speed Posted at: 2019-03-31T08:30:24.457Z Reads: 109

```
The big rocket will easily win, it has far more amps to draw from meaning more torque. It’s just up to whether someone can stay on at full throttle
```

---
## \#46 Posted by: Vanarian Posted at: 2019-03-31T10:06:39.958Z Reads: 107

```
So in the end it's not the board...it's the rider 🔥😏

Still I'd like to see them run head to head haha
```

---
## \#47 Posted by: evoheyax Posted at: 2019-03-31T16:07:43.122Z Reads: 102

```
It took days of practice to get comfortable, but I can now stay on under full acceleration every time.

Bear in mind though that with the default hummie trucks, it was more of a point and go straight acceleration. Now it’s make a sharp u turn and blast out of there acceleration. It’s a lot harder to stay on the 3 link turners, but for something like k1...

I was able to break traction and power slide through sharp turns yesterday in my first tests. So I will need to be careful taking turns too sharply and how I distribute my weight not to tail fish. But with 4wd, tail fishing should be a lot harder.
```

---
## \#48 Posted by: evoheyax Posted at: 2019-03-31T16:10:52.205Z Reads: 100

```
I would love to get more racing going! Working on something for SF.
```

---
## \#49 Posted by: Touch415 Posted at: 2019-03-31T23:45:25.082Z Reads: 94

```
The one with bigger balls wins 🤷🏻‍♂️🤷🏻‍♂️
```

---
