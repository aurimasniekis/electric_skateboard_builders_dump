# How-To: Fused XT90-S Anti-Spark Loop Key

### Replies: 32 Views: 5701

## \#1 Posted by: rpasichnyk Posted at: 2017-01-30T17:07:22.974Z Reads: 689

```
In the search of the high amp fuse I stumbled upon this. It is called strip fuse, very cheap and available for 30A, 40A, 50A, 60A, 80A, 100A. Since I'm going to use [Anti-Spark Loop Key](http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204) in my build I got the idea to combine the two.

<img src="/uploads/db1493/original/3X/d/f/dfe07334e334faf0d13939f0c81ce6359d34be3f.jpg" width="600">

The fuse is made of zinc, this metal is soft, easy to bend and cut. I shaped it a little bit with side cutting pliers.
<img src="/uploads/db1493/original/3X/1/c/1c005f2118bad3311274214ca1f2bfef4c13440a.jpg" width="400">
<img src="/uploads/db1493/original/3X/0/e/0eae27a10f6cc5795d4649a9cea569113fe49406.jpg" width="400">

Then I bent it and soldered to male part of XT90-S.

<img src="/uploads/db1493/original/3X/7/5/75817da74d95217073b538068eef139fbeeb3040.jpg" width="600">

I recommend soldering to the male part, not female like @sl33py did, because it is easier to screw up and accidentally short the male part and get some sparks if it sits in the skateboard. The male cap of XT90-S is also very cheap and easier to get, it is exactly the same as XT90 without S.

<img src="/uploads/db1493/original/3X/1/a/1a8077db991b87651d748b68a856161558bd281f.jpg" width="300">

Benefits:
• Cheaper than a MAXI car fuse
• Saves the space inside, doesn't need a fuse holder
• Easy to replace if you make 2 and carry a spare
```

---
## \#2 Posted by: jmasta Posted at: 2017-01-30T17:18:50.118Z Reads: 668

```
[quote="rpasichnyk, post:1, topic:16912, full:true"]
In the search of the high amp fuse I stumbled upon this. It is called strip fuse, very cheap and available for 30A, 40A, 50A, 60A, 80A, 100A...
[/quote]

Wow, good find!  I actually just made a loop key last night since my anti-spark switch got fried.  Now I want to make another using your technique


[quote="rpasichnyk, post:1, topic:16912, full:true"]
I recommend soldering to the male part, not female like @sl33py did, because it is easier to screw up and accidentally short the male part and get some sparks if it sits in the skateboard. The male cap of XT90-S is also very cheap and easier to get, it is exactly the same as XT90 without S.
[/quote]

I agree with this... with one caveat.  You're right that it would be better to have the XT90S male wired inline with a female XT90 loop key; with the key disconnected, a female "live" end is much easier to accidentally connect the poles**.  BUT I would only recommend this if you are NOT using XT90 connectors anywhere else in your build. I almost wired my loop key just as you've described, but my battery pack has a XT90S male output.  Building a female XT90 loop key would mean I also just built a "shorting adapter"... aka a very convenient way to blow up my battery, if for some reason it was hooked up incorrectly


**NOTE: With a loop key, touching the two poles together would not actually be a short in this case. It would just connect the circuit.
```

---
## \#3 Posted by: wmj259 Posted at: 2017-01-30T19:30:48.362Z Reads: 577

```
Is it strong enough to be pulled out?
```

---
## \#4 Posted by: sl33py Posted at: 2017-01-30T23:27:44.814Z Reads: 559

```
[quote="rpasichnyk, post:1, topic:16912"]
I recommend soldering to the male part, not female like @sl33py did, because it is easier to screw up and accidentally short the male part and get some sparks if it sits in the skateboard. The male cap of XT90-S is also very cheap and easier to get, it is exactly the same as XT90 without S.
[/quote]


Cool writeup and pics.  This would be great to add to any loop key as added insurance (fused).

One thing though - This has no anti-spark as you have it setup now.  This is just a fused xt-90 loop key.

Adding this exact setup to the anti-spark loop key would be super simple and give you the best of both worlds (anti-spark, AND fuse).

HTH
```

---
## \#6 Posted by: PXSS Posted at: 2017-01-31T02:37:26.565Z Reads: 535

```
He has the female XT90-S on the other side. 

@jmasta. I think you have female and male confused. The male is the one with the male bullets in it, the female is the one with the female bullets in it. XT90-S only come in female variant.

E: If you plug in your loop key directly to your battery, you have bigger issues and should honestly not be building these :joy:

XT90-S anti spark were made to replace the battery connector (female) and not the way many in here do it where they solder a male to the battery. It is extremely bad practice to solder any kind of male connector to a battery as it could easily be shorted by a metallic surface or any conductive debris.

E2: Regarding @jmasta note, absolutely not. Touching both terminals of the batteries with your hands will not kill you... Where did you get that from????
```

---
## \#7 Posted by: jmasta Posted at: 2017-01-31T03:06:17.118Z Reads: 525

```
[quote="PXSS, post:6, topic:16912, full:true"]

@jmasta. I think you have female and male confused. The male is the one with the male bullets in it, the female is the one with the female bullets in it. XT90-S only come in female variant.[/quote]

I'd argue that is up to interpretation.  Yes, the XT90S plug has embedded female bullet connectors, but it physically goes into the XT90 socket. It that sense it can be viewed as either male or female. Even the internet disagrees:

Plug defined as female:  http://www.getfpv.com/xt90-power-connectors-female.html

Same plug defined as male:  https://hobbyking.com/en_us/nylon-xt90-connectors-female-5pcs-bag.html
```

---
## \#8 Posted by: PXSS Posted at: 2017-01-31T04:55:38.855Z Reads: 520

```
@jmasta 
Straight from the authentic manufacturer Amass website: 
AMASS female XT60 connector with 12awg soft silicone wire AM-9024B
<img src="/uploads/db1493/original/3X/9/f/9f73d5c5d01c08e76b2b6f08941a97b5f0c6422f.jpg" width="500" height="500">

I did not mean to offend you and no I dont know you but it's true, its bad engineering to put male plugs on a battery. Check literally all LiPo makers that have XT, EC or Deans connectors and tell me which end is on the battery.This is done for a reason. If you are making a design with a loop key in it then obviously you can take precautions but if you connect a short across your battery, that is on you for being careless. Not that you'd ever be able to get the whole thing on (just ask one of our interns who shorted a 10S10P pack. Spoiler, the bullets melted and sparks flew everywhere as he dropped the connector). If you are the designer and only user, you should know your system well enough to not make that kind of mistake.

By the way, here's proof you cannot kill yourself holding both terminals of a 10S4P pack. I've also done this on a 10S10P pack but cannot post pictures

<img src="/uploads/db1493/original/3X/3/9/3920320477bebbe8512cf1521563d2f33e2fe811.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/4/f/4fb6cc5eef09a84807b2bf76fc430b79f0f3d804.JPG" width="375" height="500">

Sorry for the crappy angle on the second picture.
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2017-01-31T05:09:58.622Z Reads: 478

```
[quote="PXSS, post:8, topic:16912"]
By the way, here's proof you cannot kill yourself holding both terminals of a 10S4P pack. I've also done this on a 10S10P pack but cannot post pictures
[/quote]


HUMMM.... you also won't kill yourself if the current doesn't pass trough you heart.... Current will always choose the shorter way... and on the picture you've just shown current will only pass trough your hand :wink:
```

---
## \#10 Posted by: jmasta Posted at: 2017-01-31T05:10:52.211Z Reads: 485

```
You're using one hand. I specifically said touching the negative terminal with your other hand.  Those are very different scenarios

I edited my post so as to not scare away newcomers. However, 50V (12S) is often defined as the threshold at which many OSHA regulations begin to apply.  While it is not likely, serious injury is still possible

 > Exposure to 25V is also clearly safe with no risk to human life. It is only when we reach around 50V that we start having issues with shocks that are capable of delivering more than 13.5 W-sec in less than 3 sec. At 50V, the power equals 5W, and the calculated exposure time is 2.7 sec. (5 × 2.7 = 13.5). This assumes a “worse-case” body resistance of 500 ohms. Most people in reasonably good physical and mental shape can still react quickly enough to release themselves in 2.7 sec or less from a 50V shock. When the voltage level is 50V and above, however, it delivers too much energy in less than 3 sec, which leads to electrical fatalities.


But you are right on the naming convention. My bad!  Either way, male/female is a pretty confusing way to describe an XT connector.  Most people would probably (incorrectly) classify the XT90S as male.  It's 2017 and even our connectors don't know what sex they are anymore!!!
```

---
## \#12 Posted by: PXSS Posted at: 2017-01-31T05:58:22.957Z Reads: 480

```
@jmasta, @JohnnyMeduse  
Second picture is of me using both hands. That's why the angle is so weird. I couldnt find a way to hold probes with both hands and take a picture with my phone...

Better shot. 
<img src="/uploads/db1493/original/3X/7/5/75b31ccc06195e929a10d8341741168a64c10b50.JPG" width="666" height="500">

Also 500ohm resistance?!? Is the test subject drenched in sweat and are we applying paddles to the chest? At 100V the NIOSH states hand to hand resistance with a large contact area circuit with dry skin as:

5% population under 1200ohm
50% population under 1875ohm
95% population under 3200ohm
```

---
## \#13 Posted by: jmasta Posted at: 2017-01-31T06:06:42.545Z Reads: 468

```
Now lick them!  

:joy:

Male is female. Female is male. We're not going to die! #alternativefacts

<img src="/uploads/db1493/original/3X/9/9/9985f3344cb643311167a426ea228eaa2348be77.jpg" width="690" height="387">
```

---
## \#14 Posted by: PXSS Posted at: 2017-01-31T06:08:14.812Z Reads: 457

```
Erm ok...
I take it, you dont take being wrong well...
```

---
## \#15 Posted by: jmasta Posted at: 2017-01-31T06:10:32.085Z Reads: 448

```
That was a joke. I honestly stopped caring
```

---
## \#16 Posted by: PXSS Posted at: 2017-01-31T13:19:02.310Z Reads: 431

```
@rpasichnyk
Have you tried to burn one? I am going to order a few strips since this would be nice and cheap to make.
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2017-01-31T14:04:19.335Z Reads: 428

```
PLEASE.... you should know that wikipedia can't be a justifiable source... Also in the case of electricity and current, what is not killing you make you weaker. 

so here a interesting article about exposure to low voltage:


http://bme.ccny.cuny.edu/faculty/mbikson/BiksonMSafeVoltageReview.pdf
```

---
## \#18 Posted by: PXSS Posted at: 2017-01-31T14:20:04.727Z Reads: 416

```
Wikipedia? When did I state that as my source?
In fact the paper you linked has the same resistance values I posted earlier... (Page 5 Table 1)

I will read it fully tonight!
If there are any specific sections you want me to read, by all means let me know. Section 3, accidental electrocution looks interesting
```

---
## \#19 Posted by: rpasichnyk Posted at: 2017-01-31T19:55:05.901Z Reads: 405

```
I am going to make a test this weekend. Can't think of other 50A power source so will just put a LiPo in a fireproof bag and do it outside for safety reasons.
```

---
## \#20 Posted by: PXSS Posted at: 2017-01-31T20:07:21.302Z Reads: 407

```
I ordered a few 60A ones. Will let you know how that goes when I get them
```

---
## \#21 Posted by: wmj259 Posted at: 2017-01-31T20:43:37.850Z Reads: 405

```
I touched a tube lighting end connector with my hand by accident when I was trying to align the two  end probes that's stick  out of it to the housing. You feel this heat jump through your body when the electricity passes through you. Lucky enough my hand came off or it could have done more damage.
```

---
## \#22 Posted by: PXSS Posted at: 2017-01-31T23:12:40.381Z Reads: 391

```
Isn't that 110VAC?
```

---
## \#23 Posted by: wmj259 Posted at: 2017-01-31T23:16:58.404Z Reads: 346

```
I believe so it was in the basement. Amps do the damage, but as said before it only went through my hands. but your whole body feels hot AF.
```

---
## \#24 Posted by: PXSS Posted at: 2017-02-01T01:20:31.984Z Reads: 370

```
@wmj259 
That's a whole different story. Not only are you talking about 110V but also alternating current. 

110V is more dangerous than 42V. And current is not the only thing that matters. Human's skin resistance is not a constant, it decreases as the voltage rises as shown in the paper above, and can also vary from person to person based on health and other factors according to what I've read. As the skin burns, it's resistance drops too. At which point a current of only a few milliohms can kill you over several seconds. 

Truth is, 42V on dry skin with a small contact area, like the ones we deal with are not dangerous at all. I've assembled tens of battery packs by hand now, anywhere from 4S1P to 10S10P and never had an issue getting shocked and I constantly handle both terminals of the packs. The only time I've ever felt slight electricity flowing though me is when my forearm or hand is resting across several cells in series which feels almost identically as getting poked by untrimmed nickel tabs. Half the time I'm unsure which happened. 

110VAC is inherently more dangerous as the voltage is higher but the fact that it's alternating means your muscles wont lock up when you come into contact as you see 0amps 120 times in a second. House electricity has a frequency of 60hertz. The dangerous part is holding that for several seconds. The pulses can throw your heart off beat as it tries to match the electricity frequency and when it cannot keep up it'll lock up, and cause cardiac arrest from what I understand. 

TL;DR. Comparing 42Vdc and 110Vac is like comparing apples to oranges
```

---
## \#25 Posted by: fedestanco Posted at: 2017-02-01T01:28:44.842Z Reads: 339

```
BTW tasers dont kill (usually) and they deliver "voltage peaks at 50,000 volts and when it reaches the body it is substantially less. The volts are responsible for delivering the amps. Taser runs off 0.0021 amps at average performance. "(from the internet)
```

---
## \#26 Posted by: theroid Posted at: 2017-09-24T16:43:58.461Z Reads: 282

```
''and available for 30A, 40A, 50A, 60A, 80A, 100A'' why did you pick 50A? Is it any bad to go with the highest? I dont want to use more than 50A too, but wouldnt it be still better to go with a higher amp?
```

---
## \#27 Posted by: Hatman30 Posted at: 2018-05-12T15:35:14.906Z Reads: 215

```
taking it one step further![IMG_7584|500x500](upload://jActmSgVBGKfqGzJXu5lkqe9rrz.jpg)![IMG_7588|500x500](upload://yxOrDgkUZnk7VYJGw5v2bCorDV4.JPG)
```

---
## \#28 Posted by: ricoghardforth Posted at: 2018-09-21T08:58:49.981Z Reads: 159

```
Does the fuse need to be in an air gap to work some where near its fuse rating.  
Does any one fancy designing a 3d print file for a cover for this which includes a handle or loop to make it easy to pull out.
```

---
## \#29 Posted by: Andy87 Posted at: 2018-09-21T09:04:38.228Z Reads: 160

```
@mmaner did if it´s what you looking for

https://www.thingiverse.com/thing:2918681
```

---
## \#30 Posted by: Arzamenable Posted at: 2018-09-21T09:20:08.597Z Reads: 152

```
brilliant conclusion to the brewing squabble above. 

Makes me want to put a treasure troll or thunder cats head on my loop key.
```

---
## \#31 Posted by: ricoghardforth Posted at: 2018-09-21T10:41:04.942Z Reads: 149

```
Nice one Andy87 suberb just what I'm after.
Does any one in the uk fancy knocking up a small batch of thease and selling me a couple for a few quid each.
The last time I tried a 3d print service for some XT90 panel mounts they came back to small and wouldn't fit.
```

---
## \#32 Posted by: deucesdown Posted at: 2019-01-03T04:00:10.385Z Reads: 101

```
Oh noes what has I done?

![IMG_20190102_225156|666x500](upload://jI71raFCZLMNjos5AJClKn8XRlE.jpeg) 

@Hummie you still got that grinder?
```

---
## \#33 Posted by: Hummie Posted at: 2019-01-03T04:16:26.939Z Reads: 99

```
im making one myself now but without a fuse.  rather every micron of power.  

used the grinder yesterday.  if you have one you find so many things to grind.
```

---
## \#35 Posted by: mmaner Posted at: 2019-01-03T04:23:37.748Z Reads: 98

```
I can't work on a Jeep without a side grinder, so many stuffs to remove 😀
```

---
