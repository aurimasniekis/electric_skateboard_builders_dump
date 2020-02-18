# First Build - Arbor Axis &#124; 2 x TB 6355 190kv Motor + FOCBOX &#124; 10s3p 30Q&rsquo;s &#124; 97mm Flywheels

### Replies: 4 Views: 668

## \#1 Posted by: sumthingawsome Posted at: 2017-11-28T03:15:19.777Z Reads: 134

```
Hopefully I format this well. I'm in the middle of the planning/buying stage for my first build; had to jump on some of the Black Friday/Cyber Monday Deals. So, here's my (admittedly disgusting) parts list so far:
<img src="/uploads/db1493/original/3X/7/4/745f3bc429ca8427c339a0f7a589605240a1b4c1.png" width="690" height="224">
*[Original spreadsheet](https://docs.google.com/spreadsheets/d/11QZRE0WCPxqE9Y9JO9l0Eoi4Cb5y8tFge5CSbSeG9bE/edit?usp=sharing)*

I believe I'm just missing some electronics. I did jump on the 6355's that were on sale over the 6374's even though my campus is pretty hilly - do you guy think 2 x 6355 @ 10s, 36:14 gearing will give me decent enough power? I don't think I could've justified the jump in price for 6374's.

What I'm missing is BMS + Switch and a charger. I think I'm set on getting a cheap BMS to handle charging alone and an additional anti-spark switch for the FOCBOX's, e.g.:

* [Luna Cycle on/off switch](https://lunacycle.com/remote-on-off-solid-state-switch/)
* [The first Google result for "10s bms"](https://bmsbattery.com/bmspcm/713-10s-13s-30a-50a-lipo-battery-bms-system-bms-pcm.html)

Opinions and/or suggestions? Honestly I've had a hell of a time trying to find BMS's, but I'm trying to avoid group buys.

Finally, the charger - this is probably a stupid question, but what voltage am I looking at for a charger? I'm pretty sure 4.2V was the nominal voltage for the 30Q's, so is it as easy as 10 x 4.2 = 42V for a charger? Any suggestions for websites I can look at or a specific charger? Another potentially stupid question, but does/can the BMS handle cutting the charger off once all the cells are at nominal voltage? I just realized I had no idea what circuitry handled that, unless there's something inside chargers themselves that does it?

Anything else I've overlooked? Any suggestions, tips, pointers, etc. etc.? I appreciate any help I can get with this since it's my first build and goodness knows I'm gonna screw at least a couple things up!
```

---
## \#2 Posted by: ShutterShock Posted at: 2017-11-28T04:05:50.155Z Reads: 120

```
First thing, great job researching everything before posting and buying! Great to see someone that will be less likely to make a mistake.

Just gonna try to go through some questions in order:

Personally, I have a dual 6355 setup on my board, at 12S with the same gear ratio and 83mm wheels.  I am not sure how much more the larger 97mm wheels will affect your torque, but I assure you they will be a much nicer ride than my clone flywheels.  You made a great choice there.  If you find that you have issues with torque, you could switch the motor pulley to a smaller size and add an idler to squeeze some extra torque out of it.  My 6355 setup has not met a hill I can't conquer yet.  Granted I am only 150lbs ~ 68kg, but I haven't needed more power.  I run my motors sensored, with hybrid mode on my VESC and have no issues starting from a standstill either.  In other words, you will probably be fine, but there are ways to improve your setup later if need be.

You made a great decision going for FOCBOX's, as I blew one of my TB vescs for no reason?  I honestly don't know how, but one day it just threw a DRV error.  Anyway, I am upgrading to FOCBOX's and wish I had done it to begin with.  For your BMS, most quality ones come from SuPower (batterysupports.com) or Bestec.  Bestec requires a minimum order of two, which is why you see so many groupbuys.  There is a chance that @thisguyhere may have a left over 10s charge only BMS from the recent groupbuy but you will have to wait and see.  I picked one up from his groupbuy and have no problem trusting him as he is a seasoned member and is basically the groupbuy king :smiley:

You are correct about the charger.  It should be the 42V kind, with the same math that you did.  I would look at eBay for chargers, search for 42v Lipo charger, or 10S lipo charger, here is one that I came up with from a quick search. 
https://www.ebay.com/itm/42V-3A-Charger-for-36V-37V-LiIon-liPo-Two-wheel-self-balanced-vehicle-Battery-EU/321534184919?hash=item4adcee4dd7:g:p2MAAOSwVFlUJP9Y

You can simply chop off the connector and use an XT-60 or go ahead and find the female plug to connect to your board.

Other than that, the charger and BMS work together to ensure that your cells don't explode.  So assuming you wire it up right, there shouldn't be any problems.

Don't cheap out on your enclosure, you will probably regret it in the long run.  I 3D printed mine, and am pretty happy with it, but there are tons of people on the forum that make enclosures, you can find some of them here:
https://www.electric-skateboard.builders/t/enclosure-directory/37787?u=shuttershock
```

---
## \#3 Posted by: sumthingawsome Posted at: 2017-11-29T19:30:07.355Z Reads: 71

```
Thanks a bunch for your response, you answered a lot of my questions! I guess as far as motors go I'll have an upgrade path down the road with the large trucks at least, but it sounds like the 6355s will work for now.

Also yeah, I heard some bad stories about TB vesc's, so I decided to jump on that FOCBOX sale, and considering this is my first build I might be using that $40 warranty pretty soon too :eyes:.

I'll have to check out some of the group buys, I guess I shouldn't skimp on the BMS since buying 30 new batteries would be a shame, lol.
```

---
## \#4 Posted by: ShutterShock Posted at: 2017-11-29T19:42:40.068Z Reads: 67

```
Of course!  Glad to help.  The TB ones are usually hit or miss, pretty solid for the most part, but I would never have passed up on the focbox sale haha

I think you will be happy with the 6355's as well
```

---
