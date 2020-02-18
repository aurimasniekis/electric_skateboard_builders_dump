# One calculator to rule them all?

### Replies: 47 Views: 6106

## \#1 Posted by: saul Posted at: 2017-05-26T08:22:36.245Z Reads: 834

```
Its been a while since I did anything to my website, mostly it was just for my portfolio to brush up on web stuff.
but I feel like making something useful.

<s>I already did a basic [speed](http://esk8.today/2017/01/03/how-fast/#more-365) and [range](http://esk8.today/2016/12/28/how-far-can-i-ride/#rc) calculators.</s>
Edit: these are offically obsolete! please use [calc.esk8.today](http://calc.esk8.today/) for both speed and range. 

These were just using a basic plugin, I want to make a new one from scratch, probably with bootstrap and some js or something. But the question is of course, what does the perfect esk8 calculator need?

Ideas:
----------
1. Speed
2. Range
3. Hill grade
4. Compare
5. Save/download/upload config
6. Price compare(eventually)
7. Board Weight esimate?

Obviously you are the ones using it! so what do you think?
----------
```

---
## \#2 Posted by: NickTheDude Posted at: 2017-05-26T14:19:23.290Z Reads: 738

```
Cool! It seems like we have a lot of calculators for stuff like top speed and range. I'd like to see one that can give you rough estimates of performance.

Something where you could input your max volts/amps, rider weight, frontal surface area, hill grade, etc and it would show you power output, potential 0-60 times, hill climbing capability, torque output etc.

I have no idea how feasible that would be but I think it'd be super useful.
```

---
## \#3 Posted by: Okami Posted at: 2017-05-26T18:05:57.326Z Reads: 613

```
nice tool @saul

I think u should get some more publicity  with this.. :D so yeh gonna post here.

--

 I really like the calc esk8 style and simplicity, if yours could be made in similar way (for range) that would be great.. otherwise a bit hard to get where to get what or maybe it was just me who didnt get the whole page loaded with all the numbers and fields at the first shot.
```

---
## \#4 Posted by: saul Posted at: 2017-05-26T22:59:42.590Z Reads: 497

```
Some of this would be possible but I need more torque curve data for various motors. I know there are some for sk3s from the group buy. 

Till someone makes a dyno it'll be difficult to have real comparisons.

I'll play with some math and see what I can do quickly with minimal input first.
```

---
## \#5 Posted by: saul Posted at: 2017-05-26T23:02:21.462Z Reads: 449

```
Thanks, the current one was tossed together in an hour or so.

For this one I'll give a dedicated page, clean mobile friendly layout. I saw the code for calc.esk8.it is on GitHub, need to check the licence and maybe I'll learn some Ruby to build off that, not sure yet.
```

---
## \#6 Posted by: saul Posted at: 2017-05-28T04:15:43.694Z Reads: 411

```
Basic template is up. <s>its non functional, but</s> it should give an idea of what it will look like and how it will work.

[calc.esk8.today](http://calc.esk8.today/)
----------

Battery section is working.
<s>logic is done, just need to add fields so should have range and speed in a bit!</s>

Update: Speed and Range work!
```

---
## \#7 Posted by: Okami Posted at: 2017-05-28T04:45:56.478Z Reads: 379

```
looks way better. thanks for taking a look at calc esk8 and finding the source code :)
```

---
## \#8 Posted by: saul Posted at: 2017-05-28T05:15:22.355Z Reads: 360

```
lol theres a link to the source on the bottom right corner.

But i'm not using it. this is all new! ;)
```

---
## \#9 Posted by: saul Posted at: 2017-05-28T22:17:34.601Z Reads: 334

```
[eSk8 Calculator](http://calc.esk8.today/)
----------


Ok speed and range work!
auto update.
Next up I think I'll do download/upload json config files.

@mmaner This one looks alot better! let me know what you think!
```

---
## \#10 Posted by: mmaner Posted at: 2017-05-29T00:14:35.354Z Reads: 317

```
@saul  Lol, I was just kidding brother 😀
```

---
## \#11 Posted by: Okami Posted at: 2017-05-29T21:10:51.211Z Reads: 317

```
can u ask @lox897 to pin it? Otherwise im afraid we gonna loose this one in all the other threads.. if there is a special category for tutorials, that would be nice and then maybe it could be moved there ? (though i think there is no such category yet - for tuts)

--

As about the site itself:

<img src="/uploads/db1493/original/3X/4/e/4ea7451e7804e308cbdacf511e01680523931f42.png" width="690" height="211">

The Capacity info does not seem right. can you just make the page to 'average'' / round the number to 2 digits behind the comma?

Also - make an option to chooce mountainboard or longboard.

The speed data looks very okay! It even says: Estimated Energy consumtion.. but I think it did not work for me :\ as the range numbers stayed the same..

Otherwise - very nice work, easy way to calculate watt hours for the pack now :)
```

---
## \#12 Posted by: lox897 Posted at: 2017-05-29T21:46:24.485Z Reads: 268

```
I think we have enough things pinned for now. If you want to keep this near the top please try and get other people's opinions and regularly post on it.
```

---
## \#13 Posted by: Okami Posted at: 2017-05-29T22:05:05.927Z Reads: 258

```
yeh I get you.. maybe someone should suggest to make a seperate category or similar.
```

---
## \#14 Posted by: mmaner Posted at: 2017-05-30T01:20:12.759Z Reads: 250

```
Is there anyway to add the car rating for lipos and amps for li-ion to get the max amp output?
```

---
## \#15 Posted by: Okami Posted at: 2017-05-30T01:51:28.100Z Reads: 251

```
@mmaner  what do u mean by:

> car rating for lipos  ??

Like is it possible to recharge car battery or what? :)
```

---
## \#16 Posted by: saul Posted at: 2017-05-30T02:40:05.862Z Reads: 265

```
I fixed the round error. 

for the energy use, you have to enter you average. 18 is what i've been getting for single drives.
and I think about 25-30 for dual.

If you can give an estimate for mtb, I can add a dropdown option, like on battery type.
I think 30-40 whr/mile?

just take your battery capacity and divide by average range per charge.
```

---
## \#17 Posted by: saul Posted at: 2017-05-30T02:42:33.328Z Reads: 256

```
[quote="mmaner, post:14, topic:23937, full:true"]
Is there anyway to add the car rating for lipos and amps for li-ion to get the max amp output?
[/quote]

I was just thinking of that! I think max cont Amps per cell, peak amps, C rating charge/discharge for lipo.

from this I can add max power, charge time, pack amps....not sure what else?
```

---
## \#18 Posted by: Okami Posted at: 2017-05-30T02:53:09.345Z Reads: 250

```
yeh charge time feature would be really sweet! I used to have it on one of those RC calcs but then the calc crashed and I had to do it on my own each time :D

though.. i usually just charge Amp hours now, thats how I know how many kilometers I can do / need to do.
```

---
## \#19 Posted by: mmaner Posted at: 2017-05-30T03:03:19.256Z Reads: 248

```
I meant C rating, auto correct 😀
```

---
## \#20 Posted by: mmaner Posted at: 2017-05-30T03:04:54.301Z Reads: 257

```
I'll be thinking on it and let you know.  I'm always checking to see what max amp discharge (max & continuous) is when I building or spec's a pack.  Just figured it would be handy.  The webapp looks great btw.
```

---
## \#21 Posted by: saul Posted at: 2017-05-30T06:50:12.405Z Reads: 227

```
new features are up. I think I covered most of it.
need to figure out something for the color codes.. and thanks.
```

---
## \#22 Posted by: markyoe Posted at: 2017-05-30T07:14:06.934Z Reads: 219

```
Looks great! That will be really handy. What factors is the charge time base off of?
```

---
## \#23 Posted by: E-Boarding Posted at: 2017-05-30T07:39:47.342Z Reads: 240

```
for Hillclimb/Torque and Weight you can use this experimental calculator or maybe adapt some of the formulas to include in your calculator

https://www.electric-skateboard.builders/t/path-of-esk8-build-tree/16774/19
```

---
## \#24 Posted by: Okami Posted at: 2017-05-30T07:50:44.578Z Reads: 256

```
<img src="/uploads/db1493/original/3X/e/9/e9b0da13752977c28546faf373081cec426d99fb.png" width="540" height="500">

Colors are okay! I would advise to 'make a space'' / seperation between the long column.

After Total battery energy or after range fields, perhaps there should be a seperate blank spot then continue the column further.. i hope u get what i mean by this :)

---
Or make it 'hidden''so that user has to click on it to reveal the info

Tabs - Power, Capacity, Range, Power output, Charging time

Motor / esc rpm speed, eboard speed
```

---
## \#25 Posted by: saul Posted at: 2017-06-03T07:54:10.950Z Reads: 238

```
[quote="Okami, post:24, topic:23937"]
Or make it 'hidden''so that user has to click on it to reveal the info
[/quote]

i'll try to add in a simple/advanced version soon.

for now I added a basic hill grade estimate using the calculations shown [here](https://engineering.stackexchange.com/questions/6756/calculating-torque-needed-to-climb-a-graded-hill).
keep in mind this is only based on rider/board weight and **continuous power** since I can't find enough info on torque of 50mm motors. and in most cases (not hubs) the torque multiplier of 2-4x from the belt/chain/gear drive gives a surplus of torque as long as you can put out enough power!!

basically it give the max hill grade you can go up at full speed with give cont. power.
```

---
## \#26 Posted by: saul Posted at: 2017-11-02T10:37:55.689Z Reads: 216

```
Simplifed my calculator a bit.
the old version is still availible at http://calc.esk8.today/advanced



----------

http://calc.esk8.today/
----------
```

---
## \#27 Posted by: Acido Posted at: 2017-11-02T13:10:23.953Z Reads: 203

```
Tell me about number 18, is it like minimum energy use for single drive or what
Can you tell me what number should i use for single drive 100kg driver?
```

---
## \#28 Posted by: saul Posted at: 2017-11-03T00:27:47.829Z Reads: 189

```
[quote="Acido, post:27, topic:23937, full:true"]
Tell me about number 18, is it like minimum energy use for single drive or what
Can you tell me what number should i use for single drive 100kg driver?
[/quote]

its the average energy use that I get for my single drive yes.
I sugguest you find you own avg.
How to:

Enter your info on the calc. note down 
Total Battery Energy:	185.00 Watt-Hours (W-hr)
Then do a full battery drain on a ride.
lets say you got 10 miles. 
then 185/10 = 18.5 w-hr per mile.
or for dual would be around 8 miles?
so 185/8 = 23.1 w-hr / mile.
```

---
## \#29 Posted by: scepterr Posted at: 2017-11-03T00:54:40.300Z Reads: 163

```
Very nice, is it possible to generate a URL for a specific config?
```

---
## \#30 Posted by: saul Posted at: 2017-11-03T01:23:55.196Z Reads: 158

```
thats the next thing on my list.
should be pretty quick.. maybe tonight...
```

---
## \#31 Posted by: Acido Posted at: 2017-11-03T05:41:34.646Z Reads: 158

```
Ye the thing is im building my skate
```

---
## \#32 Posted by: saul Posted at: 2017-11-03T07:59:00.106Z Reads: 154

```
i'm about 70kg. i get 16-18 whr per mile with a single. using the default specs on my calc.

i would guess around 20. but no higher than 25 (dual drive avg)... and you will may end up with a few extra miles depending on the batt...
```

---
## \#33 Posted by: Acido Posted at: 2017-11-03T08:42:36.938Z Reads: 159

```
My bat is 10s4p 440wh and with 25wh per mile i would get 28km that would be great since im 100kg with a backpack or something
```

---
## \#34 Posted by: revise Posted at: 2017-11-05T03:59:17.775Z Reads: 150

```
Getting connection refused - did url change?
```

---
## \#35 Posted by: saul Posted at: 2017-11-05T05:32:53.043Z Reads: 157

```
no, I think my server had an issue today.
I was also getting an error on the main page. 
looks good now..but i'll double check!
```

---
## \#36 Posted by: revise Posted at: 2017-11-05T16:11:36.881Z Reads: 152

```
Working again here! Thanks, you're the best.
```

---
## \#37 Posted by: saul Posted at: 2017-11-08T09:35:39.668Z Reads: 158

```
[quote="scepterr, post:29, topic:23937, full:true"]
Very nice, is it possible to generate a URL for a specific config?
[/quote]

Had to work out a few bugs...mostly i just never liked web programming. 
but 
(EDIT): it works, but shareable is slower because it needs to reload the page, for now.
so the main page is the quick version,
Shareable at http://calc.esk8.today/config/
advanced http://calc.esk8.today/advanced/

example config
http://calc.esk8.today/config/?type=3.7&scells=12&pcells=1&cc=5&da=50&mda=100&kv=200&poles=14&eff=90&wheel=90&mp=15&wp=36&wpm=18
```

---
## \#38 Posted by: scepterr Posted at: 2017-11-25T19:34:12.792Z Reads: 154

```
Had another idea, being able to export a graphic with your specs so it can be shared and linked back
Like what speedtest.net does
```

---
## \#39 Posted by: saul Posted at: 2017-11-26T16:49:39.163Z Reads: 152

```
i'll try at some point. for now you can just link a screenshot..
```

---
## \#40 Posted by: saul Posted at: 2017-12-15T00:39:49.467Z Reads: 169

```
i see more mobile users. does the layout work on a small screen?
there are some display options I could play with...

<img src="/uploads/db1493/original/3X/7/5/75cb5c82d63aceb4e2f18b46066021263a1b24e8.png" width="371" height="500">
<img src="/uploads/db1493/original/3X/1/c/1c244debd3f090e532b77db7cb049b1321d671e3.png" width="295" height="500">
<img src="/uploads/db1493/original/3X/f/7/f7756cf5d5e7c958ee14c55c1c35033954baf551.png" width="380" height="500">
```

---
## \#41 Posted by: fredrikinn Posted at: 2018-05-23T12:03:04.370Z Reads: 138

```
Nice calc dude, great work!

But is the "Max % Hill Grade" right? on the advanced calc. Maybe i put in something wrong, but i got around 70-90 % hill climb. Am i reading it wrong? I tryed my board in a few different hills and it cant do all of them.
```

---
## \#42 Posted by: Benjamin899 Posted at: 2018-11-08T13:09:55.526Z Reads: 115

```
do you guys also get a server not found message when you try to access the calculator
```

---
## \#43 Posted by: KrisKraanen Posted at: 2018-11-09T20:31:49.601Z Reads: 113

```
yes! help !
```

---
## \#44 Posted by: CarbonV Posted at: 2018-11-17T09:54:32.063Z Reads: 109

```
I think the site is officially down :frowning:
```

---
## \#46 Posted by: Riako Posted at: 2018-11-17T10:33:45.496Z Reads: 108

```
thx !!! I was lost to not being able to use _calc.esk8.it_ :disappointed_relieved: 
I will try this one. It looks good, much more complete and detailed, NICE !
```

---
## \#47 Posted by: epster Posted at: 2018-12-01T14:24:37.502Z Reads: 97

```
Yup I do man :(
```

---
## \#48 Posted by: b264 Posted at: 2019-03-15T02:56:14.960Z Reads: 66

```
I remade this at https://calc./
```

---
