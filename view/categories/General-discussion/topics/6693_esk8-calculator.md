# Esk8 Calculator

### Replies: 56 Views: 10238

## \#1 Posted by: makevoid Posted at: 2016-07-27T12:36:03.584Z Reads: 968

```
Hi all, 

I'm a heavy user of this calculator: http://toddy616.blogspot.co.uk/2013/07/electric-skateboard-calculator.html which I think it's really great. Two features I was missing from it:

- rememberable URL
- a Save feature 
(not a multiple save, just one save and automatic reload of saved data on page refresh was enough for me)

Then I decided to build it, meet:


### [calc.esk8.it](http://calc.esk8.it)


---

---

- has good defaults
- has save functionality
- can change from lipo to li-ion battery type (will change the base nominal voltage)
- took me less than a day to code it


this is the repo of the project: https://github.com/makevoid/esk8-calc

thanks to @toddy616 for the original version

if there are bugs please tell me :slight_smile: 

enjoy!
```

---
## \#2 Posted by: Bender Posted at: 2016-07-27T12:47:02.021Z Reads: 578

```
Looks great!
I'd love the ability to do multiple set up comparisons :grin:
```

---
## \#3 Posted by: makevoid Posted at: 2016-07-27T12:49:43.628Z Reads: 527

```
open two browser windows :stuck_out_tongue:
```

---
## \#4 Posted by: Photorph Posted at: 2016-07-27T13:11:39.381Z Reads: 492

```
Nice, thank you!
```

---
## \#5 Posted by: shred Posted at: 2016-07-27T13:11:52.764Z Reads: 484

```
awesome, looks pretty neat too! 

I might have a feature request though, since we have the discussion right motor kv for vesc and stuff, might be a good idea to as well add ERPM calculation results, just a idea.
```

---
## \#6 Posted by: makevoid Posted at: 2016-07-27T13:23:34.901Z Reads: 447

```
ERPM is Engine RPM right? That should be Motor RPM on the right side of the page... (I could put an ERPM label in there...)
```

---
## \#7 Posted by: brams Posted at: 2016-07-27T13:28:56.784Z Reads: 418

```
No it's Electrical RPM
```

---
## \#8 Posted by: Bender Posted at: 2016-07-27T13:29:21.332Z Reads: 406

```
It's electrical rpm motor, rpm x7 for a 14 sator motor I believe
```

---
## \#9 Posted by: shred Posted at: 2016-07-27T13:33:04.380Z Reads: 408

```
Not sure, it actually might be just a VESC related value, I didn't find the actual wording for ERPM. 

Here is the post from @chaka I did relate to:
http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#10 Posted by: treenutter Posted at: 2016-07-27T13:50:09.804Z Reads: 383

```
@makevoid thanks this is awesome! Great work! This is a nicer looking package than the one we've always used.

I've always felt that rider weight should be a factor that can be added to the calc. collectively we should figure out the math required to add this input, since we all agree that it plays a huge role.

Also, some day let's add battery capacity (mah) to the calc so that riders can predict a little bit about ride time and distance assuming ideal conditions. You could use @lowGuido's chart about riding time as a simple input to begin with. 

Finally, how can we express torque in this calc? It would be useful to use the rest of the inputs along with rider weight to determine the hill-climbing ability of the build.
```

---
## \#11 Posted by: Maxid Posted at: 2016-07-27T14:21:56.341Z Reads: 355

```
[quote="treenutter, post:10, topic:6693, full:true"]
I've always felt that rider weight should be a factor that can be added to the calc. collectively we should figure out the math required to add this input, since we all agree that it plays a huge role.

Also, some day let's add battery capacity (mah) to the calc so that riders can predict a little bit about ride time and distance assuming ideal conditions. You could use @lowGuido's chart about riding time as a simple input to begin with. 
[/quote]

you could use this one:
https://www.elektro-skateboard.de/wiki/wissenswertes/strom-spannung-reichweite-vii
```

---
## \#12 Posted by: Jinra Posted at: 2016-07-27T14:24:57.999Z Reads: 325

```
It's actually a 12 stator motor with 14 magnets (7 pole pairs)
```

---
## \#13 Posted by: Ulfberht Posted at: 2016-07-27T18:24:12.585Z Reads: 310

```
@makevoid YES!! This is pretty cool. I like the old ESK8 calculator, but I love this one! 
:star: :star: :star: :star: :star: :star: :star: :star: :star: :star: :star: :star: :star: :star: :star: :star: :star: :star: :star: :star: :star: :star: :star:
```

---
## \#14 Posted by: Jinra Posted at: 2016-07-27T18:27:35.199Z Reads: 311

```
I like the page, but have a small criticism on it. One reason toddy's calculator was nice was because it easily fit in 1 screen, but on this one I have to scroll down to see everything. It'd be nice if you could readjust everything to fit in 1 screen :)

Also, could you add a 100th's digit for the ratio? Right now it rounds the ratio up. (Example: 36/16 shows as 2.3:1 ratio when it's 2.25:1)
```

---
## \#15 Posted by: mason Posted at: 2016-07-27T19:39:12.524Z Reads: 294

```
slap material design on it and it would be perfect :)
```

---
## \#16 Posted by: makevoid Posted at: 2016-07-27T20:07:43.213Z Reads: 295

```
good observations! thanks for the feedback, I rounded gear ratio to the 2nd decimal now and added some custom css on top of bootstrap's default to shrink the vertical spacing a bit, does it fit now? otherwise I can put the gearing column on the right so there are 3 columns not 2 in the top row :)
```

---
## \#17 Posted by: makevoid Posted at: 2016-07-27T20:08:59.630Z Reads: 295

```
It's actually bootstrap, maybe we can find a better bootstrap theme or color scheme than the default grayish one? :D
```

---
## \#18 Posted by: Jinra Posted at: 2016-07-27T20:10:53.607Z Reads: 288

```
Thanks! Still have to scroll though :(
```

---
## \#19 Posted by: makevoid Posted at: 2016-07-27T20:34:57.006Z Reads: 301

```
3 columns here we go :D
```

---
## \#20 Posted by: Ulfberht Posted at: 2016-07-28T00:55:06.491Z Reads: 362

```
[quote="makevoid, post:19, topic:6693"]
3 columns here we go :smiley:
[/quote]

Perfect!! :thumbsup:
A cooler background would just be an added plus! 
NIce work!
```

---
## \#21 Posted by: JLabs Posted at: 2016-07-28T02:23:04.957Z Reads: 368

```
Here is a testimate to how accurate this is *mind blown* (science tends to do that to me)
<img src="/uploads/db1493/original/2X/b/b6eec67586101d5849fa40b35920cfdc7348fb3e.PNG" width="371" height="353">
<img src="/uploads/db1493/original/2X/e/e3ce3834179b222d368c23e0ce56b545ff90fb56.png" width="281" height="500">

I think that if you would be able to fine tune the 'weighted' speed you could get it dead on. Maybe add another field where you can input your own weight, and add like 4 pounds for the electronics. Anyway great work!
```

---
## \#22 Posted by: barajabali Posted at: 2016-07-28T03:41:42.724Z Reads: 303

```
Great job @makevoid thank you for this!
```

---
## \#23 Posted by: Jinra Posted at: 2016-07-31T08:26:53.698Z Reads: 295

```
I'd like to make another request if you can accommodate :) With Toddy's calc I can input decimals into the 's' count on the battery cell section. This was useful because I can simulate what my speed would be under full charge or various voltages in between.

I'd like it if I could either also put decimals for the 's' count on this calculator or if I could put voltage manually instead. This would make me completely convert to this calculator!

Thanks again for your work.
```

---
## \#24 Posted by: Michaelinvegas Posted at: 2016-07-31T08:58:55.083Z Reads: 265

```
And thanks for not making the background black ... To many dark colored backgrounds out there
```

---
## \#25 Posted by: Workaround Posted at: 2016-07-31T17:46:33.448Z Reads: 256

```
I would just prefer manual voltages. Or just for lipos do 4.2V as a max speed and 3.7V as min speed.
```

---
## \#26 Posted by: sismeiro Posted at: 2016-07-31T18:52:30.379Z Reads: 261

```
[quote="Workaround, post:25, topic:6693, full:true"]
I would just prefer manual voltages. Or just for lipos do 4.2V as a max speed and 3.7V as min speed.
[/quote]

I think it could be done by adding more battery voltage presets:

Li-ion Full (4,1 V)
Li-ion Nominal (3,6 V) 
Lipo Full (4,2 V)
Lipo Nominal (3,7 V)

Note: values mais be wrong but I think this is it.
```

---
## \#27 Posted by: Jinra Posted at: 2016-07-31T18:58:57.271Z Reads: 244

```
liion and lipo area both full at 4.2v
```

---
## \#28 Posted by: hugohammarstrom Posted at: 2016-07-31T20:33:05.621Z Reads: 247

```
[quote="sismeiro, post:26, topic:6693"]
I think it could be done by adding more battery voltage presets:
[/quote]

What about adding a slider ranging from 0v to 4.2v this way you can simulate every possible voltage
```

---
## \#29 Posted by: zeno Posted at: 2016-08-02T17:03:12.994Z Reads: 244

```
**eRPM = (voltage)x(kv rating)x(pole pairs, 7 for most 50-63mm motors)**

e.g.: 37 volts (10s) with 200kv motor and 7 pole pairs:

37*200*7 = 51800 eRPM. From what i've read you do not want this to go beyond 60000 on the **VESC**
```

---
## \#30 Posted by: makevoid Posted at: 2016-08-05T15:07:06.634Z Reads: 248

```
- added eRPM calculation
- number of cells is now a float (you can add decimal values) @jinra

I'll probably add more voltage presets later like full/nominal/min for both lipo and li-ion 

- **new feature!** pastable configuration link

This is my configuration:

#### [My Conf](http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":8,"motor-kv":190,"system-efficiency":80,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":97}|) 
(using the forum link feature)

My conf (long extended link):

http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":8,"motor-kv":190,"system-efficiency":80,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":97}|

The link is a bit long because it has in it all the paramters required but it was easy to implement. Having the values in the link means that I don't need to store it anywhere (db) / make the user log in and stuff...

(refresh with shift pressed to clear the cache and see the latest version)


edit:  modified the link so it works with the forum in both forms
```

---
## \#31 Posted by: zeno Posted at: 2016-08-05T19:18:08.635Z Reads: 218

```
Nice updates!
```

---
## \#32 Posted by: Ulfberht Posted at: 2016-08-06T21:32:24.194Z Reads: 216

```
@makevoid  Awesome! This looks great!
```

---
## \#33 Posted by: baxter Posted at: 2016-08-20T05:33:46.797Z Reads: 218

```
@makevoid 

I'm not sure if you are still interested in tinkering with this tool anymore, but have you considered adding an option, or revising the calculation to set a target speed? I think this function would be really useful to new DIYers who may have restricted budgets, or already have certain hardware (i.e. speed controllers restricted to 6s voltage).  

I reckon the less experienced or technically minded DIYer would find this really useful, and give them an opportunity to reverse engineer a board that will operate efficiently to the specifications and capabilities they want, rather than potentially buying incompatible motors/escs, or operating them at too low a voltage.

If you could put in your targeted top speed (weighted), and perhaps some other variables  perhaps available voltage, wheel sizes (which may already have been purchased), it could provide guidance in terms of motor and wheel pulley ratio will need to purchased to get to the speed they want. 

You might also put in an range estimation (for flat ground) based on the amp hours of the battery they may already have. 

If the tool could do this, then it would take a lot of the guesswork out ensuring that first builds are successful (at least electrically speaking).

Not sure if this is feasible, but I can imagine esk8 parts vendors using this sort of calculator on their websites to recommend certain components, instead having their products and their technical specifications (perhaps in drop down boxes) in the fields of the calculator.  (nudge nudge!)
```

---
## \#34 Posted by: Photorph Posted at: 2016-08-20T06:23:36.556Z Reads: 182

```
This is awesome!
```

---
## \#35 Posted by: Okami Posted at: 2016-08-20T06:34:12.064Z Reads: 178

```
I like your idea very much.. I remember myself entering values numerous times, just to get to see what output speed will I get.. This could optimize the process, for sure..

I know it is hard to estimate but someone more calculations savy could also come up with a way to calculate torque, although it seems ppl are usually fine, if they don't go way too extreme on some of the parameters for their builds.
```

---
## \#36 Posted by: Adam0311 Posted at: 2016-08-20T07:23:54.162Z Reads: 181

```
This should a sticky thread. Super useful.
```

---
## \#37 Posted by: lox897 Posted at: 2016-08-20T09:16:56.249Z Reads: 182

```
Calculator is exact. Tested it today on my board. 80% efficiency and I am 45kg
```

---
## \#38 Posted by: makevoid Posted at: 2016-08-20T12:47:44.770Z Reads: 196

```
thanks for the in-depth comment

I'll probably try do an new 'staging' version of the calculator some time soon, even if right now I'm more focused and exploring the vesc uart interface (hopefully I will not break any other vescs ^^)

all your points are valid, let's separate them even if in the ideal world we would have an almighty solve-all tool:

- Load **defaults / presets** - esk8 database

requires a "database" to pick data from

my opinion: very good, would be awesome, but it's a great effort - it requires a "database" (can even be a spreadsheet / a markdown / csv file hosted on github) that needs to be maintained / updated and checked (declared specs vs actual specs can vary)

also that would probably be better in/with @Okami 's project instead of retro-fitting this on a simple value calculator like this one

links: http://www.electric-skateboard.builders/t/new-builder-list-of-known-and-commonly-used-parts/2983/1 - http://www.electric-skateboard.builders/t/new-builder-list-of-known-and-commonly-used-parts/2983/1 

but I agree, a tool like that it would be awsome

---

- Calculate **range** based on battery wh

That would be good but I think it will be very approximate!

There are few issues in doing a good range calculation, there are few factors that can really vary the outcome: hills, quality of asphalt (both not really well defineable), weight (that's a big factor), mechanical efficiency (drive train, bearings etc, hubs), wind, average speed ... 

the good thing is that there are some easily factorable values like travel speed + motor kv + gearing but I don't think they're enough

Maybe a statistical analysis ( one was started here http://www.electric-skateboard.builders/t/ride-time-how-long-can-you-ride/1316/5 ) would be better?
I think we could try to have both but still, that requires managing data, not only fixed formulas (easier), some effort, but yes it could be very useful.

p.s. I like to tackle quick wins ^^ so if you find an utility that can be coded quickly (<1 day), that is useful and that doesn't needs maintainance (e.g. you just need to make sure it stays online, no need to update/recheck etc.), then I can probably do it do it :slight_smile: .
```

---
## \#39 Posted by: Okami Posted at: 2016-08-20T23:51:41.739Z Reads: 180

```
About the database - 

As of now it is this far:

http://gct-hp.de/esk8/index.php

It has its interface but the data output with tables and parameters to choose from are still missing.

@Deathcookies is the guy to contact, if you''ve got any other ideas or you want to help.

@karma tried to take part in this project, although I am not sure how far did @deathcookies arrange the process between them.

---
So far it looks promosing to me, it just need to be finished, so any help would be great, especially from people who know how to output data fields / records and similar stuff!
```

---
## \#40 Posted by: karma Posted at: 2016-08-21T14:05:07.110Z Reads: 181

```
@Okami, @DeathCookies sent me massage 5 days ago and said I could start helping but unfortunatly I started university 6 days ago and I have no time at the moment. I will contact him if I get any spare time. :)
```

---
## \#41 Posted by: clayskaight Posted at: 2016-09-26T19:50:28.920Z Reads: 141

```
Hi there! I am new but I thought id contribute this, I just made it for range or distance instead of speed, feel free to check it out! https://jscalc.io/calc/rdJYgcAquv9oqdcu
Thanks,
Clayton
```

---
## \#42 Posted by: makevoid Posted at: 2016-09-26T20:02:08.876Z Reads: 143

```
wow it looks awesome! I didn't know about https://jscalc.io , pretty cool! :thumbsup:


my [values](https://jscalc.io/calc/rdJYgcAquv9oqdcu#%7B%221%22:190,%222%22:36,%223%22:24,%225%22:97,%226%22:10000,%227%22:15,%228%22:36%7D) < the range is pretty much that
```

---
## \#43 Posted by: Hillso Posted at: 2016-09-27T20:08:17.730Z Reads: 140

```
by your calculator, the larger the motor pully the bigger the range. so if you go light speed you have lots of km's
https://jscalc.io/calc/rdJYgcAquv9oqdcu#%7B%221%22:149,%222%22:43,%223%22:20,%225%22:125,%226%22:10000,%227%22:10000000,%228%22:1%7D
```

---
## \#44 Posted by: clayskaight Posted at: 2016-09-27T22:13:02.291Z Reads: 140

```
@Hillso So with both my calculator and the speed calculator that makevoid made if you put the massive motor gear with the tiny wheel gear it will give bad results (http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":200,"system-efficiency":80,"motor-pulley-teeth":100000000,"wheel-pulley-teeth":1,"wheel-size":83}|) < example, this is because as long as you can get enough tork to move the board this speed is possible, but that amount of torque would be insane and unrealistic. Both calculators should work close to perfectly if you give it proper numbers to work with. The calculators do not include the torque number because most hobbyists don't know the amount of torque they have... only the wattage.
Thanks for the feed back though...
Clayton
```

---
## \#45 Posted by: Mobutusan Posted at: 2016-09-27T22:29:24.645Z Reads: 126

```
I can't seem to enter the cell count as a decimal. Am I missing something?
```

---
## \#46 Posted by: makevoid Posted at: 2016-09-27T23:16:03.228Z Reads: 128

```
lol you have to be quick (I should fix that), but really if you're quick (like in half a second 2 digits) and you insert a dot as decimal separator it works :D sorry about that ^^
```

---
## \#47 Posted by: Mobutusan Posted at: 2016-09-28T00:41:50.653Z Reads: 127

```
Thanks for the tip. I figured it out. You have to enter the numbers first then go back and add in the decimal point.
```

---
## \#48 Posted by: Hillso Posted at: 2016-09-28T05:00:57.500Z Reads: 129

```
even for normal numbers, I thought the lower the top speed the larger the range.
[22 km](https://jscalc.io/calc/rdJYgcAquv9oqdcu#%7B%221%22:190,%222%22:36,%223%22:20,%225%22:83,%226%22:10000,%227%22:16,%228%22:36%7D) for [36 km/h](http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":10,"motor-kv":190,"system-efficiency":80,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":83}|)
[30 km](https://jscalc.io/calc/rdJYgcAquv9oqdcu#%7B%221%22:190,%222%22:36,%223%22:20,%225%22:83,%226%22:10000,%227%22:20,%228%22:36%7D) for [48 km/h](http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":10,"motor-kv":190,"system-efficiency":80,"motor-pulley-teeth":20,"wheel-pulley-teeth":36,"wheel-size":83}|)
oh I get it. it's like that because you get to the same speed with lower voltage on higher top speed, so lower watt. but than you need higher amps so no. idk
```

---
## \#49 Posted by: clayskaight Posted at: 2016-09-28T17:37:56.264Z Reads: 128

```
That part is calculated using the amps, the slower you go the less amps you will pull and therefor the farther you go!
```

---
## \#50 Posted by: Hillso Posted at: 2016-09-28T20:45:27.716Z Reads: 130

```
but according to your calculator the faster you go the farther you go. or I'm dumb? idk.
```

---
## \#51 Posted by: byob Posted at: 2016-11-06T17:59:31.718Z Reads: 117

```
So glad i found this, thanks
```

---
## \#52 Posted by: davidbonde Posted at: 2018-01-10T22:53:15.088Z Reads: 72

```
How do you guys decide what to put in the efficiency tab?
```

---
## \#53 Posted by: Snowi Posted at: 2018-03-11T21:30:46.854Z Reads: 59

```
What is this R value that eventually multiply to mph estimate?

![image|469x500](upload://loSwXvU5xMtdtbzH1q1MsFliiyy.png)
```

---
## \#55 Posted by: Benjo Posted at: 2020-01-14T10:03:49.200Z Reads: 14

```
Anybody know what that magic number R is?
```

---
## \#56 Posted by: EnderWiggin Posted at: 2020-01-17T17:30:04.557Z Reads: 12

```
Yes, I calculated it out for you.

**Original**:

R = 0.00003728226<br>
Top Speed = 4499 RPM * 82mm * pi * R * 2.25 =  **19.2 MPH**


**Variables**:

RPM<br>
Wheel Diameter in mm (W) <br>
Circumference(C ) <br>
C = W * PI<br>
Gear Ratio (G) <br>
Top Speed = RPM * C * (1/G) =  **mmPH**<br>


Top Speed = mmPM * 6.21371e-7 (mm/miles)* 60 (M/H) = **MPH**

Top Speed= RPM * W * PI * (1/G) *  6.21371e-7 (mm/miles)* 60 (M/H) = **MPH**<br>
Top Speed= 4499 RPM * 82mm * PI * (1/2.25) *  6.21371e-7 (mm/miles)* 60 (M/H) = **19.20434198 MPH**

Now that we know how they got MPH we know that R is:

R= 6.21371e-7 (mm/miles)* 60 (M/H) = 0.00003728226

R is the conversion form mm per minute to miles per hour.

**Note**: The gear ratio is 1/G. this is not clear in the equation.

Hope this helps like!

Check out the calculator i made a while back!

https://www.electric-skateboard.builders/t/google-spreadsheet-for-easy-and-fast-calculations/13337?u=enderwiggin
```

---
## \#57 Posted by: Benjo Posted at: 2020-01-17T17:35:57.868Z Reads: 11

```
Thank you! Very helpful. Also I will definitely check out your calculator :)
```

---
