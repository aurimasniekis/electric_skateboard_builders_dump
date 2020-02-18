# First build (Carvon v2 Dual, 10S4P SPACE Cell Pro 4, Ollin VESCs)

### Replies: 64 Views: 16584

## \#1 Posted by: scottkellum Posted at: 2016-09-22T02:26:02.921Z Reads: 631

```
I really like the utility and DIY aesthetic of @RunPlayBack’s boards so based this build off of his.

Having ridden Boosted and the Acton Blink I wanted to start with a deck that had a kick tail for maneuverability. I went with a JET deck with a tail that is long, but can still be kick turned. I also carved out a layer of wood from the deck to recess the case slightly into the deck.

<img src="http://i.imgur.com/rOGC4Ub.jpg">

A SPACE Cell Pro 4 10s4p battery fits nicely into this cutout, but I had to cut the corners off as the wheels were biting them.

<img src="http://i.imgur.com/9vwObBE.jpg">

Here is an early mockup of the wiring with the old 12s ESCs I was running, they ran strong, but I wanted more control so upgraded to Ollin VESCs

<img src="http://i.imgur.com/ryMZyAL.jpg">

After a weekend of riding it hard, and sometimes towing a friend up hill, one of the ESCs burnt up. Fortunately I had already ordered the upgrade to VESCs. apologies for the electronics gore.

<img src="http://i.imgur.com/WaOQiew.jpg">

While waiting for the new ESCs I went to RadioShack to buy LEDs on their closing sale and wired those into the front and back trucks.

<img src="https://scontent-lga3-1.cdninstagram.com/t51.2885-15/e35/14294973_1785657055042688_499994497_n.jpg?ig_cache_key=MTMzNjYzNTAzNDM3MTU0OTM2OA%3D%3D.2">

Now I have a BEC powering the low voltage electronics (2.4Ghz receiver and LEDs) and the VESCs just power the wheels. Cleaned up the wiring and all the connections to reduce risk of failure.

<img src="http://i.imgur.com/TQBLoWO.jpg">

Here are the VESC settings (as of September 21, 2016) and I’m still not happy with them, if anyone has any feedback let me know. It doesn’t accelerate or brake as hard as the previous ESCs, but also feels much smoother. I had max input at 42v but that kept causing an error so bumping it up to 57 (VESC default) prevents the breaks from failing but I’m worried I’m overloading the battery.

<img src="http://i.imgur.com/FLdgsUi.png">

In terms of safety I got triple8 elbow and knee pads and a T8 downhill racer full face helmet. I also have sector 9 slide gloves I hope to build a remote directly into, like power gloves, so that I can stay safe and wear gloves while maintaining good control over my board.

I’ll be up in NYC over the weekend riding with a number of friends who are in the esk8 community, mostly Boosted fans. If any of y’all know Sam Sheffer, gonna try to get him into the DIY scene a bit. Feedback welcome, especially on VESC settings, I’m learning a ton in doing this.
```

---
## \#2 Posted by: Titoxd10001 Posted at: 2016-09-22T02:52:46.285Z Reads: 509

```
Dope build man! I remember seeing this on Instagram. I don't own carvon motors but I think upgrading to v2.5 might help
```

---
## \#3 Posted by: scottkellum Posted at: 2016-09-22T03:05:03.433Z Reads: 499

```
Thanks! Yeah I live in an area with lots of hills and thought about the upgrade but these motors seem strong enough to pull me up them with the right settings.
```

---
## \#4 Posted by: Jinra Posted at: 2016-09-22T03:21:56.497Z Reads: 474

```
You should change battery Regen to -8a per VESC. -20 is to high and will charge the battery higher than its rated max current.
```

---
## \#5 Posted by: Titoxd10001 Posted at: 2016-09-22T03:23:55.066Z Reads: 447

```
You might be drawing more amps with v2 vs v2.5 which is never good for the battery. Some setting changes might help @LEVer should have the  optimum vesc settings
```

---
## \#6 Posted by: lox897 Posted at: 2016-09-22T07:58:52.626Z Reads: 413

```
Images don't work for me. Sounds good though!
```

---
## \#7 Posted by: scottkellum Posted at: 2016-09-22T09:08:32.060Z Reads: 399

```
Thanks, should be working now
```

---
## \#8 Posted by: Ackmaniac Posted at: 2016-09-22T09:09:03.199Z Reads: 390

```
If you want them to accelerate harder especially at low speeds you need to increase the motor amps to maybe 80. But I don't know how much the carvon can handle. So it is at your own risk. I guess your old ESC did not care about that and gave the motor as much amps as he wants.
```

---
## \#9 Posted by: RunPlayBack Posted at: 2016-09-22T13:19:42.312Z Reads: 389

```
Nice work Scott! Very clean build but I'm probably bias because I have a soft spot for Jet decks. A few things stand out to me in regards to your VESC settings:

"Motor max: 60.00A" looks good and theoretically you could bring it to 70.00A on Carvon V2's but it's not a significant difference.

"Max ERPM: 100,000.00" is high and the Carvon's will take it but I typically keep my ERPM at 70,000.00 for efficiency. This also depends on your weight and what kind of terrain you're riding on. I don't weigh much and I ride primarily on flats.

"Batt max: 40.00A" feels a little high for the Space Cell. I believe both VESC's should be programmed to total a 40.00A draw from the battery. So basically 20.00A on each VESC. Someone correct me if I'm wrong.

My voltage limits on the original Space Cell are:

Min input voltage: 8.00 V
Max input voltage: 57.00 V
Battery cut off start: 35.20 V
Battery cut off end: 33.20 V

Hope some of this helps!
```

---
## \#10 Posted by: scottkellum Posted at: 2016-09-22T14:02:26.020Z Reads: 353

```
Thanks! these settings are super helpful. Enertion’s website says peak output is 80a and I removed the 40a fuse. Maybe I’ll go easy on the battery and split the difference. I don’t weigh much but have a number of hills, what is ERPM exactly and do higher numbers provide more torque? I’m not doing much long range riding so using more juice isn’t a concern.
```

---
## \#11 Posted by: scottkellum Posted at: 2016-09-22T14:02:58.873Z Reads: 323

```
awesome thanks! I’ll adjust that
```

---
## \#12 Posted by: RunPlayBack Posted at: 2016-09-22T14:14:10.408Z Reads: 320

```
ERPM is the max RPM's your motor will reach at top speed. It's how you can speed limit your board from going too fast. I prefer to stay under 25.
```

---
## \#13 Posted by: Jinra Posted at: 2016-09-22T15:08:30.294Z Reads: 321

```
The cells are rated for 80a continuous in 4p and I have mine set to 40a per VESC for max draw. They never draw 80A continuous, however, and it's nice to have the extra power on demand.

Do you actually hit 70k erpm on carvons? I would've thought the VESC would error out at those speeds.
```

---
## \#14 Posted by: anon33082420 Posted at: 2016-09-22T16:17:18.787Z Reads: 315

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#15 Posted by: RunPlayBack Posted at: 2016-09-22T16:59:44.574Z Reads: 317

```
I'm not quite sure if I've hit 70k, how do I measure it, through BLDC tool while riding? For a long time I had it set to 100k which is what I'm assuming just maxed out the RPM/top speed for Carvons. After my friend's accident I started playing with the ERPM to speed limit the board. I found that 50-60-70k (beginner / intermediate / advanced) is kind of the average settings on Carvons for someone who weighs 135-170 lbs. So depending on whose riding the board, I tweak the ERPM.
```

---
## \#16 Posted by: Titoxd10001 Posted at: 2016-09-22T18:10:47.123Z Reads: 311

```
Wouldn't the speed to reach 60k rpm on a 1:1 ratio be like 80mph+ with 149kv motor
```

---
## \#17 Posted by: Jinra Posted at: 2016-09-22T23:45:46.937Z Reads: 308

```
for 1:1 systems your erpm shouldn't be that high sure to generally lower kv. Most likely the limits you've been setting haven't been doing anything if they're at 70k. What's the kv of your motors? Assuming 100kv with 7 pole pairs, you should be hitting ~30k erpm tops with 10s. You can still limit speed by limiting erpm, but it'd have to be much lower with hubs.
```

---
## \#18 Posted by: scottkellum Posted at: 2016-09-23T13:01:03.509Z Reads: 306

```
Thanks everyone in this thread for all the feedback! The board is running smooth and strong, even while taking the hills in my neighborhood.

@Jinra @RunPlayBack maybe I’ll write a little web app to help calculate rpm limits based on target mph/kph. With FOC on the limits don’t work but might be handy for those running in BLDC mode.
```

---
## \#19 Posted by: scottkellum Posted at: 2016-09-24T16:09:20.966Z Reads: 300

```
@Jinra @RunPlayBack made a little app for RPM calculations. Hopefully my math is correct, pretty sure it is: https://scottkellum.github.io/Esk8-RPM-finder/
```

---
## \#20 Posted by: Titoxd10001 Posted at: 2016-09-24T18:18:11.979Z Reads: 303

```
I think you have to multiply times 7(#of poles) to get erpm
```

---
## \#21 Posted by: scottkellum Posted at: 2016-09-24T18:33:34.192Z Reads: 290

```
Thanks! I'll add another input later for that. I knew the numbers felt low.
```

---
## \#22 Posted by: scottkellum Posted at: 2016-09-29T13:05:36.624Z Reads: 284

```
Made a video of this build with a friend last night:

https://www.youtube.com/watch?v=9lrqwuwgFdU
```

---
## \#23 Posted by: evoheyax Posted at: 2016-09-29T16:01:52.324Z Reads: 281

```
@scottkellum Do you have any overheating shut downs on your vescs? I've been ridding the dual carvon v2's for the past few weeks through the tough hills of San Francisco while I upgrade the bearings to ceramics in my 4wd motors, and I get my first vesc shut down at about 15 blocks of riding. Was riding 10s4p, had these issues. Upgraded to 12s4p, and it's slightly worse or the same. According to my vescs, I pull 60 amps continuous (30 per motor) almost the entire route (even on flats) until the vescs start shutting down from heat. Chaka's vesc btw with heat sinks. Just curious if you ever have these issues?

I'm assuming this happens due to the fact I'm running at less than 40% of my no load speed for most of my route, and at best, I hit 50% my no load speed, but I never get to that 85% no load speed golden spot. i will be trying 4wd with them in the near future, which should spread the amp draw out, and get rid of these heat issues. But I have to build another deck first, haha.
```

---
## \#24 Posted by: anon33082420 Posted at: 2016-09-29T16:25:36.864Z Reads: 255

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#25 Posted by: scottkellum Posted at: 2016-09-29T16:42:43.368Z Reads: 258

```
I haven’t had any heat issues with the VESCs yet but my rolling hills aren’t as bad as SF hills.
```

---
## \#26 Posted by: evoheyax Posted at: 2016-09-29T17:10:48.414Z Reads: 266

```
The only problem with the v2.5's is the lower top speed. I need to be able to hit 40 mph at times...
```

---
## \#27 Posted by: guyguy Posted at: 2016-09-29T21:48:21.937Z Reads: 268

```
@jinra @runplayback Not sure if this is right or current but jacoby mentions that using the RPM limits on the motor configuration tab can be dangerous since the hard limit can throw you off the board (See 28 minutes into the video below). He limits the speed on his board using the Soft RPM limits in App Configuration > PPM (See 55 minutes into the video below). 

https://www.youtube.com/watch?v=5HLZaMcYRuY
```

---
## \#28 Posted by: Jinra Posted at: 2016-09-29T22:47:00.724Z Reads: 258

```
I was talking about the eRPM limits in the motor tab, not the soft/hard cutoffs on app config. AFAIK hitting the limit in the motor tab just prevents it from accelerating, but doesn't cut off.
```

---
## \#29 Posted by: guyguy Posted at: 2016-09-29T23:07:01.619Z Reads: 251

```
Yep, that's the one jacob is talking about in the video, Max ERPM under motor tab (it's actually at 29 minutes not 28) he says he wouldn't use those settings b/c it's hard rpm braking. Jacob may be wrong, I don't know - just want to put that out there if anyone wants to test out Max ERPM. 

Have you used this to limit your speed? it looks like runplayback was never that close to hitting his. 

P.S. love your honey driver build.
```

---
## \#30 Posted by: Davideariel Posted at: 2016-10-01T18:09:02.690Z Reads: 241

```
nice build man, i have the exact same setup but with a drop down board.

can you please share the final vesc configuration?

p.s. i saw a video about you on youtube
```

---
## \#31 Posted by: Jinra Posted at: 2016-10-01T19:46:49.521Z Reads: 233

```
I haven't used it to limit speed, but i think you're right soft cut off via ppm settings is probably better. Ideally you'll want to setup for the right rpm.
```

---
## \#32 Posted by: STREETSURFER Posted at: 2016-10-01T21:36:12.033Z Reads: 225

```
My vesc shuts down after I brake suddenly or go up a long hill. I am running a carvon v2 single hub, 12s4p custom pack, and an enertion vesc.
```

---
## \#33 Posted by: scottkellum Posted at: 2016-10-02T13:12:09.027Z Reads: 222

```
Hey @Davideariel, here are my VESC settings: https://www.dropbox.com/s/03kj9d55xdtgsaw/vesc.xml?dl=0

I just tweaked the battery settings slightly and haven’t ridden with the new settings much. Hope you’re enjoying your build!
```

---
## \#34 Posted by: Jinra Posted at: 2016-10-02T14:43:21.996Z Reads: 216

```
Hey Scott,

Am i wrong or is your battery cut off start set to 3.5v? I'm assuming you want it to be 35v. Also if you want a little more power and responsiveness, you can probably raise the battery max to 45-50a (60 max).
```

---
## \#35 Posted by: XIII Posted at: 2016-10-02T15:14:49.860Z Reads: 221

```
But he is running dual vesc's ? 

So if he has the fuse still in (space cell pro 4), 20A each

And with the fuse out , 40 each

Doing almost the same build and was wondering about these high battery max
```

---
## \#36 Posted by: Jinra Posted at: 2016-10-02T15:24:02.657Z Reads: 220

```
oh right, for some reason i thought he was running single.

you won't blow out the fuse with over 20a per VESC though. it'd have to exceed 40A for a while to blow.

i ran 40a x2 VESCs battery max for weeks without blowing my fuse, and i ride a lot of hills
```

---
## \#37 Posted by: scottkellum Posted at: 2016-10-03T14:34:57.011Z Reads: 223

```
Oops, thanks for catching battery cut off voltage! totally typod it, fixed now. + @Davideariel
```

---
## \#38 Posted by: scottkellum Posted at: 2016-10-05T00:37:40.760Z Reads: 222

```
Got a power glove, hacked together with the existing transmitter and lots of work to do to clean up the signal but initial testing is going well!
https://www.youtube.com/watch?v=6MCYm19PUq4
```

---
## \#39 Posted by: Jinra Posted at: 2016-10-05T00:43:23.682Z Reads: 213

```
I love it, it's so bad.
```

---
## \#40 Posted by: scottkellum Posted at: 2016-10-05T00:50:26.635Z Reads: 213

```
yeah… working on making it not bad, literally just soldered into the existing throttle control and looked at the levels.
```

---
## \#41 Posted by: guyguy Posted at: 2016-10-05T00:50:27.780Z Reads: 207

```
wow love it
```

---
## \#42 Posted by: Jinra Posted at: 2016-10-05T00:52:43.084Z Reads: 206

```
lol I was just making a reference to the movie the wizard. It's actually pretty amazing. Good luck on development!
```

---
## \#43 Posted by: anon33082420 Posted at: 2016-10-05T01:21:51.927Z Reads: 207

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#44 Posted by: scottkellum Posted at: 2016-10-05T01:28:22.886Z Reads: 213

```
Yup! Just one and trying to figure out how to wire it to get a clean signal. Soldering directly onto the rotation sensors and adjusting the levels on the VESC at the moment, not super clean but does the trick. I may need to figure out some amplifier setup on the bend sensor to get better levels.
```

---
## \#45 Posted by: anon33082420 Posted at: 2016-10-05T02:55:28.275Z Reads: 215

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#46 Posted by: scottkellum Posted at: 2016-10-06T02:29:31.847Z Reads: 209

```
https://youtu.be/OdWjv5eeF2Q got it working smoothly and it feels so good to ride with this glove. Now need to make some sort of case for it but went smoother than expected.
```

---
## \#47 Posted by: Jinra Posted at: 2016-10-06T03:34:24.924Z Reads: 211

```
Looking good! Maybe you can design some kind of kill switch on it? I imagine bracing for a fall on these might lead to disaster.
```

---
## \#48 Posted by: scottkellum Posted at: 2016-10-06T04:06:27.567Z Reads: 205

```
I’ve been debating the pros and cons of a dead man’s switch and right now having one seems more dangerous than not having one. This is because the neutral position is somewhat hard to find so if the glove is disengaged and then reengaged there may be a jolt of acceleration or braking if it’s not in the correct position. I also want to get the hang of this and find the right position for a switch that feels natural instead of just adding one. This is based off natural hand gestures and right now holding my hand up to stop while forgetting to engage the dead man’s switch is more of a concern than having the board run away from me when I fall. I did add a big fat on/off switch that can be easily toggled with gloves or any other blunt object in case of an emergency.

I’ll work on these issues. First I plan on putting a metal with good shape memory and elasticity into the drive finger to guide me back to a neutral position and then feel out a good place for the dead man’s switch. Right now I’m thinking a contact point between my index and ring finger but need to feel it out more.
```

---
## \#49 Posted by: anon33082420 Posted at: 2016-10-06T04:49:11.582Z Reads: 197

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#50 Posted by: scottkellum Posted at: 2016-10-28T13:53:53.505Z Reads: 185

```
Just got thrown riding with the power gloves, good thing I was wearing full pads, a leather jacket, and (power) slide gloves. The fall really sold me on the safety of gloves but the remote mechanism isn’t the safest thing in the world, I gotta work on that.
```

---
## \#51 Posted by: onloop Posted at: 2016-10-28T14:02:11.703Z Reads: 179

```
That sux man. I hope your ok.
```

---
## \#52 Posted by: scottkellum Posted at: 2016-10-28T14:17:50.972Z Reads: 187

```
Totally fine, thanks!
```

---
## \#53 Posted by: JullianS Posted at: 2016-10-29T07:53:30.690Z Reads: 185

```
Hey man, nice build and wow the power gloves must be amazing to ride ! Good to hear you're fine after that fall ! 

I like that slot you made for the electronics by removing a layer of wood, I tried doing the same, and this is what happened : 
<img src="/uploads/db1493/original/3X/9/f/9f4aa3315097548f04b6f6e4d264fa5c389b7873.jpg" width="183" height="250">

Completely uneven, some dips go down to the last layer... good thing it was a dummy board, do you have any advice on chiseling ?
```

---
## \#54 Posted by: Mrmoonlight Posted at: 2016-10-29T15:28:24.375Z Reads: 183

```
Ply doesn't chisel well. I would use a trimmer(router) or sand it out with a dremel or belt. I say trimmer because they're smaller. It's easier to keep the contour of your board with a smaller base. If you have a router, make sure your bit is sharp and cut the edges first. Then leave channels as you cut the rest so your router base has something to rest on. Once you only have the channels left, you can use a hand plane to cut them down. If you go the sanding route, chisel out the edges so you have a clean look, then dremel/sand down to your desired level. A scraper can help you make it all level.
```

---
## \#55 Posted by: scottkellum Posted at: 2016-10-30T14:45:10.686Z Reads: 169

```
If you want to do it right, using a chisel is not the right way. I ran with it but it’s not necessarily a path I’d recommend to others.
```

---
## \#56 Posted by: Cole4242 Posted at: 2016-12-05T15:20:51.907Z Reads: 142

```
Hey man, really like what you have done to your board. I am new to eboards and was wondering what type of hub motors you have on your board? Is there a 'sweet spot' in choosing the best motor or is personal preference?
```

---
## \#57 Posted by: scottkellum Posted at: 2016-12-05T16:27:22.603Z Reads: 148

```
I have Carvon v2 hubs, they are awesome. v3 are launching _very_ soon and they look amazing. I highly recommend them, power and ride quality of full size wheels direct driven by big motors is fantastic. Also their customer service has been top notch and he always replies to my questions right away.

Down sides may be that they are kind of pricy, would be cool if they were sensored, idk if v3 will be sensored. Basically sensors allow for better starts from a standstill in FOC but it’s not a big deal as I usually push off to start anyway.
```

---
## \#58 Posted by: Cole4242 Posted at: 2016-12-05T16:52:19.129Z Reads: 152

```
Thanks for the info. I noticed that your motors are outside the wheels. Is this a preference or does it increase performance?
```

---
## \#59 Posted by: scottkellum Posted at: 2016-12-05T17:18:12.004Z Reads: 158

```
Yeah, it may not look as pretty but it means the motor can be bigger without having to take away space from the urethane of the wheel. With v3 the wheels are not modified at all so the ride quality should be even better. I’m a big fan of Carvon and will be a return customer in the future for sure. cc @LEVer who makes the motors
```

---
## \#60 Posted by: sequoia00000 Posted at: 2017-09-27T20:08:40.170Z Reads: 97

```
I can't find where to purchase the carveon hub motors, where did you buy them if they don't offer them on their site?
```

---
## \#61 Posted by: willpark16 Posted at: 2017-09-27T20:12:35.275Z Reads: 100

```
These are no longer sold
```

---
## \#62 Posted by: scottkellum Posted at: 2017-09-27T20:41:12.430Z Reads: 97

```
As @willpark16 said, they are no longer sold, the store is here: https://www.carvonskates.com/store/c1/Featured_Products.html and you can probably use the  contact form to inquire about just the drives
```

---
## \#63 Posted by: sequoia00000 Posted at: 2017-09-28T18:42:56.378Z Reads: 90

```
Thanks bud! :slight_smile:
```

---
## \#64 Posted by: Blitz Posted at: 2018-06-24T17:48:02.188Z Reads: 43

```
what happened to this guy?
```

---
