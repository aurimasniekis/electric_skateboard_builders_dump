# Rewinding of hoverboard motor, looking for advices

### Replies: 50 Views: 2410

## \#1 Posted by: Skirra Posted at: 2018-11-28T16:06:41.975Z Reads: 205

```
Hello everyone!

For a while I have been wondering about utilizing super cheap(compared to regular 6374) hoverboard hub motors for my mtb build. I made a experiment and ordered few to play with. In orginal setup they are wired in star, which yielded 11500 erpm and around 10kmh(according to huawei app) with 11s. Later on I resoldered windings to delta, which gave 17500 erpm as expected. 
Since it gave quite low speed output I decided to rewind them for higher kv. Motors have 27 poles and 30 magnets in outer shell. Original windings had following logic: AaABbBCcC ... .
First I removed the old windings and managed to snap away the hall sensors(super easy to do) but it was not big issue since I can run it on sensorless mode. For rewinding I used 1,2 mm winding wire from local shop and made 6,5 turns per one teeth. While constantly measuring for shorts between and inside the stator I finished it after few hours. Unfortunetly when I ran motor I saw really low speed ~3000 erpm and current around 30 amps. After fail I thought maybe I did some winding accidently backward or some other error but after triple cheking everything was fine. Now, when Im out of ideas I came here to ask for some good suggestions or ideas, where I might have made mistakes. I still see quite a lot of potential on those beefy motors :slight_smile:

Here are some pictures: 
![12|281x500](upload://qPZe8bgil4Ue5h6U103qHRgHDt8.jpeg) ![23|281x500](upload://bfnHmlQ5hDRLqy2TNQ8i29IiwGa.jpeg)
```

---
## \#2 Posted by: J0ker3366 Posted at: 2018-11-28T17:00:19.024Z Reads: 185

```
&lrm; @Hummie
```

---
## \#3 Posted by: Hummie Posted at: 2018-11-28T17:10:50.206Z Reads: 188

```
Wow that’s a huge current for a no load spin if that’s what you’re saying.  I’d go to rcgroups.com and ask there. I can’t look at a winding to tell but over there a couple people do that can tell what’s up

But maybe try the winding w a really thin wire and just a turn or two and test then before going the whole hog
```

---
## \#4 Posted by: evoheyax Posted at: 2018-11-28T17:15:47.842Z Reads: 185

```
Interesting project here... If it's as simple as picking up broken hover boards from ebay, and rewinding their motors... I just wonder if these could handle the stresses of 20+mph.

I also wounder, when rewound, how much current they could handle.
```

---
## \#5 Posted by: Skirra Posted at: 2018-11-28T17:27:56.964Z Reads: 172

```
I'll check if anyone here has done anything like this here before moving to rcgroups. I have read quite a bit from here and there but haven't got answers to my questions :slight_smile: 
What you mean by turn or two? Like two turns with thin(how thin is thin in mms?) wire around few teeth? What would be the benefits of doing that? Testing the strength of magnetic field?

@evoheyax Well if you look at their mass and therefore heat dissipation then in theory they might handle quite a bit(still in testing phase). Even better, after you wind it to higher kv with thicker wire than original, you might get even more speed out of them before signs of heating starts to show. There is way too much torque available right now.
```

---
## \#6 Posted by: evoheyax Posted at: 2018-11-28T17:32:04.720Z Reads: 162

```
The point of a few turns is to test that your winding/terminating correctly.

The issue you have is a super low kv resulting in too much torque and not enough speed.

If you do say 2 turns, you should have a really high kv. My advice is to start with a few turns , measure the kv and figure out what your speed will be, and keep adding more turns until your at the right speed for you.

Then, calculate what gauge wire you can get away with, try it, and adjust if needed.
```

---
## \#7 Posted by: Hummie Posted at: 2018-11-28T17:33:17.758Z Reads: 156

```
> Blockquote

If u get some really thin magnet wire that’s easy to wind and put just a couple quick turns(wraps) on each tooth you could test the winding without doing it with hard to manipulate thick wire.the point being to make sure winding correctly.  Then it shouldn’t take anything near 30 amps w no load. 

Depending if u have the room the LRK winding is super failproof and u skip every other tooth.  Or wind two teeth and the one between to see fit
```

---
## \#8 Posted by: evoheyax Posted at: 2018-11-28T17:34:30.609Z Reads: 148

```
The other thing, is before really riding these after you figure that out, you'll want to dip the windings so they don't rattle and cuase a short.
```

---
## \#9 Posted by: Skirra Posted at: 2018-11-28T17:46:12.560Z Reads: 154

```
As I mentioned in orginal post, I made 6,5 turns. Original motor had 13 turns, somehow I assumed it could double the speed :grin: By keep adding you mean unwind the previous wire and do it again? Is there minimum amount of copper that is needed to make enough magnetic field in stator? What you mean by dipping? Applying some adhesive to coils to fix them in place?

@Hummie You can imagine the pain of winding it with this wire. I even managed to mess up at some points so I had to start everything from beginning. This thing sure needs patience.  
I never heard of LRK winding. Is it like partly winding the motor? Some example would be awesome.
```

---
## \#10 Posted by: Hummie Posted at: 2018-11-28T17:50:51.589Z Reads: 146

```
Look up LRK winding. 

The number of turns (wraps) around the tooth produce the torque and it’s independent of how thick it is so u can test with very easy to manipulate thin wire and test the kv and that it’s wound right before using a fat wire. 

Adhesive for the windings is necessary with the vibrations on an esk8.   A very thin epoxy that can take heat
```

---
## \#11 Posted by: evoheyax Posted at: 2018-11-28T17:54:15.086Z Reads: 144

```
Hummie found a company that specializes in motor winding epoxies but they are pricey...

Still, these motors are $30 each on ebay new. Even if it takes another $20 to make them usable, you'r talking $50 a motor which is a great price.

Have you solved the issue of mounting them to a skate truck?
```

---
## \#12 Posted by: Skirra Posted at: 2018-11-28T18:06:26.485Z Reads: 138

```
@Hummie Good tip on the heat conducting epoxy! I'll read a bit about LRK windings.

@evoheyax I hope I can get away with some regular epoxy for start. I just would like to see the concept of reusing those motors in this purpose :) To mount motors to trucks I removed original axle and drilled in lathe with 17mm drill bit. After that I drilled with 8 mm to get the wires to other side. Original grub screw is holding flat side of axle to stop it rotating. Whole setup looks nice and stealthy.
```

---
## \#13 Posted by: Hummie Posted at: 2018-11-28T18:08:29.935Z Reads: 128

```
Heat conducting epoxy is likely filled and will be thick and ultimately hold in the heat ironically.  U want heat resistant more so.
```

---
## \#14 Posted by: Skirra Posted at: 2018-11-28T18:10:27.101Z Reads: 125

```
Wouldn't heat resistant trap the heat inside the coils? I can imagine the venting that is going inside the motor tho.
```

---
## \#15 Posted by: evoheyax Posted at: 2018-11-28T18:11:55.330Z Reads: 115

```
You can use a cheap shitty epoxy to start with. But I wouldn't expect it to hold forever. And it'll hold more heat in also.
```

---
## \#16 Posted by: evoheyax Posted at: 2018-11-28T18:12:24.657Z Reads: 113

```
Is your long term plan to sell these to the public? Or just for yourself?
```

---
## \#17 Posted by: Skirra Posted at: 2018-11-28T18:17:06.279Z Reads: 124

```
Indeed, the idea right now is to test it and how it works. I wont have patience to wind more than two motors anyway, so I'll do it for myself :D I just like that I can order the same motor from local shop for decent price. So I don't have to hold spares and enjoy riding even more. 

But back to the original post. You both suspect the problem might be in the winding configuration? This sure looks like some coils are working against another ones.
```

---
## \#18 Posted by: Skirra Posted at: 2018-11-29T20:52:38.940Z Reads: 115

```
Just for follow-up.
 I did some tests with original windings in delta configuration and 12s. FOC mode yielded 19500 erpm while bldc pumped it up to 22500 erpm. 
BLDC, by my calculations((erpm/pole count)x tire size) could yield theoretical top speed of 30 kmh(enough for me). I guess this could be manageble with dual drive. Initial 10kmh test with 70% efficiency was made with single drive and there might be some drop of performance happening.
```

---
## \#19 Posted by: Joshua1 Posted at: 2018-12-01T07:54:01.811Z Reads: 110

```
I do hope that you might have luck with rewinding. I've only done rewinding on a DC for an RC, so I could make it go faster. I will do some more studying on this.

But one question I had was these motors can you over volt them? I have a motor on my bicycle a 48 volt 1000w and it will normally go 28 mph and I run it with 56 volt and it runs great at about 33 mph now.

Would that work on these motors, and would you just need to get a new controller or maybe use the old one..?
```

---
## \#20 Posted by: Skirra Posted at: 2018-12-01T14:36:59.938Z Reads: 111

```
In the fact it is the easiest way to squeeze more power out of them by overvolting. It gives the same effect as your bicycle motor does. Delta mode which is easy to do also helped quite a bit (square root 3 - 70% more kv). 

For me 12s is the limit, since I would prefer to stay with vescs. It has great diagnostic tool to see whats going on inside the escs and is easy to set up with remotes and stuff. 

Biggest benefit of going higher kv by rewinding would be adding more strands to winding therefore increase maximum current output. There isn't much room but I think 6 strand of 0,5 mm wire with 7-8 turns could be possible.
```

---
## \#21 Posted by: Okami Posted at: 2018-12-01T20:26:30.914Z Reads: 100

```
@Gamer43 how did u get such good speed out of your hoverboard motors? Do u know what their original kv might have been?

I think @Skirra uses 9inch ones but his speed seems to be lower, at least for now
```

---
## \#22 Posted by: Hummie Posted at: 2018-12-01T20:49:34.124Z Reads: 93

```
U could rewind for a better motor but the idea that higher kv can take more current is true but it takes more current out of a higher kv motor to produce torque and in the end there’s no greater efficiency
```

---
## \#23 Posted by: Skirra Posted at: 2018-12-01T21:05:09.704Z Reads: 97

```
@Hummie I fully agree, efficiency isn't quite what I am looking for- rather reasonable speed while staying under 20A current consumption. 
Interesting thing I noticed after I switched from star to delta is that now I'm getting some cogging at start up. I guess that loss of torque is affecting the startup. Any ideas how to fix that?

@Okami I'm running 8 inch version currently to keep board in balance with forward wheels.
Haven't done full speed test in new configuration because of the -10C that is going on outside :grinning: All the good ideas are more than welcome though.
```

---
## \#24 Posted by: Hummie Posted at: 2018-12-01T21:14:25.598Z Reads: 92

```
Higher motor current.  Maybe the phases aren’t all wound with equal turns and imbalanced voltages possible with delta.  If u had a cheap induction meter u can see if the rotor is off.  Higher motor current is an easy try
```

---
## \#25 Posted by: Gamer43 Posted at: 2018-12-01T21:23:41.628Z Reads: 94

```
@Okami
I have a pair of 8-inch hoverboard motors.

Their original top speed at 10S was only 14 mph, which comes out to a KV of about 15. The motors' windings were originally in WYE configuration. I opened up the motors and reconnected the windings to be in DELTA configuration.

The start-up is a little anemic now, as the torque per ampere is reduced by a factor of square-root(3) (and the changes I made to the VESC settings didn't compensate accordingly), but the throttle is much smoother.

I didn't have suitable high-speed front trucks on my board, so speed wobble would start at 16 mph and was really bad at 20+ mph. Sudden changes in acceleration would trigger speed wobble.
```

---
## \#26 Posted by: Skirra Posted at: 2018-12-01T21:27:16.658Z Reads: 84

```
@Gamer43 Mind to share your vesc conf? Been playing few hours with the settings for now, haven't got to a point where Im happy with results. Are you running them in BLDC?
```

---
## \#27 Posted by: Gamer43 Posted at: 2018-12-01T21:40:16.506Z Reads: 91

```
@Skirra
I am running FOC. You will want to run FOC since the torque ripple in BLDC is going to make some noise and cause inefficiencies.
You're going to want your hall sensors....... I noticed that when I reconfigured my motors into DELTA configuration, the Sliding Mode Observer on the VESC couldn't lock on until about 3500 ERPM; when the VESC attempted sensorless transitions below that speed, the motor would cog.
When the motors were in WYE configuration, the motor would cog during start-up if I ran it in purely sensorless mode. The observer has issues at low speeds; no amount of D-axis current injection would stop the cogging. 

You will want to tinker with the advanced settings.
Try a switching frequency of 25khz or higher (this made the most significant improvement), I found the sweet spot for my motors around 29-31khz.
Set Dead-Time Compensation to 0.600uS.
Set minimum current to 1 or 2 A (this was just so I wouldn't get obnoxious whining at really low throttle),
Motor Current is +-30A 
Battery Current is +-10A.
Again, start-up (on a hill) was a little anemic with these settings, 40A motor current should be sufficient for flat and hill starts.
(I apologize for not posting screenshots, the settings for some reason didn't save in VESC tool and my VESCs are locked away in an aluminum enclosure, I'll post screenshots if I have time).

If you are unable to get satisfactory results running the motor with a VESC, I recommend trying them with one of those "sinusoidal/FOC" ebike controllers, though not sure if you can find one that will work at 10S. They are actually cheaper than VESCs, but many are not programmable and are a bit bulky.
```

---
## \#28 Posted by: Skirra Posted at: 2018-12-01T22:21:25.477Z Reads: 94

```
@Gamer43 ank you for this informative post! I reconfigured my motor tab, went a lot lower with my current values and inserted same values as you told. 

After that I did FOC detection and tried if cogging is still there. This time it was gone and with enough throttle I could start from dead stop. I guess some sacrifises has to be done to get better low speed performance. 

With DTc at 0.6 there was some weird behaivour. Motor was cogging higher speeds quite violently which made me lower it to 0,1.  

With switching frequency I noticed some improvements as well. It seemed most stable between 29k - 31k as you said.

Thank you once again! Here is my conf for future readers.
![vesc%20settings%20hub|690x408](upload://sjTxN3Y7BQJ6BCvacRl6TdrOtpu.png)
```

---
## \#29 Posted by: Mich21050 Posted at: 2018-12-01T22:49:00.898Z Reads: 76

```
Why are you using the bldc tool instead of the new vesc tool? :slight_smile:
@Skirra
```

---
## \#30 Posted by: Skirra Posted at: 2018-12-04T16:53:31.202Z Reads: 70

```
@Mich21050 When I bought focboxes I downloaded software from their website and have been sticking with this for now. Am I missing some vital features compared to vesc tool?
```

---
## \#31 Posted by: Mich21050 Posted at: 2018-12-04T16:54:19.855Z Reads: 70

```
As far as I know you don't but maybe someone who has a focbox can help.... I'm only using "normal" vescs :slight_smile:
It's just the newer version...
```

---
## \#32 Posted by: Deodand Posted at: 2018-12-04T17:14:43.161Z Reads: 73

```
Are you still interested in rewinding? Currently in delta configuration you are looking at a kV of ~ 24 mech. rpm/V. If you give me all the info on the stator dimensions:

*stator inner and outer diameter (without the metal 3 prong piece) 
*slot depth
*sslot width
*slot opening width

And rotor dimensions:
*Magnet thickness
*Can thickness
*inner diameter to magnets

I've been using some simulation tools that can devise a winding pattern for you that will give you your desired kV. I'm interested to test how accurate it is in a real world application if you want to give it a go.
```

---
## \#33 Posted by: Skirra Posted at: 2018-12-04T17:52:06.928Z Reads: 66

```
@Deodand Sure no problem. I would more than thankful for some simulation. 
Do you need simply dimensions or .step file would do as well? It would be interesting to see the magnetic wave behaviour :slight_smile:

I think i'll try rewinding soon once again, my hands are already healed from last time :stuck_out_tongue_winking_eye:
```

---
## \#34 Posted by: Skirra Posted at: 2018-12-04T18:22:26.896Z Reads: 70

```
@Deodand Here you can see the requested dimensions. I quickly modelled this motor, minor hand measurment errors might be there. https://drive.google.com/open?id=1mktiQDosbIz0QMT4VzFiifR7NJLBpWP3 
.step file https://drive.google.com/open?id=10YITC8aa49_Q1IHteUZtwr1f63NU5sRi
```

---
## \#35 Posted by: Deodand Posted at: 2018-12-04T19:59:33.211Z Reads: 76

```
![image|508x500](upload://yOnJjhnvLFtH3y8AQ4nCpCbeyRA.png) 

Yeah, so used a similar AaABbBCcC winding pattern. See the above image for slot fill. With your 1.2 mm wire and 6.5 turns per tooth you should have seen a kV around 82 rpm/V in the WYE connection pattern fill density of 20% and a winding resistance of  70 mOhm. At 10 turns the kV should be around 52 rpm/V with a slot fill factor of 30% and resistance of 105 mOhm. 15 turns per tooth should get you a kV of around 35 rpm/V in the WYE connection with a fill factor of 46% and a resistance of 158 mOhm. 

I'd recommend 10 turns per tooth with a Y connection I think. It might make your life easier to use 3 parallel strands of 0.7mm wire or 2 of 0.8mm wire which will behave similar in every way but may be easier to bend into the slots etc. 

 Not sure why your windings before didn't work though, definitely a concern. Here's a few little plot of 10 turns per tooth Magnetic flux for fun: 
![image|551x500](upload://oUvzRtQG8dfoLkrLTKSqbJxVWDU.png)
```

---
## \#36 Posted by: Skirra Posted at: 2018-12-04T20:25:02.796Z Reads: 75

```
@Deodand Thanks for screenshots! What does those red spots at the ends mean?
Also can you simulate situation where wire is 1-2 mm away(offset) from stator teeth? I think this might be cause of my issue since wire might be too far away. Would be interesting to see, how it looks like in that case.
Is it possible that one pole could cancel the opposite one if they are too close? (current flow is opposite)

If we look at the calculation. Is it electrical or mechanical rpm?
```

---
## \#37 Posted by: Deodand Posted at: 2018-12-04T20:31:17.885Z Reads: 77

```
Mechanical RPM, multiply by 15 for ERPM. I don't think the problems with gap between wire and stator teeth  are causing the issue you are seeing. You would see this as some inefficiencies whereas what you describe is basically it not working nearly at all.  Probably an error in your winding pattern somewhere/somehow.

The red spots are just zones of high magnetic field concentration, probably more iron losses there since the material will get re-magnetized. Could also just be artifacts from FEA who knows.
```

---
## \#38 Posted by: Pedrodemio Posted at: 2018-12-04T21:05:02.146Z Reads: 73

```
This is MotorAnalysisPM right? been playing with it, amazing tool
```

---
## \#39 Posted by: Deodand Posted at: 2018-12-04T22:36:16.671Z Reads: 73

```
lots of fun
```

---
## \#40 Posted by: viewtop1 Posted at: 2019-02-14T16:55:20.966Z Reads: 64

```
@Deodand
Any chance you still have the Motoranalysis sim files and DXF's within reach. I must be doing something wrong, but I simply cannot get the hoverboard motor modeled.

I want to use a hub motor as a direct drive for my CNC Mill, but so am trying to work out what the turns ratio and if it is even feasible. 

Out of interest, what is the minimum amount of turns you could safely use?  3 turns? 2 turns?
I am hoping to get about 4000 to 5000 rpm out with a 28V supply, but I could also use a 48v supply.

Would be very greatfull if you could upload the sim files please.  This is the first time I am trying this kind of thing and have so far failed miserably.

Thanks
```

---
## \#41 Posted by: ElectricWizard Posted at: 2019-03-26T13:26:26.978Z Reads: 56

```
Hey If people are still interested in this thread. I have found that my motors (6.5) inch (hoverboard) when using FOC with VESC and a 13S battery from my E-Bike i get about 30-35 KPH. Its tolerable but definitely slow for longer rides. Now im calculating i could get about 38-42 KPH if i just swap the hard tire from a 6.5 inch one to an 8inch one and keep the original motors wired as is to keep some of that torque that will now be needed to startup. Also to everyone that will tell me wtf 13S wtf FOC you will blow up the chip... Actually its all fine and safe because the VESC clearly states that max voltage is above 13S, and that problem with FOC is only present in higher KV motors because of E-rpm being too big. This motor has somewhere between 10-25kv so insanely low.

Ill keep you guys updated once i get the new tire from ali express and install it.
```

---
## \#42 Posted by: Hummie Posted at: 2019-03-26T14:44:21.555Z Reads: 50

```
The low erpm is safe with 13s but you can still get voltage spikes and I think more so with such high inductance
```

---
## \#43 Posted by: ElectricWizard Posted at: 2019-03-26T15:34:45.728Z Reads: 48

```
Agreed, Would that be solved if i added capacitors to smooth voltage spikes on the motor phases? Is that even feasible?
```

---
## \#44 Posted by: ElectricWizard Posted at: 2019-03-26T15:39:07.077Z Reads: 47

```
I just thought about it and it would require some complex calcs to analyze the RLC circuit that would create (Resistance in motor windings, Inductance from looped windings and metal core and capacitors that i would be addind in phase wires). Not sure but it might actually make sense to make a damped circuit with AC calculations.
```

---
## \#45 Posted by: Deodand Posted at: 2019-03-26T15:49:26.402Z Reads: 48

```
Don't add caps or series resistance here. Neither of those will help anything. Some people have added 60V TVS (transient voltage spike) diodes to the phases but fets already have internal flyback diodes that perform similar function. Anyways I'd say if it isn't broken don't fix it. But yea no amount of rationalizing will help when you start getting close to absolute maximum ratings. Just increases the odds of things failing. Lots of people run 13s just fine though :man_shrugging:
```

---
## \#46 Posted by: ElectricWizard Posted at: 2019-03-26T15:56:35.763Z Reads: 48

```
I do agree that derating components is important and i fully understand that the lifespan of my cheap hobbyking VESC 2.14 will not be very long when i run it at near max voltage all the time. But for me the benefit of having one hoverboard motor in the rear and 2 wheels in the front make for a cool 3 wheels electric skateboard and outweigh the rewinding motor route for me personally. 

I think the only options we really have with these hub motors are to either :
-Overvolt
-Change outter diameter of tire
-Rewind motor coils
```

---
## \#47 Posted by: Rik_B Posted at: 2019-10-14T22:24:02.689Z Reads: 25

```
I know the origional post is nearly a year old now, and as such is unlikely,  however, if the winding problem is still troubling you, I think I've seen where the fault might be.
Each time you complete the winding of three teeth, and then skip 6 and begin winding again, I think that first tooth has only 6 turns, not 6.5

![20191014_225653|281x500](upload://dqXeqrm6pxrO1mYnUVFqi95d7SQ.jpeg) 

The windings on the highlighted teeth seem to begin and end on the same side of the stator, meaning a whole number of turns.
This does not happen on the first winding, as the phase wires begin on the opposite side of the stator, giving the extra .5 turn
```

---
## \#48 Posted by: bewater Posted at: 2020-01-12T23:28:05.185Z Reads: 12

```
Hello from Argentina! I don't know if this is the right place but it's the closest information I found. Someone would be kind enough to give me information about how to standardly rewind a hoverboard engine, 27 slots 30 magnets, since I only find modifications or RC engines. I would appreciate a scheme with turns per tooth, the direction of the turns and the thickness of the cable. Yes, I know it may be too much but I am sure that for those who publish here it is nothing but a very easy thing. Thank you in advance! (sorry for my google english)
```

---
## \#49 Posted by: Hummie Posted at: 2020-01-13T20:04:56.443Z Reads: 13

```
http://www.bavaria-direct.co.za/
```

---
## \#50 Posted by: Okami Posted at: 2020-01-14T19:48:16.250Z Reads: 12

```
@bewater 
U could also try to ask for info on Odrive forum, quite advanced user base, if u ask me:

https://discourse.odriverobotics.com/t/project-hoverarm/441/10?fbclid=IwAR3n9rC6XgFcREzKkjF7NUTpQJ8k5Pu-eCoAUdaw_d5fIIeuGYo0ShGRjsA
```

---
