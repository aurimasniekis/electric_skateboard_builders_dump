# FlipSky Dual FSESC4.20 Info/Review

### Replies: 309 Views: 10158

## \#1 Posted by: mmaner Posted at: 2018-10-13T14:05:40.380Z Reads: 734

```
This is my review of the FlipSky Dual FSESC4.20 100A.  This dual ESC is the same price as many other single VESC’s, it's definitely a value.  I am so surprised at how well this ESC performed.  Your not going to build a racing board with it, but for a mid-range ESC it performs above average.  

Before I get into performance, which can vary based on the gear used on abuild I want to list the gear that I used.

    Moonshine Hooch 38in Deck
    97mm ABEC Flywheels
    x2 170kv BLDC Motors
    11/36 Gearing
    10s4p Samsung 30q Battery Pack

I got speeds as high as 27 mph, which is as fast as the gearing allows on this build.  It took some experimenting to find the “sweet spot” in the config to get the most speed &amp; torque while conserving the hardware and battery life.  This is the configuration options I ended up using.

    Motor Current Max : 30A
    Motor Current Max Brake : -30a
    Battery Current Max : 50A
    Battery Current Max Regen : -40A
    Absolute Maximum Current : 120A

I did FOC detection in the beginning, just to make sure it would work, and it did.  I then went back to BLDC as I wanted to get a feel for the ESC’s operation without losing the sound of the motors to get a better feel for performance.  

I have put around 100 miles on this ESC, done much experimentation and its still running strong.  I am about to rebuild this whole board using a different gearing setup and larger wheels to see if I can break 30 mph, I feel confident.

That being said, I did have some issues.  I initially tried to run the Dual FSESC on 12s power, that didn't work.  I experienced intermittent cutouts and reboots.  Once I moved to 10s power and found the sweet spot mor motor amps (30a) I have had no more cutouts.

My recommendation for the FlipSky Dual FSESC4.20 100A is this…

Get one, build a board and see how well it performs...you will be a believer.  As long as you stay within the config specs and aren't building a racing board you will be glad you saved the money.

**VIDEO with METRICS**
https://youtu.be/NK7nLAKV1SA

**METRICS from METR**
https://metr.at/r/YjoEt

**SETTINGS from METR**
https://metr.at/m/vb8l
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-10-13T14:13:56.781Z Reads: 599

```
those settings are for each side correct? how come you set the batt max higher than the motor Max?
(edit: forgot to say good to hear, a mate just bought one @danieloath)
```

---
## \#3 Posted by: Skunk Posted at: 2018-10-13T14:16:40.796Z Reads: 587

```
Good news @J0ker3366 
Thanks for the review mmaner.  Was getting worried the 4.2 was a complete flop
```

---
## \#4 Posted by: brenternet Posted at: 2018-10-13T14:20:53.808Z Reads: 587

```
Contrary to your findings I had quite a lot of trouble with this little esc. Differences in our set up could be the reason.

Dual 170kv 6355. 10s5p 30Q. 190lb when loaded. 107mm wheels and 16/40 gearing.

I used your settings and went up and down a few notches to see if there was a sweet spot for me. Unfortunately the cut outs were rampant and the power delivery on my wheels and gearing was pretty poor.

I've benched this esc for now and will pop it into a flat ground small motor commuter on 8s some time in the future. 

With all that said... I appear to be in the minority of people having trouble on 10s. Perhaps I have a faulty esc? I'm talking to flipsky now about that possibility. Customer service is a challenge.
```

---
## \#5 Posted by: Steven1 Posted at: 2018-10-13T15:03:17.054Z Reads: 546

```
I was wondering when I would see this review here, it was uploaded to the flipsky website first :stuck_out_tongue:

 I've ordered one of these for my 10s4p battery, cause of the good reviews on this site about flipsky fsesc's . I hope I get a good one.
```

---
## \#6 Posted by: mmaner Posted at: 2018-10-13T17:07:19.390Z Reads: 533

```
Yes, both sides. It's not uncommon to use higher battery amps than motor amps, sometimes makes for a smoother ramp up on lighter gearing.
```

---
## \#7 Posted by: mmaner Posted at: 2018-10-13T17:09:29.483Z Reads: 519

```
I wanted to give them the opportunity to see it before I posted it, just trying to be respectful . 
 FlipSky had been great about communication. Sone manufacturer's aren't so I wanted to reward that.
```

---
## \#8 Posted by: BruSkater Posted at: 2018-10-13T17:09:49.284Z Reads: 507

```
Thanks for the review! Now are you running on FOC or BLDC?
```

---
## \#9 Posted by: mmaner Posted at: 2018-10-13T17:10:20.444Z Reads: 497

```
[quote="brenternet, post:4, topic:71079"]
Dual 170kv 6355. 10s5p 30Q. 190lb when loaded. 107mm wheels and 16/40 gearing.
[/quote]

That's pretty aggressive gearing, nothing wrong with that it just might be too much for a mid-range VESC.
```

---
## \#10 Posted by: Benjamin899 Posted at: 2018-10-13T17:38:49.564Z Reads: 478

```
Ok he has less Torque, but as long as he has more conservative setting shouldn't it be ok for the vesc to handle it?
```

---
## \#11 Posted by: mmaner Posted at: 2018-10-13T17:39:42.990Z Reads: 462

```
I would think so, but without actually doing it I could say. New product, new issues, new solutions.
```

---
## \#12 Posted by: Steven1 Posted at: 2018-10-13T19:00:37.134Z Reads: 458

```
Gotcha. Thanks for the review! Can't wait for this thing to arrive.
```

---
## \#13 Posted by: Blitz Posted at: 2018-10-13T19:04:58.645Z Reads: 463

```
IMHO, This ESC reminds me of overtightening soft bushings on say cheap trucks,
They stop the wobbles but just go 4 km/h faster and you have the same issue.

Focboxes run at 13s fine and that's over the rated spec of it
But this dual 4.2 ESC is rated for 12s 100a (50x2) and it has cutouts on 10s 70a (35x2)!

Would you let your wife and or kids go on a board running that esc?
```

---
## \#14 Posted by: ervinelin Posted at: 2018-10-13T19:07:39.074Z Reads: 464

```
I am running one of these.

FOC, 10S, 15/67, 6" pneumatics, 6355 190kvs

I have not stress tested it much yet but so far it has worked fine for me. YMMV
```

---
## \#15 Posted by: mmaner Posted at: 2018-10-13T19:43:47.200Z Reads: 462

```
[quote="Blitz, post:13, topic:71079, full:true"]
Focboxes run at 13s fine and that’s over the rated spec of it
But this dual 4.2 ESC is rated for 12s 100a (50x2) and it has cutouts on 10s 70a (35x2)!
[/quote]

Dude, this is half the price of 2 FocBox's, do you expect foxbox performance?  

[quote="Blitz, post:13, topic:71079"]
Would you let your wife and or kids go on a board running that esc?
[/quote]
 If I built it yes, if you built it no.
```

---
## \#16 Posted by: Benjamin899 Posted at: 2018-10-13T19:45:35.467Z Reads: 448

```
its the perfect commuter esc, cheap and reliable on conservative settings. maybe if they rework their design in the next batches.
```

---
## \#17 Posted by: Blitz Posted at: 2018-10-13T21:11:38.200Z Reads: 446

```
[quote="mmaner, post:15, topic:71079"]
do you expect foxbox performance?
[/quote]

No, But the thing is that the focbox is rated at 12s and has headroom for **safety** reasons.

But here you have an esc that's **Rated** for 12s 100a and has all kinds of faults at that point,
So you go down to 10s still having faults and then try to find that sweet spot with no glitches that could cause a  crash and end your life in some situations.

And at 30a you are like 95% to the point to where failures are totally known and to be predicted.

Bottom line if the components are rated for 12s and it doesn't work with 12s then it's **Faulty** and should be considered unsafe.
```

---
## \#18 Posted by: mtuan293 Posted at: 2018-10-13T21:54:51.198Z Reads: 432

```
Do you get cutouts? I’m running 5055 270kv with 13/35 gearing and FOC still give me cutouts. 10s battery btw.
```

---
## \#19 Posted by: Skunk Posted at: 2018-10-13T22:03:58.754Z Reads: 429

```
Isn't 270kv kinda high for 10s?
```

---
## \#20 Posted by: J0ker3366 Posted at: 2018-10-13T22:04:58.335Z Reads: 432

```
Thats where you went wrong bud. You expected. When you expect something, you're always going to be let down. Think of it like this. We are DIY'ers. We love taking things that aren't up to par and finding that @ different variables they can be par. We build board after board cause we love this ho (Hahaha you though I was going to say it.). We love it though. We love tinckering with things. Yes you can go buy a focbox and never have a concern about it cutting out or what have you. Then again thats what consumers do. But me, a diy'er, I love that I bought a 4.20 and it may not be reliable @ 10s. No worries, I'll build an 8s that will eat pretty much any 10s prebuilt its next to. Its called science and WE LOVE IT!
```

---
## \#22 Posted by: Blitz Posted at: 2018-10-13T22:29:54.847Z Reads: 417

```
esk8ts are no joke man,
A crash at 50km/h Can kill you and a board flying off at 40km/h could easily injure people.

Please just think about it.


@mmaner What do you have to say about what I wrote?
Because as of now you are the main influencer on buying these esc's

@b264 you were debating why 12s on a focbox is bad, any thoughts on this esc?
```

---
## \#23 Posted by: b264 Posted at: 2018-10-13T23:05:16.279Z Reads: 401

```
If it's made with components rated at 60V .... like DRV8302... then I would never run 12S on it.  But that's just me.  I don't like broken things.
```

---
## \#24 Posted by: Blitz Posted at: 2018-10-13T23:08:40.481Z Reads: 394

```
@b264 Did you read into this whole situation?
```

---
## \#25 Posted by: b264 Posted at: 2018-10-13T23:25:08.107Z Reads: 387

```
Yes.  I wouldn't even run 12S on other ESC if they are built with 60V parts.
```

---
## \#26 Posted by: Blitz Posted at: 2018-10-13T23:25:59.360Z Reads: 384

```
@b264 Dude, 

Don't you get that this esc doesn't work reliably on 10s when its rated for 12s!!

The topic here is about the Dual flipsky vesc 4.2.
manners review was like "I was finding the sweet spot on 10s where I won't get lots of faults when I hit the brakes"
```

---
## \#27 Posted by: b264 Posted at: 2018-10-13T23:30:40.223Z Reads: 378

```
Okay&ZeroWidthSpace;
```

---
## \#28 Posted by: mmaner Posted at: 2018-10-13T23:38:33.478Z Reads: 380

```
[quote="Blitz, post:22, topic:71079"]
@mmaner What do you have to say about what I wrote?
[/quote]
I've said what I have to say. I told you under what soecs and conditions I have found that it works, and works well. If you want to use it then use it, if you don't don't.  

I will say this, until you do actually use it you have no business being then voice of disent. 


Regarding it's soecs, it's works at 12s with 25a motor max, but I didn't like it. Regardless the stated soecs are correct. 

It's a mid-rand ESC, it does more than I expected given the cost, so your argument about performance vs. a FocBox is just silly given the cost.
```

---
## \#29 Posted by: mmaner Posted at: 2018-10-13T23:40:34.013Z Reads: 369

```
[quote="Blitz, post:26, topic:71079"]
Don’t you get that this esc doesn’t work reliably on 10s when its rated for 12s!!
[/quote]

Incorrect, not backed up by the facts. 

[quote="Blitz, post:26, topic:71079"]
manners review was like “I was finding the sweet spot on 10s where I won’t get lots of faults when I hit the brakes”
[/quote]
Never said that, not even close. Now your making statement using my name.  That is bullshit, starting to miss me off.
```

---
## \#30 Posted by: Blitz Posted at: 2018-10-13T23:55:54.820Z Reads: 362

```
OK, I was looking into the whole Flipsky thing all day today and got a little tired so I started merging all the messages So sorry for that.


I just saw this

[quote="mmaner, post:24, topic:68940"]
amps is the magic spot
[/quote]

And then a few error posts and I thought that you were telling guys if they make it 30a they won't get all the braking errors.

Not justifying stuff Just saying how that got to my head.

Nice review, If you like you can Screenshot my harsh comments make a joke post in the no words thread and then unclog me from your review post.
```

---
## \#31 Posted by: mmaner Posted at: 2018-10-13T23:57:24.975Z Reads: 353

```
It's not brakes that causes the cut outs, it's to make motor amos. Brakes have no bearing on the discussion.
```

---
## \#32 Posted by: Blitz Posted at: 2018-10-14T00:00:04.481Z Reads: 348

```
Well now, Just imagine theirs someone at the other side of that screen face palming himself for being foolish in his own ways. Live and learn just why don't I learn :frowning:
```

---
## \#33 Posted by: J0ker3366 Posted at: 2018-10-14T02:46:33.386Z Reads: 341

```
Just imagine, a world without idiots. What if, we die tomorrow? But, this and that. @BlitzI don't know how much you know but you clearly are a consumer and the focbox is for you. But still trying to drum up shit as to why the 4.20 is whatever you're calling it. Flipsky is not for consumers of the market. Its for the diy'ers. 

With that said, ill take any more of your banter into the matter as bashing and respond accordingly. As it was said by @mmaner already, until you own one and scienve it the fuck out, shhhhhhhhhhhhhhhhhhh.
```

---
## \#34 Posted by: ervinelin Posted at: 2018-10-14T02:48:42.911Z Reads: 329

```
Nope not at all... What happens when it cuts out?
```

---
## \#35 Posted by: J0ker3366 Posted at: 2018-10-14T02:54:53.899Z Reads: 344

```
[quote="Blitz, post:30, topic:71079"]
If you like you can Screenshot my harsh comments make a joke post in the no words thread and then unclog me from your review post
[/quote]

Or we can do it here. But honestly, all you're doing is looking for attention. Which is fine. But you do it around certain people and you'll play with fire. Youve been warned. DON'T POKE THE BEARS
```

---
## \#36 Posted by: mtuan293 Posted at: 2018-10-14T03:05:25.547Z Reads: 340

```
You lose control of the board - no brake or acceleration. But it’ll reset as soon as you release the throttle. On Ack’s firmware you can still hold the throttle and it automatically resets itself. 

How the heck you don’t have cutouts while literally everyone else has this issue? :thinking:
```

---
## \#37 Posted by: ervinelin Posted at: 2018-10-14T03:23:04.344Z Reads: 341

```
Why would u say "literally everyone else has cutouts" when the OP said his works just fine after he adjusted the settings. I think the main thing is not to run this at 12S.

I have some other buddies building their boards with this, so far no one mentioned about cutouts.
```

---
## \#38 Posted by: mmaner Posted at: 2018-10-14T03:24:32.604Z Reads: 338

```
10s and 30a everything is good.  I'm having a hard time u derstanding the push back on this.
```

---
## \#39 Posted by: ervinelin Posted at: 2018-10-14T03:30:26.715Z Reads: 335

```
Did 10S and >30A on yours give you problems?
```

---
## \#40 Posted by: mmaner Posted at: 2018-10-14T03:32:24.350Z Reads: 337

```
I've out around 100 miles on 10s with 30a motor max and zero cutouts, at 40a motor max I get cutouts when I hit it hard, at 60a cutouts every few seconds.
```

---
## \#41 Posted by: ervinelin Posted at: 2018-10-14T03:33:03.014Z Reads: 344

```
Every few seconds even despite going slow?

I wonder if it's a heat thing. One of my buddies who was monitoring his vesc temp reported exceptionally high temperatures even after a very short ride...
```

---
## \#42 Posted by: mmaner Posted at: 2018-10-14T03:34:15.672Z Reads: 322

```
I don't go incredibly fast but I never go slow. I did real world tests to get real world results.
```

---
## \#43 Posted by: ervinelin Posted at: 2018-10-14T03:43:26.247Z Reads: 321

```
What I mean is... Even slow riding it will cut out? Meaning you are not even drawing high amps to begin with yet it still cuts out.

Just trying to understand what is happening because mine doesn't cut out despite having my motor amps at 65A.
```

---
## \#44 Posted by: mmaner Posted at: 2018-10-14T03:46:44.296Z Reads: 320

```
I'm not sure that I have the data you are looking for. The only time I see 5mph is when I'm accelerating through it.

What pack are you running and what's your battery values?
```

---
## \#45 Posted by: ervinelin Posted at: 2018-10-14T03:51:51.088Z Reads: 316

```
10S2P Sony vtc6. I forgot what I set my battery settings at, will need to check.

I did roll back my vesc to and older firmware because i was having problems with telemetry to my remote. I wonder if that's the difference...
```

---
## \#46 Posted by: mtuan293 Posted at: 2018-10-14T04:15:20.142Z Reads: 319

```
[quote="ervinelin, post:37, topic:71079"]
Why would u say “literally everyone else has cutouts” when the OP said his works just fine after he adjusted the settings. I think the main thing is not to run this at 12S.
[/quote]

Well I have read on the forum several people have had issues with it. OP has to adjust the settings to circumvent the problem. I find myself running at 10s and still have cutouts with FOC, only after switching to BLDC the problem goes away.

So now the million dollar question is, what’s your motor and battery amps settings? You seem to run at 10s and FOC with success.
```

---
## \#47 Posted by: mtuan293 Posted at: 2018-10-14T04:22:20.035Z Reads: 305

```
[quote="mmaner, post:40, topic:71079"]
on 10s with 30a motor max and zero cutouts, at 40a motor max I get cutouts when I hit it hard, at 60a cutouts every few seconds.
[/quote]

Hmm...I set mine to 80/-80 for motor, 20/-5 for battery (10s2p Samsung 20R) with zero success (cutouts a ton) on FOC, however it runs well on BLDC. Tried reducing motor to 60/-60 and it struggled to climb hill so don’t know how it’s gonna be with 30a motor max...
```

---
## \#48 Posted by: DAddYE Posted at: 2018-10-14T04:24:28.325Z Reads: 295

```
I’m pretty pleased with the customer support. I got at this point to 6.6 changed without trouble
```

---
## \#49 Posted by: ervinelin Posted at: 2018-10-14T04:36:12.881Z Reads: 294

```
This is interesting... I have never ever had to tune settings like this for any vesc I have had. I am running these at 65/-40 I think... Battery 30/-15

My only idea is that I rolled back to an older firmware than what came with the dual 4.2...
```

---
## \#50 Posted by: mtuan293 Posted at: 2018-10-14T04:43:39.340Z Reads: 298

```
Where did you get the older firmware version? I use Ack v3.102 and have cutouts as I said above. The 4.20 came with v3.40 if I remember correctly...
```

---
## \#51 Posted by: ervinelin Posted at: 2018-10-14T04:52:35.966Z Reads: 297

```
I wonder if it's a firmware problem instead of. Hardware problem...

I happened to have an older version of vesc tool on my desktop. So I rolled back to that because telemetry for my remote was working with the older firmware.
```

---
## \#52 Posted by: Okami Posted at: 2018-10-21T07:10:34.191Z Reads: 292

```
So does anyone else run it in FOC?

Plan is to use 8s and bump settings a bit from what @mmaner recommended.

BLDC is hella noisy with high kv motors.
```

---
## \#53 Posted by: Jasonkimberson Posted at: 2018-10-21T08:04:50.740Z Reads: 294

```
thanks again for posting your settings and results.  It really helped me out as i was getting those cut outs.  I was originally disappointed in the 30a max on the motors, but even at that setting, while not the fastest board, still performs well going up pretty steep hills on AT wheels.  I do i have a set of 4.12 flipsky vescs.  Was thinking about switching out the dual for those as I hear those do not have the 30a limit problem.
```

---
## \#54 Posted by: ervinelin Posted at: 2018-10-21T08:09:31.269Z Reads: 287

```
I just fired up another deck using these dual 4.20s... FOC 50/-50/30/-15

Went out for a 20km ride just fine... Up and for small hills etc...

No dropouts, no over current warning. Again I rolled back to an older VESC firmware.
```

---
## \#55 Posted by: Jasonkimberson Posted at: 2018-10-21T08:31:33.218Z Reads: 273

```
How did you roll over the firmware?  Can you post a mini tutorial?
```

---
## \#56 Posted by: ervinelin Posted at: 2018-10-21T09:26:22.318Z Reads: 274

```
I happened to have an older version of VESCtool instead of the latest one. When I connected the flipsky up it just said mine was wrong version or outdated version. Flashed it anyway...
```

---
## \#57 Posted by: Flashgod224 Posted at: 2018-10-21T16:06:04.818Z Reads: 277

```
I am running 10s5p, Flipsky's 6354motors, 97mm flywheels and 36/15t ratio on the 4.20 dual (Running FOC)

Sooo I have been getting some cutouts when I hit it hard as well but I noted that it happens when I throttle over hard bumps/cracks on the road. I checked my logs and my Xmatic App, big woop, DRV error only when I hit those bumps. I might take it to the wizard to check it out, I am certainly not sure if changing the DRV out will do any good.

Edit: Running Motor Max 40 Motor min -55 Batt Max 30 Batt Min -18
```

---
## \#58 Posted by: mmaner Posted at: 2018-10-21T18:06:17.376Z Reads: 283

```
Just wanted to let you guys know a couple of things. I've got 250 miles in this board and it's still going strong.   I'm sure there are other settings that work, I look forward to hearing about them. 

It'll be a few days until I have more data, rebuilding in a new deck, hummie deck, yo see if I can resolve my RKP slop issues. The moonshine deck is great but they don't combine with SR RKP trucks very well because they are inset so far. 

I'll update when I know more.
```

---
## \#59 Posted by: briman05 Posted at: 2018-10-21T23:54:48.532Z Reads: 279

```
Are you running single or dual set up.
```

---
## \#60 Posted by: ervinelin Posted at: 2018-10-22T00:07:44.926Z Reads: 282

```
Something loose?
```

---
## \#61 Posted by: Flashgod224 Posted at: 2018-10-22T00:12:10.935Z Reads: 289

```
Nope... My whole set up is tight and as perfect as it gets. I have no loose wires or electronics. I don't even have any wires bending or anything. I honestly do no know whats going on lol. I went for a hill ride today and I got a DRV fault doing a half/full brake down the hill. Had to crash on some bushes and tree branches. Also I had a few cutouts going uphill while hitting cracks in the path.
```

---
## \#62 Posted by: brenternet Posted at: 2018-10-22T00:23:50.236Z Reads: 281

```
People are running this esc successfully on these stats: 

BLDC
Motor Current Max : 30A
Motor Current Max Brake : -30a
Battery Current Max : 50A
Battery Current Max Regen : -40A
Absolute Maximum Current : 120A

This is how the esc works. You are over the settings regardless of when the cutouts happen, especially with FOC. It just wont work.
```

---
## \#63 Posted by: mtuan293 Posted at: 2018-10-22T00:45:00.709Z Reads: 266

```
Dual over can bus
```

---
## \#64 Posted by: ervinelin Posted at: 2018-10-22T01:07:41.268Z Reads: 264

```
This doesn't sound good at all... sounds like it's the same issue as the others who are having cutouts when pushing the board hard...
```

---
## \#65 Posted by: ervinelin Posted at: 2018-10-22T01:08:39.334Z Reads: 259

```
Again, I have 2 boards running these on FOC without cutouts.

But maybe I don't push the ESC as hard as everyone else here, I don't know.

The only difference is I rolled back the VESC firmware to an older version so that my telemetry would work.
```

---
## \#66 Posted by: briman05 Posted at: 2018-10-22T01:20:03.839Z Reads: 258

```
That could be the cause of your issues as you have the kv to high for the battery you should be using those on a 6s-8s build and your motor amps are higher then the 100a it is rated for your current setting can be a total of 160a. So you could be experiencing the issues going up a hill because your motors are not giving you enough torques to get up the hill and you are probably experiencing sag on the pack while going up hills with your setting. I’m actually surprised that you haven’t blown the vesc if you did balls out flat road speed test.
```

---
## \#67 Posted by: briman05 Posted at: 2018-10-22T01:22:59.651Z Reads: 256

```
Thanks @mmaner for doing a well educated test with this vesc and giving a great honest review for people who are on the fence. I have been looking at this or the 6.6 dual.
```

---
## \#68 Posted by: mtuan293 Posted at: 2018-10-22T02:05:42.103Z Reads: 268

```
[quote="briman05, post:66, topic:71079"]
you have the kv to high for the battery you should be using those on a 6s-8s build
[/quote]

Is that the erpm limit of 60k of vesc4? If so, I pulled full throttle no load several times and it reached 70k ish in vesc-tool but nothing happened, so did I damage the vesc?

[quote="briman05, post:66, topic:71079"]
I’m actually surprised that you haven’t blown the vesc if you did balls out flat road speed test.
[/quote]
Well I haven’t pulled full throttle on the road yet...mostly riding at 25km/h (15mph)
```

---
## \#69 Posted by: mmaner Posted at: 2018-10-22T02:08:42.999Z Reads: 255

```
Bench testing the easiest way to mess up a vesc. Easy throttle, just to make sure it moves, then button it up get on it and ride to test.
```

---
## \#70 Posted by: mtuan293 Posted at: 2018-10-22T02:20:53.181Z Reads: 261

```
[quote="ervinelin, post:54, topic:71079, full:true"]
I just fired up another deck using these dual 4.20s… FOC 50/-50/30/-15

Went out for a 20km ride just fine… Up and for small hills etc…

No dropouts, no over current warning. Again I rolled back to an older VESC firmware.
[/quote]
Are those current settings for each of the vesc, or both of them combined? You said you use sony vtc6 in 10s2p and it has 15A max discharge per cell, so I assume you’d set 15A for each of the vesc?
What firmware version did you roll back to?
```

---
## \#71 Posted by: briman05 Posted at: 2018-10-22T02:36:24.215Z Reads: 245

```
Those values should be per vesc basically if you have a single you would do everything how yours is set up for dual you cut it in half
```

---
## \#72 Posted by: ervinelin Posted at: 2018-10-22T04:39:29.714Z Reads: 238

```
It's actually per vesc... Let me check firmware version when I am back...
```

---
## \#73 Posted by: mtuan293 Posted at: 2018-10-22T05:29:05.353Z Reads: 243

```
So I use samsung 20R in 2p, I set 20/-5 each VESC, seems about right right?
```

---
## \#74 Posted by: briman05 Posted at: 2018-10-22T11:29:43.286Z Reads: 249

```
The battery is set up right but the motor is not.
```

---
## \#75 Posted by: finges Posted at: 2018-10-22T16:07:24.627Z Reads: 263

```
I purchased a Flipsky Dual 4.2 last Friday.. Got the following email last night... It seems they know about the issues and are warning purchasers...

> Dear customers
> 
> Thanks for order our dual FSESC4.20, Just kindly reminder that:
> 
> Due to two phase design, the ESC has strict requirement on parameter setting. If not match well, it will cause over-current cut off during hard brake or hard accelerate for about 0.2s, but after 0.2s it will recover the power.
> 
> Pls cautiously consider your order. In order to avoid any after-sale service trouble to you, we’ll wait for your final decision reply to ship or not!
> 
>  Here’s our suggestion for the setting , it’s verified no such problem in this setting.
> 
> 10S battery
> Motor Current Max: 30A
> Motor Current Max Brake: -25A
> Absolute Max Current: 130.00A
> Slow ABS Current Limit: True
> 
> Battery Current Max: 30A
> Battery Current Max Regen: -25A
> 
> DRV8301 OC Mode: Current Limit
> DRV8301 OC Adjustment: 16
```

---
## \#76 Posted by: Okami Posted at: 2018-10-22T16:50:53.642Z Reads: 247

```
Hm battery max 30A really seems on low side..

Though it is still better than car escs, for example  :D
```

---
## \#77 Posted by: visnu777 Posted at: 2018-10-22T17:01:26.171Z Reads: 258

```
Its been said more than once in this thread but go for the FSESC 4.12. I'm using them now for some time (at least 500km) without any failures at 10s and up to 45A/-10 battery and 50A/-50 motor in a dual setup without any issues. I even build me a 2s booster pack going 12s without problems (I can't tell that for long term usage since 12s is too much for me, my board goes 61kph with that :D, I'll use it limited to 50kph for battery extension) You can get them for 50€ at ebay including shipping ;)
```

---
## \#78 Posted by: briman05 Posted at: 2018-10-22T17:18:38.977Z Reads: 267

```
I feel like it is user error that have been the cause of some of the issues as not being set up properly @mmaner knows how to set up a board to get the most out of it and I feel like there can be a few faulty units but I think it is mostly user error as these seem as a very good alternative I would really like to try out the 6.6 dual.
```

---
## \#79 Posted by: Benjamin899 Posted at: 2018-10-22T17:18:40.145Z Reads: 277

```
last time i check i saw them for 30€ but 20€ shipping.
```

---
## \#80 Posted by: Elitejarcool Posted at: 2018-10-23T11:24:25.441Z Reads: 299

```
Hey, Just did a small review on the FLIPSKY Dual 4.2 VESC, if you are interested in checking it out the link is at the bottom
Just wanted too put it out there with a few of my own words, for a dual 4.2 vesc its defiantly been a great product to use and l will tell you my pros and cons

Pros: 
- Dual means that I didn't have to stuff around truing to housing to separated items and link them, they came linked and stayed as 1 block and was easy just to put it into my housing as such
- There Cheap (~$230 AUD), that is still a lot but its pretty much the price for 1 Focbox, so defiantly a bonus there
- shipping was less than a week with DHL Express

Cons:
- Currently has issues with 12s configuration (from what lam told)
- if you loose one side then you pretty much loose the whole vesc as it cont be replaced if they were separated

Personal l didn't have any issues with setting it up and haven't had any since, did what l need it to do and still dose :slight_smile:

https://www.youtube.com/watch?v=czCqP4zVTWE&t=12s
```

---
## \#81 Posted by: LEE Posted at: 2018-10-23T12:25:21.996Z Reads: 300

```
I am using FSESC 4.20 in CARVON EXO.
Cutoff occurred at motor -35A.
Cutoff occurred frequently at -50A.
Now I am trying at -32A.
There is no particular problem in others.
```

---
## \#82 Posted by: walleywalker Posted at: 2018-10-24T17:50:45.019Z Reads: 292

```
You're running 12s lifepo4 cells which equates to ~10s of a lipo pack for voltage, right?  Have you run into any cut-outs with this setup? I want to run a 12S2P Lifepo4 A123 setup on the 4.20. Ideally with FOC. Have you tried FOC or only run BLDC?
```

---
## \#83 Posted by: Elitejarcool Posted at: 2018-10-24T18:05:55.703Z Reads: 288

```
Hey yes correct, lam running 12s1p A123 lifepo4, voltage is 43.8v which is close enought to just say 42v of a liion 10s pack, l have not expericned any cut out issues with it, when l frist tested it it did cut out but was because of my own mistake and me not setting the cut off limits lol, l did do a foc detection on the motors l have and was able to get the paramters but it was my frist time using VESC properly so l stuck with BLDC, l might test FOC in soon but for my current purpose l dont need it, but l dont see any reason it wouldnt work
```

---
## \#84 Posted by: ervinelin Posted at: 2018-10-25T07:22:26.781Z Reads: 281

```
I am running FW version 3.38 using VESCtool 0.94 for both my dual 4.20 VESC setups... Have not experienced cutouts thus far... I tried pushing the throttle as I did a hill climb, nothing unexpected either.. But that said I'm not a speed demon, just regular mortal speeds for me...
```

---
## \#85 Posted by: Jasonkimberson Posted at: 2018-10-25T07:53:05.120Z Reads: 270

```
One of my USB ports came off on the 4.20 ☹️
```

---
## \#86 Posted by: hiboute Posted at: 2018-10-25T07:59:59.759Z Reads: 269

```
I have the same issue on two fsesc 6.6. I’ve reported it to Flipsky.
I now only configure using the metr pro bluettoth adapter.
```

---
## \#87 Posted by: nuttyjeff Posted at: 2018-10-25T08:01:57.385Z Reads: 265

```
Yeah, had the usb pop out of my dual 6.6 too.
```

---
## \#88 Posted by: Jasonkimberson Posted at: 2018-10-25T08:08:38.681Z Reads: 265

```
How do you change to foc or bldc?  And how do you run motor detection?
```

---
## \#89 Posted by: hiboute Posted at: 2018-10-25T08:29:32.122Z Reads: 266

```
Using the metr pro module, i use the TCP bridge connection.
![image|230x500](upload://kj4kkiIjUplTw9iC8sYZj3ewWo7.jpeg)
```

---
## \#90 Posted by: mtuan293 Posted at: 2018-10-25T09:17:34.143Z Reads: 253

```
Can you do a quick run-down of your setup (motors, battery, amps setting, etc.) again? I lost track lol.
```

---
## \#91 Posted by: brenternet Posted at: 2018-10-25T09:23:07.749Z Reads: 259

```
100% agree. If you have the space use the 4.12s. Cheaper, allows for redundancy and 30-50% more powwwaaaaaaa
```

---
## \#92 Posted by: ervinelin Posted at: 2018-10-25T13:47:18.595Z Reads: 259

```
6" Wheels, 6354 190kv, 16/71 ratio, 65/-64/30/-15
97mm wheels, 5065 200kv, 15/41 ratio, 50/-50/30/-15
```

---
## \#93 Posted by: Chrisfl Posted at: 2018-10-25T17:42:26.895Z Reads: 254

```
When you say 30A max for motors do you mean 30A per motor or 15A per motor for a total of 30A for the entire board? 15A per motor seems kinda low, right?
```

---
## \#94 Posted by: mtuan293 Posted at: 2018-10-25T17:54:47.468Z Reads: 254

```
FOC right? I have cutout with FOC but it’s fine with BLDC
```

---
## \#95 Posted by: spesh Posted at: 2018-10-25T23:00:20.459Z Reads: 252

```
Oddly my 4.2 duel wont run sensored BLDC on one side but runs sensored FOC (on the bench) fine.  In BLDC it just cogs up the motor and hits maxabs.  Runs fine in sensorless BLDC too.
```

---
## \#96 Posted by: ervinelin Posted at: 2018-10-25T23:49:32.040Z Reads: 247

```
That's right, FOC. No cutouts thus far for me... Oh yes sensorless...
```

---
## \#97 Posted by: Jake2k17 Posted at: 2018-10-25T23:49:52.928Z Reads: 257

```
I already have one Torqueboards Vesc, should l get another TB Vesc for dual or just grab a dual 4.2? I have a 10s setup
```

---
## \#98 Posted by: spesh Posted at: 2018-10-26T06:56:39.563Z Reads: 259

```
I think the general consensus is that the 4.2 isn't as good as the 4.12 due to limited ability to deal with high amp draw
```

---
## \#99 Posted by: rynor Posted at: 2018-11-02T01:37:15.210Z Reads: 252

```
So its an issue with the hardware version? All 4.12 vsec layouts have less issues than say all 4.20 vsec layouts?
```

---
## \#100 Posted by: rynor Posted at: 2018-11-03T06:29:50.607Z Reads: 255

```
Just re-read the FAQ.

[quote="evoheyax, post:1, topic:2980"]
## **Variations of VESCs**

They’re are many different VESC’s on the market, and none of which are equal. Few actually use vedders BOM to the tee anymore, creating their own mods to increase stability. So buying a VESC 4.12 from one vendor is not the same VESC 4.12 of another vendor.
[/quote]
```

---
## \#101 Posted by: Pmac Posted at: 2018-11-12T06:44:54.693Z Reads: 266

```
I had cutouts at 40 motor amps per side but at 38 motor amps per side i get no more cut outs (tested by increments from 30 amps up).

I am running 9s in FOC sensorless.  2x 260kv motor with 12/40 pulleys and 83mm wheels.

Current setup is motor: 38, -30 battery: 38, -8.  The brakes are good enough to come to a complete stop going down a pretty steep hill.

I haven't tried BLDC mode yet.  I may have to, if people are having more luck with it as I need more power to get up hills as with full riding gear I am 240 pounds.

@ervinelin are you running BLDC or FOC?  Have you gone full throttle as that is when I got my cut outs.  It was never just cruising around.  It was when I asked for as much as possible from the ESC.
```

---
## \#102 Posted by: ervinelin Posted at: 2018-11-12T13:34:36.315Z Reads: 253

```
FOC... But no I have never gone full throttle yet... Again my testing has been more cruising... But people seem to have cutouts even at lower throttles?
```

---
## \#103 Posted by: mutantbass Posted at: 2018-11-12T13:35:42.813Z Reads: 247

```
guys. is FOC able to give smooth roll off from stationary on sensorless motors?
```

---
## \#104 Posted by: Linny Posted at: 2018-11-12T13:38:16.448Z Reads: 247

```
Unfortunately no, there will be some cogging still. Not as bad as BLDC however.
```

---
## \#105 Posted by: BruSkater Posted at: 2018-11-12T16:55:56.757Z Reads: 241

```
Just to make sure, you have 38 bat max on each esc or total (19+19)?
```

---
## \#106 Posted by: walleywalker Posted at: 2018-11-12T17:03:26.772Z Reads: 234

```
Does anyone know if Flipsky is trying to right this clearly incorrectly advertised product?  I understand it's an inexpensive alternative to the 6.6 and the Unity - But it's being advertised as something that it's not. 

Has anyone messed with upgrading the caps to see if it resolves some of the cut-off issues?
```

---
## \#107 Posted by: mmaner Posted at: 2018-11-12T17:06:07.707Z Reads: 229

```
[quote="walleywalker, post:106, topic:71079"]
clearly incorrectly advertised product
[/quote]

It's not incorrectly advertised, it definitely supports up to 50a per motor (battery amps).  

I really dont get why so many people are down on this.  Its literally the cheapest dual VESC available, yet people expect it work like a FocBox.  If you want FocBox performance, then buy a FoxBox.
```

---
## \#108 Posted by: walleywalker Posted at: 2018-11-12T17:12:22.190Z Reads: 225

```
It seems wrongly advertised to me with the up to 60v compatibility while simultaneously stating 50a continuous. I'm not saying I expect it to be a Focbox or Flipsky 6.6, but it seems this box doesn't like to run much above 38a at 9-10s. 

I'm just saying I think they should change their claimed specs, leave the price.
```

---
## \#109 Posted by: mtuan293 Posted at: 2018-11-13T00:24:24.599Z Reads: 225

```
[quote="walleywalker, post:106, topic:71079"]
upgrading the caps to see if it resolves some of the cut-off issues?
[/quote]

The caps on this 4.20 are the same as their single 6.6. People have been saying good things about the 6.6. Their single 4.12 is good too. So not sure what they changed to make this dual 4.20...
```

---
## \#110 Posted by: Pmac Posted at: 2018-11-13T04:41:44.507Z Reads: 223

```
@BruSkater

Yep.  all settings are for each motor.
```

---
## \#111 Posted by: Pmac Posted at: 2018-11-13T04:46:29.782Z Reads: 228

```
@mtuan293

The caps are very different.

6x 220uF on the 4.2 and 6x 470uF on the 6.6.

The single 4.12 has 3x 680uF so has more than the total of the dual 4.2 on a single.

I should clarify that I have added 4x 470uF capacitors close to the FSESC as the negative battery cable is quite lengthy in my setup.  runs nearly the completed length of the wheel base.

I have not tested whether the board acts differently with less capacitors at 38 amps.
```

---
## \#112 Posted by: Pmac Posted at: 2018-11-13T05:01:06.106Z Reads: 230

```
@mutantbass

My experience is that BLDC needs a push to start but FOC stutters slightly and then starts moving.

But I am 240 pounds and when my brother who is closer to 180 pounds rode the board with my old setup of a single 4.12 in BLDC he was able to get the board moving from a complete stand still with no cogging at all.

so weight is a huge factor.

I know adding sensors will make it a hell of a lot smoother but have not had a chance to use sensored motors as yet.  although I have 2 here waiting on my next build.
```

---
## \#113 Posted by: mtuan293 Posted at: 2018-11-13T08:22:30.838Z Reads: 239

```
I'm talking about this:

Continuing the discussion from [Flipsky 4.20 DRV8302 error, but still working?](https://www.electric-skateboard.builders/t/flipsky-4-20-drv8302-error-but-still-working/68812/11):

[quote="mtuan293, post:11, topic:68812"]
I noticed this…both their dual 4.20 and single 6.6 use the same 220μF 100V caps. People have been saying good things about the 6.6, while the 4.20 has cutout issues. Why is this? @Kug3lis any explanations?

single 6.6 on their website

![image|686x500](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/b/1/b16fb7b1edde5952ce42e186ee57ed10a10dac60_1_686x500.jpeg)


dual 4.20

![image|686x500](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/7/d/7d01cdcb2e5088453c8317a6d498287b1720ffdb_1_686x500.jpeg)
[/quote]
```

---
## \#114 Posted by: Pmac Posted at: 2018-11-13T10:01:23.431Z Reads: 231

```
i didn't realise the single one only had the 220uF capacitors.
```

---
## \#115 Posted by: LukePL Posted at: 2018-12-03T12:43:28.392Z Reads: 235

```
A new one.
https://flipsky.net/collections/electronic-products/products/dual-fsesc4-20-100a-plus-based-on-vesc-with-anodized-aluminum-heatsink

I hope they made it better and not only add antispark.... 
@mmaner any chance you will get it for tests from them?
```

---
## \#116 Posted by: mmaner Posted at: 2018-12-03T13:00:01.092Z Reads: 230

```
I kind of doubt it, they like to spred the love 😀.
```

---
## \#117 Posted by: LukePL Posted at: 2018-12-03T13:04:01.939Z Reads: 236

```
Hehehehehe they should :) You gave them good review and they are using it on their website. 
They shouldn't expect that some one will order it for science. @BarbaraZ are you the right person to make it happen?
```

---
## \#118 Posted by: Riako Posted at: 2018-12-03T13:21:57.068Z Reads: 234

```
when I see the new character down I hope it does not FAULTS anymore...
```

---
## \#119 Posted by: Pmac Posted at: 2018-12-04T05:19:34.142Z Reads: 234

```
I would be slightly worried they went from 1,320uF capacitance down to 880uF so they could fit the anti-spark switch.

A single 4.12 VESC has 2,040uF.  Wouldn't such a reduction add a lot more noise and make it more unreliable?
```

---
## \#120 Posted by: mmaner Posted at: 2018-12-04T05:20:55.925Z Reads: 229

```
At 10s 60a it should fine. Just remember these are mid-range speed controllers, they aren't high performance. Cruisers only.
```

---
## \#122 Posted by: rollinsoul Posted at: 2018-12-09T13:22:27.530Z Reads: 234

```
Hi Noob here, I'm waiting for mine to arrive. Questions, is the rf receiver for the remote built on to the board or will I have to buy a flipsky remote with chip?  Or can I just buy the receiver chip by itself as I have a couple of those remotes from my wowgo/ meepo days. 
Lastly what size jst connectors are used for the hall sensors, number pins and pitch etc? Want to connect esc to wowgo hubs. 
Thanks
```

---
## \#123 Posted by: mmaner Posted at: 2018-12-09T14:17:11.259Z Reads: 229

```
No, you will have to supply a remote and RX. The hall sensor are standard, JST 2.0. I believe.
```

---
## \#124 Posted by: rollinsoul Posted at: 2018-12-09T18:52:08.363Z Reads: 226

```
Thanks for getting back. So my only option is to buy the flipsky remote that comes with the rf module? I was hoping to avoid buying direct to China as cost and import charges to UK seem pricey. Do you know if the remote and rf be picked up in the EU?
```

---
## \#125 Posted by: mmaner Posted at: 2018-12-09T19:22:55.078Z Reads: 224

```
You can use any remote. If you want an inexpensive remote, talk to @JLabs or @thisguyhere. If you want a great remote look at the Hoyt Puck.
```

---
## \#126 Posted by: rollinsoul Posted at: 2018-12-10T15:54:56.264Z Reads: 219

```
Thanks again. Though remotes aren't the problem. I have a few, it's that I just want the rf reciever only.
Lastly do I have to buy an anti spark switch to power the vesc on and off? Excuse my ignorance this is my first build and I'm coming from a wowgo board where everything is already on the esc
```

---
## \#127 Posted by: mmaner Posted at: 2018-12-10T16:03:57.655Z Reads: 214

```
Yes, there is no power switch on the ESC itself.
```

---
## \#128 Posted by: rollinsoul Posted at: 2018-12-10T16:34:51.851Z Reads: 219

```
So I have to buy an anti spark switch then
```

---
## \#129 Posted by: J0ker3366 Posted at: 2018-12-10T16:38:21.087Z Reads: 217

```
No. You can always run a loop key. Its too early to explain shit so if you're unaware what an xt90s loop key is, I suggest using Google lol.
```

---
## \#130 Posted by: brenternet Posted at: 2018-12-10T16:57:07.995Z Reads: 212

```
I would suggest familiarizing yourself with the faq posts here on the forum before you get  building.  It'll save you a lot of expense and time.
```

---
## \#131 Posted by: rollinsoul Posted at: 2018-12-10T17:05:00.274Z Reads: 211

```
Thanks I will I didn't know it existed.
```

---
## \#132 Posted by: Mazda_bater Posted at: 2018-12-11T21:32:26.243Z Reads: 212

```
I've bought one of these and been trying to find a setup that works reliably. im too much of a fraidy cat to be hitting warp speeds but I just don't want to have it cutting out on braking or acceleration. 
I'm running sensored foc and it's fantastic to roll around the flats around my place with just one gentle slope between me and the beach but it's cut out going up and down the slope. My specs are straight from flipskys recommendations![IMG_1969|315x282](upload://1mgAz8f7PHUL4QOhPE7D2uOuuTZ.jpeg)
```

---
## \#133 Posted by: mmaner Posted at: 2018-12-11T21:38:22.343Z Reads: 205

```
are you running a bluetooth dongle so you can get telemetry?  It might be the break regen that is causing your cutouts.  I run mine at a max of -20a.  I would lower it to -20 and see if it goes away.  If not you may have  a defective cap.
```

---
## \#134 Posted by: Mazda_bater Posted at: 2018-12-11T21:41:29.210Z Reads: 198

```
Are you running yours in bldc mode? Maybe that's what I should try. I've no issue with swapping out all the caps if it solves my issues
```

---
## \#135 Posted by: mmaner Posted at: 2018-12-11T21:57:04.526Z Reads: 196

```
I am using BLDC.  I honestly don't mind it and with a tuned startup boost it rides as good as FOC.
```

---
## \#136 Posted by: sayekim Posted at: 2018-12-11T22:04:50.282Z Reads: 202

```
10s too?

I ran them on 12s on 30amps and got cut outs sporadically with max throttle and brake. 

I’d try 25amps or like mmaner says 20amps
```

---
## \#137 Posted by: Mazda_bater Posted at: 2018-12-12T03:13:08.555Z Reads: 199

```
Yeah I'm 10s2p battery dual hub motors.
```

---
## \#138 Posted by: mmaner Posted at: 2018-12-12T04:07:35.385Z Reads: 203

```
13s was too much in my experience. I've got a dual plus coming, I hope it's better on 12s.
```

---
## \#139 Posted by: J0ker3366 Posted at: 2018-12-12T04:25:23.193Z Reads: 201

```
@mmaner, thoughts please sir. I'll be running 8s with the dual 4.20. What would be your thoughts on running higher motor max @ 8s and cutouts?
```

---
## \#140 Posted by: Pmac Posted at: 2018-12-12T05:16:34.619Z Reads: 200

```
I run one on 9s in FOC and run it at 38, -30 motor and 38, -12 on battery per side.  No cut outs.

I am running 4 more capacitors at 470uF each though so that may be helping.  But i never tested it without them and i'm not going to pull the board apart to test without them.
```

---
## \#141 Posted by: ervinelin Posted at: 2018-12-12T06:15:28.247Z Reads: 200

```
So last night I upgraded back to the latest VESC firmware (the desktop tool version is 0.95 instead of 0.94) and the smallest hill I went up I got cut offs.

This is interesting... My 0.94 firmware never had these cutouts!! 

50A/-50A on both firmwares... Only the latest one spazed out... (Latest firmware comes stock in the dual flipsky>

Can someone else please confirm my findings...
```

---
## \#142 Posted by: finges Posted at: 2018-12-12T06:17:39.339Z Reads: 197

```
I down graded to .94... currently running 50/-50 without cutting out going up a pretty decent hill. Looking for the .94 android APK so I can monitor for faults
```

---
## \#143 Posted by: ervinelin Posted at: 2018-12-12T06:38:26.221Z Reads: 200

```
Great... So it's not just me then.  I too upgraded so my BT module would work. But now I get cutouts.    Grumble
```

---
## \#144 Posted by: Mazda_bater Posted at: 2018-12-12T08:29:49.302Z Reads: 196

```
Can you give me a link to the older version of the vesc tool, is really like to try it out. It's really good on sensored foc when it's not cutting out. I'm going home to change to bldc and 25a
```

---
## \#145 Posted by: ervinelin Posted at: 2018-12-12T12:36:09.780Z Reads: 192

```
Hmm... I think it's not online anymore...
```

---
## \#146 Posted by: mmaner Posted at: 2018-12-12T12:45:12.641Z Reads: 193

```
I don't know, seems like the lower voltage would be optimal, buy I worry about a lot if amps.
```

---
## \#147 Posted by: Mazda_bater Posted at: 2018-12-12T16:03:03.333Z Reads: 195

```
If it's not online and you have a copy could you possibly add it to a Dropbox and share a link. 
Has anyone tried to see if ackmaniac esc tool or different firmware from his setup has the same results?
I've changed the board to 25a in bldc mode and wanted to take it out last night but it started raining.
```

---
## \#148 Posted by: mmaner Posted at: 2018-12-12T16:12:29.213Z Reads: 190

```
I'm running ackimaniac 2.54 on mone, I had some odd issue with 3.102.  I have a dual plus coming.  I'm going to try it with stock 3.4 1st and see if I get better results.
```

---
## \#149 Posted by: finges Posted at: 2018-12-15T00:45:08.415Z Reads: 200

```
So I downgraded to .94.... ran it at 50/-50 motor 30/-10 battery.... faulted on a 20% grade at 90% throttle. No other faults outside of that. 

210 lbs
10s4p Samsung 20r/dual Flipsky 6354

![Screenshot_20181214-155657|243x500](upload://2qlTPLh4jThYcr55SZQ61zJOFhl.jpeg)
```

---
## \#150 Posted by: ervinelin Posted at: 2018-12-15T07:53:07.468Z Reads: 192

```
Does this fault case a drop out?
```

---
## \#151 Posted by: finges Posted at: 2018-12-15T08:00:19.273Z Reads: 194

```
Yep.. I was feeling pretty good going up the hill at almost max throttle... then the board lost all power and almost threw me.
```

---
## \#152 Posted by: ervinelin Posted at: 2018-12-15T08:05:16.339Z Reads: 194

```
This fault sounds different from the one using 0.95.. could it be an ERPM maximum issue?
```

---
## \#153 Posted by: finges Posted at: 2018-12-15T08:26:15.391Z Reads: 200

```
Dont think so? 10s at 190kv.. puts me at less than 50k erpm max for the motor right?
```

---
## \#154 Posted by: Benjamin899 Posted at: 2018-12-15T13:29:53.707Z Reads: 198

```
yes you are totally save regarding the erpm.
```

---
## \#155 Posted by: Mazda_bater Posted at: 2018-12-16T20:50:59.653Z Reads: 192

```
I downgraded to the vesc tool_94 and 3.38 firmware on the flipsky recommended specs running sensored foc I managed a ride without cut outs still just running 30a per vesc but the gentle slope I had problems with before was now acceptable. I'd like to make hardware changes to get past the issues and be able to run with the default firmware
```

---
## \#156 Posted by: DeathCookies Posted at: 2018-12-17T00:31:23.805Z Reads: 185

```
Did you try @Ackmaniac Firmware yet?
```

---
## \#157 Posted by: Mazda_bater Posted at: 2018-12-17T09:23:28.477Z Reads: 190

```
Not yet, can I run the equivalent 3.38 firmware from ackmaniac?
```

---
## \#158 Posted by: mtuan293 Posted at: 2018-12-17T09:56:06.904Z Reads: 194

```
Guys...let’s be done with it. This 4.20 dual has a flaw in design causing cutouts. I’ve tried vesc tool 0.94, 0.95, acks 3.102 and all have the same result: cutout in FOC while working well in BLDC.
```

---
## \#159 Posted by: ervinelin Posted at: 2018-12-17T12:29:49.418Z Reads: 193

```
At what motor currrent
```

---
## \#160 Posted by: mtuan293 Posted at: 2018-12-17T17:08:27.715Z Reads: 188

```
60/-60. Tried mmaner settings, but it’s too slow to be usable.
```

---
## \#161 Posted by: finges Posted at: 2018-12-17T17:43:09.783Z Reads: 189

```
You got 60/-60 to work in bldc?
```

---
## \#162 Posted by: Mazda_bater Posted at: 2018-12-17T18:13:30.303Z Reads: 188

```
Have you tried 50/-50
```

---
## \#163 Posted by: mmaner Posted at: 2018-12-17T18:13:58.562Z Reads: 196

```
[quote="mtuan293, post:158, topic:71079"]
Guys…let’s be done with it. This 4.20 dual has a flaw in design causing cutouts.
[/quote]

Then every VESCever made has the same flaw, a flaw that only seems to be present when you reach over amperage conditions.

[quote="mtuan293, post:160, topic:71079, full:true"]
60/-60. Tried mmaner settings, but it’s too slow to be usable.
[/quote]

Then try a better VESC.  This VESC is inexpensive and made for cruising, not speed runs.  

Let me break it down so it's simple.  This is a cheap VESC made for cheap boards.  You don't/can't go fast on cheap boards.  If you wanna go fast, get a better VESC.

[quote="mtuan293, post:160, topic:71079, full:true"]
60/-60. Tried mmaner settings, but it’s too slow to be usable.
[/quote]

As it's spec'd to only do 50a per side, 60a is probably not gonna work.  Get a Unity or a couple of FocBox's if you wanna run 60a per motor, that's what they are built for.  This is not built for that.
```

---
## \#164 Posted by: mtuan293 Posted at: 2018-12-17T18:19:50.975Z Reads: 183

```
[quote="mmaner, post:163, topic:71079"]
As it’s spec’d to only do 50a per side, 60a is probably not gonna work.
[/quote]

I thought that’s input/battery amps and not output/motor amps?
```

---
## \#165 Posted by: Deodand Posted at: 2018-12-17T18:21:26.006Z Reads: 190

```
[quote="mmaner, post:163, topic:71079"]
Then every VESCever made has the same flaw, a flaw that only seems to be present when you reach over amperage conditions.
[/quote]

The main reason I don't agree with this statement is just the way the fault is occuring. I agree this is a lower power vesc and people shouldn't expect the same performance, but when you put it under loading that is beyond what it could handle it should just run up against its thermal limts and throttle down. That is what the 4.12 design would have done. Instead it cuts power on you and throws faults, indicating that something in the design is poorly laid out. 

Not saying it isn't still useful as is, but it is a bit scary that the design seems somewhat flawed in how its measuring things such that it can't safely throttle itself like the 4.12 does.
```

---
## \#166 Posted by: mmaner Posted at: 2018-12-17T18:25:12.940Z Reads: 187

```
[quote="Deodand, post:165, topic:71079"]
when you put it under loading that is beyond what it could handle it should just run up against its thermal limts and throttle down.
[/quote]

I don't understand how thermal limits are at issue.  The issue I ran into was when a battery draw of over 40a, on either side, occurred the VESC would reset.  It's probably just my lack of understanding, I appreciate you taking the time to explain it.
```

---
## \#167 Posted by: Deodand Posted at: 2018-12-17T18:32:35.617Z Reads: 185

```
I just mean that cheaper components will generate more heat and lack of heat sink dissipate less heat. So typically in a cheaper VESC the cost saving on FETs/casing are going to cause heat to be the limiting factor on the power the unit can push. 

With the 4.20 it seems more like they have an issue with their layout or its possible its an issue with too little bulk capacitance. Either way it would cost them nearly nothing on the BOM/Fab to make some slight layout changes or up the bulk caps and they'd be able to eliminate the cutouts and the unit would be able to properly run into its thermal limits at the same price point. But I guess getting someone to fix the design also costs money up front and people are buying it as is so...
```

---
## \#168 Posted by: DeathCookies Posted at: 2018-12-17T18:35:30.513Z Reads: 184

```
Thats why they have a fs420 plus :D
```

---
## \#169 Posted by: mmaner Posted at: 2018-12-17T18:35:55.811Z Reads: 183

```
That makes sense.  FYI, FlipSky has a plus version of the Dual out now.  I've got one in coming.  Ill see if it's any better.
```

---
## \#170 Posted by: DeathCookies Posted at: 2018-12-17T18:39:29.406Z Reads: 182

```
We should get a badge for getting ninjad at replies :see_no_evil:
```

---
## \#171 Posted by: Deodand Posted at: 2018-12-17T18:45:20.948Z Reads: 187

```
Looking at the new layout now. Definitely doesn't look like they made much changes to the layout and they removed two of the bulk caps to make room for their power switch. Maybe it was an issue with one of their passives though and they got it fixed, would be pretty silly to launch a new product with the same issue as the previous generation. At least there's a workaround with the current limit settings.
```

---
## \#172 Posted by: mmaner Posted at: 2018-12-17T18:48:55.717Z Reads: 185

```
Yeah, it's definitely taking some work to get it going reliably.  At the price point its useful for getting people to build rather than buy pre-builts which is why I'm hopeful.  

I have heard of a couple of people using the Plus version reliably on 10s.
```

---
## \#173 Posted by: Deodand Posted at: 2018-12-17T18:53:17.115Z Reads: 180

```
Yeah, I'd like to release something cool/tiny at that price point for the same reasons. It's tough because the margins are slim but perfect for that entry level board. Let us know how it goes!
```

---
## \#174 Posted by: mmaner Posted at: 2018-12-17T19:17:22.143Z Reads: 183

```
[quote="Deodand, post:173, topic:71079"]
Yeah, I’d like to release something cool/tiny at that price point for the same reasons. It’s tough because the margins are slim but perfect for that entry level board.
[/quote]

Its a catch 22 problem, for sure :slight_smile:
```

---
## \#175 Posted by: Bobby Posted at: 2018-12-21T05:34:13.049Z Reads: 189

```
Just wanted to give you a big thanks @mmaner !!! Put the dual flipsky with settings you provided on a pair of koowheel 97mm hub motors and im in love!!!  A 10s5p battery gets me over 30mph easy!! Running unsensored in foc. Did a lil speed run today and although i was pushing it...I didn’t even give it the max throttle (wanted to tighten up some stuff and have a bit more light). ![image|281x499](upload://rsZEGtMVQFjxtxlnY0WDJ7vKXH9.jpeg)
```

---
## \#176 Posted by: Turboboard Posted at: 2018-12-22T05:21:21.603Z Reads: 183

```
So I have a little problem with my flipsky dual 4.20, it might be my motors, I don't know. I have a 10s battery, 6374 190kv 3300w motors, 15 tooth motor pulley, 72 tooth wheel pulley and 8" pneumatic tires. Anyway the vesc is stock, no adjustments. I can prevent the motors from spinning with just my fingers. When they do start spinning they have incredible power and torque. Should I change some settings? Something else I'm missing?
```

---
## \#177 Posted by: Benjamin899 Posted at: 2018-12-22T13:01:42.443Z Reads: 183

```
what is the problem? Either they have torque or they don't.
```

---
## \#178 Posted by: mmaner Posted at: 2018-12-22T13:38:54.928Z Reads: 185

```
Did you do motor detection and setup the current values?
```

---
## \#179 Posted by: Turboboard Posted at: 2018-12-22T15:27:24.129Z Reads: 192

```
Well, that's the reason my ESC is still stock, I can't get it to connect to either one of my tools 😄 I have both ackmaniacs vesc tool and metr. I'm trying to connect via USB, not happening
```

---
## \#180 Posted by: J0ker3366 Posted at: 2018-12-22T16:28:39.136Z Reads: 190

```
Why the hell!!!? If you haven't ran motor detection why are you running the motors? Never! Figure out why it wont connect before you do anything.
```

---
## \#181 Posted by: Turboboard Posted at: 2018-12-22T20:55:30.589Z Reads: 189

```
Any ideas wy it won't connect? The USB cord is connected but my computer isn't sensing the esc
```

---
## \#182 Posted by: Benjamin899 Posted at: 2018-12-22T21:01:34.366Z Reads: 188

```
is the usb cable able to transfer data?
```

---
## \#183 Posted by: Turboboard Posted at: 2018-12-22T21:51:23.664Z Reads: 185

```
Not sure, it came with the esc
```

---
## \#184 Posted by: Benjamin899 Posted at: 2018-12-22T21:53:32.318Z Reads: 181

```
take a usb calbe that you know transfers data
```

---
## \#185 Posted by: kalebludlow Posted at: 2018-12-22T22:32:30.107Z Reads: 183

```
If it were me, I would assume that the included cable can be used for data.
```

---
## \#186 Posted by: mmaner Posted at: 2018-12-22T22:54:47.348Z Reads: 183

```
It's probably a driver issue.
```

---
## \#187 Posted by: finges Posted at: 2018-12-22T23:16:24.188Z Reads: 182

```
You said you tried acks and metr.. have you tried the stock vesc-tool? https://www.vesc-project.com/vesc_tool.. also.. are you powering the vesc via a battery?
```

---
## \#188 Posted by: Benjamin899 Posted at: 2018-12-22T23:20:43.413Z Reads: 184

```
basicly cover the super basics, after that you got a real problem on your hands. 
@kalebludlow you never know. doesnt hurt to use another usb to test it.
```

---
## \#189 Posted by: J0ker3366 Posted at: 2018-12-22T23:39:21.092Z Reads: 188

```
[quote="Turboboard, post:183, topic:71079, full:true"]
Not sure, it came with the esc
[/quote]

Checking this tonight when I'm home as to if my cable does the same thing. But I'm willing to bet 
[quote="mmaner, post:186, topic:71079, full:true"]
It’s probably a driver issue.
[/quote]
```

---
## \#190 Posted by: Bobby Posted at: 2018-12-23T01:21:23.160Z Reads: 180

```
I personally used the vesc tool and it works fine. Did u upgrade the firmware using the vesc tool
```

---
## \#191 Posted by: Turboboard Posted at: 2018-12-23T04:06:15.153Z Reads: 179

```
Just downloaded the stock vesc tool, gonna try that and yeah I'm powering the vesc with a battery
```

---
## \#192 Posted by: Turboboard Posted at: 2018-12-23T07:41:45.693Z Reads: 184

```
You guys are awesome! Downloaded the stock vesc tool, bought a data USB, was able to connect, changed a few things then took it for a test ride. I wasn't ready for the torque and power, it tossed me off😂 though that might have been due to motor gears too (went from a 16 tooth to a 15). My new motors are twice as powerful as my last ones, the VESC is WAY better too. My last speed controller was just a normal ESC
```

---
## \#193 Posted by: Mazda_bater Posted at: 2018-12-24T11:06:58.517Z Reads: 184

```
The cord supplied with my flipsky esc wouldn't work either I used a Samsung phone cord to get my computer to recognise the connection
```

---
## \#194 Posted by: Kug3lis Posted at: 2018-12-24T11:35:47.161Z Reads: 180

```
When they include non data usb cable for data communication damn those chinese :laughing:
```

---
## \#195 Posted by: Benjamin899 Posted at: 2018-12-24T12:20:27.264Z Reads: 186

```
thats why IT always asked if you have turnt it off and on again and if all calbes are connected.
```

---
## \#196 Posted by: Deodand Posted at: 2018-12-25T23:25:55.133Z Reads: 182

```
Probably just a faulty cable if I had to guess. That'd be something special to do a power only cable when the power doesn't even connect :smile:
```

---
## \#197 Posted by: artSkate Posted at: 2019-01-01T23:02:35.392Z Reads: 185

```
![image|666x500](upload://gqQjtR0O7kwpUnme0xA7UrQavIG.jpeg) ![image|666x500](upload://oQ6k32MYInYddNLWi7YQ3xvyB2Y.jpeg) ![image|666x500](upload://hULgfXYzOSRrEMQwZl4AgRJ8lpJ.jpeg) 

My experience with this vesc was not a good one. Im runningg 10s5p HG2 li-ion pack. 6374 200kv motors.

I started out with recommended settings bldc 30a per motor etc... board had cutouts during hard accelaration (it was not a big deal to me).  I had to accelarate in bursts or gradually. Foc with the same settings worked, but had more frequent cutouts. Iv put around 20 miles on the board with this settings.  I did an experemental set up: 45a per motor with batt current max at 60.  Riding on a flat ground at a decent speed, i did about a 2 second accelaration burst.  Cutout happend, but contrary to previous cutouts, esc did not come back on.  I turned off/on the esc and tried throttle again. Only one motor was spinning. I turned the esc off and walked home (about one mile).  At home, i connected esc to my computer to see if maybe i need to run motor set-up wizard again. Motor that was running (slave side), had no issues. Master side motor Displyed a fault: bad detection or something similar. That was all in bldc mode. Well, i thought i would give foc detection a chance. Thats when fsvesc shorted.  I was dodging components of esc, smoke, and blinding light as i was reaching to disconnect xt-60 loop switch. By the time i got it out, it was too late. Esc was fried. Two 5p cells of the battery went flat. Insulation rings on the surviving cells were in the poor shape, making them unuseable.  So, not sure what went wrong here... this did cost me a good chunk of time and some american dollars. Flipsky did fefund me for esc.  Ive since rebuild the battery and placed my old unbranded 60 dollar dual motor ebay esc that spits out 30 a per motor, never cuts out, and requires no programming (also feels torquier and gets me same top speed and better climbing than flipsky).  You guys make your own decisions on this product, but im not a flipsky believer.
```

---
## \#198 Posted by: artSkate Posted at: 2019-01-01T23:03:39.206Z Reads: 182

```
![image|375x500](upload://qgE5yRlsIBaK8UDzaOaXeJwbfQy.jpeg)
```

---
## \#199 Posted by: Benjamin899 Posted at: 2019-01-01T23:30:41.855Z Reads: 180

```
mmh, your battery need some more insulation. nothing to do with the Fsesc though.
```

---
## \#200 Posted by: mmaner Posted at: 2019-01-01T23:31:43.051Z Reads: 176

```
What leads you to believe it was the ESC that shirted and what part of the ESC?  I'm just curious, I can't think of anything that would cause that kind of battery issue other than maybe a phase wire short.
```

---
## \#201 Posted by: artSkate Posted at: 2019-01-01T23:54:48.306Z Reads: 183

```
Here is how it went down:  

1. connect to faulty esc with bdlc tool in bldc mode
2. Run detection several times, but keep on getting detection fault.
3. Switch to foc detection on the affected side. Do two attempts at detection. In the middle of 2nd attempt of foc detection, i see a cloud of smoke rolling out of my esc enclosure, followed by esc pieces flying away from the esc.  It prob took me about 10 seconds to pull the plug (because of the esc literally being on fire).  12 ga motor wires along with capacitors and parts of pcb fused together. My battery was starting to smoke as well.

4. Right before esc caught on fire,  motor was making a noise as if it was trying to spin.

5. Like i mentioned previously, the same motor works fine with unbranded simple esc after the incident.

Based on where the short started and motor still working fine, i arrived at the coclusion that short started in the esc.
```

---
## \#202 Posted by: artSkate Posted at: 2019-01-02T00:07:18.979Z Reads: 190

```
![image|281x499](upload://p8XhHzWBYHJOShdq3V7cG8Q20Ho.jpeg) 

I take my time building batteries. This is not the first one i build.  Never had a battery short on me.  

This is how it looked before i took it apart. 

Ive put extra isulation rings on positive terminals.  Each side of the battery was shrink wrapped.  I used 3 layers of 8mm .15 nickel strip.  Balance cable wires were ran in an insulation channel to prevent potential contact with negative battery core.  Each side of this battery was individually shrink wrapped.  1/2inch rubber devider was placed between two sides of the battery. Than, all of that was wrapped in a thick shrink wrap.  Any possible friction point i would either pad or wrap with electrical tape before shrink wrap.
```

---
## \#203 Posted by: Benjamin899 Posted at: 2019-01-02T00:23:21.916Z Reads: 186

```
mmh FOC you said, well i read that FOC does put more strainn on the mosfets, maybe that started a chaninreaction ?
```

---
## \#204 Posted by: artSkate Posted at: 2019-01-02T00:57:22.577Z Reads: 189

```
Going forward, a fuse is going to be a must for my future batteries.
```

---
## \#205 Posted by: Mazda_bater Posted at: 2019-01-11T17:03:45.133Z Reads: 192

```
I'm going to replace all the caps on mine and see if that solves the issues I'm having I've ordered some 470uf100v it seems strange to me that with the dual 6.6 they run 6x 470uf100v then on the single 6.6 they run 3x 220uf100v I've found them as a company to be available for contact and quite supportive.
```

---
## \#206 Posted by: LukePL Posted at: 2019-01-11T18:30:07.762Z Reads: 195

```
I hope it will help. Let us know.
```

---
## \#207 Posted by: Turboboard Posted at: 2019-01-18T03:07:06.961Z Reads: 195

```
So I've noticed a lot of people have been experiencing cutouts with this ESC. If running dual motors do the cutouts happen with both motors or just one? I'm only getting cutouts on one motor, (running dual 6374s), if my remote is in fast mode and trying to accelerate quickly. Gradual acceleration is no prob. If my remote is in slow mode, (same speed as fast mode😂) then I have no problems. Fsesc has identical settings on both sides. Any ideas why only one motor would cutout?
```

---
## \#208 Posted by: mmaner Posted at: 2019-01-18T03:42:57.137Z Reads: 190

```
Both sides are programmed the same? What are your current limits?
```

---
## \#209 Posted by: Turboboard Posted at: 2019-01-18T14:43:58.215Z Reads: 184

```
Motor max: 30A
Motor max brake: -30A
Battery max: 40A
Battery max regen: -30
Absolute max current: 130A
```

---
## \#210 Posted by: mmaner Posted at: 2019-01-18T14:44:44.452Z Reads: 176

```
10s or 12s?  Try lowering battery max to 30a.
```

---
## \#211 Posted by: Turboboard Posted at: 2019-01-18T14:55:42.701Z Reads: 169

```
Im running 10s
And thats the thing, ive tried +/- 10 on all the current settings
```

---
## \#212 Posted by: mmaner Posted at: 2019-01-18T15:02:52.486Z Reads: 173

```
I dont know, have you tried contacting FlipSky technical support and see what they have to say?
```

---
## \#213 Posted by: Turboboard Posted at: 2019-01-18T15:08:13.966Z Reads: 175

```
No, thats next on the list. Ive gotten more help from you guys, (and gals) than ive ever gotten from contacting any companies
```

---
## \#214 Posted by: BruSkater Posted at: 2019-02-04T20:36:32.571Z Reads: 177

```
Has anyone tried an 8s battery with the dual 4.20? I wonder if one could up the amps from @mmaner 's config if we drop de series count... Anyone has any clue?
```

---
## \#215 Posted by: Raf1 Posted at: 2019-02-22T16:07:32.018Z Reads: 177

```
Does anyone know what happened if one of the VESC in flashing red? It still turns on and goes blue and green but then it starts to blink red. I would really appreciate the help![IMG_20190222_160315|690x388](upload://mnM0ivfG7pY5q7xBeuyJYvXKLWQ.jpe![IMG_20190222_160338_1CS|690x388](upload://sUzm4SPsDS1TbXqb4PL32s0sHQk.jpeg) g)
```

---
## \#216 Posted by: Raf1 Posted at: 2019-02-22T16:08:32.878Z Reads: 176

```
![IMG_20190222_160315|690x388](upload://mnM0ivfG7pY5q7xBeuyJYvXKLWQ.jpeg)
```

---
## \#217 Posted by: mmaner Posted at: 2019-02-23T01:29:47.060Z Reads: 170

```
Plug it up to the VESC tool, go to the terminal and type faults.
```

---
## \#218 Posted by: J0ker3366 Posted at: 2019-02-23T02:14:26.285Z Reads: 174

```
Dual 4.20
35/-35
50
40

Dual 5065 sensorless in foc on 10s lipo. No cutouts or hicups as of now.
```

---
## \#219 Posted by: Raf1 Posted at: 2019-02-23T10:33:16.741Z Reads: 171

```
I did what you said and it said that there wasn't any faults detected.
![image|690x387](upload://oyliFWaxUEJ2ilTMeLpdi5Ncjqe.png)
```

---
## \#220 Posted by: mmaner Posted at: 2019-02-23T14:20:05.717Z Reads: 167

```
Does it still work?
```

---
## \#221 Posted by: Raf1 Posted at: 2019-02-23T14:31:24.696Z Reads: 173

```
Nope the VESC doesn't resond at all and the light is still falshing red.
```

---
## \#222 Posted by: mmaner Posted at: 2019-02-23T16:11:50.115Z Reads: 172

```
Run faults again
```

---
## \#223 Posted by: M.Hboards Posted at: 2019-02-27T03:38:04.680Z Reads: 169

```
@mmaner have you found any significant difference between the regular 4.20 dual and the plus besides the anti spark switch? Also do you find the built in antispark on the plus realiable and do you know if theres a way to add a battery indicator after the switch so it turns on/off with the rest of the board?
```

---
## \#224 Posted by: mmaner Posted at: 2019-02-27T04:15:49.154Z Reads: 171

```
It works at much higher amps, more reliable. 

The AS switch seems fine for now, I've not run it ling enough to say it's reliable. I've never seen a reliable AS switch so I'm not sure what it would look like 😃. 

There is no way to attach a votlmeter after the switch. I use a voltmeter that has a built in switch.
```

---
## \#225 Posted by: Winfly Posted at: 2019-02-27T07:16:31.534Z Reads: 167

```
How about 12s?
```

---
## \#226 Posted by: mmaner Posted at: 2019-02-27T12:59:08.852Z Reads: 163

```
I'm running it at 12s, I've run it at 10s on the bench but it's 12s on the board.
```

---
## \#227 Posted by: DAddYE Posted at: 2019-02-27T13:03:36.311Z Reads: 166

```
So you’re saying that the 4.20 plus is reliable (no faults) and runs 12s ?
```

---
## \#228 Posted by: practicalprojects Posted at: 2019-02-27T13:16:49.842Z Reads: 165

```
Thanks for putting the time into this review. Mine has been working kind of ok but every so often the power switch pops out, is this the 'drop out' issue people have been having or could this just be due to vibration which is what I'm suspecting?
```

---
## \#229 Posted by: mmaner Posted at: 2019-02-27T14:07:39.970Z Reads: 163

```
 as long as you stay under 50 battery amps, I have been.
```

---
## \#230 Posted by: mmaner Posted at: 2019-02-27T14:08:22.984Z Reads: 166

```
yeah, you should put a drop of hot glue over the connecter, vibrations will make lots of things come loose.  Loctite and Hot Glue FTW.
```

---
## \#231 Posted by: Meeep Posted at: 2019-02-27T14:19:33.839Z Reads: 167

```
Have you tested FOC? Main reason I am waiting for Unity is for FOC.
```

---
## \#232 Posted by: mmaner Posted at: 2019-02-27T15:25:03.275Z Reads: 167

```
I did test FOC for about 30 miles, but I'm not a big fan of full-on FOC mode. I typically just run hybrid if anything.
```

---
## \#233 Posted by: practicalprojects Posted at: 2019-02-27T17:44:03.517Z Reads: 162

```
Ok will give that a go thank you!
```

---
## \#234 Posted by: humanisticnick Posted at: 2019-03-04T19:15:22.423Z Reads: 159

```
I'm looking for anyone with practical knowledge of this. I have an extra FSESC 4.20 that I bought in a group buy. I was going to use it in my "nicer" board but I went 12s so I ended up getting the 6.6 dual for that. Now I have this extra one laying around.

I have a DIYEBOARD 10s5p dual belt (I know everyone hates them but honestly it works great) that I was considering swapping the 4.20 dual in for to replace:
http://www.diyeboard.com/v11-dual-belt-motor-sine-wave-foc-esc-speed-controller-p-522.html

My question is: I use the board currently with 150mm wheels and climb tons of hills (live in pittsburgh) it does this pretty well. Would this 4.20 dual have as much performance? I know it will be smoother but will it still deliver as much power? The specs on the cheepo esc list 50A continuous where as everyone is setting these to only ~30.

Any advice would be appreciated.
```

---
## \#235 Posted by: BillGordon Posted at: 2019-03-04T23:06:58.569Z Reads: 156

```
I have the same motors on one of mine and use a pair of 4.20 singles with them. I have them at 35a and it's meh, but anything above that is a cut-off fest.

Now to answer your question: the 4.20 setup is less powerful by a depressing margin. The top end is not bad, but the ESC grunt is not there. (I always kick start, so it's not a deal breaker.) If the braking hadn't been worse than sugar-free gummy bears, I could have easily lived with the DIYE esc.
```

---
## \#236 Posted by: humanisticnick Posted at: 2019-03-05T01:04:39.547Z Reads: 156

```
Exactly the feedback I was looking for. Thanks man
```

---
## \#237 Posted by: BillGordon Posted at: 2019-03-05T11:09:20.639Z Reads: 160

```
👍 (10 chars)
```

---
## \#238 Posted by: MiniChopper4Me Posted at: 2019-03-19T20:09:38.854Z Reads: 159

```
I have the non-plus version, dual.  Used it in a rebuild.  Mine seems to like to shut down and not  turn back on until I disconnect and reconnect the power.  @BillGordon Is this what you mean by "cutoff fest"?  It likes to do this when I full accel followed by full brake/reverse.

My settings currently are 40 -40 40 -6 on each side, with a 10S4P 30Q pack. I'm also using Ackmanic FW, and running my hub motors in BLDC sensored mode.  There are no issues in detection or startup or general usage, only when I do extreme control inputs with the board on the bench.  I'm not crazy enough to try reproducing these inputs while riding the board, but I have had it cut out and had to unplug/plug back in the loop key to get it working again.  I have no idea if I'm doing it right, but I haven't been able to get any kind of fault or error message while hooked up to the VESC and generating the error.  I'd be most appreciative if anyone could walk me thru how to see what my FSESC is complaining about, or even if possibly I just have a crappy one.

Thanks in advance!
```

---
## \#239 Posted by: Bobby Posted at: 2019-03-19T21:10:28.104Z Reads: 156

```
Has anyone noticed the esc takes like a little time to warm up? I have it set using your parameters and I noticea bit of a lag in acceleration.... Once i get going  everything  works out but There is a power dip that occurs usually when i first start my ride
```

---
## \#240 Posted by: mmaner Posted at: 2019-03-19T23:03:26.337Z Reads: 155

```
Set it to 30/-30/30/-10 and see if it's any better.
```

---
## \#241 Posted by: ryansinatra Posted at: 2019-03-19T23:10:59.669Z Reads: 157

```
I'm sure this question has been asked, but did we come to the consensus that two single 4.12 is better or dual 4.20?
```

---
## \#242 Posted by: mmaner Posted at: 2019-03-19T23:12:06.284Z Reads: 159

```
I prefer the dual 4.20 plus, but as long as you stay at 30 battery amps or less the not plus dual is dependable.
```

---
## \#243 Posted by: ryansinatra Posted at: 2019-03-19T23:22:03.048Z Reads: 160

```
Plus is out of stock :/ the single 4.12 is reliable yeah?
```

---
## \#244 Posted by: mmaner Posted at: 2019-03-19T23:38:31.556Z Reads: 161

```
I've never used one, I would assume so.
```

---
## \#245 Posted by: visnu777 Posted at: 2019-03-20T13:56:15.124Z Reads: 158

```
For me FSESC 4.12 is reliable (still). I run two of them with 50A/-50A motor + 40A/-15A battery each and they work like a charm. I killed some of them but it was all my fault :)

Edit: in FOC@10s
```

---
## \#246 Posted by: ryansinatra Posted at: 2019-03-20T16:29:09.048Z Reads: 154

```
What settings would you use for two of them in BLDC?
```

---
## \#247 Posted by: Benjamin899 Posted at: 2019-03-20T19:07:44.226Z Reads: 156

```
i use mine in BLDC with Battery 30A/-8 and motor 50/-50, values for each.
```

---
## \#248 Posted by: ryansinatra Posted at: 2019-03-20T19:13:53.579Z Reads: 154

```
Thank you. Is that with 10s?
```

---
## \#249 Posted by: kalebludlow Posted at: 2019-03-20T21:39:10.853Z Reads: 153

```
I run dual FSESC4.12 at 12s in BLDC. 35A/-10 and 60/-60

Never had any issues with them at all
```

---
## \#250 Posted by: Gamer43 Posted at: 2019-03-20T23:20:37.054Z Reads: 150

```
If you guys are willing to do a little SMD soldering, there's a rather trivial change that allows the 4.20 to handle +-60A motor and battery current.

Swap out the gate resistors from 4.7 ohm to, if you have the original: 47 ohm, the plus: 22 ohm.
```

---
## \#251 Posted by: Benjamin899 Posted at: 2019-03-21T13:22:34.258Z Reads: 147

```
yes i run it 10s
```

---
## \#252 Posted by: jun1208 Posted at: 2019-03-23T03:30:03.110Z Reads: 151

```
I just got mind yesterday and the vesc seems to only run on the right side of the PCB...

The LED doesn't light up like the right side and I can't find any switch to toggle the built in can bus...

Any help is appreciated :+1: 

The blue led just light up for a few milliseconds and shuts off...

https://youtu.be/nCQ9XWpDJk0
```

---
## \#253 Posted by: Schtekarsten Posted at: 2019-03-23T07:58:35.179Z Reads: 151

```
Hello buddy! looks like you have a tiny tiny bride on the left drv ship. clean that up with a soldering iron and se if it works.

if you dont know what I mean have a look at 13min in on this video: https://www.youtube.com/watch?v=0A8nzc24Mzw&t=28s
but skip the solder wick part just run over it with your iron

and while you are at it I would swap out the resistors on to some 22ohms. there should be a thread about it
```

---
## \#254 Posted by: jun1208 Posted at: 2019-03-23T09:13:31.387Z Reads: 151

```
Do you mean here on the vesc? The circled up part :thinking:

 ![IMG_20190322_233915__01|465x500](upload://3Msh4ERXLXxdzNGwdmYIWlZS8uL.jpeg)
```

---
## \#255 Posted by: Schtekarsten Posted at: 2019-03-23T11:12:06.720Z Reads: 144

```
Yes charrrrrrr
```

---
## \#256 Posted by: jun1208 Posted at: 2019-03-23T11:17:41.635Z Reads: 147

```
So I just run my solder iron through it but I'm a noob, how do I get them off the PCB?
```

---
## \#257 Posted by: Schtekarsten Posted at: 2019-03-23T13:02:28.888Z Reads: 147

```
Yeah! jump to 16min in the video
And make sure you have a nice clean shiny tip on your iron, and add some flux if that doesn't help. Basically when the pins gets hot they will wick up the solder so to speak.
```

---
## \#258 Posted by: jun1208 Posted at: 2019-03-23T14:02:51.804Z Reads: 141

```
What would actually happen if theres bridge on the drv chip tho?
```

---
## \#259 Posted by: Schtekarsten Posted at: 2019-03-23T14:09:35.807Z Reads: 141

```
It is likely that it will work like normal as soon as you remove the bridges on the drv chip.
something else might be fried but I doubt it.
```

---
## \#260 Posted by: jun1208 Posted at: 2019-03-23T14:13:34.077Z Reads: 141

```
Thanks for the pointers man! 

So I'll just follow your video and heat up the solder and kinda wipe the solder off with the heated tip eh? 

I just don't hope to mess up the whole vesc...
```

---
## \#261 Posted by: Schtekarsten Posted at: 2019-03-23T14:17:45.699Z Reads: 140

```
Well it is already fucked so you wont fuck it anymore unless you intend on running it as a single Vesc.
And no you wont fuck it up just dont keep the iron on the pins for more than a few seconds and you should be golden.
```

---
## \#262 Posted by: JohnnyMeduse Posted at: 2019-03-23T14:18:21.256Z Reads: 143

```
That bridge is normal, don’t worry about it.

If you don’t have any light it could be a short on the 3.3v, I you have a multi-meter you could check it.
```

---
## \#263 Posted by: banjaxxed Posted at: 2019-03-23T14:20:04.533Z Reads: 146

```
Do a warranty if you can
![image|281x500](upload://to6KPmy2H2PnvFpK0QOsDLjPt5s.jpeg)
```

---
## \#264 Posted by: jun1208 Posted at: 2019-03-23T14:21:26.219Z Reads: 144

```
Then do you have any idea on what's wrong with mine?
```

---
## \#265 Posted by: jun1208 Posted at: 2019-03-23T14:22:32.613Z Reads: 142

```
Yea warranty is my last resort as shipping back to China is expensive and the shipping will take forever too...
```

---
## \#266 Posted by: JohnnyMeduse Posted at: 2019-03-23T14:26:57.438Z Reads: 140

```
It could be short on the 3.3v or on the 5v
```

---
## \#267 Posted by: Schtekarsten Posted at: 2019-03-23T14:29:50.403Z Reads: 141

```
Yeah you should listen to the wizard and to not a moron like me.
but that's wired though because I have myself had two separate times a solder bridge on my drv chip on the flipsky 4.20 Vesc's when I did the resistor testings, and both times I had the bridged side not lighting up similar to jun's vesc. and both times when I removed the bridge It solved the problem. 
Idk just my experience with bridging regarding the 4.20 vesc's
```

---
## \#268 Posted by: jun1208 Posted at: 2019-03-23T14:34:54.128Z Reads: 138

```
The odd thing is that blue led **did light up** for a few milliseconds before going off...

Just that the LEDs on the right side stays on...
```

---
## \#269 Posted by: jun1208 Posted at: 2019-03-23T14:36:19.609Z Reads: 137

```
Thanks for your insight brother, so you're saying that you have personal experience exactly the same with my vesc is that correct?
```

---
## \#270 Posted by: Schtekarsten Posted at: 2019-03-23T15:02:54.495Z Reads: 135

```
Yeah But listen to jonnymedusa he really knows his stuff and I don’t
```

---
## \#271 Posted by: JohnnyMeduse Posted at: 2019-03-23T15:03:34.539Z Reads: 138

```
I don’t think your a moron your reasoning was  good, a short never look good on a chip. I would never had look at the picture if you haven’t mention a short.

But once you cross reference the location with the schematic, you realize that it won’t matter for this specific configuration.

![image|281x499](upload://tm8HT939lduXiHPH0OSZ7WbgpEm.jpeg) 

[quote="jun1208, post:268, topic:71079"]
The odd thing is that blue led **did light up** for a few milliseconds before going off…
[/quote]

Was th can connected?
```

---
## \#272 Posted by: Schtekarsten Posted at: 2019-03-23T15:08:01.265Z Reads: 137

```
The can bus is integrated in the design on the 4.20 plus version, unlike the toggle switch on the regular dual 4.20 Vesc
But you are right, because my bridges were caused by myself and located on the other side of the drv chip and most likely bridging different polarity pins.
```

---
## \#273 Posted by: jun1208 Posted at: 2019-03-23T16:16:33.185Z Reads: 135

```
Yea like what @Schtekarsten mentioned, it's a built in can bus connection so there's no switch for that... 

You mentioned that it might be a short on the 3.3v and 5v, how can I check that by myself? 

I apologise in advance because I don't know electrical methodology that we'll...
```

---
## \#274 Posted by: Mich21050 Posted at: 2019-03-23T16:21:12.836Z Reads: 134

```
If their design is based on the vesc 4.12 you could simply measure the 5v rail via the ppm cable. :slight_smile:

For the 3.3v rail it would be a bit more complicated. :slight_smile:

@jun1208
```

---
## \#275 Posted by: Schtekarsten Posted at: 2019-03-23T17:09:51.698Z Reads: 134

```
Oh jun1208 what I would do if I were you is talk to Flipsky and send it back. The plus version is not very reliable anyways and the anti-spark will die sooner or later running the vesc useless.
And if possible I would wait until the new 4.20 comes out with the modified resistors so you dont have to do the swap yourself and then just add a ugly XT90S loopkey to that.
```

---
## \#276 Posted by: JohnnyMeduse Posted at: 2019-03-23T18:58:59.703Z Reads: 138

```
[quote="jun1208, post:273, topic:71079"]
You mentioned that it might be a short on the 3.3v and 5v, how can I check that by myself?
[/quote]

I do really know their design but you could check with a multimeter in diode Check in you have continuity between the 5v and the GND, and between 3.3V and the GND. I'm not sure but I think if you remove the heatshink, they should be indicated on the mask of the pcb near each connector. 

Also, if could take a picture of the underneat, I'm curious to see if they use both 5V reg from each DRV

here is also a step by step to check the 3.3V, but I'm not sue if will work great in this case, since they might have change the denomination of each components

https://www.electric-skateboard.builders/t/no-power-to-enertion-vesc/7600/8?u=johnnymeduse

And as @Schtekarsten I agree that it is probably best to contact flipsky, and check what they can do for you.
```

---
## \#277 Posted by: Schtekarsten Posted at: 2019-03-23T19:56:09.480Z Reads: 129

```
But like someone mentioned in mine and Gamer43's thread earlier: https://www.electric-skateboard.builders/t/flipsky-4-20-a-explanation-to-the-mystery-and-how-to-stop-the-cutouts-entirely/87824/43 

If you like swapping out resistors you might have a few people standing on your doorstep with their 4.20 based vesc's. As well as depending on the type of mosfets flipsky ends up using, you might want to offer some upgrades there as well. But that will be quite costly as you need 12 of them and on top of that you need to match the mosfets with the right resistors values to keep the slew rate in check.:v:
```

---
## \#278 Posted by: jun1208 Posted at: 2019-03-25T13:56:46.168Z Reads: 124

```
I haven't got a multimeter with me so I can't check as of now...

This is the pic of the vesc front and back

![IMG_20190325_215533|666x500](upload://iEofureT353GKXChEns5fi23q38.jpeg) 
![IMG_20190325_215549|666x500](upload://f0z9TGG1FUpAbdxHrNGHUN8Q5IP.jpeg)
```

---
## \#280 Posted by: jun1208 Posted at: 2019-03-27T00:26:50.382Z Reads: 120

```
Great work from both of you guys in that thread :+1::+1::+1: 

I don't see myself replacing the ones on this VESC unless I want a one way ticket to the bin for the VESC 
:sweat_smile: 

Flipsky has offered to send me a replacement but they will only send the non plus version, which means I have to get an AS switch in order to use it...
```

---
## \#281 Posted by: J0ker3366 Posted at: 2019-03-27T00:42:09.267Z Reads: 121

```
[quote="Schtekarsten, post:275, topic:71079"]
The plus version is not very reliable anyways
[/quote]

Im just going to assume this is personal opinion and leave it be.
```

---
## \#282 Posted by: Schtekarsten Posted at: 2019-03-27T07:30:34.752Z Reads: 120

```
Get a xt90s loopkey instead then
```

---
## \#283 Posted by: Schtekarsten Posted at: 2019-03-27T07:33:16.303Z Reads: 124

```
Nop, I actually would love the the switch to be reliable, as that would be to my best interest.
But don’t say I did not warn you. Sure it probably won’t blow the first time but, sooner or later.
```

---
## \#284 Posted by: jun1208 Posted at: 2019-03-27T08:41:43.273Z Reads: 126

```
I think that's what I will do for now...

Do I understand how to wire a loop key correctly?

![Loop%20Key|690x444](upload://Aovs4dFKU73vnw7jAeJRFVKf9qo.jpeg)
```

---
## \#285 Posted by: Bardakon Posted at: 2019-03-27T14:13:35.701Z Reads: 124

```
i'm about to build one with:
- 2x170 kv motors

-2x flipsky 4.12

-8 inch wheels

-10s4p samsung 30q  battery

do you think its gonna go good together? what's your opinion and tips?
```

---
## \#286 Posted by: Benjamin899 Posted at: 2019-03-27T14:16:32.728Z Reads: 125

```
4.12 works like any other 4.12 vesc.
```

---
## \#287 Posted by: Schtekarsten Posted at: 2019-03-27T14:52:33.140Z Reads: 129

```
I would not even look at the 4.12 vesc's to be honest, especially If you intend to use AT-wheels on the board. The 4.20 is just soo much better value for money, and would be the minimum in terms of power needed to run a half decent AT-setup. And flipsky should be shipping all their new 4.20 vesc's from now on with the modified resistors. They just haven't had time to update their website yet. 

if anything I would look upwards towards a focbox or 6.6 vesc and not down towards the 4.12 if you are going for a AT-setup. But then again if that is the case I would use a larger battery and 6374 motors. But if that is the case you are looking at a different price point.
```

---
## \#288 Posted by: Schtekarsten Posted at: 2019-03-27T15:01:40.708Z Reads: 130

```
ya that is correct. I know loop keys are ugly as f*** and you loose them and all that, but that will be the most robust solution as of now. If you don't want to pay some good money for a solid anti-spark.
```

---
## \#289 Posted by: mmaner Posted at: 2019-03-27T15:12:09.825Z Reads: 131

```
[quote="Schtekarsten, post:283, topic:71079"]
Sure it probably won’t blow the first time but, sooner or later.
[/quote]

This is true of all AS keys that do not incorporate a pre-charge circuit, not just FlipSky's.
```

---
## \#290 Posted by: Benjamin899 Posted at: 2019-03-27T15:30:39.688Z Reads: 134

```
i use an xt 90 anti spark, when do i know that thing is broken?
```

---
## \#291 Posted by: mmaner Posted at: 2019-03-27T15:38:00.405Z Reads: 135

```
An XT90S is a loop key, not an Anti-Spark switch.  You will know when a loop is broken, trust me :).
```

---
## \#292 Posted by: Benjamin899 Posted at: 2019-03-27T15:45:49.128Z Reads: 136

```
i figured, but good to know.
```

---
## \#293 Posted by: landonkun Posted at: 2019-03-27T23:58:33.205Z Reads: 134

```
Was wondering if someone could give me some insight with my 4.20 dual issue. I'm used to single vescs, so the dual is a new world to me.

I'm using Ackmaniac's tool/firmware. Followed tutorials on how to properly set up master/slave, did motor and input wizards with no trouble, made sure to split max battery/regen in half, and everything looked fine.

The issue is when I slowly push the throttle of my Nano-X to about 25%, only one motor (I think on the master vesc side) starts to turn, and it isn't until I push it further that the second motor starts to turn. Even at full throttle, by eye, it looks like the first one is still turning faster.

Is there a setting I could be overlooking?

If more info is needed, I'll post vesc settings, but it's all pretty default. 40/-40 motor, 30/-20 battery.
```

---
## \#294 Posted by: jun1208 Posted at: 2019-03-28T00:31:42.181Z Reads: 132

```
Are you running sensorless or sensored? 
Did you try riding it?
```

---
## \#295 Posted by: landonkun Posted at: 2019-03-28T00:44:20.822Z Reads: 130

```
Sorry, I guess I was skimping on the details.

Running sensorless in BLDC (for now.. will try FOC later). Haven't actually tried riding on it, in case I was missing a critical setting.
```

---
## \#296 Posted by: jun1208 Posted at: 2019-03-28T01:07:44.456Z Reads: 128

```
If I'm not mistaken, motor cogging while bench testing on sensorless is normal :+1:

Tried push start and ride it then it should be fine :slight_smile:
```

---
## \#297 Posted by: landonkun Posted at: 2019-03-28T01:13:06.171Z Reads: 135

```
Yeah, I was familiar with cogging on my single vesc build. It's not so much cogging as just not starting at all. Like.. first motor will cog up until about 5-10% throttle, then starts to spin after that. 2nd motor won't move at all until about 25%, where it starts to cog, then start up. I thought maybe I was missing something.

But I guess I should just go give it a go :) Snow is finally melting too.
```

---
## \#298 Posted by: jun1208 Posted at: 2019-03-28T09:33:40.004Z Reads: 136

```
When I was running sensorless last time, I was also shocked by the motor cogging while bench testing :frowning_face:

1 side of the motor doesn't seems to move even when I apply the throttle, but they all run ok after riding it so I guess that's just how sensorless runs :slight_smile:
```

---
## \#299 Posted by: Mazda_bater Posted at: 2019-03-31T03:09:48.073Z Reads: 133

```
Are you configuring both vescs? Like connecting the USB to vesc 1 and vesc 2 and both motors are identically configured
```

---
## \#300 Posted by: landonkun Posted at: 2019-03-31T03:33:18.559Z Reads: 136

```
Yep. Started on vesc 0, did motor detection, then input wizard. Next did vesc 1 motor detection, then input wizard again, this time setting it to slave vesc.
```

---
## \#301 Posted by: Mountainboard83 Posted at: 2019-04-19T15:35:51.215Z Reads: 136

```
Theyr junk i have 2 of them unfortunately and both have constant cutouts on even mild amp settings. Ive been pretty much limited to 30a or less and had to increase throttle and brake ramping time just to make it rideable.
```

---
## \#302 Posted by: chrischo1996 Posted at: 2019-04-19T16:15:59.564Z Reads: 139

```
These issues have been fixed in the newest iteration since March 27, check this thread for more info.
https://www.electric-skateboard.builders/t/flipsky-4-20-a-explanation-to-the-mystery-and-how-to-stop-the-cutouts-entirely/87824
```

---
## \#303 Posted by: brenternet Posted at: 2019-04-19T16:30:52.096Z Reads: 137

```
Yeah, your info is old unfortunately. Someone has figured out how to fix these and the newest version does not suffer the cut outs. They are improving, which is great really.
```

---
## \#304 Posted by: humanisticnick Posted at: 2019-06-07T17:58:54.669Z Reads: 102

```
Can anyone confirm if the newest (for sale right now) Dual 4.20plus still has cutouts? I am looking at replacing my Diyeboard esc, 10S and dual 5055
```

---
## \#305 Posted by: DAddYE Posted at: 2019-06-15T00:38:58.141Z Reads: 94

```
It has cutouts. Not severe. I got like a couple of them in the past 2 months during hill climb or when the motors/VESC were hot. 

I’m 12s at 40A battery. Motor 60A. I’m running elofty DD on Haggy wheels. 

Here my last error:

https://metr.at/r/zyFJu
```

---
## \#306 Posted by: Gamer43 Posted at: 2019-06-15T18:24:27.032Z Reads: 87

```
Just for reference, I tried those settings on TB 4.12 hardware and get ABS Overcurrent faults when full throttling at a standstill xD.
```

---
## \#307 Posted by: niuva Posted at: 2019-07-21T17:56:48.932Z Reads: 72

```
So does the dual FSESC 4.20 Plus actually support push to start (turn on), or is that just an urban legend? I want to get rid of the power switch that came with it.


I feel like a fool for trying to push my new board like a madman to get it to turn on. When I ordered it I was certain I read that it has push to start feature, but now that I try to find any mention of it I can't seem to find any.  Am I missing something, or just retarded?
```

---
## \#308 Posted by: jun1208 Posted at: 2019-07-22T06:23:30.101Z Reads: 68

```
I don't think so it does tbh..

Normally they will name the one with push to turn on the 'smart' variant :thinking:

And the power button with be the click type instead of the springlock type :+1:
```

---
## \#309 Posted by: Mic1 Posted at: 2019-12-08T09:11:00.521Z Reads: 41

```
Just want to grab this thread up again and asking if it is possible to loop the original build-in anti spark switch and make a XT90s on the battery side instead? If yes, how?
```

---
## \#310 Posted by: Mic1 Posted at: 2019-12-14T12:22:59.055Z Reads: 30

```
No one who has an idea?
```

---
## \#311 Posted by: BillGordon Posted at: 2019-12-14T19:58:42.864Z Reads: 29

```
Dude, this forum is mostly dead now. Head over to the new forum if you want help.
```

---
## \#312 Posted by: SeanHacker Posted at: 2019-12-14T23:48:13.757Z Reads: 28

```
I might have some ideas [here](https://bit.ly/2okbm7J)...
```

---
