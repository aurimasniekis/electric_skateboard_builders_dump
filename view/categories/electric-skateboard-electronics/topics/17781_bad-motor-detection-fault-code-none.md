# Bad Motor Detection: FAULT_CODE_NONE

### Replies: 42 Views: 2484

## \#1 Posted by: ARollNation Posted at: 2017-02-16T05:28:12.382Z Reads: 146

```
Whats up guys, I'm running 10s to my VESC and its powering a 290kV Turnigy motor. 

All was dandy until mid ride my board basically lost all power from the motor. My batteries were at 40V so I don't think its a voltage issue. Since then I cannot get the VESC to detect the motor in bldc, yet it won't spit out a fault code. I'll attach some screenschots of my BLDC

Any advice would be much appreciated!

-Aaron

<img src="/uploads/db1493/original/3X/e/9/e9dd513282f903de19e41112185c5a60b1e84f4c.jpg" width="690" height="327">

<img src="/uploads/db1493/original/3X/5/e/5e564189b1e0c875e5ae551fc96bc5c33618fa57.jpg" width="690" height="387">

<img src="/uploads/db1493/original/3X/d/7/d73eba876665bb4eeec055c861371aa3f031af60.jpg" width="690" height="387">
```

---
## \#2 Posted by: Namasaki Posted at: 2017-02-16T05:33:03.388Z Reads: 137

```
do the red lights keep blinking?
290kv at 40v is way over the vesc erpm limit. that can kill the drv chip
```

---
## \#3 Posted by: ARollNation Posted at: 2017-02-16T05:41:17.082Z Reads: 134

```
Yeah, it blinks three times when powered on
```

---
## \#4 Posted by: lox897 Posted at: 2017-02-16T05:46:02.114Z Reads: 127

```
Where is the VESC from? Is it a VESC X? 290kv on 10S VESC probably killed it
```

---
## \#5 Posted by: Namasaki Posted at: 2017-02-16T05:49:32.395Z Reads: 123

```
3 red blinks at startup is normal. any red blinking after that is not
```

---
## \#6 Posted by: ARollNation Posted at: 2017-02-16T05:54:21.805Z Reads: 120

```
Ok correction, it blinks 4 times on start up.. Is that abnormal?
```

---
## \#7 Posted by: ARollNation Posted at: 2017-02-16T05:56:55.600Z Reads: 117

```
Enertion... and from what I read after I got it is that they arent the best to buy from.

Its not the VESC-X, It was from their September batch if I remember correctly
```

---
## \#8 Posted by: lox897 Posted at: 2017-02-16T05:58:23.384Z Reads: 118

```
@EnertionSupport could help you diagnose the problem. Send a few pictures of your VESC please
```

---
## \#9 Posted by: ARollNation Posted at: 2017-02-16T06:02:09.916Z Reads: 116

```
I've been in contact with them via email previously and they referred me here haha
```

---
## \#10 Posted by: Blasto Posted at: 2017-02-16T06:10:07.648Z Reads: 114

```
Try doing a motor detection then go in the terminal and type faults
```

---
## \#11 Posted by: ARollNation Posted at: 2017-02-16T06:12:15.462Z Reads: 111

```
it returns "FAULT_CODE_NONE"
```

---
## \#12 Posted by: Blasto Posted at: 2017-02-16T06:13:38.143Z Reads: 110

```
what does the motor do when performing a motor detection
```

---
## \#13 Posted by: ARollNation Posted at: 2017-02-16T06:15:02.430Z Reads: 107

```
Nothing at all, doesn't spin up or even make noise
```

---
## \#14 Posted by: Blasto Posted at: 2017-02-16T06:16:21.387Z Reads: 106

```
and i'm assuming it returns detection fail?

show some pics of your setup
```

---
## \#15 Posted by: ARollNation Posted at: 2017-02-16T06:26:54.275Z Reads: 104

```
yeah just "Bad Motor Detection" 

I'll try to upload some pics tomorrow, the lighting in my room is terrible. 

From what @Namasaki said I may have fried my DRV chip.. Is there a way I can check with a voltmeter or somethin?

 My only other guess is a poor solder joint connection somewhere, but all look and feel secure.. 

BTW thanks for takin the time to help guys!
```

---
## \#16 Posted by: Blasto Posted at: 2017-02-16T06:35:02.660Z Reads: 101

```
you would get a DRV fault code in the terminal if your drv would be dead. I'm suspecting your motor connections or your motor itself. 10S with 290Kv, that guy is working orvertime.

one way to test your motor, unplug it from the vesc, short 2 leads at a time (motor side) and try to turn your motor by hand. do you feel resistance from it? or touch all 3 of them together and try to spin the motor by hand
```

---
## \#17 Posted by: ARollNation Posted at: 2017-02-16T07:02:22.778Z Reads: 99

```
Ahh, I see. 
I am using a thicker internal wire gauge on the connecting wire from the motor to the vesc, think that could be causing some sort of internal resistance causing it to fault?

I will try that and report back with details
```

---
## \#18 Posted by: Blasto Posted at: 2017-02-16T07:07:04.666Z Reads: 102

```
[quote="ARollNation, post:17, topic:17781"]
I am using a thicker internal wire gauge on the connecting wire from the motor to the vesc, think that could be causing some sort of internal resistance causing it to fault?
[/quote]

Not quite sure what you mean, but bigger gauge wire would not cause any faults. Appart that it is harder to solder/splice
```

---
## \#19 Posted by: ARollNation Posted at: 2017-02-16T07:14:46.506Z Reads: 100

```
sorry I worded that poorly. Im using 10AWG all the way from the vesc to the motor its just that the wire I used in between them was really stiff instead of it being the type thats made of a bunch of fine silver wires twined together, I have stuff like this. 

I remember having trouble with it bonding when first trying to solder the connections up. 


<img src="/uploads/db1493/original/3X/b/4/b4c971d9bf8d2c9fdd0261b3c2b35d10f6bc76ce.jpg" width="281" height="500">
```

---
## \#20 Posted by: Blasto Posted at: 2017-02-16T07:21:56.737Z Reads: 93

```
I dont want to steer you in the wrong direction, reason why high strand count wires are used is they handle vibrations much better and are much more malleable. Check the conductivity of your connection with a meter. A broken connection within the jacket of the wire is very possible with that type of wire
```

---
## \#21 Posted by: ARollNation Posted at: 2017-02-16T07:23:43.346Z Reads: 90

```
Yeah I was noticing a trend with all the other builds but I used what I had lying aroung atm :sweat_smile:
```

---
## \#22 Posted by: ARollNation Posted at: 2017-02-16T07:30:38.608Z Reads: 92

```
this joint connection isnt in the best place either.<img src="/uploads/db1493/original/3X/4/6/46fb6624286440fd7599c5033f25d2137917754a.jpg" width="690" height="480">
```

---
## \#23 Posted by: TarzanHBK Posted at: 2017-02-16T09:46:33.657Z Reads: 88

```
Well, I wouldn´t ride a 10s with a 290kV. You need to get something like a 190kv motor and set your erpm limit to 60000.
You´ll probably kill your DRV if you ride like that a few more miles!

Also I think you broke the erpm record with that combination :D
```

---
## \#24 Posted by: JohnnyMeduse Posted at: 2017-02-16T13:57:18.231Z Reads: 84

```
First, if you lost power and have a FAUL_CODE_NONE error, in most cases it is a bad connection from the motor to the vesc, one of the surrounding component of the mosfet circuit is broke down or badly solder.

Second, these 10awg cable you seem to use are to rigid, that why you should use 10awg **silicone wire**, and because they are so rigid they might put unwanted pressure on soldering joint inside your motor or on the vesc. 

Third, if you running sensor, check your sensor cable, be sure that they are all get a good connection.... Or try to run a new motor detection and check if all the sensor are detect.
```

---
## \#25 Posted by: ARollNation Posted at: 2017-02-16T19:59:20.229Z Reads: 75

```
Lmao unfortunately I didn't educate myself enough on the erpm limit when buying my motor. I'm surprised the chip hasn't blown yet considering I've rode it 5-10 miles since it was built! Its pretty quick though, hit 24 MPH with a 12-40 ratio :grin:
```

---
## \#26 Posted by: ARollNation Posted at: 2017-02-16T20:03:40.443Z Reads: 75

```
Yeah I was thinking it could be some sort of a connection issue. I'll upgrade my wire and see if that helps.
```

---
## \#27 Posted by: Blasto Posted at: 2017-02-16T20:27:18.233Z Reads: 74

```
[quote="JohnnyMeduse, post:24, topic:17781"]
that why you should use 10awg silicone wire
[/quote]

Even 10AWG is overkill, i would stick with 12AWG, easier to solder and handle
```

---
## \#28 Posted by: bdemissi Posted at: 2017-09-07T03:05:19.421Z Reads: 57

```
if its blinking when you are doing the motor detection what does that mean?
```

---
## \#29 Posted by: Namasaki Posted at: 2017-09-07T04:11:26.447Z Reads: 58

```
[quote="bdemissi, post:28, topic:17781, full:true"]
if its blinking when you are doing the motor detection what does that mean?
[/quote]


Do you mean it's blinking red during motor detection?
```

---
## \#30 Posted by: bdemissi Posted at: 2017-09-07T04:24:28.468Z Reads: 58

```
yes it blinks red 4 or 5 times and it says bad motor detection
```

---
## \#31 Posted by: Namasaki Posted at: 2017-09-07T04:36:22.219Z Reads: 57

```
remove the belt and pulley if you haven't already and unplug the phase wires. Then turn the motor by hand to make sure nothing is restricting its rotation. Like  something on the motor hitting the mount plate like a shaft key or circle clip.
Or the screws that hold the motor on the plate, if they are too long they could be scraping something inside the motor.
```

---
## \#32 Posted by: bdemissi Posted at: 2017-09-07T05:28:12.103Z Reads: 56

```
i have tried that. the problem still occurs
```

---
## \#33 Posted by: ARollNation Posted at: 2017-09-17T08:28:09.331Z Reads: 53

```
After trying the diagnostic terminal again and typing 'faults' I received the code: "FAULT_CODE_DRV8302" 

Any advise on ESC repair or does it look like I need to drop some cash for a new ESC?
 
I also need to either choose a new motor, one with a lower kv or reduce the cell count in my battery setup. 

Suggestions as to which one would be a better call?

Thanks everyone,

A-Aron
```

---
## \#34 Posted by: GhettoFab.rictation Posted at: 2017-12-22T07:50:05.944Z Reads: 44

```
I am having no faults and no motor detection I bought the turnigy sk3 192kv motor off of ebay and I'm worried there is a short in the mtor is there a way to check with multimeter? When I go to detect the motor it blicks once green then once green again when it's done and states motor detection failed bottom right corner.
```

---
## \#35 Posted by: dg798 Posted at: 2017-12-22T12:25:20.237Z Reads: 43

```
Not sure how to check but I had the same problem as you and it was because of a horrible in the motor. However me being me decided to continue running motor detection and eventually the short in the motor caused the drv to fry. Don’t try to keep using the motor until you know it doesn’t have a short.
```

---
## \#36 Posted by: GhettoFab.rictation Posted at: 2017-12-22T18:50:38.270Z Reads: 35

```
thank you for the advice! I checked the motor with a esc and it worked so I also checked the resistance of my vesc wires and got 0. Maybe I am using the wrong bldc tool for my vesc? Although it is writing configurations sometimes it takes me 2 clicks on writing configuration for it to work. Maybe it is my cable connecting the vesc because I am using kind of a dinky one. Wouldn't it have issues connecting or writing configurations if that was the case??? Still getting bad motor detection, no fault codes, and green lights when trying to bench test it or motor detect... I am thoroughly frustrated with myself for not being able to know the solution and solve this because I'm 70% sure it's a simple fix.... ughh :rage:
```

---
## \#37 Posted by: GhettoFab.rictation Posted at: 2017-12-22T18:58:19.810Z Reads: 35

```
<img src="/uploads/db1493/original/3X/d/b/dbc3e7584db562574ac28a3119097a3c14d8b263.jpg" width="690" height="388">
```

---
## \#38 Posted by: ARollNation Posted at: 2017-12-22T20:06:54.420Z Reads: 31

```
To check if there is a short in the motor, with it disconnected from everything short two of the phase wires together and spin the motor with your hand. Does it feel harder to turn compared to none of the phase wires being shorted? If it does that means the motor is fine. Shortin all three should give even greater turning resistance
```

---
## \#39 Posted by: ARollNation Posted at: 2017-12-22T20:07:48.831Z Reads: 31

```
Where did you buy your VESC?
```

---
## \#40 Posted by: GhettoFab.rictation Posted at: 2017-12-22T20:23:54.147Z Reads: 32

```
I tested motor on another esc so thankfully that checks out. I checked all solder joints and vexc wires from the mosfets have 0 resistance so that's not the issue. But the vesc was from ebay or amazon about a year ago I can't remeber which it's 2.18 firmware 4.12 model.
```

---
## \#41 Posted by: GhettoFab.rictation Posted at: 2017-12-22T20:26:18.717Z Reads: 35

```
<img src="/uploads/db1493/original/3X/0/5/05548766df03b0f1c114a27386fa1c427f4f809a.jpg" width="690" height="388"> <img src="/uploads/db1493/original/3X/c/7/c7420ec7760458dc9513e18930abe010ebb5622e.jpg" width="690" height="388">
```

---
## \#42 Posted by: banjaxxed Posted at: 2018-06-27T13:17:04.791Z Reads: 21

```
Here's something that happened to me today, resetting a slave focbox to default, no problem connecting via USB, CAN seemed to fail in forward mode.

Motor detection was not a problem but it was noiseless! 
No faults on the VESC tool console.

Switched motors to see if there was a problem there.

Finally I did the obvious and took the ESC back out of the enclosure and there it was the DRV has obvious signs of damage
```

---
