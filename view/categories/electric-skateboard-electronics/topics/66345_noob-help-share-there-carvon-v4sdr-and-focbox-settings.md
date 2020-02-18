# Noob help.. share there carvon V4SDR and focbox settings

### Replies: 8 Views: 199

## \#1 Posted by: Frenchy Posted at: 2018-08-28T14:10:02.393Z Reads: 75

```
Ok folks I've been reading so much I know there is alot on that search section.. but I'm scrambled eggs brains.. and watching alot of videos how to set up vesc not much out there for the FOCBOX..lots of vedder style vesc setting..I'm very shitty with computers ..please be nice ..I'm terrible ..deeply sorry for the horrible question in advance....so I've gotten to the final part of tuning coming up next day or two..I've already don'e the basic bench test and setting what came with the focbox running the most upgraded version and what ever is stock setting on 57v . Set the detection but could not get the sensors to work..maybe it is and I'm just dumb...I set it up works on initial test but when I disconnect and unplug the USB the foc box and motors do nothing..works with USB installed while in the program .. it will only work sensorless off the program ...I haven't changed a thing and I'm running a split ppm set up..I have a canbus wire but I was very very nervous to use it as this is my first set up attempt...and plan to use it but one step at a time ...learning ....I've downloaded the enertion vesc tool.. I've set both up split ppm separately and they work on sensorless only off the vesc program..just wondering if the stock setting in the focbox fine for the carvon drive ...motor 40+ and 40- ..57v ..battery max 25 and Regen -12...I'm sure the stock setting wouldn't hurt the esc..I took for a quick five ten min boot couple days ago when I got it all together ..got no cut outs on the throttle and did not get hot at all the focs or the motors ...holy powerful motors Jesus it pulls so hard after 5km or so ...my God a 1/4 to 1/3 of the stick I don't think it was half throttle at all ...it fuckn pulled so hard to 40km easy before speed wobble kicked in...lost five pound of shit that moment..went home ...and there is the hole joystick left..so touchy ..lol..easy gonna be a 40 mph whip easy... I have a lil noise at the first second or two when i start to hit the breaks..the other I notice was when I hit the throttle with no load the wheels don't kick in right away together one will cog first.. but i don't feel this under my feet with a load tho..but unloaded it will bounce from one side to the other..its not the same motor doing it ..so lil confused..maybe this is from running non sensor??.is this normal?? ..mayby from splitting the ppm there is a delay to one vesc..??.I have a 12s2p 30q torque board battery i think the bms is 40amp max not 100% sure tho does anyone know what is the max bms on it..love to bypass it if i can ..any help with some setting and what ppl have to explain to get this tuning part wrapped around my head..and as for advanced tuning section can someone explain how all this works which figures I can play with and where to find..min and Max numbers to install....as I read a shit pile but some terms and language I have issues understanding and I find there is always a person that argues says something totally different and scramble my brains again..so if anyone can dumb it down would be amazing or share your v4sdr and focbox specs with me to try out ..or at least give me directions and  formulas to find what I'm looking for as I can do math I know most physics as I'm a electrician but do not know a thing on small electronics and motors..I work with big power..13000v min to 50000volt stuff..a grasp on low voltage getting there I think..LOL ..thanks for your time and help folks cheers.. 
PS..now if I should BE running the canbus wire for these drive and not split ppm.. a nice secure detailed way would be amazing ..I'd love to run foc and traction control and i want to get a bluetooth to run and watch my specs..but I'm terrible with computers and shit like this..just scared to melt the premium products..but I want to learn ..thanks alot folk cheers..
Here are my specs so far which is stock focbox settings..
![IMG_20180826_153228|666x500](upload://bwQomVNJGUnaRze8sFlTcLfEJKF.jpg)
![IMG_20180826_153254|666x500](upload://zg0k2AUmpKcuL8bNCojzThMbf7w.jpg)
![IMG_20180826_153305|666x500](upload://3CstFFdBxBWIp1GCNUGBZrsDIjK.jpg)
```

---
## \#2 Posted by: Saturn_Corp Posted at: 2018-08-28T16:46:08.230Z Reads: 57

```
I'm new to this as well and only finished up my carvon build a few days ago. Canbus is easy, you just have to secure it so it won't rattle around and get unplugged when your focboxes are on or else one might bite the dust. I myself am going to get a hot glue gun this weekend for the same reason.

I'm running:
motor max: 60
motor min: -55
batt max: 40
and that's more than enough for me right now. I'm happy at 30mph and this easily gets me there.
```

---
## \#3 Posted by: Frenchy Posted at: 2018-08-28T17:09:42.623Z Reads: 57

```
Thank you sir very much appreciated for the reply..there isn't much on the  speed drives from carvon .I know I weight 145 lbs and at 1/4 to 1/3 throttle that thing fucks right off haven't got enough balls yet to get passed 25 mph 40 km and to squeeze that trigger past a 1/3 throttle max so far..it pulls so hard..and there is a shit pile of throttle left..like I'm barely touching the remote it's a widow Maker that's for sure..I just want to ride it ..but nevous that it's set up ok before I go out beating this thing down and really trying this thing out..so from what I got now is alot less then your specs so I should be fine with out frying anything and I'll just add as I get use to it and grow on it ..thank you again much appreciated big time 
Cheers
```

---
## \#4 Posted by: Saturn_Corp Posted at: 2018-08-28T17:20:38.699Z Reads: 52

```
Yah you gotta be careful until you get really comfortable with it. Yesterday I was accelerating hard and let off the throttle only to almost fall forward off the board. I didn't, instead I lost balance and fell off the side and hurt my shoulder and knee. Still haven't taken it past 3/4 throttle except when I first start moving.
```

---
## \#5 Posted by: Frenchy Posted at: 2018-08-28T17:42:34.798Z Reads: 39

```
O shit I hope you heal up fast man..being hurt sucks ..i use to race quads and broke about 70,% of my body in just one accident ..I break a bone at least once a year snowboarding dirtbiking or skateboarding been to the hospital lots for months worst feeling ever being usless ...must take full caution as they are definitely wild motors..the mid range power is crazy..heavy lean into throttle ..I find it will break the tires loose on me if I'm leaning to forward ...reminds me of my Yamaha banshee on the boost bottle..and I haven't even experience the full throttle yet...I always push start I just skated most of my life from 10 im 34now..  just a common thing for me I always catch myself pushing around...and I say to myself hey dumb dumb you have a motor ..lol...so I don't really find them that weak in the low rpm..as ppl complain about..maybe cause they are alot heavier ..it don't have off the line power like my duel blink but after 10kmh I'll fuckn blow 🍩 around  that thing ..what size tires are you running ..I have 97 and 90 just not sure Which one to choose..I now Jarry said 90 for 2wd and 97 4wd..but it already has a pile of torque after 5kmh rolling it ..im really light at 65kg...and the 97just gonna make it top end faster which 30mph I don't think I want to pass any ways..I have some playing aroind to do I guess this weekend..thank you again for the help and information much appreciated
```

---
## \#6 Posted by: Saturn_Corp Posted at: 2018-08-28T19:12:55.956Z Reads: 32

```
I'm using 97mm flywheels. These things are like you're rolling on jello it's so soft. Although I weigh 120lbs. I agree with what you said about having enough power at low rpm, sometimes when I take off from a stop I'll start to wheelie on accident lol. Scares me a little bit every time. it definitely doesn't go up steep hills fast though, thankfully I live in a pretty flat area.
```

---
## \#7 Posted by: Saturn_Corp Posted at: 2018-08-28T19:16:56.948Z Reads: 31

```
What do you think of the sound they make? I like going under bridges and slamming the throttle, sounds like a TIE-fighter lmao.
```

---
## \#8 Posted by: Frenchy Posted at: 2018-08-28T19:29:06.661Z Reads: 31

```
Lol so you know what I'm talking about then..your a light weight like me..so for you to go up a steep hill make sure your going at least 20k and it will power up that hill from what I've been told  it will eat that hill at speed you have to be in the mid range ...I'll be doing a shit pile of testing this weekend..and the 74A flywheel are like Jello barly feel any bumps...and I'm use to driving a Acton blink s2 duel hub motor  so rough now I can't even ride it after my one ride on the carvon..and as for the sound of this this is so cool..I like the silent hubs before I got this ..now I just want to streight pipe it out like it's a race car or bike ..but no exhaust lol..love the sound ..doubt I'll go foc ..might try it ..but I think I fell in love with the sound..I've heard some gear drives and was on the iffy on the sound ....but this thing sound just fuckn awesome..
```

---
