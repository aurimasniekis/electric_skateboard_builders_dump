# 300KV Motor, Trying not to fry vesc, help

### Replies: 40 Views: 1638

## \#1 Posted by: Sander Posted at: 2017-12-02T21:47:07.168Z Reads: 152

```
Hey!
I hear if the motor spins too fast, have too high RPM it will fry the VESC, so how can I limit it and prevent it?

This is the motor I have http://alienpowersystem.com/shop/brushless-motors/aps-6374s-sensored-outrunner-brushless-motor-300kv-3200w/

Thank you.
```

---
## \#2 Posted by: E1Allen Posted at: 2017-12-02T22:01:02.715Z Reads: 147

```
Anything over 7s will be above 60k ERPM which is vesc limit.  Most people use lower kV motors so you can run higher voltage less amp draw.
```

---
## \#3 Posted by: E1Allen Posted at: 2017-12-02T22:02:53.560Z Reads: 140

```
Also you can limit ERPM limits on the vesc to 60k/-60k.  Make sure you do not check the box that says limit ERPM with torque. I've heard it applies the brakes at full speed.
```

---
## \#4 Posted by: Sander Posted at: 2017-12-02T22:47:56.555Z Reads: 121

```
Well, im using 12S... So thats why I asked, but the torque should be fine because I have a gear ratio of 2.6, which means the motor gotta turn 2 rounds to turn the wheel 1 time?

I only see "Limit ERPM with negative torque", so I gotta uncheck that one and limit the Max ERPM to 60 000?

Since I have a 300KV motor with a 12S setup, it means it will draw much more amp, and the battery will drain faster?

If I had a 100KV with a 12S setup would that mean it would draw less amps?
```

---
## \#5 Posted by: Namasaki Posted at: 2017-12-02T22:56:35.805Z Reads: 108

```
Limit ERPM with negative torque is the box you need to uncheck.
There is no advantage to using a 300kv motor with the erpm limited to 60k
Since the 300kv motor has less torque, you might draw higher amps and you may experience problems with the motor overheating.

You would be better of to see if Alien will let you return that motor for credit on a 170kv motor.
```

---
## \#6 Posted by: Sander Posted at: 2017-12-02T23:08:46.636Z Reads: 97

```
Thanks, but overheating is not a problem. It will be sealed with oil.
Hmm, if I had the 170KV motor, it would be around 47kph, on 44.4V, thats why I bought the 300kv, because of much more speed... so I would always be able to limit it to 50kph so I wouldnt feel powerloss when the battery is at 3.3, because it would still be able to drive in 50kph. 
But if I had the 170KV motor I could change the middle gear to a 30 teeth instead of 25 teeth, and the other to 10 teeth.
```

---
## \#7 Posted by: scepterr Posted at: 2017-12-02T23:10:09.693Z Reads: 90

```
Getting to that speed will be a problem with no torque, unless you're traveling 1 way, downhill 😉
```

---
## \#8 Posted by: Sander Posted at: 2017-12-02T23:12:42.673Z Reads: 90

```
So you say I should change it to the 170 kv? If I do would i reach 50kph with no problem?
```

---
## \#9 Posted by: scepterr Posted at: 2017-12-02T23:16:58.862Z Reads: 87

```
With the right wheel size and gearing at 12S should be very doable
You could use a 190kv motor, assuming most are actually lower kv you'll be at the limit with 12S
```

---
## \#10 Posted by: Sander Posted at: 2017-12-02T23:17:30.419Z Reads: 82

```
@scepterr
btw, shouldnt my gear reduction fix this issue with the 300kv motor?
My gear ratio is 2.6
"While in many applications gear reduction reduces speed and increases torque"
The wheel is 90mm.
```

---
## \#11 Posted by: scepterr Posted at: 2017-12-02T23:19:38.437Z Reads: 77

```
I'm doing 50kph on 190kv 10S 15/44T 107mm and I haven't hit my top speed yet
Edit:40 not 44
```

---
## \#12 Posted by: Sander Posted at: 2017-12-02T23:21:23.010Z Reads: 78

```
Cool, but you have the opposite of gear reduction which gives you more speed and less torque, mine gives me less speed and more torque. Well if the torque is that bad, I will return it.

You have a gear ratio of 0.3 I have 2.6.
```

---
## \#13 Posted by: scepterr Posted at: 2017-12-02T23:23:21.827Z Reads: 74

```
Sorry it's actually 40T not 44 and it's 2.67 ratio..
http://calc.esk8.today/config/?type=3.7&scells=10&pcells=3&cc=3.0&da=20&mda=60&kv=190&poles=14&eff=90&wheel=107&mp=15&wp=40&wpm=18
```

---
## \#14 Posted by: Sander Posted at: 2017-12-02T23:27:12.354Z Reads: 73

```
oh, mhmm, well here is mine.
http://calc.esk8.today/config/?type=3.7&scells=12&pcells=1&cc=5.2&da=20&mda=60&kv=300&poles=14&eff=97&wheel=90&mp=25&wp=65&wpm=18

So should I just return it? Or just test it out my geared hub motor when it is finished?
```

---
## \#15 Posted by: scepterr Posted at: 2017-12-02T23:28:15.077Z Reads: 68

```
I would exchange if possible
```

---
## \#16 Posted by: Sander Posted at: 2017-12-02T23:29:24.190Z Reads: 68

```
Ok, I have contacted them.
But that means I gotta make a 30 teeth gear now for reaching 50kph with ~3.3V.
So the gear ratio will be 2.17.
```

---
## \#17 Posted by: scepterr Posted at: 2017-12-02T23:30:39.774Z Reads: 71

```
You need the basic 15/36 90mm setup..

http://calc.esk8.today/config/?type=3.7&scells=12&pcells=1&cc=5.2&da=20&mda=60&kv=190&poles=14&eff=90&wheel=90&mp=15&wp=36&wpm=18
```

---
## \#18 Posted by: Sander Posted at: 2017-12-02T23:31:07.641Z Reads: 69

```
Lol, cant do that. I have a geared hub motor. With a planetary gear.
```

---
## \#19 Posted by: scepterr Posted at: 2017-12-02T23:31:26.773Z Reads: 73

```
Oh well I dunno then 😋
I was wondering where you were fitting 66teeth..lol
```

---
## \#20 Posted by: Sander Posted at: 2017-12-02T23:32:01.072Z Reads: 72

```
Well, thank you any way :blush: 
<img src="/uploads/db1493/original/3X/b/a/baa1c895ec6ac9ad7866fe7d7aad9798e7efb331.jpg" width="503" height="500">
```

---
## \#21 Posted by: scepterr Posted at: 2017-12-02T23:32:57.495Z Reads: 67

```
Yeah that thing looks awesome, considering you are the only one with it... I dunno maybe try the 300kv see what it does
```

---
## \#22 Posted by: scepterr Posted at: 2017-12-02T23:34:30.641Z Reads: 66

```
If you are able to keep the rpm low enough mechanically to stay around 60k erpm....might be interesting
```

---
## \#23 Posted by: Sander Posted at: 2017-12-02T23:34:35.146Z Reads: 68

```
Yeah I saw other people on the forum created this thing, but I wanted to create my own since there are  no place to buy them and they are expensive AF to buy, but not to make. So I created my own with not watching the other concept because I want to be proud of it :stuck_out_tongue:

So I will make the gear holder, gear and the whole planetary gear very soon in the CNC class, but the teacher says using a 3d program to make toolpath uses to much time, so I gotta hand program the coordinates in the machine, which is a pain in the ass.
```

---
## \#24 Posted by: scepterr Posted at: 2017-12-02T23:36:10.047Z Reads: 66

```
I'm curious to see how it handles the torque deficit
```

---
## \#25 Posted by: scepterr Posted at: 2017-12-02T23:39:21.554Z Reads: 68

```
I would still have some spare drvs and fets around just incase 😉
```

---
## \#26 Posted by: E1Allen Posted at: 2017-12-03T00:04:00.750Z Reads: 62

```
He could do vesc6 with 100k ERPM limit. Not budget friendly unless you have no budget
```

---
## \#27 Posted by: scepterr Posted at: 2017-12-03T00:06:37.187Z Reads: 61

```
Vesc 6 erpm limit is over 150 if I remember correctly, diff motor would be cheaper
```

---
## \#28 Posted by: BigBoyToys Posted at: 2017-12-03T07:09:54.713Z Reads: 60

```
People are using the FOC box on eBikes at near 100k erpm.  I havent seen anyone above 60K om them with esk8's though. 

Ive spun my 350KV motors to just over 100K erpm on my VESC6's as well. Ive heard 150K tested for the VESC6 as well.
```

---
## \#29 Posted by: Eboosted Posted at: 2017-12-03T07:27:35.477Z Reads: 61

```
I run 190kv on 12s on full load with focboxes, never had issues
```

---
## \#30 Posted by: pat.speed Posted at: 2017-12-03T08:35:43.051Z Reads: 56

```
I have seen another build like this that used a 300kV motor I think he used a 1:3 reduction.  Here's the build


https://www.electric-skateboard.builders/t/first-build-dual-hub-motor-internal-planetary-gearbox-4260-300kv-vesc/20111
```

---
## \#31 Posted by: E1Allen Posted at: 2017-12-03T08:41:58.793Z Reads: 54

```
So your intent is to do a planetary gear as well?  If so your higher kV motor would help make up for the gear reduction but you are still dealing with ERPM limits.  Not planning on the traditional hub motor or belt style?
```

---
## \#32 Posted by: E1Allen Posted at: 2017-12-03T08:51:01.315Z Reads: 56

```
What's your intended battery, gear ratio, and motor kV currently planned?  I've read back through. Trying to see what your current intent is so you can get to your intended top speed
```

---
## \#33 Posted by: Frank Posted at: 2017-12-03T12:57:51.897Z Reads: 53

```
Nice! Another planetary gearbox but I am very interested in how it turns out. How are you going to build it? The biggest motor I could fit was a 42mm (45mm actually but there is not 45mm out runner) because of the bearings.

Something I did not say in my topic is that the oil lubrication of the gearbox failed. The oil seals are giving to much friction. Therefore, I will use grease instead.

Also interested in how you going to program a gear by hand because a good gear is not a simple curve and the size is small. My gears have a radius of 0.3mm.

I hope you will make a build of it!
```

---
## \#34 Posted by: Sander Posted at: 2017-12-03T16:00:59.940Z Reads: 46

```
@Frank we have a lathe where I can use a gear module to cut it out. All I have to do is divide 360 degrees on teeth number to find out how much I have to turn the material to cut the gears. 

<img src="/uploads/db1493/original/3X/b/0/b06617388352055aac188bc35dd649ebde88055c.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/0/f/0f60d0f18e4056cbb31f2295eb35da1981bf208f.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/f/5/f505b8a18954a7fd0a161311c6f156ddacfc422c.png" width="690" height="388">
```

---
## \#35 Posted by: Frank Posted at: 2017-12-03T16:13:31.110Z Reads: 44

```
i dont want to put your design down but how are you going to make this:
<img src="/uploads/db1493/original/3X/7/6/7681ba2890fec6f695d66c2518f6e311bbd36fa6.png" width="206" height="256">

also are you only going to use a 1 bearing for the "wheel" at the back and in the front you will use the gears?

at least wat is the air gap between the motor and the "wheel" mount/ringgear
```

---
## \#36 Posted by: Sander Posted at: 2017-12-03T16:18:23.748Z Reads: 43

```
Nah, please be honset so I can make it better.

About that gear, I dont really know.. But I will find a way.
Between there it is 0.1mm, so you say it will be friction there and I should have made it fixed with the motor so it will always be a gap between the gear holder and the motor gear? But I could make the bearing of the motor come half way out so you "connect" the motor gear on it. I was thinking of using a screw on the side of one of the poles that goes inside the motor to lock it.

Axle goes inside there and the Gear Holder will be fixed and not move outwards after screwed in.
<img src="/uploads/db1493/original/3X/7/b/7bece8ea97a451178430613d926ad9bf17361a18.jpg" width="690" height="388">
```

---
## \#37 Posted by: Sander Posted at: 2017-12-03T16:28:54.813Z Reads: 41

```
Well, I had some others design ready, but they where for a smaller motor. This you see now is what I made for 2 hours ago...
```

---
## \#38 Posted by: Frank Posted at: 2017-12-03T16:32:15.872Z Reads: 39

```
to be honest I don’t think you can make the part that way. I made the same part out of 2 pieces and press fit it together but in your design, it will be impossible because of the small back plate.

0.1mm is way to less. To turn it by hand it will be fine but then something else will come. Eddy current (not an electrical expert or something but this is told to me) when you place something to close to your motor it will work as a brake (eddy current brake). In this case, it will be bigger than just a plate because your outer ring is also turning in the opposite direction. This will make your wheel a massive brake for your motor. What will result in lots of heat within minutes.
```

---
## \#39 Posted by: Sander Posted at: 2017-12-03T16:42:00.239Z Reads: 44

```
I will make a bigger gap, but I think I solved the issue with getting a fixed gear.

<img src="/uploads/db1493/original/3X/0/e/0e1c7b25d74818c38c7dc88461637e718f29eb77.jpg" width="690" height="388">

Its possible to machine both part now.

The gap between the outer ring and the motor is 3 mm, so it will create a lot of heat when braking then...
```

---
## \#40 Posted by: Ulfberht Posted at: 2017-12-05T00:11:11.921Z Reads: 30

```
[quote="Sander, post:1, topic:39971"]
I hear if the motor spins too fast, have too high RPM it will fry the VESC, so how can I limit it and prevent it?
[/quote]
From Vedder's site: 
"2. Change the KV of the motor. Yes, this can be done quite easily without rewinding the motor. Almost all outrunners are connected using a delta-connection. By removing the heatshrink of the motor wires, they can be split up and reconnected in a star-connection. This reduces the KV by a factor of sqrt(3) = 1.73. For this modification, we can use a motor with a KV of 188 * sqrt(3) = 325. There are several hobby motors available close to that KV, so that is no problem. I have tested this modification on several motors and it works really well."
http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/
```

---
