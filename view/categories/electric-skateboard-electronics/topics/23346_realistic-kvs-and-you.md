# Realistic KV&rsquo;s and you

### Replies: 57 Views: 4439

## \#1 Posted by: Jinra Posted at: 2017-05-18T01:38:33.678Z Reads: 555

```
I've historically found advertised KV's to be a bit off from real world values and wanted to start a discussion of everyone's personal experience. This can hopefully shed light to various motors from various manufacturers and help builders purchase correctly with eRPM in mind.

[This](https://www.electric-skateboard.builders/t/the-dual-big-boy-12s-lipo-5000mah-tbs-12s-120amp-esc-tbs-63mm-6355-230kv-83mm-or-90mm-clone-fly-wheels/3913/4?u=jinra) was a topic I saw talked about for a bit last year. Although the comment I'm linking is purely anecdotal, I saw [some users](https://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125/157?u=jinra) test the KV themselves as well which resulted in lower kv's than advertised.

In regards to @chaka's motors. He kindly shared his methodology of calculating kv from VESC real time data which you can find [here](https://www.electric-skateboard.builders/t/ollinboardco-om5065-200kv-sensored-motor/3409/351?u=jinra). The gist is [Power / Motor Current = Motor Voltage], eRPM / 7 pole pairs / Motor Voltage = KV @ 95% duty cycle. Since the VESC only runs at 95% duty cycle max we finally divide by .95 to get the actual KV of the motor. As you can see from the link, chaka's calculations were pretty on point lending a result of 197kv for his 200kv motor.

I've applied the same math to @JLabs Polar motors (and soon @Kaly's motors when I get them) and found that his 190kv 6355 motors have a calculated kv of 179kv. A bit lower than advertised, but this makes it easier to apply to higher voltage setups without too much worry of hitting eRPM limits.

<img src="/uploads/db1493/original/3X/f/3/f3055a169ef7fd69f1bf51f1d36ef609dac9b3c7.png" width="690" height="153">

For the above example 42W / 1.21a = 34.71v.   41309erpm / 34.71 / 7 / .95 = 178.96kv

If you're willing to test your motors out, please post your results here so we can gather data about motor KV's! If I get enough responses, I'll start a Google Sheet for it. If you'd like to contribute but aren't sure how to get the values, post a screenshot of your real-time data tab while under full throttle and I'll do it for you!

**TL;DR: Some motor KVs are lower than advertised, let's gather data here!**

**More TL;DR**

* **chaka's 200kv motor = 197kv calculated**
* **Jlabs' Polar 190kv motor = 179kv calculated**
* **Kaly's 230kv motor = 200-210kv calculated (20 samples)**
```

---
## \#2 Posted by: JLabs Posted at: 2017-05-18T02:05:42.572Z Reads: 477

```
I think this is the first time I saw something like this, cutos for something new! 

As for the kv, they are specd to +/- 8kv. So theoretically you should receive a 182-198kv motor. In your case it seems like it was a little off. 

For future orders I am becoming more strict on the quality of the motors, and this will now be one of many main pints of focus. 

-Jared
```

---
## \#3 Posted by: Blasto Posted at: 2017-05-18T02:45:46.516Z Reads: 449

```
@Jinra as a FYI, if you go in the terminal and type "kv" the vesc will give you the kv in erpm (divide number by pole pairs)
```

---
## \#4 Posted by: Jinra Posted at: 2017-05-18T02:46:45.157Z Reads: 434

```
Good call! I'll check it in a bit and compare to my calculations.

EDIT:
@Blasto Ran 'kv' in terminal and pretty much got it right on point at 180.5 kv calculated and 180.9 in terminal.
```

---
## \#5 Posted by: Kaly Posted at: 2017-05-19T02:07:58.988Z Reads: 385

```
One thing you need to do here is to remove the erpm limit on the motor configuration by extending it to +- 100000 ERPM.

This way you will get the real Kv without any limiting from the VESC configuration settings.

also if going the terminal KV command way make sure to press the throttle with one hand while typing the KV command with the other this way you will get the current KV at that particular time. 

Kaly's 230Kvby the  REAL TIME TAB

<img src="/uploads/db1493/original/3X/9/1/912aada6b44990292d3bfaa75d0affa18c98fd3f.jpg" width="408" height="300">

AVerage Kv By Terminal Kv command 
<img src="/uploads/db1493/original/3X/0/8/084d3291b29d8e614ee43f11816b54d97a938570.jpg" width="250" height="493">

214.66Kv
```

---
## \#6 Posted by: Jinra Posted at: 2017-05-19T02:24:34.294Z Reads: 335

```
Don't use the limiter myself :sunglasses:
```

---
## \#7 Posted by: Jinra Posted at: 2017-05-19T05:19:49.090Z Reads: 331

```
UPDATE! - Added results for Kaly's 6355 230kv motor in OP.

Given my findings with Kaly's motors I think this is the reason you never have to set an eRPM limit for your 12s 190kv builds @longhairedboy. If your actual kv is lower than advertised, then you'd be gracefully under the eRPM limit even given ideal conditions (50.4v) which means at full charge with zero voltage sag.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-05-19T06:23:09.786Z Reads: 318

```
Awesome thread @Jinra
I'm gonna do the test soon and give you the findings for the APS 6355 190kv HEV motors that I'm using.
should the test be done with belts off or on or does it matter?
```

---
## \#9 Posted by: Jinra Posted at: 2017-05-19T06:33:10.924Z Reads: 307

```
I do it with no belts or load what-so-ever to get best scenario results.

My methodology includes running the test 10 times using 'kv' in terminal as well as manually calculating a couple times to get an average.
```

---
## \#10 Posted by: fraannk Posted at: 2017-05-19T06:43:29.712Z Reads: 296

```
Alien HEV 230KV 6355 is about 216KV irl
```

---
## \#11 Posted by: longhairedboy Posted at: 2017-05-19T11:37:54.827Z Reads: 293

```
That would mean that neither my motors nor the original R-SPEC 6355 190s were actually 190s. 

Which wouldn't surprise me in the least. My guess is they just come up with a wind count and wire guage that would get them close, apply that count when they wind it,  and then bin it as a 190. 

The interesting bit is when using 80% efficiency they do deliver what the esk8 calculator says they do provided you're in my weight class. So even if they are, for example, 185 or something, they still act like a 190.
```

---
## \#12 Posted by: Okami Posted at: 2017-05-19T12:46:10.300Z Reads: 278

```
mh nice that someone brought this out a bit more..

I remember same thing (kv being lower) was said about torqueboards motors a while ago, so im glad to see some other motors being tested..

Cool to see, they are actually lower in values, both better for power and for erpm limit, I assume :slight_smile:
```

---
## \#13 Posted by: longhairedboy Posted at: 2017-05-19T14:34:50.229Z Reads: 273

```
i remember that to. Seems like they gave him a really hard time about it.
```

---
## \#14 Posted by: Namasaki Posted at: 2017-10-02T00:16:40.234Z Reads: 255

```
Alien HEV 6355 190KV tested at 172KV
Alien HEV 6374 200KV tested at 174KV
```

---
## \#15 Posted by: Mobutusan Posted at: 2017-10-02T05:07:00.939Z Reads: 244

```
Very interesting. Thanks for posting your results. Did you measure that through the VESC tool? I've got a pair of Torqueboards 190kv (2 slightly different can styles) and a pair of 230kv (your old ones) 6355's that in interested in testing. I've heard it rumoured that the older 230kv motors were actually closer to 190kv.
```

---
## \#16 Posted by: Namasaki Posted at: 2017-10-02T05:20:00.348Z Reads: 248

```
the easiest way is to use the terminal command.
Type KV and send it several times to get an avg reading of erpm per volt  then divide that by 7 to get the motor KV value.
I was able to do this using a bluetooth module and Metr app.
I ran this test with belts and wheels on.
Then I pulled the belts off and retested and got a slightly higher value.
<img src="/uploads/db1493/original/3X/c/a/ca4f2475b02c4b054dc0ac9a6b654c8083b968c7.PNG" width="281" height="499">

https://metr.at
```

---
## \#17 Posted by: Aeroquiv Posted at: 2017-10-02T07:51:33.241Z Reads: 228

```
Racerstar 5065 200 kV tested at 184 kV
```

---
## \#18 Posted by: UniqueSnowflakeN27 Posted at: 2017-10-02T15:28:29.065Z Reads: 222

```
TorqueBoard 75KV hubmotor tested at 85,56KV. 

Did I do something wrong? The trend seems to be lower KV than advertised.

Here's the numbers: 37667 / 33,1 / 14 / 0.95 = 85,562

<img src="/uploads/db1493/original/3X/e/1/e1f353aa845b20115ba26170462910cfdf4b5743.png" width="690" height="388">
```

---
## \#19 Posted by: Namasaki Posted at: 2017-10-02T15:43:06.301Z Reads: 211

```
Try this. 
Type KV in terminal and send while holding throttle. 
The vesc will report erpm per volt. 
Divide by 7 and you will have your motors true KV
```

---
## \#20 Posted by: Jinra Posted at: 2017-10-02T16:33:02.152Z Reads: 213

```
Sorry mistake in my original post. you should multiply by .95 instead of divide which gives you 77.2 pretty close!

Apparently it's too old for me to edit

EDIT: wait i was correct the first time divide by .95
```

---
## \#21 Posted by: Jinra Posted at: 2017-10-02T16:34:13.043Z Reads: 208

```
In his case he has to divide by 14 since he has more pole pairs
```

---
## \#22 Posted by: Namasaki Posted at: 2017-10-02T17:33:50.142Z Reads: 207

```
Oh, that's right, it's a hub motor
```

---
## \#23 Posted by: Vanarian Posted at: 2017-10-02T18:03:52.286Z Reads: 209

```
Thank you for this tip ! Ok so in fact I should have IRL values of 80.7Kv instead of 85Kv for my motors. Need to mesure !
```

---
## \#24 Posted by: longhairedboy Posted at: 2017-10-02T18:17:17.314Z Reads: 212

```
I was JUST NOW explaining to somebody why you can use 190KV rated motors at 12S and get away with it without bumping the ERPM limit.

Here is the answer right here. 

No motor is what its rated at. Better motors are closer, but none of them are precise. 

Now i want to go home and see what mine actually are. Probably around 180 as well.
```

---
## \#25 Posted by: Namasaki Posted at: 2017-10-02T18:40:02.391Z Reads: 205

```
I'm shocked how far off my APS HEV motors  are and they're supposed to be precision motors.
Maybe mechanically but certainly not electrically
```

---
## \#26 Posted by: longhairedboy Posted at: 2017-10-02T18:47:45.975Z Reads: 203

```
dude. They're Alien. 

But to make you feel better, i'll pretend to be shocked when i find out what my branded Maytech's are.
```

---
## \#27 Posted by: telnoi Posted at: 2017-10-04T06:42:08.373Z Reads: 195

```
Since the same manufacturer appears to be selling similar motors through banggood under the brand racerstar (only different sizes), I am not surprised. They are known as a low quality and low performance motor in the fpv racing community.
```

---
## \#28 Posted by: Cobber Posted at: 2017-10-04T06:52:53.418Z Reads: 195

```
more than 5% +/- scorpion will change em over ;)
```

---
## \#29 Posted by: longhairedboy Posted at: 2017-10-04T13:28:42.798Z Reads: 183

```
aren't racestars what Evolve is using? or did i mis-hear a rumor?
```

---
## \#30 Posted by: Okami Posted at: 2017-10-04T14:01:44.509Z Reads: 183

```
Yeh i would also like to hear some feedback about them and also from which source u got it? 

In my opinion, they seem pretty decent, not to mention they sealed case (not many open spaces) and also fact that many of them come with sensor wires and flatspot for grubscrews. 

Ive seen some low end chinese brushleas motors and for.these.u can see straight away that quality is subpar
```

---
## \#31 Posted by: telnoi Posted at: 2017-10-04T14:03:12.227Z Reads: 185

```
They have the same design, would not surprise me.
ESK8 world hasn't seen proper motors yet I think, also makes me wonder how expensive these would be if someone were to match the quality of some of the racing drone motors (a good 2207 motor costs in between 25-35 euro).

Things that make up a good motor
*Al 7075 
*N52H high temp curved magnets (curved increases efficiency)
*Single strand windings (decreases temperatures)
*Steel inserts for mounting screws
```

---
## \#32 Posted by: Jinra Posted at: 2017-10-04T14:05:24.902Z Reads: 191

```
Pretty sure I've seen some of those advertised by various esk8 motor dealers. At least the curved magnets anyway.
```

---
## \#33 Posted by: telnoi Posted at: 2017-10-04T14:12:31.798Z Reads: 192

```
Relatively certain the racerstar does not :slight_smile:
Here's a discussion on these (with banggood links).
https://www.electric-skateboard.builders/t/more-40-55-motors-from-banggood-5045-200kv-5060-280kv-5065-200kv-6368-280kv/15433

Since the ESK8 motors are allot bigger, some of the issues such as softer alu might not be an issue.  Racerstar  
 is known as a low budget brand with OK-ish parts. Their ESCs on the other hand are top notch. If they ever release one for the ESK8 world...

http://www.miniquadtestbench.com/racerstar-br2205-2600kv.html
Just for reference, a trusted review on one of their multi rotor motors. You can clearly see the design ethics that are also used for their ESK8 motors...and surprise surprise, the KV is allot lower than stated in the specs. The performance also sucks.
```

---
## \#34 Posted by: longhairedboy Posted at: 2017-10-04T14:25:12.331Z Reads: 185

```
know your components, don't trust the labels. 

yeah that's basically every hobby known to man. Clock speed vs thread count. Megapixels vs lensing and sensor quality. C rating vs actual capacity for discharge, the list goes on.
```

---
## \#35 Posted by: Namasaki Posted at: 2017-10-04T15:42:35.527Z Reads: 185

```
I have been using the Alien HEV motors for a while now and I have not found them to be low quality or low performing. 
Mechanically they are good quality  imo. 
The 10mm shaft is machined in close tolerance so the bearings don't fit sloppy. 
Performance wise, they offer good torque, run smooth and relatively cool. 
My 6355s are so quiet that it sounds like I'm running FOC when I'm running BLDC.
The low actual KV is minor imo. 
But then I'm not talking about drone motors.
```

---
## \#36 Posted by: telnoi Posted at: 2017-10-04T15:45:46.952Z Reads: 181

```
As I mentioned, I suspect the larger size makes up for it.
If you ever have the pleasure of comparing it to a high-end motor with the aforementioned magnets, let me know. These are allot stronger. Also, I doubt you will need more speed though a better efficiency would be nice. Same power/less amps.
```

---
## \#37 Posted by: Namasaki Posted at: 2017-10-04T15:46:50.908Z Reads: 178

```
I don't know of any better motors available for Esk8
```

---
## \#38 Posted by: Jinra Posted at: 2017-10-04T15:48:08.230Z Reads: 184

```
I can't imagine every esk8 targeted dealer has it wrong when it comes to motors, some of them have to have it right using choice motors; and within these dealers there doesn't seem to be too much difference between the performance of said motors.

Not sure if you've tried boards like the Raptor 2 or even newer Evolves, because those motors are indeed very strong.
```

---
## \#39 Posted by: telnoi Posted at: 2017-10-04T15:49:22.629Z Reads: 185

```
might be made to specification then. Could still be that different magnets are used for Evolve. Could you link to one of these spec sites?
```

---
## \#40 Posted by: Jinra Posted at: 2017-10-04T15:52:26.400Z Reads: 188

```
I don't have motor specifics for you sorry. However, I do know that various retailers on this forum have sold their motors with their own specs, which probably contribute to decent quality motors. The ones I know of from the top of my head are @JLabs and @Kaly, but there are more as well.
```

---
## \#41 Posted by: telnoi Posted at: 2017-10-04T16:06:26.301Z Reads: 182

```
maybe they can chime in. Would be good to know if there is a difference between the racerstar motors, APS etc.
It's not all about KV.
```

---
## \#42 Posted by: Jinra Posted at: 2017-10-19T04:58:11.067Z Reads: 185

```
WOW, just did a kv calculation on @JLabs motors and they're WAY off.

The 6355 208kv motors I got tested at 171kv, though a small disclaimer, I did test this in FOC, I'm sure it'd be closer to the 208 advertised value if I ran BLDC.

46799 / 41.09 / 7 / .95 = 171kv

EDIT: redid it in BLDC and got 181kv!

<img src="/uploads/db1493/original/3X/7/d/7d75f1555904f1dbc1998e6169cb4104f12f2623.png" width="690" height="459">
```

---
## \#43 Posted by: biggdaddyhawk Posted at: 2017-12-09T05:47:04.941Z Reads: 165

```
How does the "turns" of a motor correlate to kv . I only  have  rc car experience from when I was a kid. We never worried about kv, it was all about turns. Maybe they are similar or proportional.  Stock motors had like 21 turn s and gave long run times. And 18 turns gave more top end speed with the sacrifice of a shorter run time. These were all brushed motors though. With  brushless it seems to be not about the turns but about kv. I just bought some tacon 160 bigfoot motors and did notice in the specs that they are 8turn and can handle 14s. Has anybody tested the true kv of these yet. Just intrerested
```

---
## \#44 Posted by: E1Allen Posted at: 2017-12-09T06:16:42.535Z Reads: 167

```
Turns determine kV is all. Basically the same thing.  Vesc have the 60k ERPM or higher depending on which one you buy.  Lower kV higher TQ.  The concern is blowing drv chips above 60k ERPM on high kV and voltage builds. But everyone here uses various voltage and motor size based on range, speed, budget, ect of each build.
```

---
## \#45 Posted by: biggdaddyhawk Posted at: 2017-12-11T17:04:32.726Z Reads: 168

```
So knowing the tru kv of a motor is probably more important for motors and battery combinations that max out the 60k limit. So inputting an advertised kv spec that is off will destroy the drv b/c of the edrpm. I mean some of these kv ratings are way off and there needs to be a comprehensive list to correct these bogus advertised ratings. I just don't see why they would give specs that are rounded off and not dead on. Testing the tru kv of a motor should be #1  thing before vesc setup and battery choice. Before I stumbled upon this I would have just plugged in factory specs for kv when my  vesc came in the mail.
```

---
## \#46 Posted by: longhairedboy Posted at: 2017-12-11T20:35:05.185Z Reads: 167

```
Actually.. if the KV is lower than stated and you do the calculations based on the stated KV the following will happen:

* the board will be slower than anticipated and a little more torquey than expected
* the board will be far, far less likely to come anywhere NEAR the ERPM limit so blowing up DRVs isn't going to be an issue unless you do something silly. 

@Jinra Do one of my motors. They're stated at 3100 watts and 190KV. Its a standard sensored 6355 from Maytech. I would do it myself but for posterity and purity it would be better if somebody else did it. 

I've never done it but i suspect theyr'e somewhere in the realm of 170 actual KV as well, which is why i can use them with such wild success at 12S on FocBoxes and VESC 4.12s because they're nowhere near the ERPM limit even at full throttle, yet they deliver monstrous power at all ratios. 

No skateboard motor is the actual advertised KV. ITs all horseshit. Find the motor that looks like it can handle your shit. Specs are all marketing garbage. You have to open the shit up and see the copper and feel it. Smell it. Roll the stator around on your chest sensually and absorb the magnetic chi. Don't let anyone see you do that, they'll laugh and post it on youtube. 

or just get the big fucking motor with the mountain of copper and iron in it.
```

---
## \#47 Posted by: BigBoyToys Posted at: 2017-12-11T22:27:04.030Z Reads: 157

```
I measured kV on my APS 8085's and they were slightly above their stated rating but almost dead on at 350
```

---
## \#48 Posted by: Jinra Posted at: 2017-12-11T23:13:04.470Z Reads: 159

```
My @chaka motors were actually only a couple kv off, but I've seen them vary wildly between vendors.
```

---
## \#49 Posted by: faithfulpuppy Posted at: 2017-12-12T01:49:47.913Z Reads: 156

```
@longhairedboy i can test your motors when they (and their mounts) arrive. Shouldn't be until next year but hey that's not so far away!
```

---
## \#50 Posted by: biggdaddyhawk Posted at: 2017-12-13T00:48:04.590Z Reads: 142

```
I think if a list is made we can see which ones are way off and we can have faster more efficient setups
```

---
## \#51 Posted by: Bjork3n Posted at: 2019-02-03T09:45:15.936Z Reads: 79

```
![56|690x388](upload://sH3i32B0fCWvjbXk9Yo7gyZVnQK.png) 

Maytech (eskating 190kv) 
Messured kv 160kv, quite a bit off whats advertised haha.

38788/ 36.5 / 7 / .95 = 159kv

Tested in FOC
```

---
## \#52 Posted by: Jinra Posted at: 2019-02-03T10:20:54.281Z Reads: 76

```
you should run the `kv` command in terminal for a more accurate calculation
```

---
## \#53 Posted by: Bjork3n Posted at: 2019-02-03T10:37:36.591Z Reads: 76

```
![37|690x388](upload://jE801stoeaBAaliAVjURQggO6aW.png)
 
This is what I got when running bldc
```

---
## \#54 Posted by: Jinra Posted at: 2019-02-03T10:50:40.085Z Reads: 75

```
yep thats 187-197 kv
```

---
## \#55 Posted by: Bjork3n Posted at: 2019-02-03T15:11:34.580Z Reads: 70

```
Thats weird. 
My max speed is 42km/h on full charge and the esk8 calc says it should be 47km/h with 190kv motors.
If i put in 170kv in the calc the calculated speed seems spot on!

6374 motors with 10s battery 
16/36 and 97mm wheels.

Cant do the kv calculation in the terminal when using  FOC...weird.
```

---
## \#56 Posted by: Sebike Posted at: 2019-02-03T16:02:47.826Z Reads: 69

```
Edit: With the maytech 190 KV motor, 10S battery on full charge, 16/38 ratio and 97 mm wheels I get around 44-45 km/h top speed.

I never managed to get a KV read in BLDC-tool terminal either (in FOC mode).
```

---
## \#57 Posted by: Winfly Posted at: 2019-02-04T06:48:11.496Z Reads: 59

```
you need to run a bldc detection before using the kv command.
```

---
