# Battery Longevity

### Replies: 47 Views: 1783

## \#1 Posted by: darkkevind Posted at: 2017-06-13T15:59:19.934Z Reads: 149

```
Quick question. I have 3 x 3s Lipos in series, they're all 5000mah 25c.

I've been out on my board today, they were all practically fully charged but I only got 5.1 miles out of them before the ESC cut the voltage to preserve them... Does that sound right to you?

Using the same cells, is there a way to get more distance? 

What would be the best configuration for Li-ion batteries to get the a greater distance from them? I can drop voltage down to 22.2 as that's what I had before and was quite happy with...
```

---
## \#2 Posted by: wmj259 Posted at: 2017-06-13T16:58:10.701Z Reads: 140

```
I have my 3x3S lipos in series also but it lasts me 3-4 hours of cruising and speed riding. 
I have my cutoffs at 3.6 and 6374
```

---
## \#3 Posted by: darkkevind Posted at: 2017-06-13T18:49:09.379Z Reads: 125

```
Hmmm, that's odd. My packs are a little 'puffy' maybe they've had it!?

Maybe they weren't fully charged after all? I thought they were but to be honest, I'd done some ESC testing (setting up my VESC) before going out but not miles worth...
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2017-06-13T19:40:39.069Z Reads: 113

```
You can estimate about 1 mile per Mah running at 6s ...that's abt normal
```

---
## \#5 Posted by: darkkevind Posted at: 2017-06-13T19:43:05.206Z Reads: 107

```
So if I ran 6s instead of 9s and my batteries are 5000mah, I can expect 5 miles?

Would that mean that if I changed it to be 5000mah 3s in parralel, I'd get 15 miles?
```

---
## \#6 Posted by: Michaelinvegas Posted at: 2017-06-13T19:44:19.780Z Reads: 101

```
Well I just noticed ur running 9s ... what lipos are u using? What's the c rating?
```

---
## \#7 Posted by: darkkevind Posted at: 2017-06-13T19:45:56.125Z Reads: 102

```
Turnigy 11.1v. 25c
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2017-06-13T19:46:40.023Z Reads: 96

```
To be honest you'd prob be closer to 7 - 9 miles on 9s
....
Do you have a lot of hills? Rough roads?
```

---
## \#9 Posted by: darkkevind Posted at: 2017-06-13T19:48:24.307Z Reads: 98

```
I was mainly on the flats today, like one small slight incline of a hill for about 100m
```

---
## \#10 Posted by: Michaelinvegas Posted at: 2017-06-13T19:49:07.365Z Reads: 98

```
Def should be getting more than 5 miles then mate
```

---
## \#11 Posted by: darkkevind Posted at: 2017-06-13T19:50:22.757Z Reads: 92

```
:angry: That's annoying! Think my packs must be kaput!
```

---
## \#12 Posted by: Michaelinvegas Posted at: 2017-06-13T19:51:31.958Z Reads: 92

```
Nah ... recheck your wiring... puffy lipos .... it's a thing as long as they ain't really getting deformed
```

---
## \#13 Posted by: Michaelinvegas Posted at: 2017-06-13T19:52:52.153Z Reads: 90

```
Also check wheels and belts for drag just incase something is binding.... 

Other option is to get a higher rated battery with higher c rating
```

---
## \#14 Posted by: Michaelinvegas Posted at: 2017-06-13T19:54:07.722Z Reads: 91

```
One way of telling if lipos are bad is if the cells drift a lot or a cell discharges way faster than the rest.. if your cells do none of these..they are fine
```

---
## \#15 Posted by: darkkevind Posted at: 2017-06-13T19:54:33.085Z Reads: 90

```
When I got the packs they were around 25mm thick, they're about double that now! :astonished:

I've checked that nothing's dragging, it's a chain drive and everything seems to be very smooth...
```

---
## \#16 Posted by: darkkevind Posted at: 2017-06-13T19:55:22.636Z Reads: 88

```
I'm going to go and check each cell in a mo and see where they sit. I've not charged it since I got back from this ride today so that'll give me a good indication.
```

---
## \#17 Posted by: Michaelinvegas Posted at: 2017-06-13T19:55:55.542Z Reads: 83

```
Never had a chain drive ...maybe someone here has some relevant experience with them and the effect on range
```

---
## \#18 Posted by: Michaelinvegas Posted at: 2017-06-13T19:56:29.552Z Reads: 80

```
Letting them cool is always a good idea before recharging them
```

---
## \#19 Posted by: darkkevind Posted at: 2017-06-13T19:57:15.763Z Reads: 78

```
Oh yeah, I got back hours ago... they're stone cold Steve by now :thumbsup:
```

---
## \#20 Posted by: darkkevind Posted at: 2017-06-13T20:06:15.367Z Reads: 77

```
That's weird, I've just checked the voltage of the whole pack in series and it's still got 34.4v in it!?
```

---
## \#21 Posted by: Michaelinvegas Posted at: 2017-06-13T20:06:35.534Z Reads: 68

```
Then it's the voltage sag
```

---
## \#22 Posted by: darkkevind Posted at: 2017-06-13T20:06:51.665Z Reads: 64

```
How you mean?
```

---
## \#23 Posted by: Michaelinvegas Posted at: 2017-06-13T20:10:18.717Z Reads: 66

```
Depending on battery, brand, c rating, temp and other stuff .... voltage sag will trip your voltage cut off.... but when I come off throttle the voltage comes back up...

I'd try a higher c rated battery in your case
```

---
## \#24 Posted by: darkkevind Posted at: 2017-06-13T20:12:26.058Z Reads: 68

```
Right, I see. Thanks :thumbsup:

That would explain why going down the slight hill on my way back to the car at the end of the ride it almost seemed like it gained some guts again?
```

---
## \#25 Posted by: jaykup Posted at: 2017-06-13T20:18:26.637Z Reads: 67

```
Running 9s (recommended with your setup) voltage cut-offs should be:

3.6 x 9 = 32.4v cutoff - may be able to do a little less than 3.6 but I'm not as familiar with Lipos as Li-ion.

If your batteries are puffy they are likely dying/dead.  Probably from over-discharge if you were draining 9s batteries to 22v!

If you have a balance charger then just full charge one 3s pack at a time, and fully discharge it on the charger to measure your amp hours.  These things are like $25-30 on ebay.

Secondly, if you have a VESC and a BLE module you can run ackamaniac's app and see how many watt hours you are actually consuming and compare that to the batteries specs.

Lastly, voltage will drop when under load, and slowly rise again once left alone for a bit.  But around 3.6v (32.4v for 9s) for lipo is basically dead.
```

---
## \#26 Posted by: Michaelinvegas Posted at: 2017-06-13T20:28:47.882Z Reads: 60

```
That's the regen giving you a bump
```

---
## \#27 Posted by: darkkevind Posted at: 2017-06-13T20:29:09.218Z Reads: 63

```
Ah of course!
```

---
## \#28 Posted by: Achmed20 Posted at: 2017-06-13T21:16:49.639Z Reads: 63

```
[quote="darkkevind, post:5, topic:25284, full:true"]
So if I ran 6s instead of 9s and my batteries are 5000mah, I can expect 5 miles?

Would that mean that if I changed it to be 5000mah 3s in parralel, I'd get 15 miles?
[/quote]

its all about the Watts and thats calculated Volts * Amps = Watt.
if you just put them in paralel, the watts would stay the same
36v * 5A = 180Watts
12v * 15A = 180 Watts

btw, im running a 9S 5000mah set as well and i reach something about 18-20km (~10 miles)
```

---
## \#29 Posted by: darkkevind Posted at: 2017-06-13T21:18:46.833Z Reads: 60

```
OK I see. So how would I go about getting more miles?
```

---
## \#30 Posted by: Achmed20 Posted at: 2017-06-13T21:27:00.012Z Reads: 59

```
technicaly only by increasing the watts. which means adding more cells.
since you are using lipos anyway, you could just go for 12S which will give you 1/3 more range
or add 3 more 3s 5000mah battery in paralel which will double your range

it also depends heavily on how you are driving. if you are accelerating often and hard, your battery wont last long. accelerating takes lots of juice. jsut cruising along is what gives you range.

edit: new lipos need to be "burned" in by the way. that basicly means charging and discharging them 2 or 3 times before using them. if you jsut charge them and them start hammering them, yourt chance of killign them is rather high.
```

---
## \#31 Posted by: darkkevind Posted at: 2017-06-13T21:29:38.878Z Reads: 58

```
Thanks for that.

To be honest, today, although I was stop starting quite a bit because I was filming, I mostly cruised and only tried out top end once for a few seconds...

I was mostly at half throttle for at least 4 of my 5 miles
```

---
## \#32 Posted by: Achmed20 Posted at: 2017-06-13T21:38:24.533Z Reads: 56

```
well you should get at least 8-9 miles with a 9S setup. i get like 10miles with only 80% charged batterys (missing a charger with the right amount so 80% is all i get :D )
what motor and gear ratio are you using???

since your battery are puffy already, i realy recommend getting rid of them and buying new ones. 
the borderline minimum charge for lipos shouldnt be lower then 3.2Volts per cell. on a 9S setup thats a minimum voltage of 28.8V. so if you realy downed them to 22V allready, your probably killed your pack anyway
```

---
## \#33 Posted by: darkkevind Posted at: 2017-06-13T21:41:55.923Z Reads: 57

```
It's possible I killed them with my last ESC as it didn't have cut off protection etc.

I'll look in to getting some new batteries, I'm thinking of going for Li-ion this time though with a BMS. What configuration would you recommend to get me around 10 miles of range?

My pinion is 10T and the sprocket is 30T (it's a chain drive).
```

---
## \#34 Posted by: Achmed20 Posted at: 2017-06-13T21:56:36.312Z Reads: 54

```
dont underestimate li-ions ^^
if you want to do it right, then you need something like a 10s4p build (4 packs of 10 batteries) which cost allready ~200€  not counting in a BMS. that would be at least 50€ extra. and li-ions dont come prebuild which means you have to build everything on your own. and you want that to be at least 3 packs because li-ions are nowhere near the discharge rate of a li-po pack.
1 single 1s 25c 5000mah lipo pack can deliver 125Amps while a single li-ion battery delivers 10c tops. thats 25-30 amps.
```

---
## \#35 Posted by: darkkevind Posted at: 2017-06-13T22:08:22.246Z Reads: 51

```
Yeah I'm thinking of using Samsung 30q 3000mah.

I was thinking of making an 8s4p pack. Would that be OK?
```

---
## \#36 Posted by: Achmed20 Posted at: 2017-06-13T22:20:27.503Z Reads: 49

```
thats up to you. id probably go for a 10s at least.
```

---
## \#37 Posted by: darkkevind Posted at: 2017-06-13T22:43:07.931Z Reads: 51

```
Yeah but why's that? What would the difference be? Range or speed, or both?
```

---
## \#38 Posted by: anorak234 Posted at: 2017-06-13T22:59:28.553Z Reads: 52

```
Yo!! Listen to @jaykup!!! If you have been draining them to 22.2V this is VERY bad for them and explains the puffiness as well as loss of capacity! Please dispose of them safely, do some research on safety with lithium batteries, and buy a Lithium ion battery
```

---
## \#39 Posted by: darkkevind Posted at: 2017-06-13T23:14:37.991Z Reads: 56

```
Err, I have been listening to everyone... I'm not 100% sure if I have in fact been draining them too low but two of the three packs are a bit 'puffy'.

I'm thinking about replacing them with Li-ion. As you can see. From my posts above.

I'm trying to ascertain which would be the best configuration for me for cost and range . . . which you'd know . . . if you read my posts . . .
```

---
## \#40 Posted by: sprocket12 Posted at: 2017-06-14T00:09:00.447Z Reads: 68

```
So I just 'disposed' of two Zippy 8000 mAh Lipos.  Youtube has a lot of examples of disposing.  I created a discharge circuit with a 12v lightbulb.  If you are getting rid of them, hook up the light bulb and place it somewhere safe until the light is no linger lit.  Use a voltmeter and make sure the battery shows under 1v.  At this point, it is safe to dispose.

If you haven't worked with Lipos before, you should know that they can become unstable when abused (ie over/under/load charge).  A damaged pack can become a roman candle quick!  And it can take a while before the chemical reaction turns into flames.  They should be removed and stored in a fireproof container when not in use.

Now, with that said, I am moving to Li-ion batteries.  They are more expensive and @Achmed20 is counting the costs in building a pack.  My 8s1P (2 x 8000 mAh 4s1p Zippy's) would get me about 12 miles. I have a 6374 motor (I think.  I'm at work).  An 8s4p pack of 3000 mAh will give you 12,000 mAh, or about 18 miles if you are using a similar motor and gear ratio as I am.  If I have found the correct reference for the battery you wish to use, it is a continuous 15 amps.  Across 4 packs that's 60 amps.  Your Lipos were more like 125 amps.  Your torque will drop (acceleration) but it will be doable.
```

---
## \#41 Posted by: jaykup Posted at: 2017-06-14T05:13:51.852Z Reads: 58

```
I can get 21 miles on a 444 wh battery pack (12s4p 25r) on a single 6374

+1 to the 10s4p 30q pack (440 wh) - range of 20 miles or so.

vs 8s4p 30q pack (355 wh) - range of 15 miles or so and less acceleration
```

---
## \#42 Posted by: darkkevind Posted at: 2017-06-14T07:00:44.135Z Reads: 57

```
Thanks @sprocket12 & @jaykup , I'd be happy with 15-18 miles of range...

Having said that I think I'll go with 10s4p.

I'm thinking I'll use my puffy lipos to start a fire in my garden incinerator.... :smile:
```

---
## \#43 Posted by: SpeedSloth Posted at: 2017-06-14T10:46:30.990Z Reads: 53

```
Here's a little table I made to help me select a battery configuration. It may help you decide what you need:

<img src="/uploads/db1493/original/3X/5/2/5258f3222eae0dbd59393aba594d357c6afe0cf4.png" width="690" height="228">
```

---
## \#44 Posted by: darkkevind Posted at: 2017-06-14T10:50:55.677Z Reads: 54

```
Cool, thanks! :thumbsup:

I think I'd be happy with 10s3p or 10s4p :D Between 15-20 miles is ample for me...
```

---
## \#45 Posted by: darkkevind Posted at: 2017-06-14T10:54:57.773Z Reads: 54

```
Hey, I just realised what's happening with my Lipos to screw them up! My IMAX B6 is overcharging them!! The readout when charging isn't reading right! :rage:
```

---
## \#46 Posted by: SpeedSloth Posted at: 2017-06-14T10:58:41.457Z Reads: 54

```
I'd go with the 4 to increase the C rating and hence reduce the stress on the batteries. This should increase their lifespan.
```

---
## \#47 Posted by: darkkevind Posted at: 2017-06-14T14:58:01.343Z Reads: 50

```
I've definitely killed my Lipos! Only managed to get 2.5 miles from a full charge today before the board became pretty much useless... I could walk quicker :unamused:
```

---
