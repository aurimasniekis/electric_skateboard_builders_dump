# First Build. Need help deciding everything!

### Replies: 37 Views: 2207

## \#1 Posted by: bigredbakery Posted at: 2016-09-19T04:00:41.864Z Reads: 176

```
Hello, 

I have built a few regular longboard before but I want to try to built an E-board. I have been doing alot of research but am still confused by some of the electronics. Hoping for a board that has a 10 mile range with a top speed around 22mph. Here is what I am thinking for components so far:

**Board:**
A custom board from ebay
<img src="/uploads/db1493/original/3X/5/8/5818fa4c316c0d51079074c63f2378e3184c29f1.jpg" width="281" height="500">
**wheels:**
Orangatang Kegel 80mm 80a
I want the purple 83a more but they seem to be hard to find.
**Controller:**
I want to eventually build a wii nunchuck but in the mean time I got one from another user - http://www.electric-skateboard.builders/t/mini-remote-group-buy-part-3-10-remotes-36-for-one-or-two-for-70-shipped-usa-ordered/9136
**Motor:**
where I need some help. I would like a single motor with a little more power so I was thinking of getting a Turnigy Aerodrive SK3 6364 213kv or 245kv. Let me know if this is a stupid idea.
**ESC:**
I am probably going to get a VESC but does it matter where I get it from? Enertion? Carvon? 
**Battery:**
This is probably where I need the most help deciding. I don't think I have the ability to make my own battery packs. It seems like alot of people have two 6S batteries. Is there a reason people don't just buy a single 12C battery. Also if I buy two batteries do I need to get two of anything else to go with each battery. For 6S batteries I was looking at the Zippy 5000mah 30C http://www.hobbyking.com/hobbyking/store/__8590__ZIPPY_Flightmax_5000mAh_6S1P_30C.html
but is the 30C too much because there is 20C and 50C.
**Mounting:**
was planning on getting 12:36 ratio with 5mm pitch but I don't know what the best belt width would be (9mm, 12mm, or 15mm) 
I don't like the idea of welding the motor mount to the truck so I was looking into 3d printed mounts for the Caliber II's or having one machined. does the enertion mount work with a turnigy motor?
**Trucks:**
Caliber II

Thank you for helping me! Sorry if I am clueless!
```

---
## \#2 Posted by: michaeld33 Posted at: 2016-09-19T05:41:28.698Z Reads: 166

```
1. Purple Kegels aren't that hard to find... But the purple ones aren't as good. https://www.daddiesboardshop.com/orangatang-kegel-longboard-wheels-80mm
2. Don't mess with the nunchuck, trust me, I had one, and it's no good, these 2.4ghz remotes are much better.
3. Motor - go with the 245kv if you are using 6s.
4. VESC is fine but if you are going 6S you can always use a Car ESC, which is what I'd recommend.
5. That battery is fine.
6. Uhh, 12:36?? Noooo..... I'd recommend 16. On my 6S setup, I use a 20:36. With 12, the belt will skip ALOT and you will have no speed practically.
7. The Enertion motor mount is actually pretty good, so I'd go with that, it will work fine with the SK3.

Here is the calculated speed with what you recommended: 
13.59mph with the 245kv motor
11.82mph with the 213kv motor.

With what I recommended:
18.12mph with the 245kv motor and the 16:36 gear ratio. But 6S with an 80mm wheel setup won't get you very fast. The fastest 6S setup is with a 20:36 ratio, which is not reccomended by many.
```

---
## \#3 Posted by: bigredbakery Posted at: 2016-09-19T13:48:15.109Z Reads: 150

```
That's too bad about the nunchuck.

Would this ESC be good for 6S? http://www.hobbyking.com/hobbyking/store/__33984__TrackStar_150A_GenII_1_8th_Scale_Sensored_Brushless_Car_ESC_PC_Programmable_.html

Does the 30C rating for the 6S battery matter much? also if I go with two 6S batteries in series do I need to get two of anything else to go with each battery?

Thanks for the tip about the gear ratio. I will definitely go with your suggestion.
```

---
## \#4 Posted by: michaeld33 Posted at: 2016-09-19T18:17:41.883Z Reads: 130

```
That's pretty expensive, I used an X-Car hobbyking esc. Very inexpensive
```

---
## \#5 Posted by: sl33py Posted at: 2016-09-19T19:01:21.744Z Reads: 131

```
[quote="bigredbakery, post:1, topic:9822"]
wheels:Orangatang Kegel 80mm 80aI want the purple 83a more but they seem to be hard to find.
[/quote]
Good choice - like Michaeld33 said - i would go with the softer orange vs purple (80a vs 83a duro).  Softer will help with bumps and rough roads better.  Larger wheels also help, but those are a great wheel.

[quote="bigredbakery, post:1, topic:9822"]
Controller:I want to eventually build a wii nunchuck but in the mean time I got one from another user - http://www.electric-skateboard.builders/t/mini-remote-group-buy-part-3-10-remotes-36-for-one-or-two-for-70-shipped-usa-ordered/9136
[/quote]

I've seen far too many signal loss issues to recommend anything except the GT2b.  Yes it's a bit bulky, but for $25-30 it's a rock solid steal.  Then pay to get a new enclosure printed, or print one if you can for really cheap.  A few hours if you go super slow max to swap into the smaller pocketable enclosure you get printed.  (badwolf (a bit thin walled and flimsy so don't recommend any longer), mad munkey, baby buffalo (thumb throttle), master cho - pick one)

[quote="bigredbakery, post:1, topic:9822"]
ESC:I am probably going to get a VESC but does it matter where I get it from? Enertion? Carvon?
[/quote]

The best IMO are @Chaka's.  A bit more $ though.  If on a super budget i might try the [new vendor who's running a "pre-order" special](http://www.electric-skateboard.builders/t/83-vesc-from-axle-pre-order/9240).  @torqueboards has always been solid for me too, but i don't think there is any warranty on them unless purchased additionally.

For a moderate setup (10s or less) and BLDC (not FOC), with lower kv motor so you avoid the 60k ERPM trouble zone (more than this looks to kill DRV chips - why we've usually said no 200kv or higher on 12s), just about any of the current crop of VESCs i think will work for you.  If you are pushing the limits, you might want @Chaka's with additional cooling and some updated caps at select locations.   

[quote="bigredbakery, post:1, topic:9822"]
Battery:This is probably where I need the most help deciding. I don't think I have the ability to make my own battery packs. It seems like alot of people have two 6S batteries. Is there a reason people don't just buy a single 12C battery. Also if I buy two batteries do I need to get two of anything else to go with each battery. For 6S batteries I was looking at the Zippy 5000mah 30C
[/quote]

Batteries will usually depend on your board and both wheelbase room to install them, and ground clearance (flex of the deck or ride height).  I prefer smaller batteries in series for flexibility vs one big honking battery - usually cheaper, smaller, and cheaper!  So flexibility wise i can run 2x 3s for 6s, or 3 x 3s for 9s, or 4 x 3s for 12s.  Or give it to a friend to try and take a few out for 6s (lower speed and less "punch" power).  Not quite "modes" like production boards (Boosted, Evolve, Marbel, etc.), but better than handing a 12s super powerful board too a noobie and watching them crash or hurt themselves.

I target a capacity and C rating that "claims" (i don't really believe their marketing) about 100 amps continuous discharge capacity.  So a 5000mAh 20c or better (20c * 5Ah = 100a).  I wouldn't look at the 65c batteries unless they were just the smallest size and density you wanted an the c was bonus.



[quote="bigredbakery, post:1, topic:9822"]
Mounting:was planning on getting 12:36 ratio with 5mm pitch but I don't know what the best belt width would be (9mm, 12mm, or 15mm) I don't like the idea of welding the motor mount to the truck so I was looking into 3d printed mounts for the Caliber II's or having one machined. does the enertion mount work with a turnigy motor?
[/quote]

12t on the motor - don't do it on 9mm.  You *might* be able to do it on 12mm wide belt, but 9mm will skip.  15mm also would work i think.  I would not go below 12 and prefer 15mm for a single setup.  But i'm a heavy guy and skipping can be an issue.

motor mounts - DIYes, Enertion - both good mounts and solid IMO.  There are also quite a few others if you want to save a few $.  Just keep an eye on the motor pulley and wheel pulley costs to compare w/ a full kit that has both pulleys and a belt designed to fit.  usually it's cheaper to get the kit than parts.

I would also look out for wheel bite on a top mount deck w/ that shape.  Shouldn't be too hard, especially since you are only running 80mm kegels.

wheel gears and kegels - i think only @torqueboards has 12mm wide kegel pulleys.  You should confirm and look elsewhere too, or look at 3d printed options.  Less durable, but work pretty well it seems (with a good print of a good file).

HTH - GL!
```

---
## \#6 Posted by: Lsalt Posted at: 2016-09-19T19:08:23.137Z Reads: 102

```
Micaels calculations were not exactly correct. I would go with the 213 and depending on your weight 12-16 on the motor pulley.  has good options for that. Also if you would like a calculator that takes the guess work out of battery kv and gear ratio try Rc Calc on Android app store. You can see what speed and gear ratio plus battery voltage  and wheel size will do. If you want to go 22 I would aim for 30 or more that way you are not sluggish
```

---
## \#7 Posted by: michaeld33 Posted at: 2016-09-19T21:39:50.942Z Reads: 87

```
Sorry man, but I'm pretty sure my calculations are correct, I plugged them right into the same calculator everyone else on the forum uses, MADE for calculating the speed (including weighted speed) of electric skateboards. It's possible I inputted a number wrong, but the calculations were fine. You'd be getting a max speed of 15mph with a 213kv motor and a 16:36 gear ratio. So that's wayy off. If it was unweighted, it COULD hit 20, but you're not accounting for the efficiency of the motor when you're standing on the board. (around 70-90%)
```

---
## \#8 Posted by: michaeld33 Posted at: 2016-09-19T21:40:54.149Z Reads: 86

```
<img src="/uploads/db1493/original/3X/b/4/b4ee239b087f3744a493dfd12ba6f6b4fb0bad12.png" width="690" height="348">

Please don't say I'm wrong unless you're positive you're right.
```

---
## \#9 Posted by: Lsalt Posted at: 2016-09-19T21:55:29.908Z Reads: 86

```
Motor kv times battery voltage gives motor rpm. 
213 with 6s (25.2volts) = motor will spin 5367.6 rotations per minute 
Now divide that by your gear ratio. 12 goes into 36, motor turns 3 times and wheel turns once.
5367.6/3= 1789.2
This is how many times the wheel will spin in one minute. 
Now how much distance will the wheel cover in one rotation?
83mm wheel, divide by 2 to get radius= 41.5mm 
Times pie by 2 them by radius for circumference of wheel.
10.265748 inches
X 1789.2 rotations =18,367.4763216 inches a minute
X 60 mins
1,102,048.579296 inches 
Divide 12 for feet
91,837.381608
Divide mile 5280
17.3934434864 mph
So just plug numbers into this calc if you want specifics
```

---
## \#10 Posted by: Lsalt Posted at: 2016-09-19T22:00:12.404Z Reads: 79

```
I guess at 70 percent that would be 12.17 mph. On the low side
```

---
## \#11 Posted by: Lsalt Posted at: 2016-09-19T22:03:07.485Z Reads: 78

```
That is making calc when the battery is ran out. 3.7 per cell and I did 4.2
```

---
## \#12 Posted by: michaeld33 Posted at: 2016-09-19T22:06:20.034Z Reads: 76

```
3.7volts is _nominal_ voltage and will provide an accurate average ride speed. You don't need to defend your calculations, they're fine, but you have to take into account a couple things.
```

---
## \#13 Posted by: Lsalt Posted at: 2016-09-19T22:12:19.534Z Reads: 80

```
I never said he would do 20mph with his current setup.
My recommendation is that he should stay with a low kv motor for torque and depending on weight he should use a higher battery voltage than 6s. He should also run around a 12-16 teeth pulley depending on weight. I don't see anyone encouraging anything in the mid 200 kv motors anymore. Especially if he wants to run vesc. That's all I am saying
```

---
## \#14 Posted by: michaeld33 Posted at: 2016-09-19T22:22:07.302Z Reads: 79

```
But that's because most people don't RUN 6s with the VESC, trust me, I had a very similar setup to this on my first board, with a 149kv motor and a 16tooth pulley, and it was MISERABLE! If he want's to do 15mph, then that's fine, but it's not that fun IMO. I run a 6S 245KV on my board with a 20tooth pulley, that gets me to just about 30 mph easily. The reason it's not often heard about is because not many people who go 6S either know much yet, or don't want any speed, or want it for the simplicity.  >= 200KV isn't recommended for a 10-12S setup on the VESC because you will hit the ERPM limit, not because of them not being good. If you are willing to sacrifice ~5-7mph for torque, that's fine, but you will not have many occasions where you need that much torque. I have only ever found one hill I can't climb, and my setup uses an ~6355 size motor with a 20:36 gear ratio. AND I get really good speeds.
```

---
## \#15 Posted by: Lsalt Posted at: 2016-09-19T22:23:56.050Z Reads: 79

```
Also when he mention single 12c battery I'm pretty sure he meant 12s. So if he wants to run high volts on a vesc there's the erpm limit. So definitely get the 213 kv if that's the choices. :slight_smile:
```

---
## \#16 Posted by: zmoney Posted at: 2016-09-19T22:26:47.957Z Reads: 78

```
[quote="sl33py, post:5, topic:9822"]
If on a super budget i might try the new vendor who's running a "pre-order" special.
[/quote]

The name's Axel. James Axel. :joy: 

Anyway's we've closed pre-orders as of now. If you're still interested you can check us out at [goaxle.com](http://goaxle.com)  (extended until 9/23)
```

---
## \#17 Posted by: Lsalt Posted at: 2016-09-19T22:27:09.429Z Reads: 77

```
You're also forgetting there must be a reason he us saying 12t pulley. We need to hear back on his weight before you make any further  recommendations. 20t you must be very light.
```

---
## \#18 Posted by: michaeld33 Posted at: 2016-09-19T22:47:59.257Z Reads: 76

```
You will still hit the ERPM limit, and if you go with a 12T pulley, you will DIE! The belt will skip and it won't work well. AND **you will still hit the** **ERPM**.
```

---
## \#19 Posted by: zmoney Posted at: 2016-09-19T22:49:14.328Z Reads: 76

```
[quote="michaeld33, post:18, topic:9822"]
you will DIE!
[/quote]

That's a nice way to put it
```

---
## \#20 Posted by: michaeld33 Posted at: 2016-09-19T22:58:47.883Z Reads: 73

```
I used to have a belt that skipped. Couldn't break in time, almost flew right into traffic. Thankfully I was able to save myself.
```

---
## \#21 Posted by: Lsalt Posted at: 2016-09-19T22:59:39.230Z Reads: 67

```
Lol you wont die. I run 13t. Have to tighten well cuz does slip very little when it's warm. Heres a good read about erpm. It has its limits and wiggle room. You will however be dissapointed with 245kv on vesc. 
http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#22 Posted by: zmoney Posted at: 2016-09-19T23:00:36.988Z Reads: 63

```
I would try looking for something like 190 KV or 200KV.
```

---
## \#23 Posted by: michaeld33 Posted at: 2016-09-19T23:00:53.768Z Reads: 62

```
I am very light. But I'm not the only one riding with 20T, there are other people on this forum who ride with it. I was actually given the pulley for a setup from a friend of mine. I have never heard of 12T pulley being used, if the weight of OP is really important, than a bigger motor would be more important, OP could use a 149kv motor, with MUCH more copper in it, run it with a 16 or 18 tooth pulley and still have all the torque OP needs.
```

---
## \#24 Posted by: Lsalt Posted at: 2016-09-19T23:01:27.431Z Reads: 61

```
Exacly. Reason is setting in here.
```

---
## \#25 Posted by: michaeld33 Posted at: 2016-09-19T23:01:53.115Z Reads: 62

```
I mean I almost did, the belt skipping isn't necessarily a problem except for the fact that it will destroy your belt, it's not being able to break.
```

---
## \#26 Posted by: Lsalt Posted at: 2016-09-19T23:05:26.634Z Reads: 65

```
We are not looking for extremes. We are looking for what is "optimal" :slight_smile:
```

---
## \#27 Posted by: Lsalt Posted at: 2016-09-19T23:07:19.009Z Reads: 66

```
It will be funny when the op shows up and corrects us all hahahaha
```

---
## \#28 Posted by: michaeld33 Posted at: 2016-09-19T23:07:53.850Z Reads: 69

```
I don't understand what you mean... In general, for anyone, I would recommend a board with a 190kv motor, a 10S battery, and a 16:36 gear ratio. For those that like 6s, I recommend a 245KV motor, 16(or 18):36, and 90+mm wheels.
```

---
## \#29 Posted by: Lsalt Posted at: 2016-09-19T23:14:41.993Z Reads: 64

```
He is saying 12s though....read it two 6s or one 12c...I think he means 12s
```

---
## \#30 Posted by: bigredbakery Posted at: 2016-09-20T02:20:10.804Z Reads: 52

```
Didn't mean to start a holy war. I did mean 12S.

I think I am going to go with a 213kv motor, 10S battery and 16:36 gear ratio. That seems to make the most sense.
```

---
## \#31 Posted by: michaeld33 Posted at: 2016-09-20T02:23:50.665Z Reads: 54

```
I know, I'm just saying that I don't usually recommend "extremes"
```

---
## \#32 Posted by: michaeld33 Posted at: 2016-09-20T02:25:01.069Z Reads: 52

```
Ehh well... Shot down... That setup sounds great! Should get you around 26-30mph
```

---
## \#33 Posted by: bigredbakery Posted at: 2016-09-20T02:25:31.764Z Reads: 54

```
Thank you for all your help!
```

---
## \#34 Posted by: bigredbakery Posted at: 2016-09-20T02:26:05.855Z Reads: 53

```
I'll try to remember to post pictures of the completed build here
```

---
## \#35 Posted by: michaeld33 Posted at: 2016-09-20T02:36:42.380Z Reads: 53

```
Are you going to turn this into a build thread? If so you should update the title to be the proper format.
```

---
## \#36 Posted by: Lsalt Posted at: 2016-09-20T05:59:13.451Z Reads: 53

```
Yup 10s would do the trick. Heres my 10s
5s series then parrallel. 10000mah <img src="/uploads/db1493/original/3X/2/f/2fb1dac573ac91769e68bd357b37a8e980e340de.jpg" width="666" height="500">
```

---
## \#37 Posted by: BexBle Posted at: 2016-11-07T22:16:02.982Z Reads: 40

```
how do i link them in parellel and series?
```

---
