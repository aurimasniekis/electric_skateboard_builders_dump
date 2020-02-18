# 3000W Electric Unicycle Build!

### Replies: 52 Views: 1346

## \#1 Posted by: kuphjr Posted at: 2019-02-12T22:27:39.843Z Reads: 303

```
It’s not an esk8 build but I feel an electric unicycle is more akin to an eboard than an electric bike so I’ll post here.

I am planning a build similar to the Gotway with a more powerful 3000W motor with a 20.9”x2.75” tire. It will have a 20s3p 30Q battery and will be controlled by gyroscope and accelerometer connected Arduino with a DAC output to control a Kelly speed controller. I will make the frame out of 1” aluminum tube with CNCed plates brazed to the tube to hold the wheel axel.

This project is going to take a long time and I’m just getting a parts list together now and drawing up plans. I plan to log everything in this thread for anyone interested. Stay tuned for blueprints & parts list sometime in the next few weeks!
```

---
## \#2 Posted by: kuphjr Posted at: 2019-02-12T22:29:21.485Z Reads: 297

```
I’d like to hear from anyone who has ridden or owns a commercial electric unicycle. What can you tell me about them? What design aspects do you like? What could be improved?
```

---
## \#3 Posted by: evoheyax Posted at: 2019-02-12T22:45:01.199Z Reads: 288

```
@psychotiller What was that crazy one wheel thing I saw you riding?
```

---
## \#4 Posted by: psychotiller Posted at: 2019-02-12T23:08:44.791Z Reads: 273

```
Yup! Fun at slow speeds. I'd never go full speed on one again. Very unstable over bumps and uneven terrian. Had I not had my helmet on, I'd probably be dead.
```

---
## \#5 Posted by: kuphjr Posted at: 2019-02-12T23:22:05.327Z Reads: 256

```
That bad huh. Which one did you ride? I assume a larger & wider tire might help absorb bumps. I’m going to get a dual sport 110/80-14 motorcycle tire.
```

---
## \#6 Posted by: iKNOWaFATman Posted at: 2019-02-12T23:27:27.242Z Reads: 235

```
I hate builds like this.




Build it then post everything at once. The suspense is killing me alresdy.
```

---
## \#7 Posted by: kuphjr Posted at: 2019-02-12T23:37:18.340Z Reads: 228

```
If I do that I forget to take pictures until the very end. I want to document the process as much for myself as the community. That way I can just link someone when they ask me about it.
```

---
## \#8 Posted by: kuphjr Posted at: 2019-02-12T23:43:25.913Z Reads: 223

```
Could I do smoother single track trails around 15-17 MPH w/ a few months practice?
```

---
## \#9 Posted by: psychotiller Posted at: 2019-02-13T00:00:27.413Z Reads: 217

```
https://www.instagram.com/p/BrhLYJdFiPi/
```

---
## \#10 Posted by: psychotiller Posted at: 2019-02-13T00:18:00.825Z Reads: 208

```
Definitely!! But I'm not kidding about sudden instability. I was getting really good on it. Confidence is your enemy. Its heavy too. I was riding it at night in familiar territory. Road crews had been grinding our streets though, and I didn't see the rut. It turned and started to run me into a new mustang. I planted my foot between the one wheel and the car and it turned/flipped instantly. The first parts of me to hit the ground were my head, my fist, and shoulder. 

JT was on his board and I was riding along side of him. Fastest I got it up to was 19mph. Probably only going 15 when I fell.

Fun to goof around on. PLEASE wear a helmet on it though.
```

---
## \#11 Posted by: kuphjr Posted at: 2019-02-13T00:43:00.661Z Reads: 190

```
Of course! Safety first!

So is that wheel DIY? If so who made it? I am a little worried about getting the self balancing software to run properly on Arduino and it would be nice to have contact info for someone who has already done this. I am a 3rd year computer science & electrical engineering student so I do already have a pretty good idea of what I am doing, but knowing a veteran always helps.
```

---
## \#12 Posted by: Sn4pz Posted at: 2019-02-13T00:47:45.248Z Reads: 181

```
I think that, although the current implementation of the over-tilt protection isn't bad, it could certainly be improved and made more user/commercially friendly.

I can't speak for any brand or euc other than the ninebot c+ or something like that, but that one has very quiet beeps and *decent at best* tactile feed back that youre going too fast/ leaning forward too much.
```

---
## \#13 Posted by: kuphjr Posted at: 2019-02-13T00:51:22.911Z Reads: 166

```
I think making a super loud beeper attached to the Arduino shouldn’t be too hard
```

---
## \#14 Posted by: kuphjr Posted at: 2019-02-13T00:53:23.789Z Reads: 160

```
Could you explain a bit more about the beeps? Does it allow the speed controller to go over continuous rated current but only for a short burst before give you a warning that it’s gonna cut power to protect from overheating?

That is my guess
```

---
## \#15 Posted by: kuphjr Posted at: 2019-02-13T00:54:01.751Z Reads: 157

```
Or does it beep to let you know if you lean farther forward it doesn’t have enough power to keep you upright and you will fall?
```

---
## \#16 Posted by: Sn4pz Posted at: 2019-02-13T00:54:03.647Z Reads: 151

```
Also an indication of throttle, like the amount left. 

Riding in BLDC mode is nice because you always know how much throttle you have left, but with foc(the EUCs are quiet, I would equate them to foc) its difficult to gauge that off of the sound the motors make. 

I little DaVeGa style cluster inbetween your crotch or something with a hyper visible screen that shows current PPM position

idk something like that :man_shrugging:
```

---
## \#17 Posted by: Sn4pz Posted at: 2019-02-13T00:56:43.548Z Reads: 148

```
so there are two scenerios when it will beep and provide "push back"

a) you lean your body too far forward for the device and it is thrown out of wack and it gets very angry. It will try to push your feet back and will beep angrily. 

b) If youre traveling too fast, it will let you know when you reach the max speed of the EUC, and then apply the "push back" to apply breaks, and will beep if you continue to speed up. BUT BUT BUT IF YOU CONTINUE TO SPEED PAST THE WARNINGS IT GOES COMPLETELY LIMP

**_THAT NEEDS TO BE CHANGED_**
```

---
## \#18 Posted by: Sn4pz Posted at: 2019-02-13T00:58:30.775Z Reads: 143

```
If youd like Id be cool sending you my ninebot to toy around with

just got to send it back in one piece :rofl:
```

---
## \#19 Posted by: kuphjr Posted at: 2019-02-13T02:03:54.207Z Reads: 167

```
That would be super super awesome if I could!!!  I really wanted to buy a commercial electric unicycle just to try it out but I couldn’t really justify spending all the money for something that I would only use until I finished my own DIY build.

We can work this out in the future. I can PayPal you for the shipping and everything. I wouldn’t want to have you send it until it is nicer though.  No place to ride in Minneapolis until late April.
```

---
## \#20 Posted by: topcloud Posted at: 2019-02-13T02:16:39.428Z Reads: 169

```
https://youtu.be/OBhoSBDUPsU?t=133

this is what happens when you don't listen to the beep
```

---
## \#21 Posted by: kuphjr Posted at: 2019-02-13T02:32:10.227Z Reads: 165

```
Oh yeah I saw that video. Crazy! My electric uni should have a theoretical top speed of 40 but I don’t ever plan to do more than 25 MPH. Hopefully that will eliminate any worry if something like this happening.
```

---
## \#22 Posted by: topcloud Posted at: 2019-02-13T03:06:14.780Z Reads: 160

```
on a unicycle, when one wheel loses traction in a straight line, the rider can skate (coast) over things - you just don't want to slide sideways (when turning)

on EUC, when you see a patch of sand or water, the key is to stand up straight, without any acceleration or regenerative braking - and try to 'float' over the obstacle.

else, the wheel can lose traction and, if accelerating, the EUC will street the rider.  beep beep and the Gotway SuperX is just 2000W.

If you want to do something custom, check out Bel & Bel in Barcelona - they're at the cutting edge of custom EUC.  https://www.instagram.com/belybel_artworks/

![28%20PM|423x500](upload://kNxIrCKaLf5dysVd2vGdIuhW3wR.jpeg)
```

---
## \#23 Posted by: kuphjr Posted at: 2019-02-13T03:47:28.595Z Reads: 141

```
Wow! That is beautiful! I had no idea something of that caliber existed for electric unicycles!
```

---
## \#25 Posted by: ARetardedPillow Posted at: 2019-02-13T08:52:23.947Z Reads: 121

```
I want to see this happen! I love both my EUCs and my Eskates but an EUC is just more practical in everyday life, take the board out for group rides and for looking cool :sunglasses: , EUCs for everything else
```

---
## \#26 Posted by: Sn4pz Posted at: 2019-02-13T09:35:49.843Z Reads: 117

```
Seriously. Lol. 

Everyone looks at me funny when I say respect the beep / click depending on the product, but they don't end up pushing it's limits all the way 😂😂

No one wants to street face
```

---
## \#27 Posted by: xilw3r Posted at: 2019-02-13T09:53:39.164Z Reads: 112

```
[quote="psychotiller, post:4, topic:84056"]
full speed on one again. Very unstable over bumps and uneven terrian. Had I not had my helmet on, I’d probably be dead.
[/quote]

+10000 for the ATHF dub on that vid :D
```

---
## \#28 Posted by: kuphjr Posted at: 2019-02-14T18:42:45.932Z Reads: 90

```
What exactly is meant by “push back”. Does that mean the wheel ramps up throttle to give the feeling of pushing back against you while your leaning forward?
```

---
## \#29 Posted by: kuphjr Posted at: 2019-02-14T18:43:44.192Z Reads: 88

```
I’m analyzing some open source self balancing code, I found a file called “kickback” and it seemed to ramp up or down depending on if the unicycle was in its balanced state or not.
```

---
## \#30 Posted by: kuphjr Posted at: 2019-02-14T18:47:02.129Z Reads: 82

```
What I can do is have it beep loudly at 3000W. That is the continuous rated current. However, the motor can burst up to 4800W for up to 10 sec, so I should still be safe at 3000W contiuous. I doubt I will ever get even close to that much power anyways.
```

---
## \#31 Posted by: kuphjr Posted at: 2019-02-14T18:49:00.566Z Reads: 84

```
And that would let you know to lean backward before the controller cuts lower to protect itself from over current.
```

---
## \#32 Posted by: kuphjr Posted at: 2019-02-14T18:49:27.245Z Reads: 85

```
Sorry for weird out of order comments.
```

---
## \#33 Posted by: Sn4pz Posted at: 2019-02-14T18:59:39.459Z Reads: 92

```
No so, basically, how I figure the pedals push back is they have their own motor that engages itself in the pedals and changes them from this position (over acceleration) \ to the equilibrium --

![owdrawtilt|690x346](upload://jZUeewATZpf0ELeMpH0XDyUFVK2.png) 

E: Push back, in this case, is defined as the pedals readjusting under you to help you decrease speed

E E: added the N to hopefully establish the fact that the uni isnt moving, the pedals are
```

---
## \#34 Posted by: Sn4pz Posted at: 2019-02-14T19:10:14.754Z Reads: 87

```
I think you should have it beep at 15 and 20 mph, but how are you going to *do* the foot pedals, are they going to be motorized like the Ninebot One C+s? Or are you hoping to go a more simple route
```

---
## \#35 Posted by: Sn4pz Posted at: 2019-02-14T19:14:36.041Z Reads: 82

```
As a simple explanation as to what 3 means on the picture that Im convinced they use Current and RMP/ERPM to operate the pushback / motorized pedal cutout

Under full battery, the device can take any sort of "pull" that you throw at it, doesnt give an overspeed beep or even a overtilt beep.

Under a certain %, I find the 'yellow' zone is where this happes: the cycle starts to beep like crazy at the smallest nudge of power (overtilt, over speed AND overcurrent)

^^ IMHO, This is the largest issue with the Ninebot One

 If i could uncap my ninebot, I would. 
I dont give a fuck about the range or the negative battery wear, I would rather use it than have it sit in my closet collecting sleepytime dust
```

---
## \#36 Posted by: kuphjr Posted at: 2019-02-14T19:44:52.986Z Reads: 69

```
I was really hoping I could go a more simple route.  I really don’t need to implement push back in my own design I think as long as I don’t go crazy accelerating. Like I said, I’m never going to actually hit 3000W. Implementing battery warning beeps is easy too to prevent low voltage cutoff.
```

---
## \#37 Posted by: Sn4pz Posted at: 2019-02-14T19:50:55.692Z Reads: 73

```
I think you should think in terms of ERPM / RPM instead of Wattage, not that wattage is bad, but just remember that Wattage varies at different speeds and that its entirely dependent on "startup"( as you begin to move) wattage. 

Ever see a video of an EMTB that uses a VESC overlay? If they JAM the throttle, the wattage and amperage sohots up until the ESC doesnt need to keep the constant wattage and amperage up to maintain your speed.

E: this information is NOT APPLICABLE to the VESC while its in wattage mode, as thats completely different
```

---
## \#38 Posted by: kuphjr Posted at: 2019-02-14T19:56:06.491Z Reads: 70

```
Well the only option I have of controlling a speed controller is 0-5v input.  I think I kind of have to roll with that. The speed controller has a sufficient E RPM limit that I am not worried about reaching.

There may be someone on the electric unicycle forum who is doing an open source speed controller, but that sounds like an endeavor that will take some time, even with me writing the code.
```

---
## \#39 Posted by: Sn4pz Posted at: 2019-02-14T19:57:34.214Z Reads: 74

```
I agree its going to be tricky, but if youre up for it youre up for it :) 

Do you plan on using some sort of pressure pads?

E: I dont mean that you would hit the MAX RPM of your controller, but rather you set a speed that you dont want to exceed (RPM corelates with a simple equation) so that once the controller hits that, the speed is gently throttled down or something
```

---
## \#40 Posted by: kuphjr Posted at: 2019-02-14T20:01:38.447Z Reads: 72

```
It really comes down to developing a formula to take the angle from the IMU and output a 12 bit number that represents a voltage from 0-5v for the DAC converter.
```

---
## \#41 Posted by: kuphjr Posted at: 2019-02-14T20:06:23.219Z Reads: 72

```
Then I should just be able to feed that into the kelly speed controller.  I would let the speed controller deal with it from there.  I wouldn't bother setting a max ERPM set by the speed controller, I just won't accelerate past where I am comfortable.
```

---
## \#42 Posted by: kuphjr Posted at: 2019-02-14T20:08:19.226Z Reads: 65

```
This seems to have worked in an instrutable from a few years ago. A digital IMU and using a higher clock rate Teensy over an Arduino should make it even better.
```

---
## \#43 Posted by: Battosaii Posted at: 2019-02-14T22:16:26.418Z Reads: 62

```
That's Ron from my group he's a cool guy but now he's alot more careful he was too fast to hear the beeping and it gave out on him.
```

---
## \#44 Posted by: topcloud Posted at: 2019-02-14T23:06:55.315Z Reads: 59

```
We think your bro is positively heroic for sharing that video; helps us all be safe. Please, convey my sincerest thanks and I appreciate you letting us know, my brother. Be well!
```

---
## \#45 Posted by: Rod12579 Posted at: 2019-02-14T23:45:42.749Z Reads: 52

```
Yeah I was the one who took him to the hospital that night... 💀... respect the beep 🤙🏾
```

---
## \#46 Posted by: Sn4pz Posted at: 2019-02-14T23:53:51.758Z Reads: 53

```
Yes! This is also a huge problem when at speed, you can no longer hear the hum of the motor either  because its so quiet.... no gauge as to how far along the trigger you are :(( 

You really have to be careful with this type of device, as its a guaranteed "superman" dismount when you dive fowards :grimacing:
```

---
## \#47 Posted by: RonsWorldMiami Posted at: 2019-02-15T02:49:57.566Z Reads: 52

```
Hey this is Ronald (AKA) RonsworldMiami. Thanks a lot for watching and sharing with others. The video was meant to let us EUC riders see the danger if we don’t “Respect The Beep”  or choose not to where a helmet! The protective gears saved me from severe injuries I’m  just happy now it was just a  dislocation and two major muscle tear in my shoulder! Better than being brain dead 💁🏾‍♂️. Please wear gear!  I love EUC the video is not to  discourage anyone from riding one I’ll never stop lol I just wish there was better safety features on it. Maybe slow down the rider if he/she is overpowering the unit. The beep going fast you could barely hear it do to wind noise and the helmet. The tilt back is great but if your overpowering the unit and set off the tilt back that might require more power to pull up the rider and eventually causing the unit to fail and face plant the rider lol. I really appreciate you guys for watching and I hope you guys come up with a better safety feature. O from the tons of comments I got on the video it did not hit the car! lol thanks guys and if your ever in Miami come join ESK8MIAMI  and ride with us!
```

---
## \#48 Posted by: RonsWorldMiami Posted at: 2019-02-15T02:59:21.531Z Reads: 46

```
Man i can’t thank you enough for taking me to the Hospital!! I really appreciate it till this day!!
```

---
## \#49 Posted by: mmaner Posted at: 2019-02-15T03:26:34.289Z Reads: 44

```
Hey brother, glad your doing ok. Haven't seen ya since the summer, but I appreciate the videography. It helps people see and hear what esk8 is all about. 

Heal fast and feel better.
```

---
## \#50 Posted by: RonsWorldMiami Posted at: 2019-02-15T03:34:04.080Z Reads: 45

```
Thanks man! I’m doing a whole lot better! It’s about 90 percent healed just som slight pain when I left weights lol but nice to hear from you! Thanks again!
```

---
## \#51 Posted by: b264 Posted at: 2019-02-15T04:10:53.282Z Reads: 51

```
[quote="Sn4pz, post:17, topic:84056, full:true"]
so there are two scenerios when it will beep and provide “push back”

a) you lean your body too far forward for the device and it is thrown out of wack and it gets very angry. It will try to push your feet back and will beep angrily.

b) If youre traveling too fast, it will let you know when you reach the max speed of the EUC, and then apply the “push back” to apply breaks, and will beep if you continue to speed up. BUT BUT BUT IF YOU CONTINUE TO SPEED PAST THE WARNINGS IT GOES COMPLETELY LIMP

***THAT NEEDS TO BE CHANGED***
[/quote]

That can only be changed by making an unlimited-power device, which is against the laws of physics, and, hence, won't be built.

The best you can do is have one that is plenty powerful.

The problem with self-balancing devices is that the device itself is not in control of the speed -- you are -- because the more you lean, the more power has to be applied to keep your face off the street.  At some point you can just keep leaning forward until there isn't enough power to overcome gravity, and you will faceplant.  There is a speed at which that will happen for ***ANY*** eunicycle.  It just means a combination of

1) you must ride responsibly
and
2) don't build/buy cheap shit

But overall I don't like devices that rely on the powered drive train functioning in order to keep your face off the street -- that also includes self-balancing scooters and Onewheels and electric unicycles.
```

---
## \#52 Posted by: kuphjr Posted at: 2019-02-15T16:40:54.390Z Reads: 38

```
I think with 3000W continuous and 4000+ W burst power for 10 sec, I have sufficient power to not worry about pushback or exceeding the wheel’s power. Loud beeps should be plenty to warn me of low voltage which is the only itching thing I have to worry about. I’ll just have it beep once when it drops below 3.5v, twice below 3.4 and so on. At 3.2v I’ll just have it beep like crazy
```

---
## \#53 Posted by: kuphjr Posted at: 2019-02-15T16:42:41.230Z Reads: 42

```
Also a loud beep pattern at +/- 3000W (which I will set at +/-8 degrees) would be nice just to know if I ever even pull 3000W of power.
```

---
