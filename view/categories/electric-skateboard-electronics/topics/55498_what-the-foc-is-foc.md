# What the Foc is FOC?

### Replies: 44 Views: 2560

## \#1 Posted by: GXwagon Posted at: 2018-05-15T00:48:04.332Z Reads: 356

```
Hi there, 

I would like to know what FOC is and what it means to run your board in FOC. The more details the better.

Cheers!

UPDATE: Here is the For Dummies version for anyone looking for the same answer I was. Feel free to read down the post for more technical information. People have provided some great links and info.

Comparing FOC to BLDC could be like comparing a 4-stroke to a 2-stroke or an on/off switch to a dimmer switch. BLDC is like an on/off switch when providing power to the motor. FOC is more like a dimmer switch when providing power to the motor. Very much like your 4-stroke motor, FOC is smoother and quieter and like your 2-stroke motor, BDLC can provide more torque but is louder and more rock and roll.

FOC will accelerate faster at low RPMs because it manipulates the torque directly.
BLDC will accelerate faster at higher RPMs because of the bursts(on/off switch).

BLDC has a more raw feel to it. FOC is smoother and more refined.

FOC will lower your top speed a small amount.
```

---
## \#2 Posted by: b264 Posted at: 2018-05-15T00:48:33.690Z Reads: 351

```
[Field Oriented Control](https://en.wikipedia.org/wiki/Vector_control_(motor))
```

---
## \#3 Posted by: GXwagon Posted at: 2018-05-15T00:49:27.908Z Reads: 349

```
Sounds very technical... What does it do?
```

---
## \#4 Posted by: Deckoz Posted at: 2018-05-15T00:50:08.226Z Reads: 347

```
[quote="GXwagon, post:3, topic:55498, full:true"]
Sounds very technical… What does it do?
[/quote]

Click the link and see. It's a surprise
```

---
## \#5 Posted by: GXwagon Posted at: 2018-05-15T00:55:48.862Z Reads: 330

```
I did... Honestly I got past the first paragraph and gave up... I scanned the rest and didn't see any words I recognized. 

I can see it has something to do with torque management. 

I have heard all kinds of different stories of what it can do like make your board quieter. All I know is it sounds FOCing cool.

It would be great if someone could treat me as if I am their learning impaired nephew and break it down in a way anyone can understand. If you where selling a bag of FOCs to me how would you break it down for me and what would be the benefits. The KISS version.

I apologize ahead of time if my question offends anyone.
```

---
## \#6 Posted by: Deckoz Posted at: 2018-05-15T01:01:28.907Z Reads: 325

```
Once you read that..

https://en.m.wikipedia.org/wiki/Counter-electromotive_force

And

https://en.m.wikipedia.org/wiki/Brushed_DC_electric_motor


"BLDC" or Counter electromotive force timing control. Uses a sequence of phase pairs with timing to move the motor in a direction, not all phases have current running through them at once. This means the FETs open and close and burst, bursts are loud

"FOC" or field oriented control, has syncronous power through all the phases like AC but instead of a sine wave it is trapezoidal. Torque is modulated with constantly flowing current, as the FETs are always open with modulated gates, making it quieter.

Now as my dad told me when I was young, you can read right? Figure it out :) search is in the top right broski.
```

---
## \#7 Posted by: professor_shartsis Posted at: 2018-05-15T01:06:25.523Z Reads: 297

```
here is some information from a different discussion:
[quote="professor_shartsis, post:13, topic:26049, full:true"]
with BLDC, the current plot is “trapezoidal” and with FOC the the current plot is “sinusoidal”…

source: http://www.galilmc.com/news/drives-motion-controllers/trapezoidal-vs-sinusoidal-brushless-servo-amplifiers

“_Trapezoidal vs. Sinusoidal Commutation_

_Trapezoidal commutation is the most cost effective way of controlling a brushless servo motor.  It is perfect for higher speed applications and applications where the motor and mechanics will eliminate the torque ripple that occurs during switching current from one phase to the next.  Hall sensors are required for Trapezoidal commutation._

_Sinusoidal commutation is great for lower speed, direct drive or linear motor applications where the torque ripple of the motor phases needs to be minimized.  Since the current to the motor phases are weighted as sine waves, the torque going through the motor is smooth and has minimal ripple. It also allows the mechanics to be simplified because Hall sensors can be eliminated.”_
[/quote]

http://pubs.sciepub.com/ajeee/4/6/3/bigimage/fig2.png

http://www.orientalmotor.com/images/stepper-motors/5-phase-stepper-motors-rkii-low-vibration.jpg
```

---
## \#8 Posted by: Lionpuncher Posted at: 2018-05-15T01:41:19.930Z Reads: 265

```
Hey dude, 
@Deckoz isn't leading you astray. It's totally worth the challenge to wrap your head around some of the technical info involved with building a wicked slasher. For me, this took months of reading and studying all the builds and asking folks about why they did what they did. I promise it's not  as boring as it sounds. You tube has some good vids as well. 
Good luck man. :slightly_smiling_face:
```

---
## \#9 Posted by: RazzleDazzle Posted at: 2018-05-15T01:55:55.178Z Reads: 258

```
So would bldc make that whiney sound compared to FOC?
```

---
## \#10 Posted by: Deckoz Posted at: 2018-05-15T02:00:10.011Z Reads: 251

```
Yea... But FOC under heavy load(hi torque demand) screams too. But during normal cruising, it's just a wirrrr. Not a whine(like that AC light ballast sound that bldc makes)
```

---
## \#11 Posted by: GXwagon Posted at: 2018-05-15T15:51:01.802Z Reads: 215

```
Wow man. Fantastic answer. Well explained and visual. Explaining technical things in an easy to understand way is a talent, it's hard to do as you can see by the previous responses. Great Job and thank you @professor_shartsis !
```

---
## \#12 Posted by: GXwagon Posted at: 2018-05-15T15:54:58.761Z Reads: 206

```
@Lionpuncher I agree with you and ill get there once I begin my build over the winter. For now I just wanted a simple explanation which @professor_shartsis did fairly well.  If Neil DeGrasse Tyson can explain astrophysics to children and Texans then someone should be able to provide a similar type explanation of FOC to me. :slight_smile:
```

---
## \#13 Posted by: professor_shartsis Posted at: 2018-05-15T15:56:25.300Z Reads: 211

```
@GXwagon thanks, though the only part i actually wrote myself was this:

[quote="professor_shartsis, post:7, topic:55498"]
with BLDC, the current plot is “trapezoidal” and with FOC the the current plot is “sinusoidal”…
[/quote]

the rest of the explanation was sourced from the link and pictures included.
```

---
## \#14 Posted by: GXwagon Posted at: 2018-05-15T15:58:10.274Z Reads: 196

```
@professor_shartsis  "If you want to make and apple pie from scratch you must first create the universe"
```

---
## \#15 Posted by: professor_shartsis Posted at: 2018-05-15T16:12:59.232Z Reads: 187

```
@GXwagon i’d compare FOC to somehow making the explosions in a car’s engine a little “gentler” — you lose some power but the car runs smoother and more quietly.
```

---
## \#16 Posted by: Deckoz Posted at: 2018-05-15T16:44:41.240Z Reads: 189

```
Bldc isn't trapezoidal, it is stepped pwm current

The BackEMF is trapezoidal.

FOC is Trapezoidal or Sine, for both the current and BackEMF...
```

---
## \#17 Posted by: professor_shartsis Posted at: 2018-05-15T16:49:48.991Z Reads: 178

```
https://youtu.be/szgVUfyX8JM
```

---
## \#18 Posted by: Deckoz Posted at: 2018-05-15T16:58:13.871Z Reads: 176

```
Insta spin, while some of the libraries are in the VESC project. Requires sensors, instaspin libraries are only used in Sensored BLDC. 

Pure BLDC is PWM counter electromotive timing control. Go look at the repo.
```

---
## \#19 Posted by: GXwagon Posted at: 2018-05-15T17:03:42.207Z Reads: 177

```
Okay let me try this simple explanation thing now that I have heard some responses. 

Comparing FOC to BLDC could be like comparing a 4-stroke to a 2-stroke or an on/off switch to a dimmer switch. BLDC is like an on/off switch when providing power to the motor. FOC is more like a dimmer switch when providing power to the motor. Very much like your 4-stroke motor, FOC is smoother and quieter and like your 2-stroke motor, BDLC can provide more torque but is louder and not as smooth.

Close?
```

---
## \#20 Posted by: Deckoz Posted at: 2018-05-15T17:06:21.756Z Reads: 172

```
Yep pretty much it... 

But FOC can create more accurate torque vectoring at lower RPMs, and is more efficient. So FOC will accelerate faster at low RPMs because it can manipulate the torque directly. Where bldc will accelerate faster at higher rpms because the bursts.
```

---
## \#21 Posted by: Lionpuncher Posted at: 2018-05-15T17:07:29.236Z Reads: 159

```
I'd say that comparison is fairly apt. 
BLDC has a more raw feel to it. FOC is smoother and more refined. 
It is said to be a bit harder on the vescs in FOC than in BLDC. My controllers have never had an issue with either. I think it's just more important that you program your controller correctly.
```

---
## \#22 Posted by: professor_shartsis Posted at: 2018-05-15T17:49:09.687Z Reads: 150

```
& FOC can lower your top speed by a couple mph...
```

---
## \#23 Posted by: Hummie Posted at: 2018-05-15T18:27:38.965Z Reads: 144

```
is the top speed lower in foc due to lower power?  id have thought the speed limit was due to the motor design and pack voltage.  is the speed lower in foc doing a no-load test? ive only ever run foc and never done a no-load test in bldc.  easy test
```

---
## \#24 Posted by: professor_shartsis Posted at: 2018-05-18T22:05:31.402Z Reads: 129

```
[quote="Hummie, post:23, topic:55498"]
is the top speed lower in foc due to lower power?  id have thought the speed limit was due to the motor design and pack voltage.  is the speed lower in foc doing a no-load test? ive only ever run foc and never done a no-load test in bldc.  easy test
[/quote]

Looks like Mr. Vedder answered this question over at Vesc-Project.com:

benjamin ( https://www.vesc-project.com/node/218 ): _“Pure FOC compared to pure block commutation gets slightly lower top speed as the sine voltages would be distorted otherwise as they are in block commutation. Also, the VESC is limited to 95 % modulation and the other ESC might come a bit closer to 100%.”_
```

---
## \#25 Posted by: Deckoz Posted at: 2018-05-18T22:19:49.799Z Reads: 144

```
[quote="Hummie, post:23, topic:55498"]
the top speed lower in foc due to lower power
[/quote]

No.

FOC:
Imagine you have a wind mill, and you have three tubes with air coming out of them. The air is the current, the current can increase, and the tube exits stays the same size, because all three are modulating at once.

Bldc: 
Imagine the same scenario, but instead of all three tubes having air come out of them, pairs of 2 have the equivalent current coming out of them, in a 6 step sequence. Since the same amount of current is coming out of two tubes, as three for FOC, the velocity coming from two is faster.

Basically in really simple easy to understand terms. The same current, in the same rotation time span, is burst out of two tubes, then two different tubes etc. The result is the higher air velocity setup spins fast. But is less efficiently.
```

---
## \#26 Posted by: professor_shartsis Posted at: 2018-05-18T22:42:59.388Z Reads: 136

```
here’s a chart I found showing BLDC “block commutation” @ 100% duty cycle:

https://image.ibb.co/jSoFrT/A4700_E27_81_A1_43_FF_9_E06_52_BA63_C5_C793.jpg

^notice with BLDC only 2 of the phases have current at any given time and these are not “sine waves”

the reason I called this “trapezoidal” previously rather than “block” is, due to the inductance of the motor windings, the current does not in fact rise and fall instantly, giving a slight slope to the sides of the blocks, making them in reality appear slightly “trapezoidal...”

here’s a different chart comparing the “block” commutation with “sinusoidal” commutation:

https://performance-motion-devices.s3.amazonaws.com/uploads%2Fbadcca93-5c33-4c3f-b031-fe068df58275%2FF5_Commutation+Schemes+-+final.jpg
```

---
## \#27 Posted by: professor_shartsis Posted at: 2018-05-19T00:54:18.960Z Reads: 125

```
here’s my attempt at an animated gif of the current plot for comparison:

https://image.ibb.co/c6wGgT/F2_DDACDF_898_A_4_E8_F_97_BB_0_B6_C3_CAB7094.gif
```

---
## \#28 Posted by: Deckoz Posted at: 2018-05-19T01:01:23.387Z Reads: 126

```
[quote="professor_shartsis, post:26, topic:55498"]
block
[/quote]


![Screenshot_13|295x291](upload://imCHGITCRVpY8KA7xr22tb7sZUM.png)

PWM
```

---
## \#29 Posted by: squishy654 Posted at: 2018-05-19T02:47:57.785Z Reads: 122

```
![you-dont-go-anywhere-when-you-say-peekaboo|367x417](upload://rLMd85qjAN6IpBOH5Guhhxm3sv5.jpg)
```

---
## \#30 Posted by: Lionpuncher Posted at: 2018-05-19T05:49:10.294Z Reads: 116

```
:joy: :joy: :joy:
10 characters.
```

---
## \#31 Posted by: Naysh Posted at: 2018-05-19T16:09:30.364Z Reads: 107

```
A rule of thumb is to use BLDC on all VESCs 4.12 except for the Focbox. Only Focboxes and  VESC 6 are capable of reliably running FOC.
```

---
## \#32 Posted by: squishy654 Posted at: 2018-05-19T16:17:16.204Z Reads: 109

```
[quote="Naysh, post:31, topic:55498, full:true"]
A rule of thumb is to use BLDC on all VESCs 4.12 except for the Focbox. Only Focboxes and  VESC 6 are capable of reliably running FOC.
[/quote]
![hogwashmeterred|400x327](upload://hbrZewZCNO852prs8TO511AiWrG.jpg)
```

---
## \#33 Posted by: Naysh Posted at: 2018-05-19T17:04:54.356Z Reads: 101

```
You've run FOC successfully on your VESC 4.12 for a long period?
```

---
## \#34 Posted by: trancejunkiexxl Posted at: 2018-05-19T17:15:53.322Z Reads: 99

```
I really liked that video, sounds like kahn
```

---
## \#35 Posted by: squishy654 Posted at: 2018-05-19T17:16:44.825Z Reads: 104

```
[quote="Naysh, post:33, topic:55498, full:true"]
You’ve run FOC successfully on your VESC 4.12 for a long period?
[/quote]

For thousands of miles on multiple boards, yup..sensored foc on hk vesc..proof is in the real world testing for me, not your opinion..
```

---
## \#36 Posted by: Naysh Posted at: 2018-05-19T17:31:32.460Z Reads: 102

```
Yeah but is that thousands of miles going 20km/h  cruising speed on flats  or 40km/h with hills. What's the top speed you've achieved on your build?
```

---
## \#37 Posted by: squishy654 Posted at: 2018-05-19T17:53:46.637Z Reads: 102

```
https://youtu.be/sDaCqbPwN7M
```

---
## \#38 Posted by: mmaner Posted at: 2018-05-20T14:40:35.840Z Reads: 95

```
Dude, respectfully you are wrong.  I've got an Arbor Vugenhausen with a TB VESC, 10s3p, 90mm flywheels with almost 3000 miles on it. I throw it in the back of my truck all the time, I loan I out to n00bs, I've ridden to 30mph, ridden 10 mins up a hill.  

I have actively tried to blow it up so I can use the deck to build a dual off-set and it just won't die.  

If you use good wire, make good solder joints, use quality cells and config correctly there's nothing wrong with using a v4 VESC for FOC...those same rules should be applied to any build.
```

---
## \#39 Posted by: Naysh Posted at: 2018-05-20T17:40:45.758Z Reads: 84

```
I guess I was wrong.  I swear I've read from many senior members posts about FOC being a gamble on 4.12 with the exception of Focbox.  Could it be that running it on 12S FOC is a no no.
```

---
## \#40 Posted by: Hummie Posted at: 2018-05-20T18:46:53.247Z Reads: 83

```
So could u potentially have 1/3 less stator saturation w foc...so third more torque?  Because all three phases are used so all teeth as appears to 2/3 of the teeth?
```

---
## \#41 Posted by: professor_shartsis Posted at: 2018-05-21T04:00:11.335Z Reads: 75

```
this is kind of an interesting read:

“A comparison study of the commutation methods for the three-phase permanent magnet brushless motor”

https://pdfs.semanticscholar.org/40ac/06d3db0b82242038c2dcd20c433d5d1c74f6.pdf

https://image.ibb.co/csUiWT/A82_AAEFC_6_BC4_4708_B6_C6_BFE128_DDB7_F1.png

https://image.ibb.co/gwsyy8/32802_F14_5_EA2_4_A35_AFE0_123_A2_E429_AD4.png

https://image.ibb.co/dBMfBT/3_D4_EC104_25_CA_421_A_8820_56_D249_F4245_F.png
```

---
## \#42 Posted by: GXwagon Posted at: 2018-05-23T16:02:31.592Z Reads: 60

```
Wow that's a great visual!
```

---
## \#43 Posted by: GXwagon Posted at: 2018-05-23T16:10:22.733Z Reads: 62

```
Hey Squish, 

Thanks for posting your video. Great job and congratulations on your achievement!
I also want to thank you for posting your specs and apologize for the following noob question. Okay you said you used a 36v 27,000 mah battery. I have yet to do the research to figure out how the math works but what would that equate to when position like a 10s4p 30Q battery? As currently that's all I know.
```

---
## \#44 Posted by: squishy654 Posted at: 2018-05-23T16:41:06.544Z Reads: 56

```
for my 50 mile ride I went cheap, I used 6 balance board battery's which are very very low c rating...BUT each is a 36v 4400mah 10cell (10s2p) so when I combined them all and wired their BMS's together the entire battery was a 10s12p...I hope this answers the question. MY amp draw was still saggy, I overworked and killed 3 of the packs in the process, but that's what you get for doing things cheaply...if you used better cells, threw money at the problem, took everything I learned, the distances become ridiculous...My only limitation right now is cash...batteries are extremely expensive..
```

---
