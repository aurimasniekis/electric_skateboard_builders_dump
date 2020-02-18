# Absolutely not strong enough - what went wrong?

### Replies: 53 Views: 2028

## \#1 Posted by: davidbonde Posted at: 2018-04-27T17:41:44.472Z Reads: 402

```
I made this one... 

Battery: Samsung 18650 6s6p
Motor: Racestar 5065 140kv 
Focbox 

It can barely move it self. And a person on it... forget it. 

Have I overlooked anything? Shouldn't it be working? Can I tweek anything in bldc tool to make it work? What might need to be upgraded?  

![IMG_6694|666x500](upload://5pLtwIrUqyoE1zMGjVc0cPEyV6L.JPG)

This is full throttle 

https://youtu.be/a8rNqvD6CzY
```

---
## \#2 Posted by: RedEagle Posted at: 2018-04-27T17:42:24.403Z Reads: 384

```
Post your vesc settings.
```

---
## \#3 Posted by: Exiledd_Top Posted at: 2018-04-27T17:42:31.966Z Reads: 382

```
[quote="davidbonde, post:1, topic:53673"]
140kv
[/quote]

[quote="davidbonde, post:1, topic:53673"]
6s6p
[/quote]
 kv to low for the voltage that it's given that thing won't go past 5mph that as well motor to small and it's single drive on pnumatics
```

---
## \#4 Posted by: louwii Posted at: 2018-04-27T17:42:39.628Z Reads: 370

```
Single 5065?  That's way too small isn't it?

EDIT: I think @Exiledd_Top found the problem.
```

---
## \#5 Posted by: davidbonde Posted at: 2018-04-27T17:45:44.716Z Reads: 355

```
[quote="Exiledd_Top, post:3, topic:53673"]
and it’s single drive on pnumatics
[/quote]

I took one motor off my evolve bamboo and it was fine. Took me up pretty steep hills no problem.
```

---
## \#6 Posted by: Exiledd_Top Posted at: 2018-04-27T17:47:00.968Z Reads: 352

```
that's a esc vs a vesc,  dout it will work out u will burn that evolve motor out
```

---
## \#7 Posted by: davidbonde Posted at: 2018-04-27T17:50:38.850Z Reads: 351

```
![IMG_6695|666x500](upload://su1pK7XUcAQccz7OQCYr352yifU.JPG)
```

---
## \#8 Posted by: b264 Posted at: 2018-04-27T17:52:53.465Z Reads: 340

```
[quote="davidbonde, post:5, topic:53673"]
I took one motor off my evolve bamboo and it was fine. Took me up pretty steep hills no problem.
[/quote]

I rode my Carbon GT on one motor while the ESC was half-broken and it also was fine.  The performance was extremely underwhelming and you had to run in GT mode, but it worked fine and went up hills.  That's 10S with a single 150kv 5065
```

---
## \#9 Posted by: davidbonde Posted at: 2018-04-27T17:53:12.188Z Reads: 329

```
? 
I mean that I tested to see if a single motor could run pnumatics by taking the belt of one of the motors on my evolve. Worked fine. 

I am thinking the kv here could be the problem ?
```

---
## \#10 Posted by: b264 Posted at: 2018-04-27T17:53:34.860Z Reads: 317

```
We need to see the screen to see if your PPM input is going all the way to 100% as well
```

---
## \#11 Posted by: davidbonde Posted at: 2018-04-27T17:53:49.586Z Reads: 314

```
So maybe its the 6s thats the problem?
```

---
## \#12 Posted by: strattos Posted at: 2018-04-27T17:53:51.845Z Reads: 307

```
Yup either he needs a higher KV motor or a higher voltage battery.

Also what kind of gearing is he running? It doesn't look like the motor is even spinning that fast tho for 100% throttle.
```

---
## \#13 Posted by: Lumaci Posted at: 2018-04-27T17:54:35.193Z Reads: 298

```
140KV and 6S sounds a bit odd, for 6S i would go with something like 270KV

Also 5065 wont give you enough torq to go much faster.
```

---
## \#14 Posted by: RedEagle Posted at: 2018-04-27T17:55:00.685Z Reads: 288

```
If I were you I would set the erpm limit to 60k and -60k. 100k is fine on better hardware(vesc6).
```

---
## \#15 Posted by: davidbonde Posted at: 2018-04-27T17:59:20.342Z Reads: 290

```
I will make a video a little later.
```

---
## \#16 Posted by: davidbonde Posted at: 2018-04-27T18:00:22.922Z Reads: 286

```
Will try that.
```

---
## \#17 Posted by: RedEagle Posted at: 2018-04-27T18:01:11.906Z Reads: 281

```
Change your motor (to 63xx) and your gearing.
```

---
## \#18 Posted by: SORRENTINO Posted at: 2018-04-27T18:04:00.525Z Reads: 274

```
Your battery cutoff is above 6s at full charge :thinking:
```

---
## \#19 Posted by: davidbonde Posted at: 2018-04-27T18:04:15.202Z Reads: 277

```
That just means new motor mount as well. Hope I can do something without changing all that. If at all possible
```

---
## \#20 Posted by: davidbonde Posted at: 2018-04-27T18:05:05.600Z Reads: 274

```
aahhh.... will look in to that
```

---
## \#21 Posted by: SORRENTINO Posted at: 2018-04-27T18:08:44.992Z Reads: 245

```
@Deckoz 

10 char
```

---
## \#22 Posted by: Zimbombe Posted at: 2018-04-27T18:09:59.545Z Reads: 248

```
Nah thats just not true, i have the same Setup but use a Fvt Esc and get around 21 Km/h
```

---
## \#23 Posted by: thisguyhere Posted at: 2018-04-27T18:12:25.910Z Reads: 260

```
when you say samsung 18650, are they 25r or 30q, or something else?

try upping batt max to 100a since you're running 6p (20a * 6 = 120a continous), and motor max to 100a as well.
```

---
## \#24 Posted by: Ackmaniac Posted at: 2018-04-27T18:13:02.637Z Reads: 262

```
here is your problem
![image|690x441](upload://s8LU7UvoksCzP0JtE33d7FsjwAJ.jpg)
You set the battery cutoff start and end for a 10S Battery. but you only have a 6S.

start should be 3.0 a cell which is 18V in your case. 
And end 2.8V a cell which is 16.8V in your case.

That should do the trick. Means you were riding with the lowest possible current (1A as default) because the Vesc thought your battery is already completely dead.
```

---
## \#25 Posted by: thisguyhere Posted at: 2018-04-27T18:13:16.834Z Reads: 254

```
bingo, i was just typing this.
```

---
## \#26 Posted by: Deckoz Posted at: 2018-04-27T18:13:21.011Z Reads: 252

```
6s6p 30q is 20a* or 120a

You have 25a set.

22.1v nominal * 25a = 552watts.

Suggest setting your batt max to 60 or 70 for a single drive

22.1v nominal * 60 = 1325w


Also what @Ackmaniac and @SORRENTINO  said..fix your cuttoffs
```

---
## \#27 Posted by: Exiledd_Top Posted at: 2018-04-27T18:20:34.336Z Reads: 247

```
[quote="Zimbombe, post:22, topic:53673"]
Fvt Esc
[/quote]

again he's using vesc,  he said he tried on evolve those are esc's but that set up that he made is vesc , esc's done care and will plow through there amp hungry and could beat the crap out of them stressing them but on vesc ain't gana happen endless u run vesc6
```

---
## \#29 Posted by: davidbonde Posted at: 2018-04-27T19:02:49.823Z Reads: 238

```
30q - thanks will try that.
```

---
## \#30 Posted by: Fiori Posted at: 2018-04-27T19:24:58.093Z Reads: 239

```
> That’s a esc vs a vesc, dout it will work out u will burn that evolve motor out

What? This makes no sense....

The single motor goes faster on the evolve because the evolve is running at 10s(optimal for that kv). (well that and the incorrect vesc settings listed above). You definitely wont burn out the motor using it on a vesc... plenty of people have used 5065 motors on vesc....

I suggest you re-wire that battery to something like 10s3p and you may be a little happier. Or just get a higher kv motor
```

---
## \#31 Posted by: Exiledd_Top Posted at: 2018-04-27T19:29:29.209Z Reads: 230

```
i think I said it wrong let me rephrase,  it's single drive 5065 on AT wheels big,  if u use a esc  like evolve it will stress  more the small motor than the esc I know because I have fried a single motor on a esc. Now if it's a vesc on single small motor it will stress  more the vesc and will likely fry dvr  I know as well because I have fried 2 maytech vesc on single drive
```

---
## \#32 Posted by: Fiori Posted at: 2018-04-27T19:31:26.923Z Reads: 226

```
Evolve esc only puts 32.5 amps to each motor regardless of how many are connected. I guess i just don't know what you are saying.
```

---
## \#33 Posted by: Exiledd_Top Posted at: 2018-04-27T19:34:39.331Z Reads: 222

```
sure am staying out of this one then lol
```

---
## \#34 Posted by: davidbonde Posted at: 2018-04-27T20:12:05.051Z Reads: 227

```
@Ackmaniac @Deckoz @thisguyhere @SORRENTINO

Thanks guys. The battery cutoff seemed to be exactly the thing. Changed it to 18 / 16,8 and now I am flying! What a rookie mistake. 

Now it takes me to 20 km/h / 12.5 mph on flat ground no problem. Just as I wanted it to. This build is for my 12 years old daughter so it will be perfect for her I guess (I will not Allow her to go faster). 

You will all get a big fat kiss if I ever see you for real :) 

https://youtu.be/ZC3F-H5WpTc

I must realize that I do not completely understand those bldc settings in depth. Must do some studying in that area. 

Maybe you can help me a little of the way. I want it to be a little less reactive/agressive when accelerating. Which settings should I play with in what direction? Also, if she wants more speed down the road, would it be the motor max I should play with there? 

These are the settings as they are now:

![IMG_6700|666x500](upload://zI83wkPVMOxdV1LzmdOolv5I3u7.JPG)
```

---
## \#35 Posted by: Deckoz Posted at: 2018-04-27T20:14:07.971Z Reads: 206

```
Ok if this is for your daughter.

Set motor max to 20amps. And leave your battery amps at 25

Also if you are running bldc. Calculate the erpm to limit the speed,and then set an erpm limit.(somewhere around 12k-30k erpm or lower. Since your on 140kv)

If she wants more speed or acceleration down the road set the erpm max back to -60k +60k.and then up the motor max 5-10 amps at a time until about 60 amps.. let her get used to it after....
```

---
## \#36 Posted by: davidbonde Posted at: 2018-04-27T20:21:22.374Z Reads: 207

```
Cool thanks @Deckoz - we will play with it the coming days.
```

---
## \#37 Posted by: Ackmaniac Posted at: 2018-04-27T21:03:22.587Z Reads: 207

```
If the maximum speed you get right now isn't fast enough then you have a couple of options.
- higher battery voltage (eg a 10S battery)
- higher motor kv
- less gearing 
- bigger wheels

for a smoother acceleration  you can lower the motor max or go with one of my modded firmwares to define a throttle curve. Vedders latest official also has the adjustable throttle curve.
```

---
## \#38 Posted by: laurnts Posted at: 2018-04-27T21:25:35.196Z Reads: 207

```
This is obviously have nothing to do with motor too small when it doesnt even move at all. your battery cut off is way too high. It's 10S battery cut off setting when you're running 6S setup.
```

---
## \#39 Posted by: davidbonde Posted at: 2018-04-29T10:16:41.371Z Reads: 194

```
Adjusted the Motor max to 20a and the batt max to 25a and that is perfect for Her. Smooth acceleration that she can control. 

Also had to adjust the Motor min (regen) to -20 and the Batt min (regen) to 8 to get forgiving braking. 

Everything works great now and the Daughter are happy!

Thanks for the help.

https://youtu.be/it698FOnmlo
```

---
## \#40 Posted by: Deckoz Posted at: 2018-04-29T15:00:42.305Z Reads: 178

```
Nice man! @davidbonde 

Glad you got it working,haha she looked about as excited as the first time my wife rode.

Anyway since it's your baby girl, I know she probably won't go fast, but at least give her some gloves with that helmet so she can catch herself if she gets a little pebble. Other pads add as you see fit(if you give her more speed eventually, start with knees). But get that girl in some gloves, and hope she has fun!!
```

---
## \#41 Posted by: davidbonde Posted at: 2018-04-29T15:32:37.158Z Reads: 171

```
Yahh you are right - I will get her some gloves.

We took a 6 mile cruise today. She was leading the speed, and it was a solid 7 mph cruise :) Lets see what happens when she get more rinding time.
```

---
## \#42 Posted by: Eboosted Posted at: 2018-04-29T16:53:42.048Z Reads: 162

```
I can't wait for my baby to grow up to come along with me to ride around the world.
```

---
## \#43 Posted by: davidbonde Posted at: 2018-04-29T19:24:17.577Z Reads: 153

```
Magic happens when we go for some father - daugther time on the boards together. Finally we fund something that we both enjoy doing. That makes a huge difference.
```

---
## \#44 Posted by: davidbonde Posted at: 2018-05-16T12:32:08.933Z Reads: 149

```
[quote="Ackmaniac, post:37, topic:53673"]
If the maximum speed you get right now isn’t fast enough then you have a couple of options.

higher battery voltage (eg a 10S battery)
higher motor kv
less gearing
bigger wheels
[/quote]

Thanks @Ackmaniac. Just to be completely sure. So upping the motor max in settings won't give me more topped only more boost - right? (@Deckoz?) Only the things you mention here will give me more top speed.
```

---
## \#45 Posted by: Deckoz Posted at: 2018-05-16T12:44:51.990Z Reads: 146

```
Well it depends..

Upoing motor max only gives more acceleration. As at higher duty cycles, the amps with be more in line with bsttery max than motor max.

Your battery is 6s6p, and can support 120 battery amps, you could try upping your battery amps to allow for more watts to flow. You could he hitting a speed limit because 20a battery max right now is only providing around 440watts

Battmax:
20A * 22.1v Nominal = 440W
40A * 22.1V Nominal = 884W

If you set an erpm limit like I previously mentioned to limit speed. You can put the erpm limit back up to 60k if it was lower. 


It would first help to know what your current gearing is, and the max speed you are able to get to, to see if you are already meeting the speed potential of your setup, with load on it(your daughter).
```

---
## \#46 Posted by: davidbonde Posted at: 2018-05-16T13:06:58.700Z Reads: 131

```
Thanks..
I am actually thinking of my own board. Just didn't want to create a new thread :) 

On that I have tried to up the motor max. from 40 to 60. Fund that I got more boost but not more top speed. I don't like the added boost, I just wanted to see if upping the motor max gave me more top speed. It gives me 29 mph right now, with is actually fast enough for me. Just wanted to see if it has more in it.

The battery is a 10s6p with 30q. The battery max is currently at 25 and the gearing is 16/60 with pneumatics.
```

---
## \#47 Posted by: professor_shartsis Posted at: 2018-05-16T13:22:14.832Z Reads: 130

```
[quote="davidbonde, post:46, topic:53673"]
It gives me 29 mph right now
[/quote]

@davidbonde here is a chart showing the predicted performance you’ll get with (1) 140kv motor, 200mm tire, 16/60 (3.75:1) gear ratio, 25a bat limit, 40a motor limit, 38v battery:

https://image.ibb.co/cAK3qd/EDCC59_B4_1_DA6_4852_B657_DF8_DBE744_A81.jpg

^if you take a look at the yellow line, bottom left chart (net thrust pounds - thrust minus wind drag), it shows ~29mph top speed (as you reported) and about 23lbs peak vehicle thrust.
```

---
## \#48 Posted by: davidbonde Posted at: 2018-05-16T13:41:00.099Z Reads: 120

```
Cool - I will confuse it further :) 
My board is: dual 190kv motor. 152mm tire. 16/60 gear ratio. :) Is there a chart for that as well?
```

---
## \#49 Posted by: professor_shartsis Posted at: 2018-05-16T13:51:25.852Z Reads: 124

```
[quote="davidbonde, post:48, topic:53673"]
Cool - I will confuse it further :slight_smile:

My board is: dual 190kv motor. 152mm tire. 16/60 gear ratio. :slight_smile: Is there a chart for that as well?
[/quote]

here’s the one for (2) 190kv, 152mm tire, 16/60 ratio, 38v battery, 40a motor limit, 25a battery limit per motor:

https://image.ibb.co/jT4xGJ/36959915_A8_E3_43_B5_8_A16_A442_B0_FA7_DDA.jpg

predicted is ~44lbs peak thrust and ~30-33mph top speed

the back emf voltage from the rotor magnets exceeds your pack voltage at about 33mph so you can’t go any faster than this unless you lower your gear ratio. (red & yellow lines, top left chart)
```

---
## \#50 Posted by: professor_shartsis Posted at: 2018-05-17T00:55:29.862Z Reads: 106

```
[quote="davidbonde, post:46, topic:53673"]
I just wanted to see if upping the motor max gave me more top speed
[/quote]

@davidbonde about more top speed... here is a comparison chart first showing upping your settings from 25a bat & 40a motor limit to 60a bat & 80a motor limit, next showing switching your gearing from 3.75:1 to 2:1, which gives ~50mph top speed & 47.5lbs peak vehicle thrust:

https://image.ibb.co/hZZ7Jy/F70_AC68_A_E9_E3_4_AEE_BFB4_DB9_C6_B45_F37_A.gif

...both steps lower your electrical to mechanical conversion efficency...
```

---
## \#51 Posted by: davidbonde Posted at: 2018-05-17T06:55:10.683Z Reads: 86

```
This is kinda cool but also a bit confusing for a electrical novice like myself. 
I am correct if I get out of it that upping motor and bat limit would not give me much, but changing the gearing would give me a lot? 

[quote="professor_shartsis, post:50, topic:53673"]
…both steps lower your electrical to mechanical conversion efficency…
[/quote]
Is that good or bad or indifferent?
```

---
## \#52 Posted by: professor_shartsis Posted at: 2018-05-17T11:55:48.083Z Reads: 88

```
[quote="davidbonde, post:51, topic:53673"]
This is kinda cool but also a bit confusing for a electrical novice like myself.

I am correct if I get out of it that upping motor and bat limit would not give me much, but changing the gearing would give me a lot?
[/quote]

@davidbonde step 1 in the animation shows ~doubling the motor and battery amp limits which will ~double your peak thrust, and in turn ~double your peak acceleration and peak power, but it doesn’t really alter your top speed. step 2 shows the combined effects of upping the current limits AND lowering the gear ratio... if you look at the red line, bottom left chart, doing both of these things together will give you roughly the same thrust/acceleration you had initially, but with ~20mph greater top speed. unfortunately doubling the motor amps and acceleration quadruples the ohmic heating in the motor, which lowers the efficiency (yellow line, top middle chart and green line, bottom right chart). if you were to not increase the current limits but only change the gearing, you’d have enough power there for about 40mph (see top middle chart in the first 190kv chart) if you lowered the gearing ratio (though you wouldn’t want to go as low as 2:1 without increasing the amp limits), but lowering the gear ratio without upping the current limits will lower your peak thrust and acceleration proportionately, so you could end up going 40mph, but you would accelerate more slowly than you do now. lowering the gear ratio and upping the current limits together gives you more top speed without sacrificing acceleration, but at full throttle your motors will get hotter more quickly and your range would be a bit diminished due to the lower efficiency.
```

---
## \#53 Posted by: davidbonde Posted at: 2018-05-17T12:52:09.053Z Reads: 74

```
This is great @professor_shartsis.  Thank you for taking the time to cut it into cardboard for me. It makes sense. It would be pretty easy for me to play with, if I find the top speed to little in the future. I then just need new motor pullys and belts. Right now I am ok happy with the 27-29 mph I have. But who knows :) It is nice to see I have the opportunity.
```

---
## \#54 Posted by: SkaterBoy58 Posted at: 2018-06-26T07:49:26.914Z Reads: 60

```
@professor_shartsis  Can you please  link to that spreadsheet at all   ?  Cheers
```

---
