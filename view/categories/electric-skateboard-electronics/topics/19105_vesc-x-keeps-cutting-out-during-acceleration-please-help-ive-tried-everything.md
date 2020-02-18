# Vesc x keeps cutting out during acceleration please help ive tried everything

### Replies: 93 Views: 3776

## \#1 Posted by: Goo-shtick Posted at: 2017-03-15T18:33:45.105Z Reads: 237

```
I have a 10s4p pack that's kinda frankenstiened back together because I moved the lcd and had to change the chargeport and on / off switch  its a dual 190kv TB motors and 2 vesc x controllers with the mini remote and its worked great till now this problem happened before too and I took everything apart and did some things in bldc tool I think but don't remember exactly what and it fixed the problem for a while don't know what the problem was but now its back it cuts out under hard acceleration and wont go again till you tap the brakes then it resets right away but does the same thing again when you accelerate again I want to think I have something in bldc tool wrong cuz ive taken it apart a lot of times and resoldiered everything and it does nothing still cuts out. it runs fine on the bench with no load but as soon as you get on it and accelerat it cuts out. note if accelerate really slow and barely feather the throttle you can get it to go up to speed but the second you give it too much it cuts out . please help motor detection works fine and shows no faults and im unable to keep a laptophooked up while riding . could it be a faulty motor ?
```

---
## \#2 Posted by: Blasto Posted at: 2017-03-15T18:35:58.838Z Reads: 223

```
My eyes are hurting, post your bldc settings and pictures of your setup.
```

---
## \#3 Posted by: Goo-shtick Posted at: 2017-03-15T18:53:40.424Z Reads: 216

```
on my lunch I will try to snap shots of all my settings  and board
```

---
## \#4 Posted by: Namasaki Posted at: 2017-03-15T20:16:05.869Z Reads: 200

```
I'll take a stab in the dark. 
I'm guessing because it doesn't cut out with slow acceleration but it cuts out with quick and sudden acceleration. 
I think the problem is your drawing too many amps for your batteries and sagging the voltage so that it's tripping the Vesc low voltage protection. Maybe your low voltage cut off is set too high.
```

---
## \#5 Posted by: Goo-shtick Posted at: 2017-03-15T20:50:00.922Z Reads: 198

```
<img src="/uploads/db1493/original/3X/1/5/15db03ff3f21ba6df6b9bbde89f5b7dbbb081310.JPG" width="320" height="240"><img src="/uploads/db1493/original/3X/c/d/cd4dbf7be9582c095d0ce88119f3adffc80b31d3.JPG" width="320" height="240"><img src="/uploads/db1493/original/3X/f/f/ff03c82d1ff4882951cbe92a65bb621ff4c750d0.JPG" width="320" height="240"><img src="/uploads/db1493/original/3X/f/6/f67e8ce530305ef223ae5110ff23177219af8239.JPG" width="320" height="240"><img src="/uploads/db1493/original/3X/c/8/c8762aa9c6aff17d7c4fb5dc0fcdac06eb25fb13.JPG" width="320" height="240"><img src="/uploads/db1493/original/3X/7/9/7927896fcb883d208c69d90da07d7c0fe15dd9fc.JPG" width="320" height="240"><img src="/uploads/db1493/original/3X/a/6/a65928ad86efef2fa37e69cc2c44cc8aab5143f1.JPG" width="320" height="240"><img src="/uploads/db1493/original/3X/b/5/b536536ff2fd88da39bd8fa8b2dd66b184f7535e.JPG" width="320" height="240"><img src="/uploads/db1493/original/3X/e/8/e8ed8f51ba631a5003eca0a4ab91e604aff594de.JPG" width="320" height="240"><img src="/uploads/db1493/original/3X/0/0/009319f71ce51ac70b565fc4f8b5496e382eaeb3.JPG" width="320" height="240"><img src="/uploads/db1493/original/3X/7/5/7544b54baaf8b0564655ed67217aea5955fa7564.JPG" width="320" height="240"><img src="/uploads/db1493/original/3X/1/3/13e1832e15e7fe474dbf0005a706788eb99849cc.JPG" width="320" height="240"><img src="/uploads/db1493/original/3X/7/8/78fdbd4684e9209de32f6b141d8d089c6aa62860.JPG" width="320" height="240">
```

---
## \#6 Posted by: Blasto Posted at: 2017-03-15T20:55:19.449Z Reads: 183

```
My eyes hurt even more haha

Motor max 60A
Motor min -60A
Batt max 25A
Batt min -14A (adjust this for braking power)

Max input voltage 57V

I'm not able to see your battery cutoff start and end
```

---
## \#7 Posted by: Namasaki Posted at: 2017-03-15T21:01:20.307Z Reads: 183

```
Your pics are too blurry. Try using screenshot function.
```

---
## \#9 Posted by: Blasto Posted at: 2017-03-15T21:13:38.542Z Reads: 181

```
Most likely the batt max the problem, 60A on each vesc is beating the shit out of that poor 10S4p

So i think your swing in the dark is correct
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2017-03-15T21:15:37.298Z Reads: 181

```
[quote="Goo-shtick, post:1, topic:19105"]
I have a 10s4p pack that's kinda frankenstiened
[/quote]

How did you put your battery back together... I think it might be a bad cell somewhere in your rework.
```

---
## \#11 Posted by: Goo-shtick Posted at: 2017-03-15T21:32:51.551Z Reads: 174

```
So what should I set them at
```

---
## \#12 Posted by: Blasto Posted at: 2017-03-15T21:33:30.284Z Reads: 176

```
[quote="Blasto, post:6, topic:19105, full:true"]
My eyes hurt even more haha

Motor max 60AMotor min -60ABatt max 25ABatt min -14A (adjust this for braking power)

Max input voltage 57V

I'm not able to see your battery cutoff start and end
[/quote]

Quoting myself, sounds pretty awsome
```

---
## \#13 Posted by: Goo-shtick Posted at: 2017-03-15T21:33:54.631Z Reads: 168

```
I never disconnected any of the cells just the switch and the charge port and moved th LCD screen
```

---
## \#14 Posted by: Namasaki Posted at: 2017-03-15T21:36:38.954Z Reads: 167

```
What type of switch
```

---
## \#15 Posted by: Goo-shtick Posted at: 2017-03-15T21:39:44.276Z Reads: 170

```
It's a automotive type switch I know it's not an anti spark but I have a lot of them so I don't mind if they fail
```

---
## \#16 Posted by: Goo-shtick Posted at: 2017-03-15T21:40:35.513Z Reads: 171

```
It starts at 30 and ends at 28
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2017-03-15T21:42:15.987Z Reads: 167

```
But did made your pack yourself or did you bought it of the shelf...
```

---
## \#18 Posted by: Goo-shtick Posted at: 2017-03-15T21:44:53.166Z Reads: 167

```
It's one of dexters packs from diyelectric
```

---
## \#19 Posted by: Namasaki Posted at: 2017-03-15T21:52:13.528Z Reads: 166

```
Is it made with 25R cells ?
Rumors have it that they sag a lot. 
But unless your a big guy trying to accelerate hard uphill, I think the switch is still and will always be the problem here
```

---
## \#20 Posted by: Namasaki Posted at: 2017-03-15T21:56:04.881Z Reads: 162

```
You see, the switch has contacts that are suffering severe arcing every time you turn it on. The arcing destroys the contacts and at the least causes resistance at the switch. Even a brand new switch is ruined the first time you turn it on.
```

---
## \#21 Posted by: Namasaki Posted at: 2017-03-15T22:00:32.118Z Reads: 155

```
Wait, don't TB's batteries come with an E-switch built in?
```

---
## \#22 Posted by: Goo-shtick Posted at: 2017-03-15T23:01:38.135Z Reads: 142

```
yes but it got damaged
```

---
## \#23 Posted by: Goo-shtick Posted at: 2017-03-15T23:04:52.960Z Reads: 141

```
so you think that my board is cutting out because of the switchs im using?
```

---
## \#24 Posted by: Namasaki Posted at: 2017-03-15T23:04:57.554Z Reads: 141

```
Try connecting your battery without the switch and take it for a test ride and see if it still cuts out
```

---
## \#25 Posted by: Namasaki Posted at: 2017-03-15T23:05:39.933Z Reads: 143

```
[quote="Goo-shtick, post:23, topic:19105, full:true"]
so you think that my board is cutting out because of the switchs im using?
[/quote]


Yes I do. If anyone agrees with me click the like below
```

---
## \#26 Posted by: JohnnyMeduse Posted at: 2017-03-15T23:10:14.110Z Reads: 135

```
can you post some picture, it look like you made quite few modification to the original parts.
```

---
## \#27 Posted by: Goo-shtick Posted at: 2017-03-15T23:15:24.513Z Reads: 141

```
<img src="/uploads/db1493/original/3X/4/b/4b64eace31ed9d11b8a63a3b19c2655e68c52c00.JPG" width="640" height="480"><img src="/uploads/db1493/original/3X/9/2/9216dc3a8e416803e737a88c61e1224aaadb11b0.JPG" width="640" height="480"><img src="/uploads/db1493/original/3X/7/f/7f6db6466a8606b5220365adce276ba14dfbe003.JPG" width="640" height="480">
```

---
## \#28 Posted by: JohnnyMeduse Posted at: 2017-03-15T23:19:10.362Z Reads: 138

```
how the switch is plug ? And how do you manage to control the charging of your battery, did you leave the BMS inside ?

Also, some brand of hot glue have a really poor dielectric, that can cause some short at high current.
```

---
## \#29 Posted by: Goo-shtick Posted at: 2017-03-15T23:23:44.347Z Reads: 137

```
bms is still there
```

---
## \#30 Posted by: Namasaki Posted at: 2017-03-15T23:24:09.222Z Reads: 134

```
Looks like you still have the E-switch as well
```

---
## \#31 Posted by: Goo-shtick Posted at: 2017-03-15T23:24:58.702Z Reads: 132

```
its just a rocker switch I got from my work
don't think its special
```

---
## \#32 Posted by: Namasaki Posted at: 2017-03-15T23:25:45.147Z Reads: 129

```
But it's connected to small green and red wires that go to a circuit board. that's the E-switch
```

---
## \#33 Posted by: Goo-shtick Posted at: 2017-03-15T23:26:47.478Z Reads: 127

```
and the hot glue the same I use at work im a vibe technician for tesla and I use it to glue accelerometers on all the d.u.t's
```

---
## \#34 Posted by: Goo-shtick Posted at: 2017-03-15T23:27:39.017Z Reads: 126

```
I added those wires
```

---
## \#35 Posted by: Namasaki Posted at: 2017-03-15T23:29:27.489Z Reads: 126

```
Where do those wires connect to?
And btw I just checked your battery is made with LG HE2 cells
I think those are good cells but I'm not sure.
@PXSS would probably know about that
```

---
## \#36 Posted by: Goo-shtick Posted at: 2017-03-15T23:31:48.929Z Reads: 123

```
those wires conn to the wires that old switch was conn to but as to where those go im not sure if I paid attention to that when I had it apart I just soldered the red and green on to the ends and put that switch in
```

---
## \#37 Posted by: Goo-shtick Posted at: 2017-03-15T23:33:55.221Z Reads: 126

```
that batterey has been a nightmare first the charge port went and then my solder job went and then lcd screen stopped working and in betwwen all those was dissection and duct tape and lots of screwing around with it and then bms got wet and had to take apart and dry out
```

---
## \#38 Posted by: Goo-shtick Posted at: 2017-03-15T23:34:40.279Z Reads: 132

```
ive got just a hair under 4,000 miles on this board in like 3 months lol
```

---
## \#39 Posted by: Goo-shtick Posted at: 2017-03-15T23:36:16.895Z Reads: 126

```
ive  hit 48 mph downhill on it it does 38 on flat well it did:(
```

---
## \#40 Posted by: Namasaki Posted at: 2017-03-15T23:40:35.249Z Reads: 126

```
Hey, thats really fast. Are you a downhill long boarder?
About the wires. I'm sure they go to an E-switch so that's not the problem after all.
```

---
## \#41 Posted by: Blasto Posted at: 2017-03-15T23:48:29.393Z Reads: 121

```
Change your settings to what i suggested in post 6
  
 http://www.electric-skateboard.builders/t/vesc-x-keeps-cutting-out-during-acceleration-please-help-ive-tried-everything/19105/6?u=blasto

Your battery current is way to high on each vesc

You can always get the error if the vesc cuts out, if theres no error code, you're mostlikely hitting the low voltage cutoff
```

---
## \#42 Posted by: treenutter Posted at: 2017-03-16T00:01:26.165Z Reads: 121

```
[quote="Goo-shtick, post:38, topic:19105, full:true"]
ive got just a hair under 4,000 miles on this board in like 3 months lol
[/quote]

Wait what? you're riding 45 miles a day? Awesome!

Did we ever see the voltage cutoff parameters?
```

---
## \#43 Posted by: Blasto Posted at: 2017-03-16T00:08:42.917Z Reads: 116

```
[quote="treenutter, post:42, topic:19105"]
Did we ever see the voltage cutoff parameters?
[/quote]

We think its 33-30V, which is fine. Whats not fine is the batt max set at 60A... that's 120A on the battery
```

---
## \#44 Posted by: Ackmaniac Posted at: 2017-03-16T00:19:09.729Z Reads: 118

```
What voltage does the vesc show in the Realtime tab. Are you sure the battery is charged at the moment? 
And as @Blasto said already. You might overstressed the battery.  When you have a gearing that can do 38 mph on flats and still accelerates till 48 mph downhill then your battery worked most of the time on full power and as it seems even above. Short bursts are normally fine but if you go uphill with that gearing it's not a burst anymore. 
Didn't the VESC reduce the power because of overheating or do you use the Vesc-X? 

Finally it can be another issue. You could also buy a Bluetooth module and use my app to know what's the problem.
You can also try to add a USB cable to the VESC and tide it till you have the problem and then connect it directly to the PC (don't switch the board off) and type "faults" in the terminal tab. If you see something then let us know.
```

---
## \#45 Posted by: Goo-shtick Posted at: 2017-03-16T00:36:00.543Z Reads: 114

```
yes I do lots of downhill
```

---
## \#46 Posted by: Goo-shtick Posted at: 2017-03-16T00:37:44.492Z Reads: 116

```
i set mot max and regen to 60 , -60 and batt max to 25 tried it and it cuts out even sooner and the cutoffs are 30 and 28
```

---
## \#47 Posted by: Goo-shtick Posted at: 2017-03-16T00:39:29.409Z Reads: 113

```
i guess when i get off work i will hook my laptop back up to it and try and ride it and watch for the fault code or ?
```

---
## \#48 Posted by: JohnnyMeduse Posted at: 2017-03-16T00:48:00.743Z Reads: 109

```
Yeah, this could really help.
```

---
## \#49 Posted by: willpark16 Posted at: 2017-03-16T00:51:57.139Z Reads: 108

```
Careful with that battery i think it's a bms issue this sounds like the same issue I had
```

---
## \#50 Posted by: Namasaki Posted at: 2017-03-16T01:18:34.848Z Reads: 106

```
@willpark16 may have something there. The bms could be cutting out at high current demand.
You could bypass the bms and run the power cables straight to the vescs for a test to see if it stops cutting out.
You would see a huge spark though unless you connect it with an anti spark connector.
Too bad you don't live in San Diego, I have an extra anti spark bullet connector laying around that I used on my first build.
```

---
## \#51 Posted by: Goo-shtick Posted at: 2017-03-16T04:32:16.619Z Reads: 103

```
so I ran it with laptop connected and the fault code says undervoltage
```

---
## \#52 Posted by: Blasto Posted at: 2017-03-16T04:34:31.042Z Reads: 102

```
That narrow's it down to the battery or bms. Are you able to probe the sense cable to si if there's a parallel pack that is significanly lower than the others?

(I'm leaning towards a battery problem)

One bad cell will bring the parallel pack down, the parallel pack will bring the whole pack down
```

---
## \#53 Posted by: Goo-shtick Posted at: 2017-03-16T04:36:41.180Z Reads: 95

```
I have to dissect the battery I mean ductape pack lol ill do right now gunna go get my board out of truck just got off work they should rename Tesla ,  Stresla lol
```

---
## \#54 Posted by: Blasto Posted at: 2017-03-16T04:38:35.019Z Reads: 97

```
[quote="Goo-shtick, post:53, topic:19105"]
I have to dissect the battery
[/quote]

Just be very carefull, those batteries have some bite to them.

Try to keep it simple without destroying your whole build, try to access the sensor connector. (Large 11 or 10 pin connector that goes to the bms)
```

---
## \#55 Posted by: Namasaki Posted at: 2017-03-16T05:06:30.257Z Reads: 93

```
Before you go any farther, please tell me, how full is your battery pack when the cutting out is happening.
Is it a full 42 volts or close to that?
```

---
## \#56 Posted by: Goo-shtick Posted at: 2017-03-16T05:38:46.816Z Reads: 92

```
its at 38 now but yes it cuts out on full charge
```

---
## \#57 Posted by: Blasto Posted at: 2017-03-16T05:41:10.649Z Reads: 92

```
[quote="Goo-shtick, post:56, topic:19105"]
cuts out on full charge
[/quote]

Set your max input voltage at 57V, before anything else
```

---
## \#58 Posted by: Goo-shtick Posted at: 2017-03-16T05:43:53.116Z Reads: 92

```
I did that earliar
```

---
## \#59 Posted by: Namasaki Posted at: 2017-03-16T05:44:25.237Z Reads: 92

```
After checking your parallel packs and if they check out ok, you might try bypassing the bms on for discharge to see if it is cutting voltage because of the high current draw.
```

---
## \#60 Posted by: Goo-shtick Posted at: 2017-03-16T05:44:30.622Z Reads: 90

```
what am I probing for im looking at bms now
```

---
## \#61 Posted by: Namasaki Posted at: 2017-03-16T05:45:17.779Z Reads: 88

```
I'm pretty sure that bms is only rated for 30a and thats not gonna cut it if your discharging through the bms
```

---
## \#62 Posted by: Namasaki Posted at: 2017-03-16T05:46:05.875Z Reads: 83

```
Do you know how to bypass the bms for discharge?
```

---
## \#63 Posted by: Blasto Posted at: 2017-03-16T05:47:17.762Z Reads: 84

```
[quote="Namasaki, post:61, topic:19105"]
I'm pretty sure that bms is only rated for 30a and thats not gonna cut it if your discharging through the bm
[/quote]

But his bms took it for a while, that's why im thinking it's the cells
```

---
## \#64 Posted by: Namasaki Posted at: 2017-03-16T05:49:34.881Z Reads: 81

```
@willpark16 mentioned that he had a problem with his bms on a similar pack
I think if the cells check out ok, then I would try bypassing the bms next
```

---
## \#65 Posted by: Goo-shtick Posted at: 2017-03-16T05:56:10.871Z Reads: 83

```
so the tabs that the balance leads go to looks like they go down roughly like 4 volts as I go down to the bottom of bat 34.00, 30.00 and the next one says only 3.4 and then it goes back to 26.00 and then 22.00 then 7.4 are they supposed to be in order or is this normal
```

---
## \#66 Posted by: Namasaki Posted at: 2017-03-16T06:08:58.301Z Reads: 84

```
They are in order but the best way is to isolate each parallel group with the volt meter
each parallel group of 4 cells represents 1s  so as you go down the line in series the voltages of each group adds in

group 1 will be the end of the battery that supplies the negative (black wire) output
group 10 will be the end of the battery that supplies the positive (red wire) output
```

---
## \#67 Posted by: Namasaki Posted at: 2017-03-16T06:18:24.388Z Reads: 82

```
If you can unplug the balance harness from the bms, you can check voltage of each group at the balance connector.
```

---
## \#68 Posted by: willpark16 Posted at: 2017-03-16T06:24:47.344Z Reads: 81

```
Ask him before U open!!! He will not replace no matter weather it was faulty before or not
```

---
## \#69 Posted by: Namasaki Posted at: 2017-03-16T06:49:17.096Z Reads: 83

```
too late, its already been opened and modified
```

---
## \#70 Posted by: Namasaki Posted at: 2017-03-16T06:54:16.543Z Reads: 86

```
Here is a chart I whipped up showing how to check individual cell group voltages at the balance connector.
This is for bms's with 10 pin connectors. If your bms has 11 pin connector, you can still use this method or use the ground wire on the balance connector for the neg side of cell group 1.
<img src="/uploads/db1493/original/3X/e/0/e0f9b61540e0f46b910c58d4d2f018277946e38a.png" width="662" height="500">
```

---
## \#71 Posted by: PXSS Posted at: 2017-03-16T11:27:50.723Z Reads: 85

```
Ok. I just got to read the whole thread. It looks like you killed your cells. HE2s are okay cells but if you had duals drawing up to 60A each, that means 120A total on a 4P, comes out to 30A per cell. If you ran it like that for a while, you definitely stressed out your cells and I wouldn't be surprised if their internal resistance has gone up significantly. 

What this all means is that your cells will sag A LOT so that whenever you throttle hard, they hit the voltage cutoffs you have set. Once you let go, the voltage rises and you can ride again. Until you hit the throttle hard and the voltage sags again. 

Try this, set your cutoff start at 30V and your cutoff end at 28V. If that doesn't work, try 28V as start and 26V as end. If either fixes it, then it's your battery and you'll have to consider replacing it soon.

E: I would also suggest bringing your max batt current down to 20A on each ESC and upping the motor max current if torque is an issue at low speeds. Also Min batt current to -10A and -60A motor min.
The big ones though are the cutoffs I stated above.
```

---
## \#72 Posted by: Goo-shtick Posted at: 2017-03-16T18:05:48.661Z Reads: 73

```
so I took it all apart and found that under the switch it was massively arcing and chared where it was shorting out on a piece of exposed metal so I re soldedrd and put back to gether and still cuts out at lunch today I will lower the cutoffs to 28 and 26 and hope that works if so  I know battery wont last much longer  so which one should I get I like the tb 6355 motors and I have 3 of them so something that would work with them they are 190 kv
```

---
## \#73 Posted by: PXSS Posted at: 2017-03-16T19:22:46.762Z Reads: 73

```
No offense but I honestly suggest you have someone more experienced look at it. This thread screams fire hazard to me... you're lucky that short didn't fry your battery.
```

---
## \#74 Posted by: Goo-shtick Posted at: 2017-03-16T20:11:24.421Z Reads: 76

```
really? that's not very nice. its not like you were born with all this knowledge in complex motor controllers . you had to start somewhere and ive been building hotrods and vintage custom cars my whole life and it is called diy is it not? im not the guy that brings his car to the mechanic for a blown head gasket or engine swap that's not how I was raised sorry and everyone on this forum has been very helpful thank you. and btw everyone problem has been solved and now I have the experience in troubleshooting a good amount on the vesc and battery pack and I can share it with others sorry didn't mean to get all puffed up that shouldn't have offended me but it kinda did
```

---
## \#75 Posted by: Blasto Posted at: 2017-03-16T20:12:53.040Z Reads: 74

```
[quote="Goo-shtick, post:74, topic:19105"]
problem has been solved and now I have the experience in troubleshooting a good amount on the vesc and battery pack
[/quote]

Good stuff man!

What was the root cause?

(I go to the mechanic's for a blown head gasket haha)
```

---
## \#76 Posted by: Goo-shtick Posted at: 2017-03-16T20:14:26.981Z Reads: 72

```
  Vesc x keeps cutting out during acceleration please help ive tried everything 
PROBLEM SOLVED you guys were right  my settings have overstressed my cells and I just had to set my voltage cutoffs really low to accommodate, good learning experience im in the market for a new pack soon I guess
```

---
## \#77 Posted by: PXSS Posted at: 2017-03-16T20:33:14.988Z Reads: 73

```
Not trying to be a douchebag! Don't take it the wrong way. It's just that your life is at stake here. A short like the one you described could easily cause your batteries to explode and catch fire. I've seen these batteries blow and burn, it's not a pretty sight and it also isn't something you can kill with a regular fire extinguisher. Having that happen under your feet could be deadly...
```

---
## \#78 Posted by: Ackmaniac Posted at: 2017-03-16T20:35:12.924Z Reads: 73

```
I am curious. Whats your motor kv and how many teeth does your motor and wheel pulley have.
```

---
## \#79 Posted by: PXSS Posted at: 2017-03-16T20:36:31.613Z Reads: 74

```
Also, your voltage cutoff should never go below 25V, that is the limit for your batteries. The reason I suggested 26V is because your cells could also be out of balance which means one of the 10 packs could dip under 2.5V.

I still recommend that you check the individual voltages and make sure that they are still in balance. If not, leave it plugged in overnight and see if they get balanced. If that doesn't work you'll have to buy an rc charger and balance them manually.
```

---
## \#80 Posted by: Goo-shtick Posted at: 2017-03-17T16:51:03.542Z Reads: 72

```
I Think im just gunna call this pack doomed and done for maybye ill dissect it later on and get rid of the stupid usb chargeports and all the hot glue and ductape crap and make a spare pack out if it . btw I am running 6355 tb motors 190 kv and 36/18 gearing (I like to go as fast as possible I always have 40 is borderline fast enough anymore I would be content with 45 on flat I think . lol
```

---
## \#81 Posted by: Ackmaniac Posted at: 2017-03-17T16:59:36.666Z Reads: 72

```
And what is your wheelsize? But in your case with that high gearing I would recommend lipo batterys. They can stand the higher current. When you go 40 mph on flat you need more than 3000 watts to keep that speed. There you are already above 80A. And with your settings you can draw more. When you have a new battery then it would be awesome if you can connect my app via Bluetooth module and make a video with the app at top speed. I think everybody would like to see that.
```

---
## \#82 Posted by: Goo-shtick Posted at: 2017-03-17T17:09:48.823Z Reads: 68

```
I Know I am a engineering tech for TESLA on the R&D side I am Aware of what can happen Your not a douchbag
```

---
## \#83 Posted by: Goo-shtick Posted at: 2017-03-17T18:57:54.980Z Reads: 69

```
so your saying I should get pouch batterys instead if an 18650 pack?
```

---
## \#84 Posted by: Goo-shtick Posted at: 2017-03-17T18:58:35.437Z Reads: 71

```
wheelsize is 90 mm
```

---
## \#85 Posted by: Goo-shtick Posted at: 2017-03-17T19:00:58.668Z Reads: 70

```
I like the range with the pack I had range would be significantly compromised with lipo packs correct? and where do I get your app?
```

---
## \#86 Posted by: Ackmaniac Posted at: 2017-03-17T19:06:07.243Z Reads: 73

```
The app and firmware is available here. 
http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286

And with lips the range could be a bit less. Depends on what batterys you buy and how much space you have. But there is shitloads of info here on the forum.
```

---
## \#87 Posted by: e-Octo Posted at: 2017-03-17T19:08:47.373Z Reads: 69

```
[quote="Goo-shtick, post:83, topic:19105, full:true"]
so your saying I should get pouch batterys instead if an 18650 pack?
[/quote]

Lipo vs Li Ion 18650's - the lipos will handle higher discharge w/ less sag.  When you are pushing high speeds like this it's constant high draw/amps.  Which the li ion 18650's don't handle as well, unless you get a setup like @Chaka with 8p!

When you look at some of the high C Lipos - 45-60c with burst for a few seconds much higher - on a 5000mAh that equals (theoretical and a grain of salt for their marketing claims) = 225-325A as an example.  Realizing you are going to draw much much less than this constantly (even at your high speeds) - they will sag a lot less than a 18650 pack of reasonable size.  

That help?
```

---
## \#88 Posted by: Goo-shtick Posted at: 2017-03-17T19:09:53.910Z Reads: 67

```
what would you recommend for batterys my board has plenty of room its 41" wheelbase is 30-1/2
I Like my gearing I just want a little bit more power im almost content and happy with my setup buit
if it is possible to go a little faster and have a little more power I want ti
```

---
## \#89 Posted by: Goo-shtick Posted at: 2017-03-17T19:12:35.025Z Reads: 64

```
will the vesc x handle 225 amps?\
```

---
## \#90 Posted by: e-Octo Posted at: 2017-03-17T19:13:13.983Z Reads: 66

```
if you can go 12s it will give you more speed (higher voltage) and lower amps in general.  You'll need to be mindful of 60k ERPM limits so your motor kv will be a challenge.  **not sure if the VESC X has fixed this?**  And if you are stuck with 18650 - you'll need to add more batteries in parallel.
```

---
## \#91 Posted by: Goo-shtick Posted at: 2017-03-17T19:17:03.299Z Reads: 68

```
who sells a good 12s packs dexters out
```

---
## \#92 Posted by: mmaner Posted at: 2017-03-19T15:59:54.349Z Reads: 65

```
Check @oriol360, he has 12s packs.
miamielectricboards.com
```

---
## \#93 Posted by: Alextech Posted at: 2017-03-19T18:07:02.987Z Reads: 62

```
@barajabali And my Self could build you a 12s Pack.
```

---
## \#94 Posted by: nevstar Posted at: 2018-12-16T22:38:56.865Z Reads: 18

```
FYI - My Maytech controller has an upper slide limit of pulselength Start of 1.0010 ms and a End of 1.9990 ms, Center PuseLength is 1.4995. While changing out to the FATBOY SS and new Alien Motors 6384S I accidentally didn't write the configuration for the APP settings and took the defaults on the PPM Setting screen of 1.000ms, 2.000ms and 1.5000ms respectively. This cause CUT OUT UNDER FULL power (I guess because the 2.000 was beyond what the maytech could report. No FAULT codes were reported. Once I fixed this setting the CUT OUT Stopped completely. FYI the dropdown was set to Off (no current setting)

I hope this helps with those who experience intermittent CUT OUT of VESC Power at full throttle. Also note that on the low speed setting I never had any issues. 

TRAMPA BOARD - 136KV Trampaboards 6368 Motors - 8 sets of 10s2P 18650 cells from AliExpress. I get 40 plus miles running at an average of 22mph. Top speed on FATBOY SS with this setup is 27MPH.
```

---
