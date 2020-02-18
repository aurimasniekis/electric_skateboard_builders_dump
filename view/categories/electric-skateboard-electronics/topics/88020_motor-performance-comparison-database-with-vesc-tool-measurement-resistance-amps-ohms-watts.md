# Motor performance comparison database. With vesc tool measurement. Resistance / Amps / Ohms / watts

### Replies: 38 Views: 1412

## \#1 Posted by: taz Posted at: 2019-03-23T11:13:00.363Z Reads: 248

```
I figured since the new VESC tool gives estimated max amperage values during motor detection, it would be nice to have a database where people could compare various motors.

So let me start:

ESC: 2 x Focboxes

Motors: eskating (Maytech) 6355 190kv

Estimated amps: 43A (Factory rating 65A)

![Screenshot_20190220-174359|243x500](upload://7Ia9ZnjBzOIlVJrKVU8KIx9BppO.jpeg) 

ESC: 2 x Focboxes

Motors: eskating (Maytech) 6374 190kv

Estimated amps: 65A (Factory rating 65A)

![Screenshot_20190321-132142|243x500](upload://cfTtbfnbekxaMBp1lRCdTqv5VIa.jpeg)
```

---
## \#2 Posted by: taz Posted at: 2019-03-24T08:48:10.282Z Reads: 223

```
Although it seems there is no interest here is another motor

Esc: 2 x VESC 6

Motors: Hobbyking SK8 149kv

Estimated amps: 55A (Factory rating 80A)

![Screenshot_20190324-094437|243x500](upload://lV9iPUVqM8eA0qXXljBxEfS4Ye7.jpeg)
```

---
## \#3 Posted by: Andy87 Posted at: 2019-03-24T09:24:53.610Z Reads: 201

```
Maybe it makes sense to add the factory rating of the motor. To have a comparison what they are rated for from the seller and what the vesc measurements gave as result?
```

---
## \#4 Posted by: rich Posted at: 2019-03-24T09:32:43.979Z Reads: 202

```
Interesting thread, as @Andy87 mentioned manufacture rating would be good for comparison. AFAIK sealed Maytech are rated for 65A max like the values after motor detection. But SK8 55A only? :thinking:
```

---
## \#5 Posted by: Andy87 Posted at: 2019-03-24T09:35:52.972Z Reads: 196

```
I would be interested in the sk8 192kV as they rated to 100A what still seems a bit lot for me.
```

---
## \#6 Posted by: taz Posted at: 2019-03-24T10:05:50.307Z Reads: 197

```
This is exactly why I started this thread.

We read manufacturer's datasheets and sometimes they do not correlate with what we experience
.
At least in my case the Maytech motors feel way stronger compared to the SK8 motors in every regard. Even in steep hills although they are lower kv. That is with everything else being equal.

As you said the Maytech motors are rated at 65A by the factory whereas the SK8 at 80A :roll_eyes:

I edited the previous posts and added the factory rating.
```

---
## \#7 Posted by: DavidC Posted at: 2019-03-24T15:12:04.438Z Reads: 188

```
There is a threat about that on VESC Project website : 
[https://vesc-project.com/node/811#comment-3204](https://vesc-project.com/node/811#comment-3204) 

I've got OVERION (Maytech) MTO6374-HA-C 130KV : 
Estimated amps :  43-44A (Factory rating 65A)

Despite what says VESC-Tool 2019, il works really better with Battery max/Motor max 65A than with 45A.

I've just bought the Turnigy SK8 6374-192KV Sensored Brushless Motor, because I hoped to get 100A from it. I chose latest ACKMANIAC firmware but I'll try VESC-Tool 2019 on this one. Very interesting thread!!
```

---
## \#8 Posted by: DavidC Posted at: 2019-03-24T15:40:40.159Z Reads: 181

```
It's what you get with limited data : 

![xlsx|549x328](upload://wIawi1wLFtBGe3K5UaxBmQs18bg.jpeg) 

I don't know if VESC-Tool 2019 advised motor current depends on motor resistance only.
```

---
## \#9 Posted by: rpasichnyk Posted at: 2019-03-26T06:46:02.489Z Reads: 169

```
No interest unless this process is automated, feature request for VESC Tool?
```

---
## \#10 Posted by: Mobutusan Posted at: 2019-03-30T02:18:23.301Z Reads: 163

```
@taz Very cool thread. I somehow missed this one. I didn't know the new VESC tool had this feature. Looks like a good way to take some of the mystery out of all of these different motors. I'll do some searching, but do you know off hand if the new VESC tool is compatible with older 4.12 VESCs, FOCBOX'S, Flipsky 6.6's? I've been wanting to take the pile of motors that I have and do some actual KV testing on them but this would be one better than that.
```

---
## \#11 Posted by: taz Posted at: 2019-03-30T05:24:38.178Z Reads: 160

```
Yes it is.
On my Evo I have focboxes and it works perfectly fine (after you upgrade the firmware ofcourse).
```

---
## \#12 Posted by: taz Posted at: 2019-03-30T05:32:07.610Z Reads: 166

```
I forgot to add that I have a metr pro bluetooth module in that one.

I don't know if it will work with a hm10 module.
```

---
## \#13 Posted by: DavidC Posted at: 2019-03-30T11:55:45.835Z Reads: 159

```
**Turnigy SK8 6374-192KV Sensored Brushless Motor (14P)**

**Specs:**
KV:  **192**
Max current:  **100A**
Max Power:  **4400W**
Idle current:  **1.8A**
Resistance:  **24MΩ**
Shaft:  **8mm**
Weight:  **940g**

![SK8_6374_192KV_VESCTool106|435x470](upload://c9VejqBpWLldDUpfR9Sw7pu7WL.jpeg)
```

---
## \#14 Posted by: taz Posted at: 2019-04-05T17:12:21.891Z Reads: 150

```
It seems it does.
If you do the calculations it appears that the tool sets 60W thermal losses as the limit and calculates the max current using Ohm's law.
```

---
## \#15 Posted by: mishrasubhransu Posted at: 2019-04-06T16:01:25.845Z Reads: 149

```
Flipsky 6374. 
![Screenshot_20190326-030426|281x500](upload://jJSAq9ItXcYeVb2lUHmVPZi6DfI.png)
```

---
## \#16 Posted by: Andy87 Posted at: 2019-04-06T17:25:11.966Z Reads: 138

```
@hyperIon1 @PatRocks or anybody else who already received the 6880 190kV motors from maytech, would be nice to see what the new vesc tool says about those motors and if it is close to the specs maytech gives.
```

---
## \#17 Posted by: hyperIon1 Posted at: 2019-04-06T17:28:40.217Z Reads: 143

```
I think @PatRocks can when he is back from holiday. I won't have any until the end of next week to test.
```

---
## \#18 Posted by: PatRocks Posted at: 2019-04-07T03:28:40.508Z Reads: 141

```
Soon... ill look into it further and report asap
```

---
## \#19 Posted by: mishrasubhransu Posted at: 2019-04-09T04:13:55.579Z Reads: 147

```
eLofty 75KV direct drive motors  
![image|318x361](upload://iAwyDMGAgS8pkIF0avclZAmqEIX.png)
```

---
## \#20 Posted by: b264 Posted at: 2019-04-22T18:02:24.439Z Reads: 147

```
Torqueboards Direct Drive

https://www.electric-skateboard.builders/t/first-look-at-torqueboards-direct-drive-motor/61152/1256?u=b264
```

---
## \#21 Posted by: DavidC Posted at: 2019-05-18T17:20:30.250Z Reads: 134

```
**Turnigy Aerodrive SK3 - 6374-192kv Brushless Outrunner Motor**
![Turnigy%20Aerodrive%20SK3%20-%206374-192kv%20Brushless%20Outrunner%20Motor|425x470](upload://jvmeMbdrkVCgrnS6j4niNktT3DA.jpeg) 

_VERSUS_

**Turnigy SK8 6374-192KV Sensored Brushless Motor (14P)**
![SK8_6374_192KV_VESCTool106|435x470](upload://c9VejqBpWLldDUpfR9Sw7pu7WL.jpeg) 

_The SK3 is more powerful than the SK8 (77A-10mOhms VS 67A-13mOhms)_

_It's also lighter! (858gr VS 940gr)_
```

---
## \#22 Posted by: DavidC Posted at: 2019-05-18T17:21:13.242Z Reads: 128

```
**Turnigy G160 Brushless Outrunner 290kv (160 Glow)**

![Turnigy%20G160%20Brushless%20Outrunner%20290kv%20(160%20Glow)|435x470](upload://fP7mANu56MtFrGPUiMapWSPLqdh.jpeg)

_52A - 22mOhms_
```

---
## \#23 Posted by: DavidC Posted at: 2019-05-18T17:22:38.916Z Reads: 124

```
**C6364-KV280 EMP brushless Motor for airplane RC Outrunner**

![C6364-KV280%20EMP%20brushless%20Motor%20for%20airplane%20RC%20Outrunner|417x470](upload://zSGX7mv00UAKPujDVTKqL3H52mO.jpeg) 

_59A - 17mOhms_
```

---
## \#24 Posted by: lrdesigns Posted at: 2019-05-20T06:36:09.481Z Reads: 113

```
Hey I think this thread is awesome. I tried searching a similar thread but didnt come up with anything good. Just a few small threads here and there, most quite old. I got here by finding a single post in thread about a different subject, that led me to [vesc project thread](https://vesc-project.com/node/811) on the same thing, then a link that led me back here to this thread.  So I changed the title to make more easily searchable. 

This is my motor its

Racestar 5065, 149kv, 67mOms. 

Its been thrashed for two years so I dont know if that has any effect but the resistance is quite high even for a 149kv motor? 

![Left%20motor%2020th%20May%202019|690x126](upload://5aLB89wRcbGrY1r9ddxatfVhDvB.jpeg)
```

---
## \#25 Posted by: Pedrodemio Posted at: 2019-05-20T17:40:00.303Z Reads: 103

```
Considering that the torqueboards 5055 190Kv is 40 mOhms and they have the same size  stator, 67 for 149Kv sound about right

As Kv goes down resistance goes up for the same motor
```

---
## \#26 Posted by: BearHere Posted at: 2019-05-20T17:44:56.814Z Reads: 103

```
What is the factory kv rating?
```

---
## \#27 Posted by: Pedrodemio Posted at: 2019-05-29T17:20:32.970Z Reads: 95

```
Does anyone have the resistance for a 80XX motor? @Kug3lis or @Nowind maybe?
```

---
## \#28 Posted by: Nowind Posted at: 2019-05-29T19:56:15.615Z Reads: 91

```
Actually not Bro.
```

---
## \#29 Posted by: DavidC Posted at: 2019-08-05T06:24:20.749Z Reads: 68

```
# C80100 SENSORED OUTRUNNER BRUSHLESS MOTOR 130KV 7000W

![20150511_162901-FILEminimizer|690x388](upload://ndQlakzeTeI1aTfc9cJFEDJ8csl.jpeg) 

MOTOR: C80100
KV: 130
POWER: 7000W
WIRE WINDS: 8D
MAX AMP: 200A
ESC: 250/300A
MAX VOLT: 18S
NO LOAD CURRENT: 2,0
SIZE: 80 x 100 ( without shaft )
WEIGHT: 1.980g
SHAFT: 12mm with 3mm  KEYWAY
Accessory pack: Yes
Internal PCB with 120 degree hall effect sensors

![jpeg|435x492](upload://djIuvdVp1b9rmoEJ6JxNRElE1YS.jpeg) 

*120A - 9mOhms*
```

---
## \#30 Posted by: taz Posted at: 2019-08-05T08:56:13.851Z Reads: 63

```
That's a big boy.
Although I am slightly disappointed in the weight/power ratio.
I would expect more of the additional weight compared to a 6374 motor to go into copper.
This thing weighs 240% more than a 6374 :open_mouth:
It is a 130kV though, I would expect a 190ish kV to take even more current.
```

---
## \#31 Posted by: DavidC Posted at: 2019-08-05T16:00:49.324Z Reads: 59

```
Good point but you can run it 18S.

Enamel is a real pain to remove, more than on 6374 motors.

It doesn't look as good as SK3 motors, which are the best quality motors in my opinion (but I didn't try TRAMPA ones).
```

---
## \#32 Posted by: taz Posted at: 2019-08-05T16:45:02.202Z Reads: 57

```
You can probably run the other motors in 18s too. Essentially you can run as high voltage as you like provided the insulation in the windings holds up.
The problem for us is that most vescs can't run higher voltages than 12-13s.
I had the white 6364 154kV Trampa motors and found them lacking.
```

---
## \#33 Posted by: Hummie Posted at: 2019-08-05T17:04:17.737Z Reads: 54

```
How is the new vesc tool coming up with its amp limit and maybe it's doing what amounts to figuring the motor km?  I don't know what numbers u guys look at but the kv and resistance alone should tell u the motor km or how much heat/waste produced for a given amount of torque and can compare all motors that way: the motor km   If someone is good at math and can convert the kv to the kt and then throw the resistance number in then will have the km and we can compare all the motors with that number and only other variable being how well it can rid of the heat produced And iron losses
```

---
## \#34 Posted by: taz Posted at: 2019-08-05T17:11:22.730Z Reads: 54

```
It assumes 60W heat losses as a limit for this size of motor, so after measuring resistance and using Ohm's law it calculates the maximum amps it can take.
```

---
## \#35 Posted by: DavidC Posted at: 2019-08-06T06:18:49.937Z Reads: 49

```
Maytech 6374 130KV are 792gr and take 49A max current (according to VESCtool).

APS 80100 130KV are 2.5x heavier (1980gr) and take 2.4x more current (120/49).

Not that bad.
```

---
## \#36 Posted by: taz Posted at: 2019-08-06T06:48:20.385Z Reads: 49

```
True. I hoped a bigger percentage of that weight would go into copper though.
A man's gotta dream right ? :wink:

Bloody forum, I had forgotten how annoying the editing is here. Single enter for the win.
```

---
## \#37 Posted by: Hummie Posted at: 2019-08-06T06:56:52.834Z Reads: 46

```
[quote="DavidC, post:21, topic:88020"]
*The SK3 is more powerful than the SK8 (77A-10mOhms VS 67A-13mOhms)*

*It’s also lighter! (858gr VS 940gr)*
[/quote]

 is the kv really the same and often the kv posted by the maker isn't accurate.   3mOhms difference is a lot.   if they were the same kv then the lower resistance is a hugely better motor with less heat for same torque produced per amp.  its like..25% better at doing the job of converting electricity to torque

 without having the kv or kt in the equation i dont think you can you compare motors.

  this tool only takes the winding resistance into account telling the amount of amps that would produce 60watts of loss but missing the important amount of power that would be coming out with that loss.

  and why assume 60 watts loss is a limit of a motor anyway as its not a true limit and arbitrary.




.doesn't this tool also tell the erpm and voltage like the old tool and can work out the kv?
```

---
## \#38 Posted by: taz Posted at: 2019-08-06T07:31:06.435Z Reads: 42

```
While I don't disagree with anything you wrote, the tool provides easily attainable information.

Yes you can use it to measure the kV if you want.

The 60W as you say is arbitrary but it is a damn good estimate for a motor this size.
```

---
