# Brakes failing don’t know why please help

### Replies: 74 Views: 857

## \#1 Posted by: Halbj613 Posted at: 2019-04-17T20:49:47.693Z Reads: 176

```
Today I was riding down hill tried braking and my brakes only produced a tiny amount of brake force.

Had to bail board out and jumped off luckily I was only going 15mph board got smashed a bit.![image|669x499](upload://9AVeFwlvrLF38I9hFbNJ3K7FjMV.jpeg) 
Only new thing we’re some new motors 

but this is a pretty new build however so I don’t know for it was setup correctly

My build is tb 260kv 6355 motors
10s2p Samsung battery produces 20amps
Flipsky dual 4.12 vesc
Abec11 flywheels
Gt2b remote

Please help me probably didn’t setup bldc tool correctly please help thank you
```

---
## \#2 Posted by: Saturn_Corp Posted at: 2019-04-17T20:53:24.802Z Reads: 166

```
what are your vesc settings?
```

---
## \#3 Posted by: AlanZhou Posted at: 2019-04-17T20:57:52.347Z Reads: 162

```
You might be going over the erpm Limit
```

---
## \#4 Posted by: rusins Posted at: 2019-04-17T20:58:07.962Z Reads: 164

```
New motors that are high KV – probably means that if you didn't change your VESC settings then the previous motor min values are now producing too little breaking torque. Either that, or your BMS tripped and wouldn't accept the return voltage. Definitely share your Vesc settings.
```

---
## \#5 Posted by: Halbj613 Posted at: 2019-04-17T21:06:30.249Z Reads: 161

```
What should Erpm limit be

Don’t really understand vesc values so probably have made so many mistakes
```

---
## \#6 Posted by: Halbj613 Posted at: 2019-04-17T21:06:50.997Z Reads: 156

```
Here are pictures![image|669x499](upload://lStJQNkeXE4iZV0UPUjI4i1oCq8.jpeg) ![image|669x499](upload://m2koocEupifOhGHOYyWzvn15egL.jpeg) ![image|669x499](upload://gB61YM6Eqn6bbqc7SRuVRzfIVGX.jpeg) ![image|669x499](upload://r4ozQhaseS3ckQdCp7s9QDkJWft.jpeg) ![image|669x499](upload://iH6NPyZvvfQNJlMmATWGBP5Y3fv.jpeg)
```

---
## \#7 Posted by: Halbj613 Posted at: 2019-04-17T21:10:07.851Z Reads: 142

```
I know that I probably made some big errors main one Is with the throttle and brake curve I think I got that one wrong
```

---
## \#8 Posted by: Battosaii Posted at: 2019-04-17T21:10:57.285Z Reads: 143

```
Were you close to a full charge? Brakes will fail with a smaller battery at or near full capacity. The vesc has no where to dump the extra energy so it jusy wont brake.
```

---
## \#9 Posted by: Halbj613 Posted at: 2019-04-17T21:11:37.806Z Reads: 142

```
Probably around 90% charged
```

---
## \#10 Posted by: Halbj613 Posted at: 2019-04-17T21:11:52.573Z Reads: 141

```
Is that the only reason
```

---
## \#11 Posted by: Battosaii Posted at: 2019-04-17T21:11:52.743Z Reads: 139

```
Found your problem
```

---
## \#12 Posted by: Battosaii Posted at: 2019-04-17T21:13:00.642Z Reads: 136

```
Should be imo try doing the same thing in a safer manner if you can but with 50% charge and no other changes i bet it will brake perfect.
```

---
## \#13 Posted by: Halbj613 Posted at: 2019-04-17T21:14:07.021Z Reads: 138

```
I tried braking before with board upside down on half charge however I could feel how easy it was to turn the wheel
```

---
## \#14 Posted by: Battosaii Posted at: 2019-04-17T21:14:58.767Z Reads: 133

```
Ive had this happen to me on a 10s3p with 97% battery it was quite the scare. I believe someone makes a product now to fix this problem with smaller batteries.
```

---
## \#15 Posted by: Halbj613 Posted at: 2019-04-17T21:15:38.913Z Reads: 127

```
Are you sure that is the only reason still dead scared about it
```

---
## \#16 Posted by: Halbj613 Posted at: 2019-04-17T21:18:06.499Z Reads: 127

```
Is there any problem with settings
```

---
## \#17 Posted by: Saturn_Corp Posted at: 2019-04-17T21:23:27.206Z Reads: 125

```
They look good to me, but I'm no expert. 

You said your battery could do 20 amps total or per motor? I see you have it set as 30 per motor for a total of 60. What configuration and cells does it use? lipo/liion?
```

---
## \#18 Posted by: rusins Posted at: 2019-04-17T21:38:24.502Z Reads: 123

```
Your "absolute maximum current" is set to only 30A, I would suggest resetting it to the default value which is a bit above 100A if I recall. A sudden current spike from breaking could have easily passed that.

Also, I noticed that you have dual VESCs over canbus (I assume that's how the Flipsky dual works since it has 2 usb ports). Make sure you have the same motor settings for both, and also this means your battery current limits are too high! Assuming your battery is from Samsung 30Q cells (which are good for 20A per cell), your battery limit should be 20A per VESC, and charging ("battery current max" aka regenerative breaking) limit should be like 10A per VESC. (Which is still 2.5x higher than rated for the cells, but hey you have a small battery and breaking is important, just try to be easy on it to preserve longevity of the battery)

I wonder if it really was the BMS or something that cut off as you were trying to put too much amps into it.
```

---
## \#19 Posted by: rusins Posted at: 2019-04-17T21:39:47.790Z Reads: 119

```
Yeah you do have quite an interesting throttle curve :smiley: Maybe just set it to linear for the moment to keep things simple while testing :upside_down_face:
```

---
## \#20 Posted by: Halbj613 Posted at: 2019-04-17T21:42:40.569Z Reads: 119

```
Lion I think it can do 20 per motor I have it set at 30 because I am not exactly sure about the amount
```

---
## \#21 Posted by: Halbj613 Posted at: 2019-04-17T21:44:56.370Z Reads: 114

```
Yeah thought so it’s just that I am used to having a longer range on the throttle because I used to use a 4 speed remote for the cheap Chinese esc
Either way I am getting a focbox now in the Easter sale 2 for 400$
```

---
## \#22 Posted by: Saturn_Corp Posted at: 2019-04-17T21:55:02.726Z Reads: 112

```
You're gonna have to be more specific than that if you want to know the true amperage it can supply and know it's limits. 10s2p?samsung 30q's or something else? What does the label on the side say? If it's working now (minus brakes lol) you can't be too far off. Just better to know than to guess and potentially slowly degrade the pack, or maybe get more power out of it than you realize.
```

---
## \#23 Posted by: Halbj613 Posted at: 2019-04-17T21:56:36.556Z Reads: 109

```
It’s 10s2p Samsung 30q battery around 6 months old used for around 200 miles 
I think I can get 20 amps per motor
```

---
## \#24 Posted by: Halbj613 Posted at: 2019-04-17T21:57:34.844Z Reads: 99

```
So I should change max current to the original and put the throttle curve back to linear
```

---
## \#25 Posted by: Saturn_Corp Posted at: 2019-04-17T22:03:24.343Z Reads: 95

```
Yah that pack can do 40amps and burst a bit more. Might want to go down to 20 batt amps per motor but 30 should be ok as you have it set, it just won't be able to use all 30 per each motor (sound about right everyone?)
```

---
## \#26 Posted by: rusins Posted at: 2019-04-17T22:03:48.676Z Reads: 96

```
20 amps for battery max, and 10 amps for battery regen per Vesc. Motor current max and min can stay as is, it's safe for them to be higher because the vesc converts high voltage from the battery to low voltage for the motors.

(However, 40A per motor is quite a lot :smiley: I personally run mine at 30A, but then again you have higher KV motors, so if 40 feels good then power to ya :slight_smile: )
```

---
## \#27 Posted by: b264 Posted at: 2019-04-17T22:04:17.235Z Reads: 89

```
You should not use 260Kv motors on 10S voltage with 4.12 VESC.

Use 200Kv or lower motors.
```

---
## \#28 Posted by: rusins Posted at: 2019-04-17T22:04:51.131Z Reads: 89

```
It can do 30A per motor, but not at max speed which would make motor voltage = battery voltage. That's why there are motor settings separately from battery settings to begin with :slight_smile:
```

---
## \#29 Posted by: Halbj613 Posted at: 2019-04-17T22:05:15.874Z Reads: 91

```
Why is that
```

---
## \#30 Posted by: rusins Posted at: 2019-04-17T22:07:38.531Z Reads: 90

```
Oh shoot, you're right! 260 * 42 * 14/2 = 76440 eRPM which is too much :open_mouth:
```

---
## \#31 Posted by: rusins Posted at: 2019-04-17T22:12:41.931Z Reads: 91

```
VESC 4.12 has an eRPM limit of 60k, above which strange things can happen and you shouldn't be trusting your safety with it. eRPM is calculated by multiply motor Kv by voltage and then by motor poles divided by 2, which is usually 14/2 = 7. I just assumed you'd be fine with 10S, but after doing the math I see that you are over the limit. As b264 said, you should get lower Kv motors I'm afraid.

Edit: Then again you have your ERMP limited in settings, so maybe this isn't the cause of the problem. :thinking:
```

---
## \#32 Posted by: Saturn_Corp Posted at: 2019-04-17T22:19:47.482Z Reads: 82

```
He is ordering a unity, aren't those ok with something like 100k+ erpm? He can limit the erpm to 60k until he swaps the vesc out.
```

---
## \#33 Posted by: Halbj613 Posted at: 2019-04-17T22:21:05.354Z Reads: 86

```
Yes just ordered a shared one in the sale their 200$ each
```

---
## \#34 Posted by: Dirt_Bag Posted at: 2019-04-17T23:00:16.065Z Reads: 90

```
I am glad you safely bailed before a collision. I use longboard bumpers to protect the tips of my board from impact. they would easily cover up the chipped part of yours. here are 2 links for the same generic product. 1 from usa and 1 from china

https://www.ebay.com/itm/Skateboard-Deck-Protector-Bumpers-Bump-Longboard-Dance-Board-Crash-Rubber-Strip/253944671201?hash=item3b20482be1:m:m-wYxDqEyXDZi0UVdlvEvEw&amp;frcectupt=true

https://www.amazon.com/Skateboard-Guards-Longboard-Protection-Beginners/dp/B077CQBC33/ref=sr_1_1_sspa?keywords=longboard+bumper&amp;qid=1555541952&amp;s=gateway&amp;sr=8-1-spons&amp;psc=1

they are friction fit, and stay put extremely well
```

---
## \#35 Posted by: Halbj613 Posted at: 2019-04-18T06:46:33.271Z Reads: 83

```
thanks i am in the uk so not so practical for me
```

---
## \#36 Posted by: mynamesmatt Posted at: 2019-04-18T07:04:56.963Z Reads: 82

```
like @rusins said, bring your absolute max up to 130. you'll find that fixes a few issues
```

---
## \#37 Posted by: Halbj613 Posted at: 2019-04-18T15:20:11.083Z Reads: 73

```
Tried it didn’t work
```

---
## \#38 Posted by: Jinra Posted at: 2019-04-18T15:23:58.888Z Reads: 74

```
You should also leave max voltage back at default (57), don't change settings if you're not sure what they're for.
```

---
## \#39 Posted by: Halbj613 Posted at: 2019-04-18T16:18:57.228Z Reads: 72

```
K will that help
```

---
## \#40 Posted by: Halbj613 Posted at: 2019-04-19T08:10:31.202Z Reads: 65

```
done all this they still dont work is the problem with the motors battery or vesc
```

---
## \#41 Posted by: chaka Posted at: 2019-04-19T13:25:02.365Z Reads: 64

```
You have tiny battery problems mate. How strong we can brake depends entirely on how big our pack is. The max amount you can "regen" on a 2p pack is about 10 amps but you can only expect that on a partially discharged pack. If your pack is small the voltage will rise quickly when braking and trigger an over voltage.

 It would also be helpful to hear what gear ratio and wheels size you are running. A 270kv motor is like having really tall gears so if you are not using a proper ratio to bring the theoretical top speed down to a level better suited to a 10s2p battery you will have issues.
```

---
## \#42 Posted by: pjotr47 Posted at: 2019-04-19T13:52:03.266Z Reads: 64

```
Set your motor current max on 60A 

Motor current brake max on -60A
And your max current on 120A. 

Battery current max regen: -10A
I think if you go higher then then that your BMS will cut it off. 

That was the problem I think you had. 

Set your erpm limit on 58 000

And set your throttle curve both at 0% and in a linear line.
```

---
## \#43 Posted by: Halbj613 Posted at: 2019-04-21T20:47:13.692Z Reads: 53

```
abec11 97mm

16 to 36 ratio
```

---
## \#44 Posted by: Halbj613 Posted at: 2019-04-21T20:48:10.319Z Reads: 54

```
either way was using battery on a hub driven board and it got wet and producing nearly no power now so it is probably dead
```

---
## \#45 Posted by: chaka Posted at: 2019-04-23T13:36:27.456Z Reads: 53

```
Yeeww, board was set up as a screamer! With that set up you were pumping massive amounts of current when braking. A battery 3 times the size of yours would have still been struggling with that setup.  If you drop down to a 200kv motor the system will draw much less current.

You might be able to salvage the battery. If you have a multimeter you can check the voltage on your P groups and see if one of them is bad.
```

---
## \#46 Posted by: Halbj613 Posted at: 2019-04-23T15:59:36.126Z Reads: 48

```
I am upgrading to a 10s5p Samsung 30q battery from @Tinp123 (he's a really good builder with good prices) should that work ok with those motors a unity and that battery
```

---
## \#47 Posted by: chaka Posted at: 2019-04-23T17:46:35.519Z Reads: 46

```
No, that motor is still to high of a KV value for 10s. A 200kv motor is what you want.
```

---
## \#48 Posted by: Halbj613 Posted at: 2019-04-23T18:20:50.596Z Reads: 46

```
I thought a unity can handle up to 100000erpm
```

---
## \#49 Posted by: chaka Posted at: 2019-04-23T19:19:08.359Z Reads: 46

```
>  A 270kv motor is like having really tall gears 

What is your goal? Are you trying to build a death stick that can reach 50 mph or do you just want a practical board with a 20 to 30 mph top speed? If you want good brakes you need to change the ratio or the motor.
```

---
## \#50 Posted by: Halbj613 Posted at: 2019-04-23T19:21:39.002Z Reads: 47

```
Happy to change ratio have got some 40t pulleys for abec 
What good motor pulley could I get for Tb motors
```

---
## \#51 Posted by: chaka Posted at: 2019-04-23T19:29:40.063Z Reads: 45

```
A 14t motor pulley would work with the 40t but the board will still reach around 36-38 mph so it will be on the fast side. Ideal top speed for efficiency is around 25 mph.
```

---
## \#52 Posted by: Halbj613 Posted at: 2019-04-23T19:30:54.413Z Reads: 47

```
Around 35mph should be fine 

what about a 12t though

Also will that help with braking
```

---
## \#53 Posted by: chaka Posted at: 2019-04-23T19:33:59.661Z Reads: 44

```
I don't advise going lower than 14t with a 5htd tooth profile. You get less tooth engagement and the belt will strip.
```

---
## \#54 Posted by: Halbj613 Posted at: 2019-04-23T19:34:48.822Z Reads: 47

```
K thanks a lot do you know where in uk I can source that and what bore is Tb motors 8mm or 10mm
```

---
## \#55 Posted by: Halbj613 Posted at: 2019-04-23T20:14:42.028Z Reads: 44

```
Is there any way I could limit the motor to a certain amount of Kev or something
```

---
## \#56 Posted by: chaka Posted at: 2019-04-23T20:22:07.165Z Reads: 44

```
Probably 8mm.

The VESC is amazing but it won't change the resistance in your motor windings. Only way to change the KV on your motors is to rewind them with more turns on the stators.
```

---
## \#57 Posted by: Halbj613 Posted at: 2019-04-23T20:34:57.756Z Reads: 40

```
[quote="chaka, post:56, topic:90918"]
rewind them with more turns on the stators.
[/quote]
That’s a no

So what do you say I should do except scraping the motors
```

---
## \#58 Posted by: briman05 Posted at: 2019-04-23T20:48:01.361Z Reads: 36

```
I will second/third or forth what everyone has said and get motors with a lower kv.  Yes the unity can handle higher erpm however you are still running the risk of issues.

please read [this article](https://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125) about KV for each battery.  Only experienced builders/ riders should be messing with kv and battery and speed.
```

---
## \#60 Posted by: Halbj613 Posted at: 2019-04-23T21:47:37.662Z Reads: 29

```
The thing about that article is that it is based on a cell being on full charge most the time cells are 3.7v

So 8450/37 is 227kv which is t that far off a 260kv motor
Also couldn’t I limit it to 33v or so as then it would work with 260kv fine
```

---
## \#62 Posted by: b264 Posted at: 2019-04-23T22:04:17.400Z Reads: 28

```
[quote="Halbj613, post:61, topic:90918"]
<del>What </del><del>motor </del><del>do </del><del>you </del><del>suggest</del>
[/quote]

If "cheap" is your goal, get a KEDA 6364.  
If "good" is your goal, get a 6374 from @psychotiller  
For something in-between get a @torqueboards 6374 (for single-drive) or two @torqueboards 6355 for dual drive.  

Don't go over 200Kv.
```

---
## \#63 Posted by: Halbj613 Posted at: 2019-04-23T22:06:18.757Z Reads: 27

```
K so here’s is my fully composed thing

A unity can do 100000 erpm(agreed)
 
100000/7 poles is around 14200

14200/260 is around 54 

12s is 3.7*12 which is around 44(even at full charge 12*4.2 is around 50v)

So the unity and motor should all fit in together
```

---
## \#64 Posted by: b264 Posted at: 2019-04-23T22:07:18.622Z Reads: 25

```
[quote="Halbj613, post:63, topic:90918"]
A unity can do 100000 erpm(agreed)
[/quote]

What is your source for that?  I've heard that, but never seen proof.  I don't think the microprocessors are any faster than a VESC 4.12
```

---
## \#65 Posted by: Halbj613 Posted at: 2019-04-23T22:08:06.571Z Reads: 26

```
[quote="b264, post:62, topic:90918"]
two @torqueboards 6355
[/quote]

I have the larger 260kv version of these
```

---
## \#66 Posted by: Halbj613 Posted at: 2019-04-23T22:08:39.477Z Reads: 26

```
I have heard from quite a few people that this is so
```

---
## \#67 Posted by: b264 Posted at: 2019-04-23T22:08:49.366Z Reads: 26

```
No, you have the 260Kv version.  Everyone here is saying not to go over 200Kv.

The 260Kv motors would work great on 7S (29.4V max, 25.2V nominal)
```

---
## \#68 Posted by: Halbj613 Posted at: 2019-04-23T22:13:54.918Z Reads: 27

```
Here’s my source 

https://www.youtube.com/watch?v=ImhwnlukXNc

Found it on forum
```

---
## \#69 Posted by: Halbj613 Posted at: 2019-04-23T22:14:49.523Z Reads: 27

```
[quote="Halbj613, post:63, topic:90918, full:true"]
K so here’s is my fully composed thing

A unity can do 100000 erpm(agreed)

100000/7 poles is around 14200

14200/260 is around 54

12s is 3.7 *12 which is around 44(even at full charge 12* 4.2 is around 50v)

So the unity and motor should all fit in together
[/quote]

So this should be true
```

---
## \#70 Posted by: b264 Posted at: 2019-04-23T22:22:27.931Z Reads: 29

```
Do it, and then show us how.  We're giving you answers, and you are rejecting them.  You should show us how to do things a different way. 

*protip: To put an asterisk in markdown, you need to put a backslash before it.*
```

---
## \#71 Posted by: Halbj613 Posted at: 2019-04-23T22:23:56.137Z Reads: 26

```
Oh thanks for help will try with these motors if they don’t work I will switch
```

---
## \#72 Posted by: rusins Posted at: 2019-04-23T22:31:46.319Z Reads: 26

```
TB motors have a 8mm shaft.

https://www.beltingonline.com/timing-pulleys-bars-272/htd5-pulleys-285/?zenid=f2e6ii4ukptpm8c9krvjdmr433
This is a place I know of to get custom pulleys in the UK. I also get all my belts from them because they're stronger than the default ones TorqueBoards give.

What width pulleys do you have? I have 2x 12mm 14T 5M pulleys which I'd like to trade with someone for a higher tooth count (I want slightly more speed).
```

---
## \#73 Posted by: J95hicks Posted at: 2019-04-23T23:12:09.532Z Reads: 27

```
Hey, sorry to jump in on your thread but I had a similar issue and i hate making multi threads(unless i need too, plz say so).. posted here, https://www.electric-skateboard.builders/t/vesc-faq-regen-braking-configuration-bldc-tool-brake-force/353/50?u=j95hicks. But Im running dual 170kv on 12s8P setup,motor min -75, bat min -20.... maybe respond in the other thread, so i dont clog up this guys thread? but Thx
```

---
## \#74 Posted by: Halbj613 Posted at: 2019-04-24T06:34:05.404Z Reads: 24

```
How do you calculate belt size
```

---
## \#75 Posted by: Halbj613 Posted at: 2019-04-24T06:47:20.476Z Reads: 25

```
Looking to buy motor pulley 

am getting some 3D printed wheel ones
```

---
## \#76 Posted by: Halbj613 Posted at: 2019-04-24T19:29:50.732Z Reads: 23

```
So after lots of research it seems the unity similar to other newer vesc such as vesc 6. Can handle 100000 erpm
And as I think I calculated before

[quote="Halbj613, post:69, topic:90918"]
A unity can do 100000 erpm(agreed)

100000/7 poles is around 14200

14200/260 is around 54

12s is 3.7 *12 which is around 44(even at full charge 12* 4.2 is around 50v)

So the unity and motor should all fit in together
[/quote]

The 12s should be fine on a 260kv motor

If it does not work I will switch up my motors for lower Kv ones

While I am using this with my flipsky 4.12 I will try limiting the maximum voltage(would that work)

Thank you to everyone for the help 

Again the forum saved me
```

---
