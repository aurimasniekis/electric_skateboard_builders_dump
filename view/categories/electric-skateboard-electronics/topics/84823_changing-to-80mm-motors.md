# Changing to 80mm motors

### Replies: 87 Views: 1613

## \#1 Posted by: JensSjogren Posted at: 2019-02-20T17:54:27.364Z Reads: 347

```
Okay so the time is here, 63mm motors doesn't really give me that crazy adrenaline rush anymore. It's time to upgrade.. 

I currently run 2x 6374 192kv sk8 motors on a 12s5p 30Q battery and a gear ratio of 1:6. theese are my settings per Focbox/motor

max motor amps: 100
max battery amps: 50 

The plan is to use 80mm motors on etoxx gear drive 1:5. I'm mostly considering the APS 8072 165kv motor that will give me about the same top speed as my current setup but hopefully a significant improvement to torque. 

https://alienpowersystem.com/shop/brushless-motors/aps8072s-sensored-bldc-motor-165kv-6000w/

My concern is that theese 8072 motors has a rated max amp of 95A, the APS 8085 170kv has a rated max amp of 150. seems strange to me that the difference should be that big for a slightly bigger motor. 

So how big of a torque improvement can i actually expect by changing out my current setup to theese 8072mm motors? I am also upgrading to a focbox unity and a 12s7p battery so i can increase the systems abillity to provide more amps but for this i want to focus on the 6374 motors vs the 8072 motors. I am aware of the fact that the bigger motor has more copper and therefore has lower losses of power. Anyone that has experience of theese motors and could provide a good answer maybe? :)
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-02-20T18:06:33.296Z Reads: 303

```
You should stay away from the aps 8072, I've heard bad things about them making funky noises

Maybe just try a different brand
```

---
## \#3 Posted by: JensSjogren Posted at: 2019-02-20T18:10:04.244Z Reads: 299

```
well i've seen that and the opinions seems to be mixed. I would consider different options but can't really find any decent. the leopards doesn't have sensors which is a huge turn off for me. maybe the APS 8085 is better but i would also have to get a shaft rework in that case, also i like the look of the 8072. the choices seems to be very limited on the 80mm motors
```

---
## \#4 Posted by: Sn4pz Posted at: 2019-02-20T18:11:08.727Z Reads: 289

```
I mean there's always maytech, but that's import fees 🤷🤷

They do have a 8085, just checked...
```

---
## \#5 Posted by: JensSjogren Posted at: 2019-02-20T18:13:23.719Z Reads: 279

```
hmm really? I can't find any 80mm motors on maytechs webpage?

EDIT: oh okay i found it, but it's 330$ :sweat_smile:
```

---
## \#6 Posted by: Sn4pz Posted at: 2019-02-20T18:16:17.227Z Reads: 271

```
Oh shit haha I didn't see the price, my bad :) 

Good luck!
```

---
## \#7 Posted by: maxchilton Posted at: 2019-02-20T18:23:38.374Z Reads: 260

```
what about 4wd with 4x 6374's. lol
```

---
## \#8 Posted by: JensSjogren Posted at: 2019-02-20T18:28:05.606Z Reads: 258

```
Well i like the idea of popping wheelies and motors in front wont really help with that.. xD

Also i ride alot in the forest and im conserned that motors in the front will get smashed by stones and logs
```

---
## \#9 Posted by: Dornacht Posted at: 2019-02-20T18:43:52.080Z Reads: 246

```
A low kv is more important then a massive motor for large torque wheelie style, after 4000W the FocBox is the limiter
```

---
## \#10 Posted by: JensSjogren Posted at: 2019-02-20T18:49:47.226Z Reads: 238

```
well that depends on the gear ratio, on my current 1:6 gear ratio i get simular amount of torque as a 6374 130kv motor on 1:4. having a lower top speed is not an option for me so the only choice seems to be upgrading to 80mm motors. i also max out att 200 motor amps from a standstill so i cant really get any more torque out of theese motors at low speed from what i understand
```

---
## \#11 Posted by: Dornacht Posted at: 2019-02-20T19:18:13.111Z Reads: 233

```
I am just saying, Torque is equall to the current x Kt, the Kt can be drived from the Kv, The only values that will change your torque on motor output with a limit to amp output is the KV, size only allows larger continuous current draw and is listed as max Watts, 6000W is a waste of money and weight
```

---
## \#12 Posted by: Andy87 Posted at: 2019-02-20T19:26:21.310Z Reads: 221

```
Leopard 8072 plus encoder.
Seems the best way so far.
Maybe the 8085 from maytech would be an option for you too. @hyperIon1 can help you there. They sensored and sealed and unsealed available. If i‘m not wrong 160kV too.
```

---
## \#13 Posted by: Andy87 Posted at: 2019-02-20T19:29:27.263Z Reads: 216

```
[quote="JensSjogren, post:5, topic:84823"]
oh okay i found it, but it’s 330$
[/quote]


But cheaper you can’t really get something good.
The leopards are in similar price category.

I got two 8085 from aps. Still couldn’t even try them because one motor was broke from arrival.
```

---
## \#15 Posted by: JensSjogren Posted at: 2019-02-20T19:37:11.136Z Reads: 207

```
im aware that i wont reach 6000W, my current 4500W motors doesnt even reach half of their abillity. 

bigger motors has more copper = less loss of power due to lower temperature right? 

also i'm pretty sure with 80mm motors i could get more motor amps at low speed to increase the torque, there has to be a reason why some crazy people are using the 80mm motors?
```

---
## \#16 Posted by: JensSjogren Posted at: 2019-02-20T19:37:51.743Z Reads: 200

```
https://maytech.cn/collections/sensored-motors/products/brushless-hall-sensor-motor-mto8085-160-ha-c

from what i understand this price is for a single motor? 330$
```

---
## \#17 Posted by: Pedrodemio Posted at: 2019-02-20T19:41:49.026Z Reads: 195

```
Just don't ignore that if you are pushing the motors really hard, for the same current, the lower Kv will heat up more
```

---
## \#18 Posted by: Andy87 Posted at: 2019-02-20T19:42:16.773Z Reads: 194

```
Speak with @hyperIon1 if you really interested.
Can’t promise you anything, but he might get a good quote for you.

But one side note. 
A 7p 30q gives you also only 70a batt max. That you can run with a 6384 too.
```

---
## \#19 Posted by: JensSjogren Posted at: 2019-02-20T19:44:27.154Z Reads: 191

```
yes the 6384 might potentially reach that but at low speed the bigger motors should be able to reach higher motor amps to increase speed faster? i might be dead wrong about this but from what i've learned motor amps and battery amps arent the same thing
```

---
## \#20 Posted by: rusins Posted at: 2019-02-20T19:51:05.111Z Reads: 180

```
Correct! You might not be pushing your motors to the max at high speed, but when starting up from zero bigger motors (that can handle more amps or lower KV) will improve your torque. Just check to be sure that your ESC can drive the motors at whatever current you're aiming for :slight_smile:
```

---
## \#21 Posted by: Andy87 Posted at: 2019-02-20T19:51:17.870Z Reads: 179

```
[quote="JensSjogren, post:19, topic:84823"]
motor amps and battery amps arent the same thing
[/quote]

You right with it.
But if you run 70a bat and 70a Motor Max you will get a different acceleration than with bat max at 50a and motor max 70a
```

---
## \#22 Posted by: rusins Posted at: 2019-02-20T19:53:13.425Z Reads: 163

```
Battery max current will limit battery max wattage; acceleration should be the same, but at 50A battery max it (acceleration) will start to decrease at a lower speed than at the 70A max. (From what I understand)
```

---
## \#23 Posted by: Pedrodemio Posted at: 2019-02-20T19:55:30.190Z Reads: 160

```
you will get the same acceleration up to 71% of your top speed at the current battery voltage
```

---
## \#24 Posted by: JensSjogren Posted at: 2019-02-20T19:55:34.361Z Reads: 157

```
going for 12s, maybe even 13s if the focbox unity are proven safe to work with 13s, anyways it should be enough to drive the motors
```

---
## \#25 Posted by: Andy87 Posted at: 2019-02-20T19:58:33.003Z Reads: 158

```
That’s right! At low speed it will not change
```

---
## \#26 Posted by: JensSjogren Posted at: 2019-02-20T20:00:59.466Z Reads: 160

```
and this is why im interested in bigger motors since i want that crazy acceleration from a standstill
```

---
## \#27 Posted by: Andy87 Posted at: 2019-02-20T20:05:33.420Z Reads: 159

```
I don’t understand what is wrong 😅
Don’t want to say, don’t go with 80mm motors.
By no means it’s for sure fun, as min I hope so with mine 😜
But honestly my dual 6384 170kV and 1:4.7 gearing let me make crazy wheelies when pushing the throttle full from stand still and even from like 5km/h
With a 1:6 gearing the acceleration should be pretty pretty good already. 😅
```

---
## \#28 Posted by: JensSjogren Posted at: 2019-02-20T20:09:16.608Z Reads: 161

```
yeah it has great acceleration already, i guess i just got used to it and i want to be scared when i pull full throttle, when i first finnished my build i got some serious adrenaline pumping from this setup and i want that feeling to come back haha. Also i'm quite a heavy guy at 95 kg so i guess that affects the acceleration aswell. 

i clocked the acceleration. it goes from 3-4 kph (just rolling slowly) to 40 kph in just over 2 seconds
```

---
## \#29 Posted by: sk8l8r Posted at: 2019-02-20T20:17:23.769Z Reads: 151

```
I want to pimp my Bajaboard with 4 big 80xx im interested to see how you get on with whatever you try :smile:

 I'm thinking 13s5p for front and same for rear (using focboxes)
```

---
## \#30 Posted by: JensSjogren Posted at: 2019-02-20T20:20:40.515Z Reads: 153

```
hahaha but already having 4wd you feel like you need more acceleration? xD
```

---
## \#31 Posted by: Dornacht Posted at: 2019-02-20T20:39:25.190Z Reads: 151

```
So if you use the unity with a max not continuous current  supply of 300a that means your battery has to be able to supply 212.13amps, each motor would be seeing 5100watts for a brief time during hard acceleration, the continuous current is 80-100 motor amps making the maximum continuous current draw from battery 142 amps and at 12s a motor that is ratted for 3500W is a maxed out due to the limitation of the esc
```

---
## \#32 Posted by: Dornacht Posted at: 2019-02-20T20:40:40.895Z Reads: 147

```
I have both a 170kv 6374 max 3400Watts and a 6484 170kv max 4000Watts and they both draw the same current  and have the same torque, the 6384 just can outlast the other if esc limitation isn’t a factor
```

---
## \#33 Posted by: FredrikHems Posted at: 2019-02-20T20:50:52.159Z Reads: 143

```
You running 100 motor amps right now, right? I would have atleast tried to increase this first, before buying new motors. 
As far as I understood you havnt had any overheating issues with either the focboxes or motors? 
This means that you havnt pushed either of them to their limits with your current settings. Try increasing your motor amps to 120, you’ll be suprised how big of a difference it makes :smile:

This obviously only apply if you havnt had any overheating issues.
```

---
## \#34 Posted by: rusins Posted at: 2019-02-20T21:02:30.305Z Reads: 142

```
I'm not sure if the 300A Unity rating is for the battery input or the motors. In any case, even the TorqueBoards ESC boasts that it can do up to 240A for a single motor for a few seconds, so I think the Unity can safely do more. Do keep in mind that we're talking about startup acceleration, so the motors won't be running at max voltage, and therefore the power draw will be far less than what you state. I'm actually quite confused as to how you calculated all the numbers you mentioned; seem to appear out of thin air :smiley:
```

---
## \#35 Posted by: Sn4pz Posted at: 2019-02-20T21:05:26.580Z Reads: 145

```
[quote="rusins, post:34, topic:84823"]
that it can do up to 240A for a single motor for a few seconds
[/quote]

youre assuming this is right... The vesc might be able to do 240a, but how long is a few seconds? 2? 3? How long does it take for your amp load to lower because youve reached speed?

seems like a very misleading point, as ive thermal throttled with less than 5 mins of riding time, 30a each, two big hills(no crazy angles or "impossible" hill degrees)

no shot any 4.xx can take 240a for a few seconds.... except maybe chakas? Thats alot to ask for 4.xx HW

@rusins ive edited it so it reflects my complete thoughts. sorry. I have a bad habit of submitting the comment and then editing like my life depends on it for the next few minutes
```

---
## \#36 Posted by: rusins Posted at: 2019-02-20T21:06:39.997Z Reads: 140

```
It does sound a bit unrealistic tbf :thinking: :smiley:

Edit: @Sn4pz you and me both, bud! :smiley:
```

---
## \#37 Posted by: hyperIon1 Posted at: 2019-02-21T00:04:47.952Z Reads: 136

```
https://www.hyperionesk8.com/collections/brushless-motors/products/mto8085-160-ha-c-e-skateboard-motor
```

---
## \#38 Posted by: hyperIon1 Posted at: 2019-02-21T00:06:04.478Z Reads: 136

```
https://www.hyperionesk8.com/collections/esc-vesc-contollers/products/mtsesc6-6-200a-esc-brushless-motor-controller
```

---
## \#39 Posted by: hyperIon1 Posted at: 2019-02-21T00:07:50.523Z Reads: 140

```
For the water sporter........
https://www.hyperionesk8.com/collections/esc-vesc-contollers/products/mtsf300a-opto  
https://www.hyperionesk8.com/collections/brushless-motors/products/mto8085-160-g-brushless-motor-for-hydrofoil-electricc-suf-boards
```

---
## \#40 Posted by: Dornacht Posted at: 2019-02-21T01:04:44.408Z Reads: 137

```
Motor amps values  are not the same as battery amp values, if you run your motors with a multi meter connected, you would see the voltage the motors run is a lot less then power source, I have an Exel calculation sheat that graphs the voltage conversion and expected amp draw from power source. That’s how I pulled the numbers
```

---
## \#41 Posted by: JensSjogren Posted at: 2019-02-21T05:01:23.970Z Reads: 133

```
[quote="FredrikHems, post:33, topic:84823"]
You running 100 motor amps right now, right? I would have atleast tried to increase this first
[/quote]

That is correct, 100A is the manufacturer rated limit. I never even got close to overheating, one thing to consider is that i finnished my board in novemeber and have only been riding in temperatures between 5°C to -15°C. When summer comes it might be another story
```

---
## \#42 Posted by: JensSjogren Posted at: 2019-02-21T10:59:16.756Z Reads: 118

```
No one that has first hand experience regarding the 8072 motors?
```

---
## \#43 Posted by: Andy87 Posted at: 2019-02-21T11:04:25.026Z Reads: 118

```
@Riako has experience with the 8072.
Maybe @Silverline too but i‘m not sure anymore.
```

---
## \#44 Posted by: Andy87 Posted at: 2019-02-21T11:08:57.699Z Reads: 122

```
https://www.electric-skateboard.builders/t/tbe-to-be-electrified-trampa-urban-carver-aps-8072s-escape-12s4p/52021?u=andy87

https://www.electric-skateboard.builders/t/vesc-tool-motor-expert-please-look-here/57029?u=andy87

And some more just search for aps 8072.

I would also recommend to search on YouTube for the motor. You should find some interesting videos
```

---
## \#45 Posted by: chocol4te Posted at: 2019-02-21T12:27:20.488Z Reads: 112

```
Too late :cry:

I bought it and it seemed to work fine because the only battery I had was a 4s, so I never entered the RPM region with issues. By the time I built my 12s and started getting issues I couldn't return it :(
```

---
## \#46 Posted by: FredrikHems Posted at: 2019-02-21T12:36:54.196Z Reads: 110

```
If you are not overheating you can up the amps. The current you can draw is only limited by heat, as more current = more heat. There is people running 140 amps per focbox here. :sunglasses:
```

---
## \#47 Posted by: Dornacht Posted at: 2019-02-21T14:47:42.837Z Reads: 113

```
The max possible motor watts at that current limit with the max limitation of the focbox removed is still under 5000w, I don’t see why you would want to waste money on a motor you can’t even use to it’s full potential, due to limitations of the esc
```

---
## \#48 Posted by: JensSjogren Posted at: 2019-02-21T16:05:54.976Z Reads: 112

```
You still don't get the point. Im fully aware that i wont use the maximum potential of the 80mm motors, in order to do that i would also need to use 15s voltage. The point is that bigger motors has more copper and therefore less resistance, they can handle more amps at low voltage (low speed) that increases the torque at low speeds, theoreticly atleast and thats why i'm looking for opinions from people that tried 80mm motors in real life. 

The 6374 already reaches their maximal potential at low speeds, increasing battery amps will only increase the acceleration after a set point when the motors are running on higher voltage. I'm not looking for this, im looking for better acceleration from a stand still. Got it?
```

---
## \#49 Posted by: JensSjogren Posted at: 2019-02-21T16:10:15.595Z Reads: 114

```
The issues you're talking about on the 8072 appeared after changing to 12s if im not mistaken? 

Those issues includes that wierd sound or is it also something else?
```

---
## \#50 Posted by: chocol4te Posted at: 2019-02-21T16:23:40.439Z Reads: 115

```
Yes, the noise only happens at around 50% throttle for me, on a 12s. I couldn't see anything wrong even at 100% on a 4s.

The issues include the weird sound, and the vibrations which I'm not sure are good for the motor in the long term. :/
```

---
## \#51 Posted by: FredrikHems Posted at: 2019-02-21T16:28:20.577Z Reads: 110

```

[quote="JensSjogren, post:41, topic:84823"]
I never even got close to overheating
[/quote]

[quote="JensSjogren, post:48, topic:84823"]
The 6374 already reaches their maximal potential
[/quote]

You say you havnt got close to overheating, but later you say that the motors have already reached their maximal potential? One or the other must be wrong as these doesnt match. 
The motors havnt reached their full potential before they overheat. So until you have overheated your motors, you havnt pushed them to their full potential.
```

---
## \#52 Posted by: JensSjogren Posted at: 2019-02-21T17:44:28.489Z Reads: 103

```
Im considering the manufacturers rating as max in this case, which is 100A. As previously said i have only been riding in cold wheater, most of the time around -5° C, im sure they would get way hotter during summer and +25°C
```

---
## \#53 Posted by: Dornacht Posted at: 2019-02-21T18:37:00.915Z Reads: 102

```
Wasnt trying to pick a fight, sorry for any bad fellings, 80mm motors are great my friend had one on his first e-mountain bike the old turnigy ones. It worked great, can’t wait to see your next build!
```

---
## \#54 Posted by: JensSjogren Posted at: 2019-02-21T20:01:54.529Z Reads: 102

```
Hmm that's disturbing.. the 8072 seems to have some problems, maybe it's better to wait for more reliable options. 6384 APS might do for now 🤔
```

---
## \#55 Posted by: JensSjogren Posted at: 2019-02-21T20:02:42.977Z Reads: 104

```
It's all good, just got the feeling that we werent discussing the same thing so i wanted to clearly explain my goal :)
```

---
## \#56 Posted by: Andy87 Posted at: 2019-02-21T20:06:26.457Z Reads: 109

```
@chocol4te maybe this could fix your issues with the motor
 https://www.electric-skateboard.builders/t/ice-crusher-16ply-holypro-4w-chain-drive-mtb-4x-6374-170kv-aps-quad-escape-steering-damper/65823/119?u=andy87
In your case you would need to cover the windings with epoxy too.
```

---
## \#57 Posted by: Andy87 Posted at: 2019-02-21T20:08:24.154Z Reads: 115

```
[quote="JensSjogren, post:54, topic:84823"]
6384 APS might do for now
[/quote]

I had 2 broken bells on them.
Just saying... if you go with the 6384 better battle harden then after you made a bench test.
My last link explains how to do it.
```

---
## \#58 Posted by: banjaxxed Posted at: 2019-02-21T20:17:20.884Z Reads: 114

```
What's the mounting pattern compared to typical 63xx motors?

Having a hard deciding between something like this or 6384, the lack of sensors is something not sure on, massive motors can still cog afaik ?

[quote="hyperIon1, post:37, topic:84823"]
![|737x500](https://cdn.shopify.com/s/files/1/0004/5429/5609/products/Screen_Shot_2019-02-02_at_11.25.05_PM_1200x1200.png?v=1550561184)

### [MTO8085-160-HA-C E-Skateboard motor](https://www.hyperionesk8.com/collections/brushless-motors/products/mto8085-160-ha-c-e-skateboard-motor)

MTO8085-160-HA-C E-Skateboard motor
[/quote]
```

---
## \#59 Posted by: Silverline Posted at: 2019-02-21T20:20:26.969Z Reads: 107

```
yeah... those APS 8072... are crap..... i moved on...
```

---
## \#60 Posted by: JensSjogren Posted at: 2019-02-21T20:22:12.411Z Reads: 107

```
Hmm.. it's funny how my turnigy sk8 motors has worked flawlessly, even riding in heavy rain, blizzards, and muddy terrain. i thought APS was quality stuff 🤔

I got a set of etoxx mini drives that i was going to sell and get the big drives to be able to use 80mm motors. If im using 63mm motors i can keep the mini drives but i have to get lower KV, APS 6384 130KV looks like the best option for that but starting to doubt this now aswell 😅
```

---
## \#61 Posted by: chocol4te Posted at: 2019-02-21T20:26:05.464Z Reads: 108

```
@Andy87 Thanks! That looks great, I'll look into it. Do you know if it reduced the noise/vibration issue at all?
```

---
## \#62 Posted by: Klaerke91 Posted at: 2019-02-21T20:26:15.068Z Reads: 108

```
I have with these. 
https://alienpowersystem.com/shop/brushless-motors/c8085-sensored-outrunner-brushless-motor-170kv-6000w/

Havent driven that much yet but i can't give full power as the board "disappears" under you.
I have 2 of them with Etoxx direct drive 1:5 gearing and 100 max motor amp to each motor
```

---
## \#63 Posted by: banjaxxed Posted at: 2019-02-21T20:26:36.734Z Reads: 108

```
I read something about a noise problem
```

---
## \#64 Posted by: Andy87 Posted at: 2019-02-21T20:38:16.294Z Reads: 107

```
The epoxy between the magnets hold the magnets better in place. As i experience that the magnets get lose easy on aps motors this will fix that issue.
If you have a high pitching noice a an specific rpm it could be that one or more windings are lose. If you epoxy the windings too that issue could be fixed with it as the epoxy holds everything in place.
I can’t promise you anything as i don’t know from where your issues really coming, but it is a good and easy way to start with.
```

---
## \#65 Posted by: chocol4te Posted at: 2019-02-21T20:45:14.990Z Reads: 103

```
Ah okay, good to know. Thank you :D
```

---
## \#66 Posted by: Andy87 Posted at: 2019-02-21T20:50:20.187Z Reads: 100

```
Good luck 😜
```

---
## \#67 Posted by: Silverline Posted at: 2019-02-21T22:25:29.468Z Reads: 98

```
Yep.... This is mine : https://youtu.be/yxok02O2vSM

@JensSjogren Yeah.... I moved on to turnigy sk8 aswell.... They work perfect....
```

---
## \#68 Posted by: banjaxxed Posted at: 2019-02-21T22:57:08.649Z Reads: 102

```
That harmonic noise, I guess it wasn’t a one off either iirc there was another member with the exact same issue
```

---
## \#69 Posted by: banjaxxed Posted at: 2019-02-22T12:23:10.538Z Reads: 96

```
Power wise was there a drop over the 8072 APS?
```

---
## \#70 Posted by: banjaxxed Posted at: 2019-02-22T12:35:37.925Z Reads: 98

```
@hyperIon1 are these sensored? What's the hole pattern sizes?
```

---
## \#71 Posted by: Silverline Posted at: 2019-02-22T18:21:58.377Z Reads: 93

```
I have never driven with the APS. Bruno took them back.
```

---
## \#72 Posted by: banjaxxed Posted at: 2019-02-22T20:43:25.527Z Reads: 86

```
thanks good to know about this
```

---
## \#73 Posted by: hyperIon1 Posted at: 2019-02-22T21:54:00.008Z Reads: 89

```
Most of Maytechs motors have an uncensored model, but the price difference is minimal. for the 8085 hydro they only come without sensors. the esk8 version has sensors. 
For the Hole pattern, it is the same as standard 6374 motors with the addition of the second set of mount holes for the 50mm series (maytech mounts)
```

---
## \#74 Posted by: Doneone Posted at: 2019-10-19T18:37:46.217Z Reads: 67

```
Hi Jens!

Did you finish your swap to 80mm motors? I am now in the process myself and wanted to check if your results are satisfactory.
```

---
## \#75 Posted by: JensSjogren Posted at: 2019-10-19T20:59:06.069Z Reads: 65

```
Hi, yes I did. First I went with 6384 for a time, then I upgraded to 8085 motors but one of them shorted due to phase wire insulation melted when I was riding during a hot summer day, APS doesn't use silicone wires, which is pretty stupid imo. I moved on to 80100 motors that I mounted in August.

I'm going to compare them quickly here 

APS 6384 130kv on 1:4 (70A battery, 80A motor)
Pros: Great acceleration, very good energy efficiency at 18 wh/km riding at high speeds, runs cool.
Cons: limited top speed at 50 kph on full charge 

APS 8085 200kv on 1:5 (70A battery, 120A motor)
Pros: higher top speed at 60kph+ and similar torque as 6384.
Cons: they get hot, very very hot! 

APS 80100 180kv on 1:5 (80A battery, 140A motor)
Pros: stupid torque, would send me flying in an instant without the bindings, decent top speed at 55kph 
Cons: they are heavy af, big increase in consumption at around 25-30wh/km, needs to use axle extensions to fit them with etoxx gear drive, has a tendency to rip the motor mount loose (installed a pretty ugly crossbar to solve this), they get kinda hot.

6384's was great in every aspect, I'm basically to stupid to settle for anything I guess.

In summary I think the 8085's wasn't worth it, obviously couldn't handle the rated amps and wasn't that big of an upgrade compared to 6384's

 80100's are for sure a blast and they are very very powerful, not sure what I prefer though, the range I got with the 6384 motors (60km+) or the power of theese, currently getting around 40km with my 12s9p 30Q pack. They also make the board bigger and more clumpsy, I can barely jump over curbs, make 180's etc with the weight of the board atm.

Kinda miss the 6384 motors, when theese break I'll definitely dust of my old assembly
```

---
## \#76 Posted by: Doneone Posted at: 2019-10-19T22:06:08.103Z Reads: 60

```
Great information here!

I heard about the aps quality and decided not to go for it. I went for the maytech 8085 160kv sensored sealed. They are being shipped atm.

I ride in hot environments and had my 6476 160kv overheat constantly. I heard that bigger motors will mitigate the overheating.
Hope to get some torque increase as well.
```

---
## \#77 Posted by: Doneone Posted at: 2019-10-20T06:42:15.668Z Reads: 58

```
I think the KV was too high on your 8085, but I guess you wanted torque increase as well as top speed increase. I am satisfied with 50kph. Just want that crazy torque and the motors not overheating if possible 😅
```

---
## \#78 Posted by: DavidC Posted at: 2019-10-20T08:23:26.482Z Reads: 58

```
My APS 80100 130KV get less hot than Turnigy SK3 or SK8 190KV (12S).
```

---
## \#79 Posted by: Chricious Posted at: 2019-11-14T13:02:50.106Z Reads: 54

```
Hey Guys, any updates on your 8085/80100 motors?
We ware building a 2WD board with MT 6396 170KV , VESC6.6 and 12S12 30Q battery atm.
What would be a good alternative if we are not satisfied with the performance?
```

---
## \#80 Posted by: murdomeek Posted at: 2019-11-14T19:16:55.562Z Reads: 51

```
i believe maytech has 8095 motors?
top quality, but also top prices
```

---
## \#81 Posted by: Doneone Posted at: 2019-11-22T21:28:29.329Z Reads: 50

```
Yes got them in. Looks great. Had them running already on the workbench only though today. Now I need to shorten the motor wires. I struggle to solder the motor wires to connectors. The solder won't stick to the wires. Haven't had this before.
```

---
## \#82 Posted by: Chricious Posted at: 2019-11-22T21:40:47.731Z Reads: 49

```
Yes it is not that easy to solder the connectors on the wires, but with a little patients you will succeed. If you have any questions, feel free to ask and I'll see if I can help.
```

---
## \#83 Posted by: JensSjogren Posted at: 2019-11-23T21:47:01.146Z Reads: 43

```
What kind of soldering station do you use? For wires in the 12-10awg area you need a decent station in order to make good solder joints
```

---
## \#84 Posted by: Andy87 Posted at: 2019-11-24T06:54:51.934Z Reads: 43

```
You need first sand down or burn down the insulation if you want to shorten the phase wires. Very important that all windings from the phase wires need to have contact with the solder.
```

---
## \#85 Posted by: Doneone Posted at: 2019-11-24T21:21:43.286Z Reads: 42

```
I now burned them and then dunked them in concentrated acid to clean the wires. Everything seems to work fine now.
```

---
## \#86 Posted by: Doneone Posted at: 2019-11-24T21:23:07.097Z Reads: 42

```
Saw a friend of mine today. Everything sorted 👍
```

---
## \#87 Posted by: Doneone Posted at: 2019-11-24T23:39:24.966Z Reads: 41

```
![IMG_20191125_003359|690x388](upload://zPxzHVhnJqWZ9xfbT6ZQ8i4rLAo.jpeg) ![IMG_20191125_003244__01|472x500](upload://cpmIGb9Sw7uG3V1f9OYZl3hhkI8.jpeg)

Happy so far. Just 5 minutes of riding. Does what it should. Performance to be assessed.
```

---
## \#88 Posted by: EileenMaytech Posted at: 2019-12-30T11:16:42.590Z Reads: 25

```
awesome build!
```

---
