# Choosing the right motor kv for the VESC

### Replies: 349 Views: 38011

## \#1 Posted by: chaka Posted at: 2016-05-11T15:43:32.030Z Reads: 1933

```
If you have done your research you have probably found a lot of conflicting information about what KV is "best". Often times this information is given without regard to system voltage or electrical rpm limits. The VESC has an ERPM limit of 100,000 but I have found that limit to be closer to 60,000 ERPM. Vedder has stated that running higher than this is inefficient but I have also found that it causes VESC failures. 

My findings are purely anecdotal and I am not completely sure but a pattern has developed where systems designed with the 60,000 ERPM limit in mind run trouble free. 

What does this mean and how do you calculate an ideal motor kv for your particular system voltage? It is relatively simple, virtually all the motors used in eboarding have 7 pole pairs, divide 60,000 ERPM by 7 PP and we get roughly 8570 rpm. Divide 8570 rpm by your system voltage and you will have your ideal motor kv. I like to make my voltage calculation based on a fully charged voltage so 12s would be roughly 50v.     

8570 RPM/50v = 170kv - 12s
---------------/42v = 200kv - 10s
---------------/33v = 260kv -   8s
---------------/25v = 340kv -   6s

These numbers are a rough guide, you can go a little higher but use caution. If you a want a smooth running reliable system this is a good first step to help achieve that.
```

---
## \#2 Posted by: akira Posted at: 2016-05-11T16:00:45.905Z Reads: 1626

```
This is seriously more conservative than Ben's recommendations.
He was saying that 240KV should be OK with 10S.
I think it is because he s using 86000 instead of your 60000.

I hope it is cause that's what I am planning ...
```

---
## \#3 Posted by: 3sly Posted at: 2016-05-11T16:01:03.080Z Reads: 1605

```
Oh wow, first bit of information I've come across about this. Thanks! So this is again an argument for choosing a lower kV motor (if u use 12s and such) if I'm not mistaken
```

---
## \#4 Posted by: chaka Posted at: 2016-05-11T16:07:01.364Z Reads: 1562

```
Vedder actually made his calculation based on 3.8v cell voltage resulting in 225 kv at 10s. You have some wiggle room.
```

---
## \#5 Posted by: chaka Posted at: 2016-05-11T16:08:22.480Z Reads: 1496

```
Also an argument for a dual motor 6s with high kv. I often wonder how well a quad drive 3s with 680 kv motors would perform.
```

---
## \#6 Posted by: akira Posted at: 2016-05-11T16:47:14.398Z Reads: 1444

```
AH ...
Thanks for this information about the battery voltage.
I did not remember that part of the calculation.
```

---
## \#7 Posted by: Hummie Posted at: 2016-05-11T16:51:40.786Z Reads: 1361

```
Thank you for the info
When u say motors typically have 7 pole pairs what do u mean?
```

---
## \#8 Posted by: Krudte Posted at: 2016-05-11T16:59:17.815Z Reads: 1324

```
What if you plan on running Dual motors?
```

---
## \#9 Posted by: chaka Posted at: 2016-05-11T17:06:19.213Z Reads: 1295

```
I mean they usually have 7 pairs of poles or 14 poles total.
```

---
## \#10 Posted by: chaka Posted at: 2016-05-11T17:07:48.807Z Reads: 1276

```
Then you can drop your voltage and go with a higher kv due to the shared loading and lower amp use per motor but it changes nothing in these calculations.
```

---
## \#11 Posted by: Hummie Posted at: 2016-05-11T17:23:27.684Z Reads: 1243

```
Wouldn't it be 6 since there are 12 teeth?
```

---
## \#12 Posted by: chaka Posted at: 2016-05-11T17:25:48.377Z Reads: 1214

```
@Hummie here we go down the rabbit hole again? What do you mean by teeth?
```

---
## \#13 Posted by: Hummie Posted at: 2016-05-11T17:26:51.769Z Reads: 1194

```
I don't know what u mean by poles. There's 12 stator teeth and 14 magnets typically.  How does that relate ?
```

---
## \#14 Posted by: Vito Posted at: 2016-05-11T17:30:17.504Z Reads: 1177

```
My vesc is coming from chaka. i will use enertion 6372 190kv motor and 12s3p battery pack from dexter. This configuration should be ok on vesc?
```

---
## \#15 Posted by: willpark16 Posted at: 2016-05-11T17:33:32.001Z Reads: 1161

```
im 70 percent sure i saw someone post something about 190kv and 12s on the vesc as a sweet spot
```

---
## \#16 Posted by: Vito Posted at: 2016-05-11T17:37:16.520Z Reads: 1155

```
Good to know. The plan was 10s3p pack but i get a really good deal on 12s3p here in canada. Was second hand but still good deal
```

---
## \#17 Posted by: chaka Posted at: 2016-05-11T17:38:27.461Z Reads: 1146

```
Correct, it works but it is not ideal. You will lose the top end performance an never reach anywhere near the theoretical top speed.
```

---
## \#18 Posted by: willpark16 Posted at: 2016-05-11T17:41:30.901Z Reads: 1126

```
So 10s would be the sweet spot?
Edit: in regards to lifepo4 with a 245kv motor what would be ideal for the longevity of the vesc
```

---
## \#19 Posted by: chaka Posted at: 2016-05-11T17:47:50.947Z Reads: 1121

```
8570rpm/245kv = 35v

35v/3.6v per cell = 9.7 cells  

So you should be able to use a 10s lifpo4 pack with a 245kv motor.
```

---
## \#20 Posted by: Hummie Posted at: 2016-05-11T17:48:51.242Z Reads: 1095

```
Ok poles being magnets
```

---
## \#21 Posted by: willpark16 Posted at: 2016-05-11T17:49:10.990Z Reads: 1051

```
thanks. Its too bad there arent more lifepo4 builds
```

---
## \#22 Posted by: Hummie Posted at: 2016-05-11T17:53:33.862Z Reads: 1045

```
if I have an 80kv motor I could do much higher voltage except the components in the vesc are only capable of ...what?   Aren't the components voltage ratings not their true ability and while the capacitors are rated to 60 volts they maybe could do 20% more?  I'd like to try 14s if it won't blow up
```

---
## \#23 Posted by: chaka Posted at: 2016-05-11T17:54:36.669Z Reads: 1048

```
This is lifpo4 8s on an ezrun 6s esc.
As long as I kept the charge level at or below 28v it wouldn't trigger the esc's overvoltage shutoff.
<img src="/uploads/db1493/original/2X/c/cd93740e82d4c1bc366f844bf333d2d27fa57cd2.jpg" width="500" height="500">
```

---
## \#24 Posted by: willpark16 Posted at: 2016-05-11T17:55:36.594Z Reads: 999

```
im suprised that actually works
```

---
## \#25 Posted by: chaka Posted at: 2016-05-11T17:59:26.602Z Reads: 1007

```
The problem you run into when going with as high a voltage as possible is the loss in capacitance due to the increase in voltage. Better to have some headroom. 12s systems are way more finicky than 10s in that regard.

> if I have an 80kv motor I could do much higher voltage except the components in the vesc are only capable of ...what? Aren't the components voltage ratings not their true ability and while the capacitors are rated to 60 volts they maybe could do 20% more? I'd like to try 14s if it won't blow up

This is a bad design ethic in my opinion. I have always thought leaving 20% headroom in relation to factory spec was a more successful way to get a robust system. The cold hard reality is we have limited space and fairly large current usage especially for us bigger guys in the 180+ lb category. Higher voltage components start to increase the total size of the package. You will end up going through a lot of perfectly good hardware if you push everything to its absolute max.
```

---
## \#26 Posted by: Ulfberht Posted at: 2016-05-11T19:58:27.803Z Reads: 968

```
Awesome!! Great write up, @chaka
How does dual motor in the equation affect that formula. Say, I'm running 230kv on a single 10s pack. Does running dual change anything?
```

---
## \#27 Posted by: Randyc1 Posted at: 2016-05-11T20:04:23.381Z Reads: 948

```
Hi Chaka, what was your thought behind choosing (4.2V/cell),.. rather than a more average Voltage when riding ??
```

---
## \#28 Posted by: chaka Posted at: 2016-05-11T20:52:32.017Z Reads: 954

```
The only thing running dual motors does is split the work into two systems, less amps per VESC and motor. So in regards to the calculation nothing changes.

@Randyc1 I run really big packs and I think everyone should ;) so the voltage does not sag much when you have a full charge. My cells stay up around 4.05 to 4.10v per cell for quite awhile. Plus this gives the calculation a little headroom.
```

---
## \#29 Posted by: zool774 Posted at: 2016-05-11T22:03:53.023Z Reads: 948

```
''I like to make my voltage calculation based on a fully charged voltage so 12s would be roughly 50v''
Would you mind to explain this? I thought each cell voltage was 3.7V, so how come you are saying that the voltage of an 12s is 50v rather then 44.4v?
Thank you
```

---
## \#30 Posted by: chaka Posted at: 2016-05-11T22:09:51.662Z Reads: 916

```
50.3v to be exact, but yes a fully charged 12s li-ion will be about 50v fully charged.
```

---
## \#31 Posted by: zool774 Posted at: 2016-05-11T22:13:18.784Z Reads: 909

```
Thanks for clarifying it.
btw any news about those new motors?
```

---
## \#32 Posted by: chaka Posted at: 2016-05-11T22:41:44.742Z Reads: 904

```
They are in Ohio right now, I should have them by Thursday. I need to do some testing to be sure they perform before finalizing the order for the first batch, this was just a sample run. We are going to do some minimal branding with motor specs etc.
```

---
## \#33 Posted by: zool774 Posted at: 2016-05-11T22:48:37.036Z Reads: 897

```
Sounds good man:thumbsup:
keep me posted.
```

---
## \#34 Posted by: Bender Posted at: 2016-05-12T04:01:18.113Z Reads: 896

```
I found this very informative so I checked it out in VESC active monitor and found my actual measurements much lower than the pure calculations you have above.

230kv TB 6355 motor at full throttle 
in BLDC
6s is 32,000 ERPM 
9s is 48,000
12s is 66,000

in FOC
6s is 30,000
9s is 46,500
12s 61,000

It seems that 12s in FOC for my 230kv should be perfect
but I'm probably missing something
```

---
## \#35 Posted by: chaka Posted at: 2016-05-12T04:27:19.127Z Reads: 861

```
If that motor is actually 230kv than you are lucky it is still working. I ran a 245kv motor on 12s and it caused a drv failure, full disclosure is the VESC was twitchy to begin with which is why I sacrificed it for science.
```

---
## \#36 Posted by: chaka Posted at: 2016-05-12T04:33:55.882Z Reads: 857

```
@Bender I just ran my TB 230kv motor and you are right, it is showing the same results as my 192kv sk3 so it is not an actual 230kv motor.  I double checked by running an sk3 149 kv and a few others and the all gave the erpm values expected so the TB 230kv motors must be 190kv.
```

---
## \#37 Posted by: Bender Posted at: 2016-05-12T04:41:23.991Z Reads: 863

```
Very interesting...
That makes sense 
Thanks so much for checking
I really appreciate your contributions to the forum
This info is invaluable, especially for people to be able to design systems that work reliably
```

---
## \#38 Posted by: Randyc1 Posted at: 2016-05-12T13:10:25.768Z Reads: 858

```
So it also depends if you are running in BLDC or FOC correct ??

Another question Chaka ,...do you always charge your cells to full capacity 4.2v ?

Does that diminish cycle life ??
```

---
## \#39 Posted by: longhairedboy Posted at: 2016-05-12T13:31:18.500Z Reads: 843

```
[quote="chaka, post:36, topic:3125"]
so the TB 230kv motors must be 190kv.
[/quote]

that seems kind of sketchy... i wonder what's up with that. 

back on topic: i'm working on a 12S4P liion build, dual 190kv 63mm cans. Hopefully i'm not bumping up toooo close to the edge here. i figured 200+ would be too much, even splitting across two motors. 

This is very helpful info and a great guideline.
```

---
## \#40 Posted by: chaka Posted at: 2016-05-12T13:51:22.105Z Reads: 837

```
No, not really, FOC will knock a few thousand rpm off your top speed but it has the same erpm limitations from what I understand.

I tend to do full charges each time but it will give you more cycles if you only charge to 4.14v per cell.  For me it makes better sense to abuse my gear and see when and where it fails.

@longhairedboy It is actually kind of a plus in my opinion. 190-200kv works well for kids and total beginners @ 6s, a good all around board @ 8s, a rocket ship @10s.  @12s the extra voltage is wasted and you only exceed 60k ERPM with a tail wind or when going downhill so it is better to drop your KV down and keep that headroom.

I should add that I have only experienced the 60k wall when running 190-200kv motors @12s. Traveling at around 32-34 mph.
```

---
## \#41 Posted by: chaka Posted at: 2016-05-12T14:18:25.808Z Reads: 786

```
Another detail I should add, you can push the kv up to 200kv @12s but the top end will feel weak. It will have good mid range boost but it will taper off as you approach the max velocity. If you calculate based on a 60k ERPM max instead of 100k the power and boost will increase at a fairly constant rate giving you that freight train experience.
```

---
## \#42 Posted by: longhairedboy Posted at: 2016-05-12T14:21:35.638Z Reads: 770

```
@chaka what does 60,000 ERPM translate to in mph with 83mm wheels and a 15/33 pulley ratio? I left my TI 60 at home next to my typewriter.
```

---
## \#43 Posted by: chaka Posted at: 2016-05-12T14:26:50.363Z Reads: 770

```
Around 30-33mph or up to 36mph using a 3.8v cell voltage in your calculations.
```

---
## \#44 Posted by: longhairedboy Posted at: 2016-05-12T14:35:54.834Z Reads: 765

```
That's actually about damned perfect. I might just set that as my limit if its not the default already. I can't recall off the top of my head what the default is, but the guy i'm building the board for wants it capped at 35mph, and i really didn't know if it would do 35 on its own anyway given other factors besides actual and theoretical component limitations, even on a full 50v charge. But if adding this keeps things in the comfy zone for sure, then i'll add it to my checklist.
```

---
## \#45 Posted by: torqueboards Posted at: 2016-05-12T14:44:15.919Z Reads: 749

```
Wow.. that's pretty odd for that KV. They specifically stated it was tested. At least it's lower than higher :frowning: It does seem like 230KV though. I will have to start doing more testing.  Thanks for noticing guys.

Great post though Chaka. Thanks for sharing.
```

---
## \#46 Posted by: zool774 Posted at: 2016-05-12T18:59:36.712Z Reads: 729

```
do you think that would apply to the DIYes 6374 230KV 3200W as well?
```

---
## \#47 Posted by: torqueboards Posted at: 2016-05-12T19:08:53.178Z Reads: 727

```
@zool774 I think the batch that Chaka and Bender have might be an old batch but I'm not entirely positive. The best bet would be to test as Bender and Chaka have.
```

---
## \#48 Posted by: OskarCastrone Posted at: 2016-05-12T19:23:42.766Z Reads: 721

```
Do not tempt me! That would be an awesome build! Do you think you could get away with some 60A ESC's as well then? Otherwise 4 VESC's will become a bit expensive!
```

---
## \#49 Posted by: Bender Posted at: 2016-05-12T22:23:59.424Z Reads: 712

```
I just bought mine in April 
Just FYI

The good news is the performance is great!
I'm getting 15mph on 6s, 22mph on 9s on a single drive and I'm 220lbs
15/36 gear ratio and 76mm wheels

If it's a 190kv that's close to 100% efficiency according to the [esk8 calculator](http://toddy616.blogspot.com/2013/07/electric-skateboard-calculator.html?m=1)
If it's a 230kv its 80% which seems more realistic
Very strange
```

---
## \#50 Posted by: Bender Posted at: 2016-05-12T22:44:03.678Z Reads: 695

```
Just thought of something
So we're all on the same page, were testing on the bench with the drive system hooked up right?
```

---
## \#51 Posted by: WrinklyWink Posted at: 2016-05-13T11:10:10.371Z Reads: 681

```
this is so strange idk even what to think of it. did TB really sell a 190kv batch without knowing? because then it would be the only VESC-compatible 12s sensored motor for this size available..
```

---
## \#52 Posted by: chaka Posted at: 2016-05-13T12:28:26.318Z Reads: 672

```
I tested without any drive belts on the bench. Also, you will reach you calculated top speed if it is in 20-30mph range. I do not see much loss in efficiency until I reach about 30mph.

@WrinklyWink definitely a plus!
```

---
## \#53 Posted by: Bender Posted at: 2016-05-13T12:38:31.569Z Reads: 666

```
I'll test this evening without the belt to see if there is any difference
I'm just curious
```

---
## \#54 Posted by: chaka Posted at: 2016-05-13T12:43:04.828Z Reads: 677

```
Vedder and I discussed the ERPM limitations of the VESC yesterday and he confirmed some of my findings.

>  At high erpm there are few switching cycles at each commutation and therefore few adc samples, which makes it difficult to track the rotor. If sync is lost the current can rise very quickly, which can cause failures easily.
```

---
## \#55 Posted by: WrinklyWink Posted at: 2016-05-14T18:43:06.708Z Reads: 683

```
[quote="chaka, post:40, topic:3125"]
12s the extra voltage is wasted and you only exceed 60k ERPM with a tail wind or when going downhill so it is better to drop your KV down and keep that headroom.

I should add that I have only experienced the 60k wall when running 190-200kv motors @12s. Traveling at around 32-34 mph.
[/quote]

I always thought higher voltage =

* less amperage used (e.g. 17 amps vs 20 amps) (greater range)
* less heat (therefore less damaging during hot summers)

and both of the above leads to more performance headroom. One could also lend the headroom towards a higher torque pulley system. Wouldn't that bring the ERPM limits closer then? I don't find it wasteful.
```

---
## \#56 Posted by: Bender Posted at: 2016-05-15T04:27:42.486Z Reads: 662

```
I tested it out and with and without the belt on and the difference was
Almost indistinguishable, just slightly lower ERPMs with belt on.
```

---
## \#57 Posted by: chaka Posted at: 2016-05-15T13:29:03.525Z Reads: 660

```
@WrinklyWink  We are talking purely about motor rpm and erpm in these calculations. Luckily these calculations lend themselves well to the common gear ratios resulting in a very usable range of power. 

You could lower your gear ratio to get more torque on a system with high erpm but the motor will still be running inefficiently at WOT.
```

---
## \#58 Posted by: WrinklyWink Posted at: 2016-05-26T17:00:57.541Z Reads: 664

```
<img src="/uploads/db1493/original/2X/d/d8927fb71b190cae722def9ce983ad7d2cb65559.jpeg" width="666" height="500">
Well, heres the proof: 198kv. So a 200 kv motor..
```

---
## \#59 Posted by: claudiofiore88 Posted at: 2016-05-26T17:03:55.358Z Reads: 648

```
That's very interesting.  @torqueboards should definitely have a talk with his supplier.
```

---
## \#60 Posted by: WrinklyWink Posted at: 2016-05-29T01:30:36.086Z Reads: 645

```
[quote="torqueboards, post:47, topic:3125"]
The best bet would be to test as Bender and Chaka have.
[/quote]

Under your [warranty page](warranty/):
<img src="/uploads/db1493/original/2X/6/604aa4072cde1e25e3993b2a0b32771ff308c882.PNG" width="690" height="50">

What do you mean by "rigorously," if you don't test for KV? Do your strict quality controls _not include_ the KV you advertise?

[quote="torqueboards, post:45, topic:3125"]
I will have to start doing more testing.
[/quote]


I'm still waiting to hear back from your testing or an official statement about your wrongly advertised motors.

Stop puffing.
```

---
## \#61 Posted by: Michaelinvegas Posted at: 2016-05-29T01:41:06.971Z Reads: 616

```
Wow holding them to the fire @WrinklyWink....
[quote="WrinklyWink, post:60, topic:3125"]
Stop puffing.
[/quote]
I would allow @torqueboards to do a little research before you start poking at him.....
And let's put the sentences in context 

[quote="torqueboards, post:45, topic:3125"]
Wow.. that's pretty odd for that KV. They specifically stated it was tested. At least it's lower than higher :frowning: It does seem like 230KV though. I will have to start doing more testing.  Thanks for noticing guys.

Great post though Chaka. Thanks for sharing.
[/quote]
```

---
## \#62 Posted by: willpark16 Posted at: 2016-05-29T01:43:04.086Z Reads: 601

```
i would agree except when your paying the kind of money that his, onloops, or even chakas motors cost u expect the advetising on the most important thing to be correct
```

---
## \#63 Posted by: torqueboards Posted at: 2016-05-29T02:20:36.989Z Reads: 600

```
@WrinklyWink - Our 6355 230KV motors will be in the range of 220-230KV (typically).

Our manufacturers do test the KV per each motor. The option of speculation would be how different the tester which you used and the method of testing the manufacturer uses.

I've been told that the Turnigy Trackstar Motor Analyser is a bit inaccurate. This is related directly from the manufacturer. I do trust the advice but it should also be tested.

Feeding you false information is not in our best interest for us as a business, for the community and even for the consumer and industry. If it is done so, it isn't intentional.

We'll do our best to fix and verify the information.

If you feel you were tricked in anyway. Please feel free to contact me and you can return the item.

The last thing I want is for you to feel unease about your purchase.
```

---
## \#64 Posted by: Michaelinvegas Posted at: 2016-05-29T03:25:43.732Z Reads: 577

```
Not for nothing...last time I checked ...lower KV motors are a little more expensive than higher kv motors... So, looking at it...the value is there .... If the motor proves to be a lower kv and is affecting speed...that can easily be countered by a pulley change ...
```

---
## \#65 Posted by: Bender Posted at: 2016-05-29T15:16:40.095Z Reads: 580

```
I just want to say that from 6s- 12s this motor performers beautifully
I've been so impressed that this little motor can propel a 220lb man up hill
I'm extremely happy with my purchase the numbers maybe off depending on how you test it but in the real world it delivers.
```

---
## \#66 Posted by: chaka Posted at: 2016-05-29T16:03:28.008Z Reads: 572

```
IMO you guys are lucky the numbers were wrong on those motors. 230+kv motors work well at 6s and 8s but they start to lag a little at low speed when you drive the voltage up.
```

---
## \#67 Posted by: willpark16 Posted at: 2016-05-29T19:16:35.902Z Reads: 573

```
there isnt anything wrong with it but  just think all products should be tested before selling
```

---
## \#68 Posted by: Michaelinvegas Posted at: 2016-05-29T19:24:03.340Z Reads: 568

```
Like your car, treadmil, blender ? They test every one off the assembly line right?
```

---
## \#69 Posted by: willpark16 Posted at: 2016-05-29T20:11:13.661Z Reads: 566

```
beats me but i somehow get what was orginally specified and not something that goes slower or faster
```

---
## \#70 Posted by: Michaelinvegas Posted at: 2016-05-29T20:43:16.476Z Reads: 576

```
IAnd you know this because you test every thing....sorry I doubt that I'm sorry.

Let be realistic... @torqueboards orders them made...like everyone else .... Hobby King , Enertion and the like...and they count on what was ordered to be correct. Because they aren't bench testing every single piece that walk through the door...

@willpark16 you say it's slower and we say more it's has more power than spec ... And that's a plus....don't you think?

It's like getting that bonus onion ring at Burger King when you ordered just fries
```

---
## \#71 Posted by: willpark16 Posted at: 2016-05-29T20:53:40.922Z Reads: 561

```
Im simply saying that if i order 20 motors from a place you can bet ill take a few minutes to test the kv and make sure they work before selling them to people. And im not saying its a good thing but its like trying to buy a tacon that i really want but then end up getting a 190kv sk3. Maybe better in some ways but i might have really wanted that high kv
```

---
## \#72 Posted by: WrinklyWink Posted at: 2016-06-03T19:29:24.685Z Reads: 547

```
Precision is key here. People are not crucifying for more given, we just prefer accurate information. In a world where "we want more" is an out-of-control goal, "we want precision" is actually more environmentally friendly and less greedy. And it allows the extremes of said goal to be applied to empathy, allowing for a more awareness of that which is unspoken.

Under the motor specifications are 19 (!) lines of information. To include all this information is either for puffing or for engineering advantage. Since I'm hopeful that its for the latter, the seller should hope that it is correct, otherwise, leaving it uncorrected or quietly overlooking the error (even per buyer basis) shows other intentions I rather not extrapolate upon.
```

---
## \#73 Posted by: Qwiksand Posted at: 2016-06-03T21:52:21.523Z Reads: 533

```
Unfortunately, I found this post a bit too late and after running my 245kv BigFoot 160 on 10s lipo I'm getting DRV errors. I've also been switching between FOC and BLDC, which I'm also reading is a nono. 

So @chaka, heads up- I'll be sending my VESC back for a quick refit and next time I'll limit my volts.

Thanks for the awesome R&D on this front and all the up front knowledge sharing you do!
```

---
## \#74 Posted by: Ulfberht Posted at: 2016-06-03T23:06:41.358Z Reads: 528

```
From DIY warranty: " does not recommend putting a motor on a Skateboard or Longboard. Information on our website and products are only for educational purposes and not meant to be ridden"
So it really doesn't matter what the specs are now does it? These are expressly NOT intended for ESK8. LOL
```

---
## \#75 Posted by: torqueboards Posted at: 2016-06-03T23:56:16.836Z Reads: 516

```
You guys are all crazy... Putting motors on a longboard :dizzy_face:
```

---
## \#76 Posted by: Michaelinvegas Posted at: 2016-06-04T04:18:50.131Z Reads: 531

```
[quote="WrinklyWink, post:72, topic:3125"]
Precision is key here
[/quote]

Absolutely, but having an accusatory tone? As if it were negligence or indifference on his side....

I'm mean how many of his motors have you tested to even make the claim of "puffing" ... Have you tested another? Has someone else done the same test and have come up with the same results? You talk of precision .. How percise were you when you did your tests? How percise are the instrumentas that you are using? Were you precise in your investigation that @torqueboards is "puffing" the facts?  Let's get real man...those specs, written by the motor maker...It's marketing material .... All of it is...no matter if it's in paragraph form or bullet points

We're blasting down the road on a piece of wood with a motor made for an RC plane...We aren't building mini space shuttles to take us into space....or using it to save people lives .... These motors are far from what would be considered precision in certain circles...
```

---
## \#77 Posted by: Lucky8matt Posted at: 2016-06-04T08:54:53.931Z Reads: 515

```
I am new to this and have read for the past two days and not the best at electrics im more of a cnc cad milling kind of guy but I am stuck with once you have your vecs how do you connect that to your throttle controller?? I.e numb chuck or enertion hand held controller also would love other ideas on another way of controlling your throttle thanks delete if im mot ment to write this here
```

---
## \#78 Posted by: Randyc1 Posted at: 2016-06-06T00:58:11.129Z Reads: 504

```
Throttle is  controlled wirelessly with with a hand held Transmitter and a Reciever that is conected to the ESC .
```

---
## \#79 Posted by: treenutter Posted at: 2016-06-06T21:30:02.723Z Reads: 532

```
[quote="chaka, post:1, topic:3125"]
I like to make my voltage calculation based on a fully charged voltage so 12s would be roughly 50v.
[/quote]


@chaka I'm definitely not arguing, but I'm curious about why you make the calculation based off the max charge voltage instead of the nominal voltage? My experience has been that I'm only at 4.2v per cell for 5%-10% of the ride time I get, and then I'm at 3.8v for the majority of the usage. We've all seen the lipo and lion discharge histograms.... the majority of the line is flat at 3.8. 

Is it because we are at the greatest risk of VESC failure during that full voltage period? If so, could we limit amp draw or ERPM to protect ourselves if we're out of this specification?

I'm about to switch from 8S Lipo to 10S Li-Ion and I'm wondering if it's necessary to get a new motor (currently using a 245kv, but could go lower to 192KV to align with your suggestion)

http://www.ibt-power.com/bkencel/Graphs/LiIonDischGph.JPG
```

---
## \#80 Posted by: chaka Posted at: 2016-06-06T22:11:05.769Z Reads: 508

```
Some people run 245kv on 10s but it can cause problems. That is a really high ERPM. I personally don't go over 230kv on 10s. The higher you go with ERPM the higher the chance of errors and blowing a drv chip.
```

---
## \#81 Posted by: chipoi84 Posted at: 2016-06-06T22:47:52.444Z Reads: 499

```
Can't we limit the erpm through the bldc tool to prevent this issue?
```

---
## \#82 Posted by: chaka Posted at: 2016-06-07T00:21:18.432Z Reads: 504

```
Sure you can do that. You can also limit the battery current to 30 amps if your battery pack is filled with weak sauce. All kinds of compromises can be made. Not ideal.
```

---
## \#83 Posted by: Randyc1 Posted at: 2016-06-07T00:38:47.730Z Reads: 503

```
I understand a 200kv would be better on 10s ,.....but  limiting rpm on a 245kv on 10s to around 9000 rpm would keep things safe no?
```

---
## \#84 Posted by: SteveS Posted at: 2016-06-07T01:29:32.972Z Reads: 494

```
In addition to what Chaka wrote, I would point out that you would also give up torque by staying with the higher kv motor. Remember, torque is inversely proportional to kv.
```

---
## \#85 Posted by: chipoi84 Posted at: 2016-06-07T04:23:26.215Z Reads: 496

```
I understand that the torque is going to be lower, but I'm saying this so people don't have to go out and buy new motors just because their motors' kv are off by a little bit. The torque is going to be lower due to the erpm limit, but it is going to even out once the voltage goes down a little bit. In my case, I have 245kv at 10s, so the erpm limit is not going to be in effect that long anyway.
```

---
## \#86 Posted by: jrpwit Posted at: 2016-06-07T05:32:37.068Z Reads: 490

```
Wow I'm really glad I read this! Was was just about to hook my new vesc from enertion (which I have waited forever for) to a tacon 160 245kv and a 12s lipo setup. I will totally be limiting to voltage to 8s instead of the full 12s.
```

---
## \#87 Posted by: chipoi84 Posted at: 2016-06-07T05:48:27.266Z Reads: 483

```
I think you can still use the 12s setup if you want by limiting the erpm in the bldc tool. You just won't have all of the power that 12s offer at full voltage, but you still have the benefit of the longer ride time from battery with higher voltage.
```

---
## \#88 Posted by: jrpwit Posted at: 2016-06-07T05:59:46.026Z Reads: 479

```
Yup I will have to I guess. I originally set out to May my board a speed board but I guess 25 mph should be fine until I decide to get a different esc that can hand the erpm.
```

---
## \#89 Posted by: Hummie Posted at: 2016-06-07T06:14:22.727Z Reads: 476

```
What motor or battery limit are yours set to or what's considered safe?  I've been running 60/60 and read 50 is the safe max.  Is it solely heat dependent? Maybe 60 for shorter periods?  Isn't there a temp limit that would get tripped before it burned up. Don't want to go down to 50
```

---
## \#90 Posted by: Joe Posted at: 2016-06-10T12:03:28.571Z Reads: 480

```
You missed a serious factor, the revolutions in kv is per V. 
Lets say you go with a 200 kv and 24 volts, that gives you 24 * 200 RPM on a fresh battery.
What RPM will you have at 1/4 battery charge? You need motors to be around four times too fast and four times too powerful at the top of the battery life, in order to have the performance you want all the way through your battery use range.

You also need to consider your gear down ratio in the calculation.You need to consider the voltage top and bottom of battery life, gear down, kv, circumference of the wheel, desired top speed, and torque for hill climbing. I strongly suggest building a spreadsheet and plugging various numbers in.
```

---
## \#91 Posted by: Maxid Posted at: 2016-06-10T13:13:32.850Z Reads: 494

```
[quote="Joe, post:90, topic:3125, full:true"]
What RPM will you have at 1/4 battery charge? You need motors to be around four times too fast and four times too powerful at the top of the battery life, in order to have the performance you want all the way through your battery use range.
[/quote]

What? Your battery voltage will only decrease slightly while discharging.
You typically go from 4.2V to something like 3.3V per cell while spending most time between 3.8 and 3.6V.
So no you do NOT need a motor that is 4 times the speed you actually want.
See for example a Lipo discharge curve:
http://www.rctech.net/forum/attachments/electric-road/1104193d1377325541-benchmarking-best-2s-lipos-tp-extreme-5000-discharge-curve-graph.gif

Or did I misunderstand your post?
```

---
## \#92 Posted by: Joe Posted at: 2016-06-10T13:24:37.524Z Reads: 478

```
Thanks, you know your batteries way better than I do. But voltage is additive in series.

You are showing a 1.4 volt drop per cell. Assume six cells in series. For a top voltage of 22.2v, the last quarter starts with an 8.4 volt drop, 22.2 - 8.4 leaves 13.8.v So you would want about double not four times the motor.  

You are correct, with that kind of battery performance my numbers were way off. I do appreciate the feedback. Great stuff. Now I need to refactor my build specs, again, tenth time is the charm.
```

---
## \#93 Posted by: Maxid Posted at: 2016-06-10T13:34:59.267Z Reads: 471

```
No you still don't understand.
You will not have a 1.4V drop per cell.
It will be 0.7V - from 4.2 to maybe 3.5V. Anything below 3.5V is territory you should not go to with Lipos. There is almost no energy left in your battery after 3.5V anyway (look at the graph).
Also you will not start at 22.2V at 6S because you charged them to 6*4.2V = 25.2V.
That means you will go from 25.2 at full charge to 21V. That is not much and the reason why most people just use the nominal voltage for their drive train calculations.
You will spend most time around the nominal voltage of 3.7V - again look at the graph.
```

---
## \#94 Posted by: Joe Posted at: 2016-06-10T13:48:26.109Z Reads: 465

```
Thank you again, I think I need to meditate on what you just said. That is pure gold to me.
```

---
## \#95 Posted by: Sonic1 Posted at: 2016-06-21T19:09:57.715Z Reads: 462

```
This would apply for all escs more than likely, correct? Other ESC are slower and the VESC switching speed is the likely the same or better. 


i was going to use dual diagonal 530kv motor (HTD3m) at 6s which is ~93000 erpm.

But that's unweighted, and 70% of that is 57500 which should be perfect???

I could run 4s and that would put the unweighted numbers exactly in line with yours.

What's happening with the drop in eff. Does anyone know?  Flying machines don't seem to be suffering the same way. 

http://www.hobbyking.com/hobbyking/store/__65951__NTM_Rotor_Drive_600_Series_510KV_5500W_600_50_size_heli_US_Warehouse_.html

This Motor is specced for 12s and also a scary amount of amps. That's 150,000 Erpm,  presumably with some Basic atmel ESC, moving over 3 feet of blades through the air. Minimultirotors are pushing above 350,000 erpm.
```

---
## \#96 Posted by: Michaelinvegas Posted at: 2016-06-22T05:31:46.059Z Reads: 431

```
The high kv is gonna kill your motors quick if you don't run high speed most of the time
```

---
## \#97 Posted by: Sonic1 Posted at: 2016-06-22T09:44:04.809Z Reads: 438

```
Gearing with htd3m it easy to have a 5:1 ratio and calculated top speed of 21 mph. That should keep the motors very happy, 

i still don't quite understand @chaka point, or whether I should stick with 6s or switch to 4s. If the weighted top speed is 16, then 6s is the best choice.
```

---
## \#98 Posted by: Michaelinvegas Posted at: 2016-06-22T10:14:41.349Z Reads: 428

```
Calculation and practice are sometimes two different results
```

---
## \#99 Posted by: Jinra Posted at: 2016-06-22T14:58:01.792Z Reads: 431

```
youre going over the erpm limit of 60k which may give you problems and errors when running it with the VESC. Try to stick to a sub 300kv motor
```

---
## \#100 Posted by: flatsp0t Posted at: 2016-06-22T15:31:14.829Z Reads: 433

```
Maybe it works, just try it and put you resusts here.
You know, for science.
```

---
## \#101 Posted by: Sonic1 Posted at: 2016-06-22T16:04:44.153Z Reads: 426

```
I wrote out exactly what the erpm is at 6s, (weighted and theoretical) and I wrote 4s would be less. 

Either way, I would not have to change motors, and you have no basis for saying that. 

 I'd love to know why brushless motors are hitting much, much higher erpm on much slower regular esc. After all people run them on 10s and 12s, and the large  helicopters don't suddenly fall from the sky going over that limit.
```

---
## \#102 Posted by: Jinra Posted at: 2016-06-22T16:27:58.612Z Reads: 434

```
Not sure why you're taking offense to someone who's trying to help. You wrote that you'd have 93k erpm, which is above 60k, so don't say I don't have basis for what I've said, you'll have to take that up with Chaka and Vedder. Running 4s will cause a lot of current and heat; general consensus is that 6s is minimum to run on the VESC. And yes, people run the VESC on 10s and 12s, but on much lower kv motors for much less erpm.

Like @flatsp0t said, you can run it if you want, I'm just not confident it'll work well or long.
```

---
## \#103 Posted by: flatsp0t Posted at: 2016-06-22T16:30:10.325Z Reads: 434

```
Large Helis do not use VESC.
Their ESCs use Voltage control and not Current control.
It might work. With 4s the amps will kill you VESC, with 6s or more your ERPM will result in a blown DRV chip.
Thits is what @chaka and the others told you. 
Till then, i bet we will se a "buhuhu my vesc is Dead" tread.
Try it and learn or leave it and trust people with experience with the VESC.

Edit:
Ninja @Jinra
```

---
## \#104 Posted by: longhairedboy Posted at: 2016-06-22T16:42:45.738Z Reads: 412

```
Who would do such a thing? Chumps, that's who.
```

---
## \#105 Posted by: longhairedboy Posted at: 2016-06-22T16:44:51.987Z Reads: 409

```
190kv is probably the sweet spot for 12S on VESC, but i've been told it bumps up against the limits. Any who its what i use. CUZ I BUMP LIMITS YALL.
```

---
## \#106 Posted by: flatsp0t Posted at: 2016-06-22T16:46:48.064Z Reads: 404

```
Bump them to space.

...... or your VESCS back to chaka.
```

---
## \#107 Posted by: Pablo_702 Posted at: 2016-06-22T17:49:55.689Z Reads: 407

```
based on what i read here yes it looks like 190kv is the sweet spot for 12s, now i also read that if you go higher than this you might be compromising top end perfomance, what if you lower than 190kv like 149kv with 12s??? @chaka
```

---
## \#108 Posted by: Bobfandango Posted at: 2016-06-22T18:34:36.635Z Reads: 397

```
I'm running 149kv with 12s and I have noticed 2 things that you'd completely expect:  the motor has more torque for a given amount of current, and top speed is reduced (16T/40T--> theoretical top speed of ~28mph....  more than fast enough for me).  The ERPM at top speed is well below even the more conservative 60k (i.e. motor rpm max is about 6600).  

I'm not running FOC (though I'd like to) since it apparently kills DRVs with some regularity....  i.e. numerous reports of DRV errors for no apparent reason after running on FOC for any length of time.  If VESCs were easier to get or repair, I'd experiment with FOC since the low ERPM of this setup might prevent drv errors... who knows...
```

---
## \#109 Posted by: Sonic1 Posted at: 2016-06-22T22:45:31.734Z Reads: 384

```
Well, from my point of view, you ignored that I'm running 2 motors, so amps are /2. 

If you can't run 4s with 2 wheel drive without smoking a VESC, then every 1 wheel drive at 8s would also be **toast**. Do you follow? And on top of that, there's current control, so telling somebody oh buy more stuff, is not helpful.  

Again, I don't see any basis that I need new motors. Saying you're helpful, doesn't mean you are helpful. 

@flatsp0t thank you for for you answer, can you tell me why the erpm is being calculated with a theoretical erpm when the weighted rpm is less? You won't hit the theoretical RPM with some help from gravity or a tailwind.
```

---
## \#110 Posted by: Jinra Posted at: 2016-06-22T22:49:14.885Z Reads: 374

```
It doesn't matter if you're running two motors.. You're still hitting the eRPM limit of 60k regardless of whether you're on single or dual drive.
```

---
## \#111 Posted by: Sonic1 Posted at: 2016-06-22T22:51:14.895Z Reads: 376

```
You're really unhelpful, obviously I put two paths as possble and 4s path is way under that erpm.  Please stop addressing anything I have to say if you're just a troll who doesn't see facts.
```

---
## \#112 Posted by: Jinra Posted at: 2016-06-22T22:52:04.074Z Reads: 370

```
Alright, you obviously don't want my help, and that's fine. Good luck with your build, and I hope it goes well.
```

---
## \#113 Posted by: Maxid Posted at: 2016-06-22T23:00:23.520Z Reads: 376

```
[quote="Sonic1, post:111, topic:3125, full:true"]
 Plea stop addressing anything I have to say if you're just a troll who doesn't see facts.
[/quote]

To me it sounds like you are the troll here...
```

---
## \#114 Posted by: willpark16 Posted at: 2016-06-22T23:35:16.923Z Reads: 373

```
wtf have u ever contributed i didnt even know u existed until a minute ago. As for running higher kv motors the 300kv limit was set for a reason if u wanna experiment go fucking do it but dont start calling members who have helped others on more than one occasion trolls. Dont forget to let me know when u fry your vesc or overheat your motor tho:grinning:
```

---
## \#115 Posted by: lox897 Posted at: 2016-06-22T23:40:57.300Z Reads: 373

```
Here we go again... Stop calling members names. They have been here for much longer than you and are a lot more experienced. Unless you want to blow your VESC just listen. No need for more arguments.

SSIILLEENNCCEE!
```

---
## \#116 Posted by: Sonic1 Posted at: 2016-06-23T00:27:20.571Z Reads: 368

```
 The reason for 300 KV limit is because htd5 won't let you get the erpm low enough.

No esc actually can tell what the KV of the motor is, only erpm.  @chaka  wrote in this very thread about using motors above 600 KV as possible. 

There is no limit to motor KV, got it?
```

---
## \#117 Posted by: Mobutusan Posted at: 2016-06-23T01:31:40.483Z Reads: 370

```
Try it out and let us know how it goes. It's the only way to find out for sure if theory matches reality.
```

---
## \#118 Posted by: Maxid Posted at: 2016-06-23T06:17:28.591Z Reads: 385

```
[quote="Sonic1, post:116, topic:3125, full:true"]
 The reason for 300 KV limit is because htd5 won't let you get the erpm low enough.
There is no limit to motor KV, got it?
[/quote]

You are just so full of yourself.
The KV limit is there because at some points the needed reduction is just not possible anymore with the available pulleys.
Ever thought of that?
With a 500kv motor and 83mm wheels at 10S you would need 14/80 gearing to reach a speed of 50km/h.
Now have a look how big a 80t pulleys is! Well first of all maedler does not even have one in in their store so you'd have to settle with 72 as maximum (top speed would be a ridiculous 56km/h). But what diameter is a 72t pulley? It is [115mm](https://www.maedler.de/Article/17227200). Do have any idea how big that is? It is bigger than your entire wheel.
So the maximum you could go with would be a 48t pulley which would get you to 84km/h - you see that what you tell us makes no sense?
The 300kv are there for a reason!

Edit: You said yourself you want to use a 5:1 reduction with HTD3 belts. How exactly are you planning to do this?
You could go 14/72 as the 72t pulleys is 69mm but the 14t is only 13mm - that is so small that you probably can't even confidently put it on your 8 or 10mm motor shaft.

Also have fun coasting on this thing :neutral_face:
```

---
## \#119 Posted by: flatsp0t Posted at: 2016-06-23T06:22:08.920Z Reads: 365

```
Leave him, he is not worth it.
```

---
## \#120 Posted by: Maxid Posted at: 2016-06-23T06:32:48.205Z Reads: 368

```
would have been fun seeing him order these pulleys and only later realize how bad of a mistake he made :smiley:
```

---
## \#121 Posted by: flatsp0t Posted at: 2016-06-23T06:45:01.268Z Reads: 355

```
It will be, i think he does all we told wouldnt work, just because we told it.
```

---
## \#122 Posted by: Sonic1 Posted at: 2016-06-23T21:01:40.226Z Reads: 365

```
 Maybe you should expand your mind, and look around? Why are you mentioning 10s, my choices are between four and six cell. As I said.

The shaft is 5mm, 15/75 is 5:1 and  if you know that PI iis close to three...

You can figure out that it's in the neighborhood of ~ 75mm tall. Htd **3mm**  (insert formula for circumference of a circle here)

Running 97mm wheels means anything up to 6:1 is workable. 

Learn some mathing, or at least don't comment **wrongly** Dont just listen to me listen to people who have been here a while, Chaka said 610kv may be useful.
```

---
## \#123 Posted by: Maxid Posted at: 2016-06-23T21:14:04.511Z Reads: 351

```
you do realize that there are basically no pulleys for 3m upwards of 72t?
also 4s is ridiculously low - you can obviously make it work if you really want to but why would you?
There is no benefit in having a high kv motor setup like the one you are trying to build.
Also you still did not address the coasting issue - it will be a pain.
But have fun and good luck!
```

---
## \#124 Posted by: Sonic1 Posted at: 2016-06-23T22:19:14.860Z Reads: 356

```
That's all down to preference and  I have no problem with you on that.  I do have a problem when are wrong based on the facts.

 Sayiing stuff like 10mm motor shafts, and you can't get 5:1, is plain wrong. 

**14:72 done.**  both commonly available. 

But go ahead and wish that my build is impossible and "I'll learn." When you show, based on facts, you're the one who needs to learn.

 Also, there's this little thing called 3-D printing, if you want an 85 tooth gear,  have somebody print it. 

 Repeat of the facts, the ESC does not know motor Kv. It only knows erpm.  There's nothing wrong to use gearing if the math works. Htd5 is good stuff, but htd3 is fully tested too.
```

---
## \#125 Posted by: Pablo_702 Posted at: 2016-06-24T01:29:50.828Z Reads: 343

```
Guys mke love not war
```

---
## \#126 Posted by: Hummie Posted at: 2016-06-24T05:39:45.447Z Reads: 344

```
Wouldn't u need at least a 114mm wheel? To fit a pulley 72 tooth
```

---
## \#127 Posted by: Maxid Posted at: 2016-06-24T05:40:55.536Z Reads: 345

```
not with HTD3
```

---
## \#128 Posted by: Hummie Posted at: 2016-06-24T06:04:35.521Z Reads: 347

```
If u do do it with the low voltage u maybe wouldn't need an anti spark

But I think with only 14 tooth pulley and especially when paired beside the giant 72 tooth wheel ud have very few teeth engaging. I forget the site that had a pulley calculator but it would show red with too few teeth engaging.
```

---
## \#129 Posted by: Maxid Posted at: 2016-06-24T06:07:38.623Z Reads: 341

```
just let him do it - I tried to reason with him and failed.
That 14t pulley in HTD3 is a comically small 13mm in diameter :scream:
```

---
## \#130 Posted by: claudiofiore88 Posted at: 2016-06-24T06:11:46.014Z Reads: 342

```
http://www.bbman.com/belt-length-calculator/

They don't recommend having less than 6 teeth in mesh at least for htd5.  Not sure about other profiles.
```

---
## \#131 Posted by: baxter Posted at: 2016-06-24T08:46:46.309Z Reads: 339

```
I think it is evident from this thread that known (and popular) motor KV ratings, motor and wheel pulley combinations and voltages are better in terms of performance than others.  With this in mind, as there are so many variables (and $) to take into consideration when building an e-board. I would be inclined to take their advice as those people are likely to be more familiar with the technical limitations of the VESC, and the likely combinations of various hardware if you decide to use them in your build. 

As the VESC can be customised so much, it is probably a bit of a stretch comparing it with other ESCs unless you are looking at your eboard having a specific purpose. 

Perhaps  @Sonic1 you might start a build/advice thread for your eboard?  How did you want your board to do perform/handle/accelerate?  With this in mind, I am sure the forum members will be more than happy to assist. :slight_smile:
```

---
## \#132 Posted by: Maxid Posted at: 2016-06-24T08:56:09.275Z Reads: 337

```
[quote="baxter, post:131, topic:3125, full:true"]
With this in mind, I am sure the forum members will be more than happy to assist.
[/quote]

No - but that is just me :wave:
```

---
## \#133 Posted by: Sonic1 Posted at: 2016-06-24T19:08:04.161Z Reads: 334

```
Htd 3 and an idler wheel are tried and true. Boosted with htd3, and the idler has been used in DIY, and Leif board is also the exact same drive.

@Maxid dude, you were already wrong on every factual point. I don't actually care what you think is comical. But it's your opinion to keep.  But I'm gonna call you out as an jerk for continuing to post your baseless negative crap.
```

---
## \#134 Posted by: Sonic1 Posted at: 2016-06-24T19:19:03.923Z Reads: 337

```
**Exactly this.** 

If a user posts things you don't understand and don't have experience with, don't make shit up. 

10mm motor shafts lol.
50kph top speeds
No pulleys bigger than 72
300kv can't work
Too many amps*
I'm Planning stuff that won't physically fit

All baseless and wrong. *amp draw is related to battery, rider weight, style of riding, gearing etc. without knowing those you can't say there's too many amps drawn. 65a on 4s is  2000w/2.7 HP. Logs show most riders never ever sustain a load like that.
```

---
## \#135 Posted by: jrpwit Posted at: 2016-06-24T19:41:51.506Z Reads: 327

```
Bruh can you just get off this thread and go make your own build thread cause your build is irrelevant to this topic. I was really enjoying this thread until you came in and started fighting with people who have a very good reputation on this forum. I not disagreeing with your built but this is not the thread to discuss it on.
```

---
## \#136 Posted by: Maxid Posted at: 2016-06-24T19:53:39.142Z Reads: 323

```
Maybe I enjoy being comically wrong.
If my posts are indeed so baseless a moderator should please tell me and I will stop. Until then I will keep posting my crappy posts. 
:wave:
```

---
## \#137 Posted by: Sonic1 Posted at: 2016-06-24T19:56:56.923Z Reads: 338

```
I can understand your opinion, and my main question for @chaka is still unanswered.

Since it's impossible to have 100% eff for erpm, why do you calculate based on unweighted rpm and 4.2v? No one want to de sync, but vedder states as high as possible, the closer to 8700rpm the better, more eff, less heat. 

Is this related only to the people who travel above 30 miles an hour sustained?

@jrpwit  However, I will stick up for myself and the facts.  The people who think it's cool to laugh at somebody when they don't have the facts on their side don't get a free pass, no matter how long they've been posting. Not calling them on wrongness won't help the general knowledge base.
```

---
## \#138 Posted by: gericke Posted at: 2016-06-25T15:16:31.208Z Reads: 343

```
hi guys can anyone help me choosing the right esc for the motor i have this is the specs for my motor. 

KV=210 Rpm/volt
Weight = 618gram
Battery = 10 cell LiPo
ESC = 70A
Power = 2450W (160class 2stroke)
Prop = 21x14 - 23x12

if anyone can help me.. it would be my plesure. thxx
```

---
## \#139 Posted by: akira Posted at: 2016-06-25T16:38:05.348Z Reads: 341

```
VESC would be perfect.
I doubt very much that you will be able to draw 70A from the motor or the ESC.
```

---
## \#140 Posted by: gericke Posted at: 2016-06-27T04:06:20.332Z Reads: 348

```
i was thinking of using  a 125a esc would that have any problem..
```

---
## \#141 Posted by: scisslehannd Posted at: 2016-07-01T20:40:33.997Z Reads: 340

```
Does anyone know where I can buy a VESC right now without having to wait for production???
```

---
## \#142 Posted by: elkick Posted at: 2016-07-01T20:46:16.115Z Reads: 350

```
I made some today, can be shipped on Monday.
 esk8.de
<img src="/uploads/db1493/original/2X/5/5047bb43ab591ccaa0e741ead6e757c8836e4796.jpeg" width="320" height="500">
```

---
## \#143 Posted by: Blacksheep Posted at: 2016-07-01T21:41:45.408Z Reads: 331

```
How much ? And from where?
```

---
## \#144 Posted by: claudiofiore88 Posted at: 2016-07-01T21:45:52.343Z Reads: 328

```
@elkick is the owner of www.esk8.de in Germany.
```

---
## \#145 Posted by: Blacksheep Posted at: 2016-07-01T21:50:01.463Z Reads: 335

```
O ok thanks
```

---
## \#146 Posted by: SFrider Posted at: 2016-07-04T21:46:20.077Z Reads: 338

```
Hi,
I am a new builder/user to this forum and I am very excited to be getting into such a fun project.  I live in SF where there are plenty of hills and I weigh about 145-150 lbs and was wondering what components I needed.  I will be running a single motor with the VESC, with 2x 4s 5000mah 20c Lipo in series.  I bought DIYelectricskateboard's 16T/36T motor mount kit as well.  SO what I don't know is what motor I need (been told 230kv is good) and does any suggestions for a comparable but cheaper alternative to DIYelectricskateboard's on/off antispark switch. Thanks to anyone who replies!
```

---
## \#148 Posted by: Ulfberht Posted at: 2016-07-10T01:04:09.311Z Reads: 333

```
@SFrider
http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204
```

---
## \#149 Posted by: sl33py Posted at: 2016-07-11T00:17:28.013Z Reads: 331

```
@SFrider - yeah the xt-90 anti-spark loop key is the uber simplest.  Alternatively you can make your own anti-spark switch.  If you want one, i have only a couple left.  Feel free to PM me if interested.  Here's the [ES thread in their sale section.](https://endless-sphere.com/forums/viewtopic.php?f=31&t=73800&p=1113414&hilit=spark#p1113414)
```

---
## \#150 Posted by: Hillso Posted at: 2016-07-17T16:44:48.371Z Reads: 333

```
So above 8570 RPM is less efficient (and prone to failure). but I don't understand if it's more efficient to be closer to the limit from below, VESC wise. For example, Is 8s 245kv (8,232 RPM) more efficient than 6s 245kv (6,174 RPM)? I'm not talking about motor efficiency.
Thanks.
```

---
## \#151 Posted by: torqueboards Posted at: 2016-07-17T17:19:10.190Z Reads: 329

```
@SFRider - We have 6355 170/190kv in the works for people who use higher voltage ranges. 5055 280KV/190KV options as well.
```

---
## \#152 Posted by: jrpwit Posted at: 2016-07-17T17:32:05.739Z Reads: 328

```
To my understanding the erpm of 8s on a 245kv motor is 50764 erpm with 3.7 volts cell (29.6*245*7=50764) and 57624 rpm with 4.2 volts cells (33.6*245*7=57624). So even if the cells were fully charged it is below 60k erpm so it is completely safe to run a 8s 245kv setup with the vesc.
```

---
## \#153 Posted by: Hillso Posted at: 2016-07-17T17:34:28.336Z Reads: 325

```
@jrpwit Thanks for helping, but I meant to ask Is much lower erpm than the limit is less efficient than closer to the limit?. Thanks. 
well my syntax sucks.
```

---
## \#154 Posted by: jrpwit Posted at: 2016-07-17T20:07:31.733Z Reads: 323

```
Anything under the 60,000 should be good. I would think that being close to 60k would be less efficient but anything under 60k will work fine.
```

---
## \#155 Posted by: Namasaki Posted at: 2016-07-19T23:55:41.114Z Reads: 345

```
I bought one on these Trackstar motor analyzers and tested it on a couple motors:
TB's 6355 230kv  Result 197kv
Alien 6355 190kv  Result 172kv
Both motors had results lower than there rating.
You would think that this analyzer could calculate KV at any rpm but it doesn't seem to work that way.
As I turned the knob and increased rpm, the KV went higher.
Because the rpm is limited to 2s voltage which is the max this analyzer can handle, I believe that it is not giving a true analysis of either motor.
Bottom line, this analyzer was a waste of money.
http://www.electric-skateboard.builders/uploads/db1493/original/2X/d/d8927fb71b190cae722def9ce983ad7d2cb65559.jpeg
```

---
## \#156 Posted by: Jinra Posted at: 2016-07-20T00:02:08.736Z Reads: 344

```
I used the VESC and calculated kV using erpm, duty cycle, and voltage measurements during bench testing and came out to 197kv on a 200kv motor with chaka's help. You could try that.

http://www.electric-skateboard.builders/t/ollinboardco-om5065-200kv-sensored-motor/3409/351?u=jinra
```

---
## \#157 Posted by: Bender Posted at: 2016-07-21T12:15:21.257Z Reads: 334

```
My TB 230kv motor is actually 198kv according to the VESC so that seems pretty accurate to me
```

---
## \#158 Posted by: Namasaki Posted at: 2016-07-21T15:38:43.028Z Reads: 333

```
Referring to the track star analyzer, why would  the KV increase as the rpm is ramped up ?
And it stops at 197 at 8 volts. 
What would it read if I could run it at 50v?
```

---
## \#159 Posted by: Bender Posted at: 2016-07-21T17:12:38.380Z Reads: 332

```
Good point
```

---
## \#160 Posted by: Namasaki Posted at: 2016-07-21T17:48:25.333Z Reads: 335

```
60k is what I'm shooting for. 
I'm gonna go with 10s and 190kv when my Vesc's arrive.
```

---
## \#161 Posted by: jrpwit Posted at: 2016-07-21T20:32:03.187Z Reads: 330

```
Longhairboy has used 12s 190kv and hasnt had a problem or maybe he has and I just haven't seen it yet
```

---
## \#162 Posted by: CSN Posted at: 2016-07-21T20:34:15.506Z Reads: 329

```
I think Photorph said he face planted on his LHB due to some VESC issue.

I seem to recall that anyway.
```

---
## \#163 Posted by: jrpwit Posted at: 2016-07-21T20:36:43.623Z Reads: 321

```
I stand corrected then. 10s 190kv is probably the sweet spot.
```

---
## \#164 Posted by: Tarzan Posted at: 2016-07-21T20:41:13.656Z Reads: 325

```
@longhairedboy @Photorph
Can someone confirm that?
```

---
## \#165 Posted by: Photorph Posted at: 2016-07-21T21:36:51.480Z Reads: 325

```
@CSN is basically right.  Well I didn't face plant but yes I did fall off while going downhill and braking because of an intersection that was coming up....because the brake cut out.  There is an issue with the brake cutting off because braking throws back more current than the VESC was prepared to handle.  This happens during aggressive braking at speed.  

There isn't really a way to resolve it fully, besides not braking hard while bombing hills.

@longhairedboy can be a better resource about whether or not to use 12s with 190 Kv motors, since his builds are using 12s4p on a dual drive 190 Kv r specs.
```

---
## \#166 Posted by: Ulfberht Posted at: 2016-07-21T21:54:39.213Z Reads: 324

```
@photorph This may be because of using the 63mm motors. Apparently they aren't the best match for the current iteration of the VESC 4.xx, There is a thread where @chaka explains the concept in good detail. Worth a read! :wink:
http://www.electric-skateboard.builders/t/are-50mm-or-63mm-motors-better-on-v4-12-vesc/6074/2
```

---
## \#167 Posted by: Namasaki Posted at: 2016-07-21T22:10:16.982Z Reads: 317

```
[quote="Photorph, post:165, topic:3125"]
There isn't really a way to resolve it fully, besides not braking hard while bombing hills.
[/quote]
Did you try adjusting the regen current setting in bldc?
```

---
## \#168 Posted by: Namasaki Posted at: 2016-07-21T22:14:23.158Z Reads: 316

```
60000/7
8571/190
45v
190kv might be within safe range with 12s
```

---
## \#169 Posted by: Jinra Posted at: 2016-07-21T22:27:13.357Z Reads: 314

```
Not under full charge, however. That'll hit 67k eRPM.
```

---
## \#170 Posted by: jrpwit Posted at: 2016-07-22T05:57:09.629Z Reads: 303

```
Can't wait for the new vesc so everyone can stop talking about erpm!
```

---
## \#171 Posted by: longhairedboy Posted at: 2016-07-22T12:55:39.985Z Reads: 311

```
12S on Enertion 190kv motors with VESC is fine as long as you don't slam on the brakes while bombing hills, which is kind of crazy town anyway in my opinion.  The motors run warm but not too hot, and the oomph you get from that voltage is lovely. If you give yourself time to stop so that you don't have to slam the brakes its not a problem, you can even ride the brakes down a hill to maintain a low speed and never see this issue. 

I never saw it happen until i gave @photorph his board and he went all suicidal on me trying to do 40+mph down a hill then slam on the brakes. I had to armor up and deliberately try to reproduce it before i ever saw it for myself. Scared me shitless when he first told me what happened. 

Am I correct in my understanding that VESC 6 will resolve this issue? That's what i keep hearing. 

BTW that issue also happens at 10S if you put enough force against those brakes.
```

---
## \#172 Posted by: Bender Posted at: 2016-07-22T14:24:21.030Z Reads: 304

```
Have you checked the fault codes on the VESC after this? are you getting abs over current?
I've read (on vedder's forum) you can increase the Aboslute current up to 240 which seems a lot, but would prevent these (hopefully rare) large current spikes from shutting down the VESC momentarily.
I think I'm going to slowly increase the value and see what happens.
```

---
## \#173 Posted by: onloop Posted at: 2016-07-22T15:04:28.757Z Reads: 299

```
Someone who is making some sense! Well said...

I think everyone forgets the settings in vesc can be changed.... 

Everyone just blames the size of the stator... 

P.S.  you can also change regen brakes and motor and at battery...  trial & error is recommended
```

---
## \#174 Posted by: onloop Posted at: 2016-07-22T15:06:44.784Z Reads: 299

```
[quote="Ulfberht, post:166, topic:3125"]
This may be because of using the 63mm motors. Apparently they aren't the best match for the current iteration of the VESC 4.xx,
[/quote]

I wish people would stop saying this..... its rubbish.
```

---
## \#175 Posted by: onloop Posted at: 2016-07-22T15:08:42.349Z Reads: 283

```
Screen grab of your vesc settings will help.
```

---
## \#176 Posted by: longhairedboy Posted at: 2016-07-22T17:55:21.082Z Reads: 287

```
That's sort of what i've been doing. The BMSs i'm using are rated at 80amps continuous so initially i started at 80 amps absolute max, but I'm going to keep bumping it up it till it stops. I've always based my motor amps max and min  on what the BMS/cells are capable of handling comfortably, but that may not be precisely what's required here. They can absorb some burst currents and i think things can be bumped up a bit to stop this nonsense based on what's being said here along with the specs of the cells and BMS. 

In fact if @photorph is ok with it i might hang on to his board a few more days (he sent it in for maintenance for which i don't charge because i'm cool like that)  so i can try to kill myself (figuratively speaking of course) a few more times on it and get this shit ironed out directly. 

The rain lately has been very much in the way of things.
```

---
## \#177 Posted by: Jinra Posted at: 2016-07-22T17:56:49.476Z Reads: 290

```
I know you use Supower's BMS's and I actually contact Lilian from them about this very BMS. Here's what she said

>Dear Pete,

>The BMS supports Burst current. It will shut off if the current continuing over 80A, but for burst, it could do 100A for very short time.

>It supports power switch.
```

---
## \#178 Posted by: longhairedboy Posted at: 2016-07-22T18:00:34.694Z Reads: 291

```
yep that's what my sheet says too. So this could easily become a game of who would you rather shut down first, the VESC or the BMS. Honestly i'm not sure the rider would know the difference, either way they're at the mercy of their belt tension for slowing down at that point.
```

---
## \#179 Posted by: longhairedboy Posted at: 2016-07-22T18:04:08.852Z Reads: 294

```
[quote="onloop, post:175, topic:3125, full:true"]
Screen grab of your vesc settings will help.
[/quote]

i'll take all the help i can get. I'll see if i can get some clean grabs tonight and post them. I'm no savant at vesc programming so i'm sure i'm missing something.
```

---
## \#180 Posted by: Jinra Posted at: 2016-07-22T18:06:00.214Z Reads: 289

```
You could always bypass BMS for discharge and rely on the VESC and fuse for current control.
```

---
## \#181 Posted by: longhairedboy Posted at: 2016-07-22T18:13:14.776Z Reads: 302

```
One reason i haven't done that yet is because i don't think the board will completely shut down when the cell groups reach minimum voltages if the discharge is still enabled and bybassing the BMS. Its not enough to tell people to get off when it gets to a certain voltage. You have to turn their shit off for them and make them walk/push or they'll just light their feet on fire when the 48 tiny pipe bombs they're standing on over discharge because we're human and we like to think that bad things won't happen to us and its only another mile what could happen. 

I'm totally guilty of thinking this way. I've broken so much shit because of it.
```

---
## \#182 Posted by: Jinra Posted at: 2016-07-22T18:14:49.382Z Reads: 293

```
Why not use the VESC battery cut off? It's much safer than the hard cut off from the BMS anyway.
```

---
## \#183 Posted by: longhairedboy Posted at: 2016-07-22T18:20:25.689Z Reads: 293

```
i'm having a huge duh moment here, forgive me. So brain sleepy lunch after.  I think i was conflating the voltage cuttoff with the max amps and other related VESC settings. That's totally worth experimenting with and i have just the board to try it out on.
```

---
## \#184 Posted by: Bender Posted at: 2016-07-22T21:17:17.880Z Reads: 293

```
I agree that it's not definitive, but at 10-12s single drive I do think we're pushing the limits of VESC 4.
Just trying to find ways to make it work😀
```

---
## \#185 Posted by: Photorph Posted at: 2016-07-22T22:06:01.951Z Reads: 297

```
@longhairedboy go ahead hang on to it for another couple of days and experiment with the VESC settings.  Testing is probably the hard/dangerous part, so be careful out there and dress for the fall.  

The brakes cut off when when you brake hard over a long duration, or brake from fast speeds.  And like you said they sometimes cut out intermittently and then come back.... But when you're going fast that intermittent cut out feels long enough to cause major problems to your physical well being lol.
```

---
## \#186 Posted by: Titoxd10001 Posted at: 2016-07-23T01:26:48.509Z Reads: 286

```
How would the vesc fail? Torque motor spins about 67k rpm on 12s. Would it launch you off the board going full speed?
```

---
## \#187 Posted by: CSN Posted at: 2016-07-23T01:29:57.742Z Reads: 285

```
would set your wallet on fire
```

---
## \#188 Posted by: Hummie Posted at: 2016-07-23T03:13:18.889Z Reads: 289

```
Woo that's a nightmare scenario.   Why is that happening.   At fast and slow speeds?  Maybe ur hitting ur high voltsge cut off with the increased voltage coming back while braking.  Spikes up to 10 volts I think.  The regen options don't shut things down I think.
```

---
## \#189 Posted by: GhettoFab.rictation Posted at: 2016-07-27T05:20:01.548Z Reads: 283

```
Could anyone possibly help? I'm having issues with windows and connecting the right firmware. I bought a brand new vesc from Ollinboard what's the firmware version with those vesc
```

---
## \#190 Posted by: Jinra Posted at: 2016-07-27T05:41:17.267Z Reads: 291

```
If you just got it, it should come with 2.18 h/w revision 4.12
```

---
## \#191 Posted by: GhettoFab.rictation Posted at: 2016-07-27T10:44:55.035Z Reads: 298

```
When I try to upload my firmware it starts with a different ip address, after I change that it then states buffer timed out
```

---
## \#192 Posted by: rodriguejoe1 Posted at: 2016-09-02T02:07:14.917Z Reads: 283

```
QUESTION: TRAMPA MTB
DUAL 6364 136 kv, 15 MOTOR/66 SLAVE PULLEY, DUAL OLLIN 4.12 VESCS, 180 LBS AND 225 LBS  RIDERS, (ONE AT A TIME), MOSTLY FLAT RIDING 95% OF THE TIME. I WILL HAVE TO FIT BATTERIES INTO A SQUARE BOX IN THE MIDDLE. I AM LOOKING FOR BATTERY SUGGESTIONS BASED ON KV SIZE AND AVAILABLE SPACE.
```

---
## \#193 Posted by: treenutter Posted at: 2016-09-06T13:27:10.510Z Reads: 255

```
A post was split to a new topic: [New Faraday Motor for Sale](/t/new-faraday-motor-for-sale/9059)
```

---
## \#194 Posted by: ThinkChink Posted at: 2016-09-07T04:03:33.097Z Reads: 275

```
Guys I need help. I will be running 8s 8000mah 15c lipos and a 12T/36T belt pulley set with a vesc. All thats left to run my board will be a suitable/proper kv rating motor that I am pondering over. Thinking of getting a 270kv 70-80A motor (need help distinguishing what's the difference if it's 40A compared to 70A cont amp motors), but would that be ideal for, say 30km/h? Also do sensored motors make much diff on a vesc as compared to a sensorless one?
```

---
## \#195 Posted by: ThinkChink Posted at: 2016-09-07T07:13:04.754Z Reads: 274

```
Also, after doing some calculations, I've found out that my proposed set up with 270kv motors and on 8s max voltage (33.6v * 270kv * 7 = 63504 RPM) is above the 60,000 rpm limit. Is 3000 rpm above the limit consider safe or dangerous already? What would being over the limit damage?
```

---
## \#196 Posted by: Jinra Posted at: 2016-09-07T07:16:38.194Z Reads: 268

```
The VESC runs at 95% max duty  cycle so you should be safe at 60328. It should quickly drop from max voltage anyway.
```

---
## \#197 Posted by: ThinkChink Posted at: 2016-09-07T07:22:26.424Z Reads: 266

```
So hooking up a 270kv motor on an 8s is fine? How did you come up with the 60328 rpm? Can you show me the calculation? Thanks @Jinra
```

---
## \#198 Posted by: Jinra Posted at: 2016-09-07T07:37:31.292Z Reads: 268

```
 It's 95% of your max erpm. I think you'll be fine on 8s, but it's a bit too close for my comfort. I was thinking of doing 260kv on 8s myself.
```

---
## \#199 Posted by: ThinkChink Posted at: 2016-09-07T08:17:31.154Z Reads: 268

```
Thanks for the valuable information. I am quite new to this so what are the dangers if I push past the 60000 rpm limit? Does my vesc fry or my motor overheats?
```

---
## \#200 Posted by: Jinra Posted at: 2016-09-07T08:18:07.747Z Reads: 265

```
VESC can fry, namely the drv8302 chip
```

---
## \#201 Posted by: ThinkChink Posted at: 2016-09-07T08:42:50.496Z Reads: 289

```
Alright will keep that in note. I have some other questions, say a particular motor has 270kv and draws continuous 40 amps, is it any different comparing to a 270kv with 80A continuous? Like in terms of performance and durability. That being said, my battery can draw a maximum of 120A. So would I be underperforming when I fit it with the 270kv 40A continuous as compared to the 80A continuous? Any other things to take note when using a 120A batt on either both of these motors?
```

---
## \#202 Posted by: DeathCookies Posted at: 2016-09-07T08:44:56.507Z Reads: 282

```
You can accelerate faster with more amperage.
```

---
## \#203 Posted by: ThinkChink Posted at: 2016-09-07T08:53:19.850Z Reads: 274

```
So although Vesc has a continuous amp of 50A, it can handle 80A motors just fine? I'm kinda new to this. Also I need to set my battery amp limit to 80A as well if Im using this setup?
```

---
## \#204 Posted by: Jinra Posted at: 2016-09-07T08:59:43.096Z Reads: 280

```
VESC can support 50a of continuous output from the battery, but motor current tends to be higher than what is being given by the battery and is measured in AC current. I'm not sure on the specifics but you should be fine with your setup.

If you want to be cautious about erpm, I'd limit it to 60k on bldc tool
```

---
## \#205 Posted by: ThinkChink Posted at: 2016-09-07T09:21:57.611Z Reads: 268

```
Alright. Nice, I think I will proceed with this setup then. Thanks for the info!
```

---
## \#206 Posted by: ThinkChink Posted at: 2016-09-07T09:34:07.427Z Reads: 270

```
One last question. How advisable is it to buy no-brand motors from China? I mean they probably distribute to hobby retail shops and the such, then resellers might rebrand them. Im not sure if they are distributors, but I wanna know if getting a motor from turnigy or hobby sites are more recommended than buying no-brand China motors? Might be a dumb question here, but I'm curious.
```

---
## \#207 Posted by: TarzanHBK Posted at: 2016-09-07T10:14:34.908Z Reads: 274

```
there are some people buying cheap motors and are really fine with them, but there are also a few with some problems.
normally it´s not much of a difference with the price tag between a china motor with taxes and shipping, or just get a good, tested motor from one of the suppliers here on the forum.
```

---
## \#208 Posted by: ThinkChink Posted at: 2016-09-07T11:29:52.046Z Reads: 267

```
Say, even if there's problems with the motor, what's the worst it could do to a VESC?
```

---
## \#209 Posted by: Randyc1 Posted at: 2016-09-07T13:57:59.994Z Reads: 263

```
You can allways limit the erpm in the Vesc !
```

---
## \#210 Posted by: TarzanHBK Posted at: 2016-09-09T07:36:26.428Z Reads: 264

```
some people fried their vesc due to a short caused by bad motor wiring and shorting cables. Usually the DRV chip at the vesc is dead at this point and you need to get it changed.
```

---
## \#211 Posted by: ThinkChink Posted at: 2016-09-16T14:49:03.129Z Reads: 257

```
guys... now what happens if I run a 8s powering a 320kv motor? @TarzanHBK @Jinra
```

---
## \#212 Posted by: Jinra Posted at: 2016-09-16T15:01:15.920Z Reads: 260

```
limit erpm and considering getting a more suitable motor down the line.
```

---
## \#213 Posted by: ThinkChink Posted at: 2016-09-16T15:04:04.711Z Reads: 261

```
means to say that my motor will be under utilized then?
```

---
## \#214 Posted by: Jinra Posted at: 2016-09-16T15:15:51.945Z Reads: 261

```
it's not going to be running efficiently, I'm not sure what you mean by underutilized. You may be lacking in torque due to thicker windings and less copper in the stator.
```

---
## \#215 Posted by: ThinkChink Posted at: 2016-09-16T15:42:09.384Z Reads: 266

```
Is it true that the minimum for entry level eboards is 270kv to start off? Cause I've seen an instructables before using 270kv sk3 motors and I dont know if that's the highest kv value acceptable on an eboard or that it's just a resulting kv value suited for his setup.
```

---
## \#216 Posted by: Jinra Posted at: 2016-09-17T13:50:39.989Z Reads: 261

```
probably because 270kv is a good value for 6s which is the max voltage a lot of hobby escs run at. I run 10s myself which 190kv-200kv motors are great for.
```

---
## \#217 Posted by: TarzanHBK Posted at: 2016-09-17T15:41:59.861Z Reads: 276

```
our outrunner run perfect in their most efficient erpm limit with the vesc. Our current vesc version is fine with 60.000erpm.
if you exceed that, your motor could start stuttering and the vesc can´t keep up how fast it is spinning. if you stay way under 60.000erpm you´re not using the full potential and your motor eats more current, so that you´ll lose some range.
so try to pick a good combo according to chakas article :slight_smile:
```

---
## \#218 Posted by: ThinkChink Posted at: 2016-09-20T00:41:05.944Z Reads: 268

```
My vesc runs 4.18. Are there any differences regarding change in ERPM true limit? Just got it like 2 weeks ago.
```

---
## \#219 Posted by: Jinra Posted at: 2016-09-20T00:56:52.058Z Reads: 275

```
I think you mean hw 4.12, sw 2.18. No change in limit, still roughly 60k
```

---
## \#220 Posted by: Fetteperson Posted at: 2016-09-20T16:56:53.346Z Reads: 279

```
I got a little different question... 

I've got a VESC with 12s setup, current limit 50amp, everything else, default. This VESC is connected to a EMAX GT5345/08 190KV motor, then it has a gear-ration of 15/40 and 97mm wheels. Top-speed is really nice, 40+ km/h but going uphill it has no force with me (90kg, 200lbs). But my friend (60kg/ 130lbs) can go uphill with no problems. Before I had the VESC I had a 120amp ESC and with this ESC I had no problems going uphill (6s setup). 

What can I do? I don't really want a dual-motor setup. I will change gear ration to 10/40, but I guess this won't be enough. Do motors with same watt have different power in real-world? Does anyone with 200lbs+ have experience.
```

---
## \#221 Posted by: TarzanHBK Posted at: 2016-09-23T12:27:25.815Z Reads: 294

```
[quote="Fetteperson, post:220, topic:3125"]
EMAX GT5345/08 190KV motor
[/quote]

this thing is rated 85A constant, so adjust your batt max limit to 85A - that will help ;)

also have you done your motor detection?
```

---
## \#222 Posted by: Fetteperson Posted at: 2016-09-23T16:10:43.428Z Reads: 282

```
Don't I risk to break the vesc, because it is rated at 50amps constant?
```

---
## \#223 Posted by: Hummie Posted at: 2016-09-23T17:19:34.293Z Reads: 287

```
if you set it to 80 you'll be fine and have more peak power.  if you sat on the throttle too long, and actually did do 80 amps continous, there is a temp sensor in the vesc near the fets that will shut it down if it gets too hot.
```

---
## \#224 Posted by: Fetteperson Posted at: 2016-09-25T10:03:03.300Z Reads: 283

```
I have set motor max to 85amps, and it works fine now. The only problem is heat... I have bought some heatsink and will try it with that
```

---
## \#225 Posted by: bigben Posted at: 2016-09-25T22:49:59.061Z Reads: 281

```
Has anyone run a hobby king 245kv motor with the vesc on 9s lipo? Standard drive system 15 tooth 36 tooth. 
To my untrained eye it sits well if run through the calculator. 
Could I be missing something?
```

---
## \#226 Posted by: Jinra Posted at: 2016-09-25T23:03:36.540Z Reads: 280

```
you can potentially burn out the VESC as it exceeds eRPM limitations. 8s is safe.
```

---
## \#227 Posted by: TarzanHBK Posted at: 2016-09-26T14:27:28.466Z Reads: 278

```
i´m building one at the moment 9s lipo 245kv sk3 6364. Which brings the motor to a bit under the limit but i´ll limit erpm to 60000 just to be safe. 50km/h about 32mph with 13/32 83mm
:monkey:
```

---
## \#228 Posted by: GhettoFab.rictation Posted at: 2016-09-27T09:42:21.465Z Reads: 272

```
Has anyone gone to 65000 erpm or between 60k and 70k safely
```

---
## \#229 Posted by: GhettoFab.rictation Posted at: 2016-09-27T09:44:39.848Z Reads: 275

```
I have 12s 149kv wanting more out of the setup. I also need different gear ratio but until I get more parts I am curious about max amps and rpm on 6374 sk3 149kv running Samsung 25r liion
```

---
## \#230 Posted by: GhettoFab.rictation Posted at: 2016-09-27T09:46:06.565Z Reads: 268

```
If motor max is 70a can I exceed by one or two and be ok with a fan bolted on the back of it working with the integrated fan
```

---
## \#231 Posted by: TarzanHBK Posted at: 2016-09-27T10:46:03.560Z Reads: 274

```
it could work but it´s not safe! if your motor starts stuttering you could get thrown off your board. Vedder mentioned that the vesc is capable of 100.000 erpm, but a few people had problems going over 60.000. So better to stay under that and be safe. :beetle:
If you still want more after a new gear set add a second motor for a diagonal drive and gear down further, so that you get more speed and split the torque over the two motors.
Also leave the vesc max motor setting to the actual motor max. Otherwise if you exceed that and supply your motor with too much current, keep your phone ready to supply us with a video of your smoking motor :monkey:
```

---
## \#232 Posted by: GhettoFab.rictation Posted at: 2016-09-27T18:40:45.202Z Reads: 258

```
Hah ok 60k it is I'll have to wait for the gears
```

---
## \#233 Posted by: aldopopp Posted at: 2016-09-28T15:34:24.291Z Reads: 259

```
i have pretty much read all the topic, and a lot ov other articles on this forum, but i still have no idea what erpm represents... what does it mean? and how does it realte to the actual rpms of the motor running?
```

---
## \#234 Posted by: Jinra Posted at: 2016-09-28T16:09:02.380Z Reads: 257

```
erpm is the number of pole pairs the motor runs through per minute. Most 50-63mm motors have 7 pole pairs (7 pairs of magnets on the rotor can, so 14 total). This translates to 1 rpm = 7 erpm, or 60,000 erpm = 8571 rpm
```

---
## \#235 Posted by: aldopopp Posted at: 2016-09-28T16:41:09.261Z Reads: 261

```
Thanks a lot!!! I have learnt a whole lot of things about eboarding lately just thanks to this forum, so many valuable informations... The only thing holding me back right now from starting a build is the lack of funds hehehe
Thanks to the community in General too!!
```

---
## \#237 Posted by: dfox Posted at: 2016-10-01T04:14:04.593Z Reads: 260

```
so if i had 8570rpm/245kv motor 33.3v with 9s lipo would it run to hot with the vesc
```

---
## \#239 Posted by: gen3ticmutation Posted at: 2016-10-08T04:49:29.576Z Reads: 258

```
Hey guys, trying to design an eboard. Can I use a 280kv motor ([http://www.hobbyking.com/hobbyking/store/__28139__Turnigy_Aerodrive_SK3_5055_280kv_Brushless_Outrunner_Motor_US_Warehouse_.html]()) with the vesc with 5000mAh 6s LiPo batteries? it is my understanding you'd never want to have a 60a draw on your motor when the vesc is only rated for 50a draw? Thanks!
```

---
## \#240 Posted by: TarzanHBK Posted at: 2016-10-10T10:24:43.582Z Reads: 264

```
its a bit too small for a single motor depending on how heavy you are.
Best for a single motor setup: a 6364 or 6374 motor
also a 6355 or 6354 will work, but is mostly used for dual setups.

and again depending on how heavy you are, a 6s system will not work good with a vesc because of the high current draw.
```

---
## \#241 Posted by: gen3ticmutation Posted at: 2016-10-10T19:31:53.933Z Reads: 259

```
Thanks for the advice. looking into 63mm motors now.
```

---
## \#242 Posted by: Hummie Posted at: 2016-10-10T19:50:09.697Z Reads: 262

```
You can forget any amp ratings of the motor. They're mostly bull anyway and it depends how the motor is being cooled.  It's really just a temp limit related to the magnets' temp operation range.  As long as your motor doesn't get the magnets beyond this temp ur fine.  What temp are the magnets good for in ur motor?? They rarely tell.
```

---
## \#243 Posted by: jmasta Posted at: 2016-10-17T19:48:23.887Z Reads: 270

```
I am using a Turnigy SK3 6374 149kv @ 12S.  HobbyKing states it has 18 turns (18T).  Would this imply the motor has 9 pole pairs?

So then, ERPM_max = (50.4 V)*(149 rpm/V)*9 = 67,600 ERPM

Assuming this is correct, what would be a good value to program into the VESC (v4.12)?  70,000?
```

---
## \#244 Posted by: Hummie Posted at: 2016-10-17T19:49:42.915Z Reads: 266

```
pole pairs is related to how many magnets solely I think.  you likely have 14 magnets.  so 7 pole pairs
```

---
## \#245 Posted by: jmasta Posted at: 2016-10-17T19:53:34.784Z Reads: 271

```
Great thanks!  So even at max loading, my ERPM wouldn't be over 53,000
```

---
## \#246 Posted by: hackeralf Posted at: 2016-10-21T06:39:42.484Z Reads: 268

```
I'm using the 6374 170KV sensor motor and the VESC from here. http://www.michobby.com/product/vedder-vesc-for-electric-skateboards/ 
http://www.michobby.com/product/maytech-6374-170kv-brushless-sensor-motor-for-electric-skateboardse-bike-copy/
WOW, they are promoting the VESCs with limited offer now. Anyway, the VESC and the 6374 motor are pretty good. Hope it is helpful for you, folks. I was using the 5065 motors and a 120A car ESC, but the 6374 with the VESC is fantastic. You can feel it!
```

---
## \#248 Posted by: SirDiff Posted at: 2016-11-13T12:47:59.279Z Reads: 250

```
Can you please not spam your own site like it wasn't yours? We aren't stupid and those electric skateboards are not the best
```

---
## \#249 Posted by: ACIN Posted at: 2016-11-13T16:35:20.837Z Reads: 256

```
Ah sweet, was looking for this.
Now I am running TWO 190kv MAYTECH Motors (since I want the grip, the torque for hills and because I can ;)), so in theory this should match my 3 5Ah 4S1P (14.8v each) 25C LiPo's perfectly right? (8570rpm/44.4v= 193kv)

So how does running dual motors affect this? If my physics class memories don't fail me here I think that I don't need to (heck - I shouldn't) run double the voltage if I run the vescs in parallel (which I will do obviously), but the motors will suck more current, probably around double, right? 

If want to achieve around 12-14km range, firstly great torque and secondly a topspeed of roughly 40km/h (me being 65kg light, medium hills around, 15/32 Gearing, 83mm Wheels planned), should I consider upgrading the Capacity of my batteries to - say 8000mAh? (I have heard the general rule is around 6-7 miles for 5000mAh, just want some clarification for dual motors)

Cheers!
```

---
## \#250 Posted by: NickTheDude Posted at: 2016-11-13T17:13:16.657Z Reads: 240

```
12S is a bit high for a 190kV motor. Your nominal voltage is 44.4 (3.7 * 12), but when they're fully charged the voltage is 50.4 (4.2 * 12) volts. I think 10S is what most people go for.

Since the amount of watts (volts * amps) required to move you doesn't change, the amps for each of your motors is effectively half of what would be required in a single motor setup.

For range, you need to calculate the watt hours of your battery pack (how many watts can be used continuously for a full hour before the pack is empty). Watt hours is equal to amp hours multiplied by volts (1Ah = 1000mAh). A general estimate is that 10Wh will give you 1km of range.
```

---
## \#251 Posted by: Hummie Posted at: 2016-11-13T17:16:21.701Z Reads: 243

```
the vesc will put out whatever you program it to do.  What amp limit was it set at when you ran it solo? Maybe you have enough power ability already you just haven't pushed the vesc to its limit.
```

---
## \#252 Posted by: ACIN Posted at: 2016-11-13T19:31:17.051Z Reads: 243

```
Thanks so much Nick
```

---
## \#253 Posted by: fraannk Posted at: 2016-12-06T07:53:07.862Z Reads: 241

```
I've just ordered this: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6354-260kv-brushless-outrunner-motor.html
They're 260KV but 18T (which means 9 pole pairs, right?) Are these too much on 8S? It seems they are based on the calculations
```

---
## \#254 Posted by: Strange4209 Posted at: 2017-01-20T02:11:01.801Z Reads: 228

```
I just order a 6374 190kv 3150w and got a 12s2p coming with a vesc. 
(It's all coming)   x) haha

But how should this perform in your experience if I run things "not to hot, not to cold".(60-70k)
 As in top speed and range. I have 97mm wheels and enertion 15 36
```

---
## \#255 Posted by: NickTheDude Posted at: 2017-01-20T02:17:54.545Z Reads: 226

```
You can use this calculator to get an idea of your top speed: http://calc.esk8.it/

To get your range you can multiply voltage by amp hours to get watt hours. A general estimate people use is 10 watt hours per kilometer of range. Keep in mind, that estimate will change based on how hard you ride, how often you are going up/down hill and your weight.
```

---
## \#256 Posted by: Strange4209 Posted at: 2017-01-20T02:26:59.014Z Reads: 225

```
Ok thank you, I've seen this I just didn't know if the motor size (6374) made any difference compared to the 6355.. the one I've ordered is 3150 w and the smaller 190kv motor is 2500 I believe.
Also, will my set up run hot you think? Or can my vesc protect that.
Just trying to play it super safe. After a solid month of obsessive research I finally pulled the trigger on a $1000 budget. And met it perfectly with a helmet extra belts and a few other things to boot.

I am 25, 160 pounds and my citys/towns are generally flat. With a couple decent hills here n there.
```

---
## \#257 Posted by: NickTheDude Posted at: 2017-01-20T02:31:39.903Z Reads: 218

```
The only difference having a larger motor makes is that it can produce more power before overheating. The VESC is very powerful when it comes to protecting your board but it can also be a curse if you don't know how to configure it correctly. Make sure you do a lot of research and find the right amp limits for you. Being relatively low weight, you won't have any trouble in flats with that motor, but you could have a little difficulty with hills depending on how steep/long they are. Just make sure to get some speed before the hill and you shouldn't have any problems.

The beauty of the VESC is that you can set it up for whatever range of power you want, so start low and build up to what feels comfortable.
```

---
## \#258 Posted by: psychotiller Posted at: 2017-01-20T02:33:32.674Z Reads: 213

```
And my prices on those parts are better than his...
```

---
## \#259 Posted by: Strange4209 Posted at: 2017-01-20T02:44:31.092Z Reads: 227

```
Nice to actually talk to you after a month of seeing your posts.... just joined today.

I'm actually about to order one of your enclosures for now.  I was going back and forth between you and the space case and I got the space case.
But, I got a 36" bamboo drop threw coming and I worried about the flex so the space case will be for my next build. Gunna do a dual drive with a little stiffer board for the case.
```

---
## \#260 Posted by: psychotiller Posted at: 2017-01-20T02:52:02.164Z Reads: 228

```
I just made custom dual enclosures for someone with a flexy vanguard. I have the molds and they are roomier than boosted's by a long shot!

$100 bucks shipped in the USA
<img src="/uploads/db1493/original/3X/e/5/e5e8163cf0bebe546738485bac11dcd32185f32f.jpg" width="689" height="390"><img src="/uploads/db1493/original/3X/4/5/45b3e0c9bb33cffc2441b5e317420fed9c160817.jpg" width="689" height="390">
```

---
## \#261 Posted by: Strange4209 Posted at: 2017-01-20T02:52:30.323Z Reads: 223

```
And thank you for the info nickthedude. It's good to know that even with the 12s my vesc will stay happy and I can tell it to keep my motors happy too.
And power is one thing I kinda crave but I crave reliability even more.

I rode ( it like I stole it ) yamaha dirt bikes my whole life with passion and for fun, but traded off my yz450f for a Harley 2 years ago. 
Well, I won a free swagboard in a raffle at work during Christmas time and I fell DEEPLY in love with a children's toy.
All I could think was ,
More speed, more power,  more range , more stability... more more more.
Until I've found myself patiently awaiting some super sweet parts.
```

---
## \#262 Posted by: Strange4209 Posted at: 2017-01-20T03:02:44.574Z Reads: 224

```
And I was thinking your Flagshipv2 on this board I have coming to me now. It's 9 ply, coming with griptape.  Do you think it will create gaps with a Lil flex... and thinking once I have the board dialed in to just seal it off indefinitely  ( till it shells of coarse )

<imgsrc="/uploads/db1493/original/3X/5/c/5ca34d651b9812fbf016bc357c485d8d4d2aad8c.png" width="281" height="500">
```

---
## \#263 Posted by: Strange4209 Posted at: 2017-01-20T03:30:08.017Z Reads: 231

```
<img src="/uploads/db1493/original/3X/5/c/5ca34d651b9812fbf016bc357c485d8d4d2aad8c.png" width="281" height="500">
```

---
## \#264 Posted by: lox897 Posted at: 2017-01-20T19:20:51.475Z Reads: 231

```
@psychotiller @Strange4209 Please keep your posts on topic. Any more off topic posts will be removed from this thread. Please use PM. Thank you
```

---
## \#265 Posted by: Strange4209 Posted at: 2017-01-20T20:39:59.148Z Reads: 227

```
10/4 man just excited about my build....
```

---
## \#266 Posted by: sova Posted at: 2017-03-19T13:19:51.893Z Reads: 224

```
@chaka 
I have 10s LiPo batteries, 245kv motor and TorqueBoards VESC..
i calculated the ERPM: 63455.
Is the value too high, or do you still consider it safe?
```

---
## \#267 Posted by: TarzanHBK Posted at: 2017-03-22T12:15:06.419Z Reads: 221

```
limit your erpm in the bldc tool to 60.000 and you´re good to go
```

---
## \#268 Posted by: Bender Posted at: 2017-03-22T12:32:39.014Z Reads: 229

```
Also that is you no load max.
With weight on the board and a belt you'll never hit that ERPM.
Just be carful bench testing cause you can reach that ERPM and burn out the vesc so, the 60000 limit is still a good idea.
```

---
## \#269 Posted by: aras_96 Posted at: 2017-03-22T21:51:17.794Z Reads: 234

```
Hello everyone :smiley:

If i use dual turnigy sk3 260kv motors and dual vesc.
10 x 4.2 = 42v
42v x 260kv = 10,920 RPM
10,920 RPM x7 = 76,440  ERPM
You guys would advise that this is not suitable right.

So do you think this will work. dual torqueboards 190kv motors at 12s or 10s?
10 x 4.2 = 42v
42v x 190kv = 7980 rpm
7980 x 7 =55860 erpm

12 x 4.2 = 50.4v
50.4 x 190kv = 9576 rpm
9576 x 7 = 67032 erpm

Would the 190kv at 12s be okay as its going over 60000?
```

---
## \#270 Posted by: mmaner Posted at: 2017-03-22T22:22:19.343Z Reads: 224

```
[quote="aras_96, post:269, topic:3125"]
Would the 190kv at 12s be okay as its going over 60000?
[/quote]

It will be fine as long as you set the ERPM limit in the VESC settings to 60,000.
```

---
## \#271 Posted by: aras_96 Posted at: 2017-03-22T22:37:27.028Z Reads: 221

```
what would happen if i didnt set it to 60000, would the vesc blow and what would make it blow?
```

---
## \#272 Posted by: mmaner Posted at: 2017-03-23T02:02:33.450Z Reads: 216

```
Yes it would blow the VESC.  Going over 60k ERPMs is what makes it blow.   If you want to know exactly what happens I'd suggest checking out the vedder forums. A quick Google search should get you there.
```

---
## \#273 Posted by: sova Posted at: 2017-03-25T18:16:21.446Z Reads: 212

```
I will, thank you! :slight_smile:
```

---
## \#275 Posted by: Badkad Posted at: 2017-04-08T13:30:28.287Z Reads: 213

```
Does the 60k erpm apply to 7 pole motors only? 

What if I used a 4 pole motor? (not necessarily on an esk8)
```

---
## \#276 Posted by: Hummie Posted at: 2017-04-08T15:55:36.120Z Reads: 219

```
we're almost all using 14 magnets which gives us 7 switches for a full rotation.  you still have the same erpm limit and would do the same math to figure your erpm.
```

---
## \#277 Posted by: Badkad Posted at: 2017-04-08T18:26:35.004Z Reads: 221

```
So how is this working? 2200kv x 25.2v x 4 poles = 195360erpm?

https://www.youtube.com/watch?v=3puKPFVUfdc
```

---
## \#278 Posted by: Hummie Posted at: 2017-04-08T19:28:42.653Z Reads: 215

```
maybe I'm wrong but I think it's 
voltage x kv x half your poles so 7 for most of us.
or you could limit the max erpm with the bldc tool on your pc
```

---
## \#279 Posted by: PXSS Posted at: 2017-04-08T21:19:03.127Z Reads: 211

```
2200kv x 25.2 x 2 = 110880 eRPM
2200kv x 25.2 = 55440 RPM
```

---
## \#280 Posted by: NICOMUTTER Posted at: 2017-04-10T10:22:45.622Z Reads: 209

```
Hello Hummie,
I saw that you probably have the same VESC that me, and I have some questions about it, coulsd you help me on it ? ;)
```

---
## \#281 Posted by: Hummie Posted at: 2017-04-11T20:14:06.049Z Reads: 210

```
We likely all have similar vescs and I'm no expert but if u have question...
```

---
## \#282 Posted by: NICOMUTTER Posted at: 2017-04-12T08:18:24.256Z Reads: 208

```
I sent you an mail :)
```

---
## \#283 Posted by: Jammeslu Posted at: 2017-04-12T11:26:18.262Z Reads: 213

```
quick question, what would work the best in terms of balance between top speed, tourqe and battery efficiency if I run 8s3p      245kv or 213kv both turnigy sk3 63xx motors
```

---
## \#284 Posted by: Eboosted Posted at: 2017-04-17T07:05:57.094Z Reads: 215

```
Is it possible to datalog ERPM via HM-10 bluetooth device?
```

---
## \#285 Posted by: rpn314 Posted at: 2017-04-26T13:52:58.471Z Reads: 213

```
[quote="Eboosted, post:284, topic:3125, full:true"]
Is it possible to datalog ERPM via HM-10 bluetooth device?
[/quote]

Most do that I'm aware of. Any of the apps that are getting a speed from the VESC itself (ie. that isn't based on the GPS of the mobile device) use ERPM, the motor pole count, the gear ratio, and the wheel size to calculate it.
```

---
## \#286 Posted by: Eboosted Posted at: 2017-04-27T02:40:52.106Z Reads: 197

```
Thanks man! I'll try that ASAP
```

---
## \#287 Posted by: dedinski Posted at: 2017-04-27T22:15:49.647Z Reads: 195

```
Have you tried the 9s 245kv combination? Does it work well?
```

---
## \#288 Posted by: TarzanHBK Posted at: 2017-04-30T07:42:13.974Z Reads: 199

```
That combination will rip your a++ apart 😃
Should work really well, but you have to limit erpm
```

---
## \#289 Posted by: dedinski Posted at: 2017-04-30T08:07:13.465Z Reads: 192

```
Are you using this configuration?
```

---
## \#290 Posted by: TarzanHBK Posted at: 2017-04-30T08:09:40.659Z Reads: 197

```
No. I left my first Board with 6s 245kv and a car esc and continued with 190kv 10s vesc dual
```

---
## \#291 Posted by: dedinski Posted at: 2017-04-30T08:16:27.641Z Reads: 205

```
Would you say its a big difference between the two? Id live to try a dual, but no one here uses eskate..
```

---
## \#292 Posted by: TarzanHBK Posted at: 2017-04-30T08:24:51.670Z Reads: 206

```
It's much smoother and powerful. Especially if you live in a hilly terrain, if you weight more than 80kg or if you just wanna go BOoom ☺
```

---
## \#293 Posted by: Eboosted Posted at: 2017-04-30T17:58:24.257Z Reads: 199

```
How reliable would be to run 12s on 190KV limiting ERPM on the VESC? Is it too risky?
```

---
## \#294 Posted by: Daan_vZon Posted at: 2017-05-01T14:27:33.066Z Reads: 194

```
@chaka I use a 10S (**_36V_**) Space Cell Pro4 battery and a 6355 **_260KV_** EPOWER MOTOR. According to your calculations this results in 65.520 ERPM. Is this a good setup? Or is it wise to limit the ERPM on the VESC? I use an Enertion VESC-X. Not sure how much ERPM it is able to take.
```

---
## \#295 Posted by: Eboosted Posted at: 2017-05-01T14:42:31.033Z Reads: 189

```
Have you used this setup at maximum speed? Have you restricted maximum ERPM on VESC settings?
```

---
## \#296 Posted by: Daan_vZon Posted at: 2017-05-01T15:03:38.155Z Reads: 192

```
No, still assembling this setup, since my VESC had a failure and I have to wait until replacement parts arrive. So I haven't been able to use it at maximum speed yet, but I didn't restrict the ERPM on VESC settings yet either. I think it would be wise to set these at around 60.000 instead of the standard 100.000 right?
```

---
## \#297 Posted by: Eboosted Posted at: 2017-05-01T15:51:51.943Z Reads: 183

```
Yes, you need to do that
```

---
## \#298 Posted by: Jinra Posted at: 2017-05-01T16:05:06.940Z Reads: 192

```
IIRC someone set their eRPM limit on the VESC, but it's a hard limit meaning the VESC was shutting off when they hit that limit. I haven't confirmed this myself, just something i remember reading.

That said, it's much better to correctly configure your hardware, I'd get a =< 200kv motor for a 10s setup and leave the erpm limit alone. I use 10s 200kv personally and left the eRPM at the default 100k
```

---
## \#299 Posted by: boardman5000 Posted at: 2017-05-01T17:45:57.049Z Reads: 191

```
@Jinra what motor setup are you using if you don't mind me asking?
```

---
## \#300 Posted by: Jinra Posted at: 2017-05-01T18:07:42.065Z Reads: 193

```
My two builds. One is 10s 200kv, the other is 10s 190kv:

https://www.electric-skateboard.builders/t/honey-driver-honey-velocity-v3-deck-caliber-iis-83mm-evolve-gt-wheels-dual-om5065-200kv-space-cell-pro4-diy-pulleys-enertion-pulley-bones-super-reds-enertion-mounts-winning-remote-chaka-vescs-build-complete/5760

https://www.electric-skateboard.builders/t/carbonated-enertion-vescs-hi5ber-overtaker-custom-10s4p-25r-pack-with-cell-level-fusing-abec-flywheels/10879
```

---
## \#301 Posted by: Eboosted Posted at: 2017-05-03T06:38:59.320Z Reads: 186

```
If we compare a 230KV with a 190KV 6355 motor on 10S, would the 230KV have noticeable less torque from a dead stop?
```

---
## \#302 Posted by: boardman5000 Posted at: 2017-05-19T14:52:44.431Z Reads: 177

```
I would think it would be pretty noticeable, I'm not 100% since I havent tested this on the street though. I know my unsensored 230kv "feels" like it's got next to no torque compared to my buddies 190kv sensored , if that makes any sense lol.
```

---
## \#303 Posted by: Eboosted Posted at: 2017-05-19T15:18:39.221Z Reads: 178

```
What's pullies are you runing in the 230kv? 10S battery?
```

---
## \#304 Posted by: NickTheDude Posted at: 2017-05-19T16:28:00.772Z Reads: 178

```
If you change the pullies of the 230kV to match the top speed of the 190kV torque would be identical. However you'd hit the ERPM limit on a VESC with the 230kV.

Without changing the pulley the 230kV setup would be ~10km/h faster than the 190kV which is pretty significant.
```

---
## \#305 Posted by: Jinra Posted at: 2017-05-19T16:31:09.903Z Reads: 182

```
In my post about KV's I found that my 230kv motors run at about 210 which puts me below eRPM limit. You should be able to run 230's on 10s just fine on some motors.
```

---
## \#306 Posted by: Eboosted Posted at: 2017-05-19T16:55:25.608Z Reads: 177

```
Thanks @NickTheDude and @Jinra, those are the answers I've been looking for.

For a 15/40T pulleys think I found the sweet KV spot @ 230KV, I also researched the 230KV is much easier to push than a 170KV or even 190KV motor
```

---
## \#307 Posted by: NewbieBoardBuilder Posted at: 2017-07-03T14:00:46.675Z Reads: 156

```
So I can't do 190kv for a 12S?!?!
```

---
## \#308 Posted by: jaymu86 Posted at: 2017-07-03T14:03:25.884Z Reads: 156

```
Stick with 10s and read read read erpm limit
```

---
## \#309 Posted by: NewbieBoardBuilder Posted at: 2017-07-03T14:05:18.153Z Reads: 160

```
[quote="jaymu86, post:308, topic:3125"]
read read read erpm limit
[/quote]

ERpm limit of what? Where?
```

---
## \#310 Posted by: wafflejock Posted at: 2017-07-03T15:04:06.985Z Reads: 157

```
Use the search, type erpm see answers.  People here don't mind helping but don't make people spoon feed you info you can search by clicking the search icon.  If you can't find the answer or don't understand then post your question and reference the stuff you've read and what you don't understand.
```

---
## \#311 Posted by: NewbieBoardBuilder Posted at: 2017-07-03T18:11:47.220Z Reads: 161

```
<img src="/uploads/db1493/original/3X/f/6/f6de8b741bf5bcc3d199233ac83c525652ecb269.PNG" width="281" height="499"> I think diy electric has it wrong then?
```

---
## \#312 Posted by: jaymu86 Posted at: 2017-07-03T19:14:20.569Z Reads: 152

```
No follow what he tells you if buying his equipment just Kno that setup is very close to erpm limit
```

---
## \#313 Posted by: NickTheDude Posted at: 2017-07-03T19:17:29.135Z Reads: 153

```
@NewbieBoardBuilder learn what kV, voltage and the VESC ERPM limit are. Then you'll never have to ask a question about it again and you can figure this stuff out without constantly having to consult people.
```

---
## \#314 Posted by: NewbieBoardBuilder Posted at: 2017-07-03T20:14:11.060Z Reads: 160

```
I've done my research! Why are you worried about ERPM limits if you can just set a max on the vesc?
```

---
## \#315 Posted by: NewbieBoardBuilder Posted at: 2017-07-03T20:15:34.065Z Reads: 168

```
<img src="/uploads/db1493/original/3X/2/2/229309081c5480ad0c68388d53b78be0d3d8264e.JPG" width="454" height="500">
```

---
## \#316 Posted by: jaymu86 Posted at: 2017-07-04T01:33:57.852Z Reads: 164

```
Sometimes you gotta pretend they not there lol
```

---
## \#317 Posted by: NewbieBoardBuilder Posted at: 2017-07-04T15:47:05.440Z Reads: 158

```
But I'm pretty sure I'm right!!
```

---
## \#318 Posted by: jaymu86 Posted at: 2017-07-04T16:01:46.862Z Reads: 160

```
If you are sure and you see it done before and working than copy the plan and execute it. Plain and simple 98% of the ?'s you asking have been answered
```

---
## \#319 Posted by: Hummie Posted at: 2017-07-04T18:49:19.074Z Reads: 157

```
Isn't it around 6000 erpm that it was decided is a safer speed for the Vesc?
```

---
## \#320 Posted by: Jinra Posted at: 2017-07-04T18:54:31.909Z Reads: 155

```
I'm getting flashbacks from the devin arguments
```

---
## \#321 Posted by: joeadams101 Posted at: 2017-07-04T19:22:09.540Z Reads: 155

```
Hey @Jinra  long time no talk. I decided to go back to the 6372 enertion motor and still overheating the vesc lolll. I miss my 170kv 5065.... Shit has anyone solve this problem yet? I am curious cause I am going on a cruising tour today and dont wanna be stopping every 5 mins on hills to cool off.... Thanks Jin
```

---
## \#322 Posted by: Hummie Posted at: 2017-07-04T19:37:00.042Z Reads: 158

```
maybe it was chaka who tested and said while you can hit 8000 erpm the vesc is prone to failure at those high speeds and safer at 6000ish.  maybe that was just in FOC?
```

---
## \#323 Posted by: Eboosted Posted at: 2017-07-04T19:46:53.911Z Reads: 163

```
I run 190kv on 12S, I've never exceeded max ERPM it runs like a dream! 

170kv are good but 190kv are much better for 12S
```

---
## \#324 Posted by: Jinra Posted at: 2017-07-04T20:07:02.506Z Reads: 164

```
That's what he said in this thread. Basically 8570+ rpm will fry the vesc (60000 rpm)
```

---
## \#325 Posted by: Hummie Posted at: 2017-07-04T21:06:31.803Z Reads: 167

```
  are you saying 8500 erpm is the limit and 6000 erp was thought to be a safe max for foc or also bldc?
```

---
## \#326 Posted by: Jinra Posted at: 2017-07-04T21:16:34.687Z Reads: 165

```
no idea about FOC, I have no experience with it myself. Where did you see this 6000rpm number?
```

---
## \#327 Posted by: Hummie Posted at: 2017-07-04T21:30:05.130Z Reads: 172

```
i thought it was chaka who said that 6000 being a safer speed for both or one of those programs @chaka

aha the first page...found it
```

---
## \#328 Posted by: emcauliff Posted at: 2017-08-24T20:14:34.858Z Reads: 156

```
Is this under load or spinning on your desk?
```

---
## \#329 Posted by: Bender Posted at: 2017-08-25T11:39:26.164Z Reads: 157

```
This was on the bench.
I didn't have a way to test under load at the time. The max under load for that motor and my weight (220lb) is ~85% of those numbers.
```

---
## \#330 Posted by: emcauliff Posted at: 2017-08-26T16:49:25.519Z Reads: 159

```
Thanks Bender. I just finished my first board. Im running a 245kv SK3 6364 on 10s with 16;36 gears on 90mm wheels. Its twitchy and hauls ass, but I fear my kv is too high and I'm looking for trouble. Drags me (220 lb also) up hills with no problems. Ill be trying to tweak limits in BLDC today, fingers crossed I can keep this thing alive for a bit, but the more I type this response, the more I think I should get a lower KV motor coming from HK.
```

---
## \#331 Posted by: deucesdown Posted at: 2017-09-01T19:45:45.690Z Reads: 165

```
Does setting ERPM limits actually protect the VESC completely? And if it does, will it do it at the expense of your skin, chucking you off or removing brakes?

Does anyone know exactly what the RPM limits (Max and Min ERPM) does? Does VESC suddenly cut power? Gradually roll off?

And the flip side for if you're coasting downhill approaching the Max ERPM.

And the "Limit ERPM with Negative Torque".  Does this mean brakes are applied? At the Max ERPM, or before?

And I noticed in BLDC tool the Max/Min ERPM section's title is "RPM Limit (BLCD only)" so they don't apply to FOC?

Holy shit I said "And" a lot, but here's another one. And in the App->PPM section there's a soft ERPM limit. I suppose this could keep you safe from throttling beyond 60000 ERPM, but not from coasting downhill faster than 60000 ERPM?
```

---
## \#332 Posted by: deucesdown Posted at: 2017-09-01T20:33:38.667Z Reads: 166

```
Found [This post by ackmaniac with respect to "Limit ERPM with Negative Torque"](http://www.electric-skateboard.builders/t/disappointing-torque-and-speed/7648/60?u=deucesdown):

> Thats the parameter. When it is disabled then it simply shuts off the 
> VESC. When it is enabled it brakes when it exceeds the MAX ERPM.

Covers most of my questions.
```

---
## \#333 Posted by: onepunchboard Posted at: 2017-09-02T03:51:01.072Z Reads: 167

```
coasting down for over erpm limit can kill vesc. tho to do that with my board I have to go 70kph. so not many will break the negative erpm. there was a guy in this forum happened this.
personally tho this sounds like urban legend. I set my bar to 65k and free spine many times, yet still riding with. it probably depending on ver of vesc too.

as for bldc goes negative rpm limiting really put me off the balance everytime. It brakes soon as off throttle
```

---
## \#334 Posted by: Blitz Posted at: 2018-01-16T00:12:52.827Z Reads: 145

```
So focbox with 190kv motor and 9s 30c battrey is a good pair right?
```

---
## \#335 Posted by: b264 Posted at: 2018-01-16T05:19:42.137Z Reads: 149

```
It's okay but 250kv might be a bit better.
```

---
## \#336 Posted by: MannyM0E Posted at: 2018-03-21T05:12:16.403Z Reads: 132

```
Would you not recommend 170kv on 10s ?
```

---
## \#337 Posted by: Linny Posted at: 2018-04-04T13:05:05.926Z Reads: 130

```
Hi guys, i'm working on a first build and have been reading a lot of threads on the forums.
I did a dual drive and read the earlier posts that a 190Kv will be best on a 12s. 
However, i'm using a 6s pack, with dual 6355 190Kv motors from TB. 
What will the performance be like, as comparing to a 12s?
```

---
## \#338 Posted by: TarzanHBK Posted at: 2018-04-04T13:18:59.352Z Reads: 127

```
http://calc.esk8.it/ ;)
```

---
## \#339 Posted by: Linny Posted at: 2018-04-04T13:26:28.241Z Reads: 130

```
Thank you Tarzan, so the difference is in the top speed...
Not that i'd have the balls to go more than 25km/h anyway
```

---
## \#340 Posted by: TarzanHBK Posted at: 2018-04-04T13:30:14.972Z Reads: 132

```
Start with what you have and if your confident enough and have a little practice on the board, simply update the battery. The rest of your system is able to do that :slight_smile:
And you can always limit specs in the Vesc tool.
```

---
## \#341 Posted by: Acidfie Posted at: 2018-04-04T13:55:55.381Z Reads: 132

```
[quote="chaka, post:41, topic:3125, full:true"]
Another detail I should add, you can push the kv up to 200kv @12s but the top end will feel weak. It will have good mid range boost but it will taper off as you approach the max velocity. If you calculate based on a 60k ERPM max instead of 100k the power and boost will increase at a fairly constant rate giving you that freight train experience.
[/quote]


so suitable for higher speed around 50kph - 30mph do you think is staying at 10S and lowering gear reduction or going 12S? i have 2 190kv motors, and want to go 12S
```

---
## \#342 Posted by: Hummie Posted at: 2018-04-04T15:00:32.004Z Reads: 129

```
hes been gone for ages.  its really 6 or half a dozen.  if you want to be more safe with electronics 10s is a bit safer but otherwise the differences youre talking about...12s would be a bit more efficient and that's about the only difference.
```

---
## \#343 Posted by: Deckoz Posted at: 2018-04-04T16:21:21.164Z Reads: 130

```
[quote="longhairedboy, post:105, topic:3125"]
CUZ I BUMP LIMITS YALL
[/quote]

I'm a bumper too @73k across the stars
```

---
## \#344 Posted by: PeterMcKane Posted at: 2018-04-25T00:26:34.411Z Reads: 123

```
I got a 213kv with a 2x 5S batteries in a series (so 10S). i calculated 7881 RPM. You guys think this is safe?

also what kind of failures would happen if i exceed that erpm number?
```

---
## \#345 Posted by: Pedrodemio Posted at: 2018-04-25T01:55:28.361Z Reads: 122

```
What VESC?
```

---
## \#346 Posted by: PeterMcKane Posted at: 2018-04-25T04:06:26.241Z Reads: 120

```
I have TB VESC. but might change to Maytech. any other recommendations?
```

---
## \#347 Posted by: Eboosted Posted at: 2018-04-25T05:02:54.310Z Reads: 117

```
Focbox best choice atm
```

---
## \#348 Posted by: PeterMcKane Posted at: 2018-04-25T06:13:01.362Z Reads: 120

```
well tryna to look into vesc because its more cost-effective. i also heard focbox is slightly overkill currently.
```

---
## \#349 Posted by: Eboosted Posted at: 2018-04-25T06:14:17.216Z Reads: 120

```
You heard wrong, a VESC6 might be overkill though
```

---
## \#350 Posted by: Pedrodemio Posted at: 2018-04-25T18:48:03.735Z Reads: 115

```
I wouldn't recommend going over 60k in any of them

In personal experience, unless TB drastically improved quality control I wound't even buy their VESC
```

---
## \#351 Posted by: PeterMcKane Posted at: 2018-04-26T00:49:17.953Z Reads: 113

```
VESC6 isnt even out yet i think
```

---
## \#352 Posted by: meesie Posted at: 2018-05-21T20:15:33.864Z Reads: 116

```
You can use that setup, But only if you have a programmable esc (maytech or focbox for example) because you can set an erpm limit on them
```

---
## \#353 Posted by: Bshady3 Posted at: 2018-06-03T06:40:20.668Z Reads: 104

```
WOW! just read 347 posts to catch up!

I was talking to another forum member @M.Hboards and he told me about the new FocBox Unity coming out and suggested I use it for my Dual E-MTB build. 

Here is my build as of now:
Motor: Tacon big foot 160 - 245Kv motor - 8 pole
Batteries: 12s Lipo
ESC: Flier 12s 120A ESC 
Gear Ratio: 5:1

In order to run dual motors, I need another ESC. I already have another Tacon Big Foot. Buying new motors is out of the question so unless the FocBox works with my setup I'm not getting them. The flier is still cheaper and although the startup isn't as good everything else is awesome!
My setup is insane! at top speed i reach 45mph(72.5kmh)!!!! I still have some brains so I limit the speed on my Flier to 50% (25mph). On grass, I draw a max current of 35A but that is only a peak current. The sheer power of 12s is amazing!

Regarding the FocBox, my setup technically has 98000 ERPM. But since I never ride more than 50% is it safe to say that my ERPM will not go above 98000/2 = 49000? this will be below the 60000 that seems to be the limit for the FocBox. 
If my assumptions are right I can ride up to 30mph before I hit the 60000 limit which is fast enough for me.

thanks and sorry for any missing details or extra details its 3AM in new york!
```

---
## \#354 Posted by: 808Chopz Posted at: 2018-08-23T17:29:06.609Z Reads: 64

```
[quote="Bshady3, post:353, topic:3125"]
WOW! just read 347 posts to catch up!
[/quote]

Yap! It's fun red.
```

---
