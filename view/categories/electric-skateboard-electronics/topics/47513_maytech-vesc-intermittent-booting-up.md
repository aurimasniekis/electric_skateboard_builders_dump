# Maytech Vesc, intermittent booting up

### Replies: 37 Views: 1230

## \#1 Posted by: cliofreak Posted at: 2018-02-26T14:41:18.687Z Reads: 122

```

Hi, my Vesc is now intermittent. Blue light on VESC when I opened up enclosure then no connection with Vesc Tool.
Then randomly light changed to normal and remote worked.

So, now I have to turn the vesc on and off about 15 times for it to work correctly. What would cause this!!?
I changed some parameters within the Vesc Tool (I was playing it safe before so was advised on here to change some parameters). I then took a ride for a few miles and it was pulling great and totally fine. Then next day, turned it on an nothing. Then I opened it up and took pics. The turned of and on a few times to try to connect to vesc tool and failed. Then randomly started working. Rode it for a further 8 miles totally fine. Now it takes 10-15 goes at powering on.

Any ideas!?

I got Vesc from eskate.eu in Italy.

Im in uk![IMG_0196|375x500](upload://mmblGkPkraMxtpRAuNFmXMvyWmk.jpg)![IMG_0195|666x500](upload://gMPCJSZp1OBfF23amHw3YItdixi.jpg)
```

---
## \#2 Posted by: Martinsp Posted at: 2018-02-26T14:46:14.208Z Reads: 109

```
Make sure the problem is not HW related so check connectors, BMS and battery than move on to the VESC because. it is easier to check connectors just unplug everything maybe check voltages and plug it back, see if it changes anything.
```

---
## \#3 Posted by: Scoo_B_SK8 Posted at: 2018-02-26T14:53:04.066Z Reads: 106

```
what is you method of "On/Off"?
-loop key
-eswitch
-plain ole plug and go
?
```

---
## \#4 Posted by: cliofreak Posted at: 2018-02-26T14:53:32.356Z Reads: 102

```
Its an e-switch with built in anti-spark
```

---
## \#5 Posted by: Scoo_B_SK8 Posted at: 2018-02-26T15:06:23.994Z Reads: 87

```
soo when you go for a ride while this is going on...does it cut out on you?

EDIT; i kinda wanna say its a short somewhere.  i know when i F up on an arduino wire up and try to connect  via serial (usb) it doesn't connect or power up. does the LED come on immediately then goes out right away?

you have multi-meter?
```

---
## \#6 Posted by: cliofreak Posted at: 2018-02-26T15:22:35.241Z Reads: 82

```
I have a multimeter but Ive not probed around yet.
When it powers on eventually, its fine! No cut outs or anything.
```

---
## \#7 Posted by: Scoo_B_SK8 Posted at: 2018-02-26T15:53:15.845Z Reads: 76

```
here is what i would do...
test starting from battery...
then eswitch...

if you have a fuse DBL check it is not 1/2 blown.
```

---
## \#8 Posted by: ZackoryCramer Posted at: 2018-02-26T16:54:05.728Z Reads: 69

```
I had an issue like yours once and it was due to a faulty receiver. The vesc would randomly cut out in split second intervals, and after a while it just broke. Maybe try a different pair and try running the motors using the vesc tool. I changed to an rc car remote and it went fine. 🚙
```

---
## \#9 Posted by: Scoo_B_SK8 Posted at: 2018-02-26T17:34:53.551Z Reads: 73

```
[quote="ZackoryCramer, post:8, topic:47513"]
faulty receiver
[/quote]

as far as that avenue... this is all i can see that may or may not add clout. (the backside looks good)

![mayvesc13|375x500](upload://6NDimwNqz8uIrLOg4KEq64uHmc9.jpg)

being that having trouble connecting via serial usb i wouldn't think so, but if you had another remote around its worth a shot.
```

---
## \#10 Posted by: RedEagle Posted at: 2018-02-26T17:47:08.369Z Reads: 68

```
You rode with all that heatshrink still on?!

You should NEVER ride with heatshrink. First thing I did when preparing for the first ride was removing any and all heatshrink. You probably cooked something in the process. The vesc needs all the air it can get. Leaving it encased in heatshrink only guarantees disaster. Just my 2c.

It seems I'm the only one rocking maytech vescs without any major problems for a year around here.
```

---
## \#11 Posted by: cliofreak Posted at: 2018-02-26T19:18:49.782Z Reads: 65

```
Yeah, Ive been riding with heatshrink on. Ive never seen anything mentioned about removing it but Ill take it off as you suggest. I've studdied the results from the Metr app after the last few rides and the Vesc did get up to 78 deg when going up a long steep hill. I then swapped back to 90mm (from 100mm MBS) to see if it'd take the strain away. It did, so Ive currently got a 42T in the post to replace my 36T so there will be more torque and less heat. 

Possibly Ive cooked something but I cant understand why it'll work sometimes and not others. I'll get a closer look this evening.
```

---
## \#12 Posted by: SOICDIP Posted at: 2018-02-26T20:29:42.813Z Reads: 66

```
If it's an intermittent issue, try flexing the PCB and see if the VESC starts responding again. It may be a bad solder joint.

Is anything heating up when the VESC is not responsive?
```

---
## \#13 Posted by: RedEagle Posted at: 2018-02-26T21:27:48.087Z Reads: 67

```
It seems to me you fried the drv. Try typing faults in the console(?) tab and see if it returns anything. 
You also may or may not have shorted motor phase leads.
At this point I would just get a new vesc or replace the drv.
```

---
## \#14 Posted by: cliofreak Posted at: 2018-02-26T23:57:21.704Z Reads: 65

```
This may be the excuse ive been waiting for to buy the FocBox.

Im almost 100% sure that its a loose connection and that the VESC is fine.
I've discovered that when I turn on the board with wheels on floor, its fine everytime. When I turn it on with board on its back, it fails to boot. Must be something loose thats stopping it from booting up (yet still gives it power to the led).
```

---
## \#15 Posted by: RedEagle Posted at: 2018-02-26T23:59:16.575Z Reads: 64

```
Then check your connectors for anything suspicious, cold solder joints for example.
```

---
## \#16 Posted by: cliofreak Posted at: 2018-02-27T00:07:38.833Z Reads: 63

```
Yeah, Id have done it already but I cant get the bolts off the enclosure lol
Im afraid of rounding them out so Ive just ordered fresh new torx socket set.
Too much of the old thread lock ;)
```

---
## \#17 Posted by: RedEagle Posted at: 2018-03-01T20:31:34.715Z Reads: 54

```
Soo... any updates?
```

---
## \#18 Posted by: cliofreak Posted at: 2018-03-01T20:43:03.289Z Reads: 56

```
Still waiting on Torx socket set. The weather is snow joke!
```

---
## \#19 Posted by: Bjork3n Posted at: 2018-03-01T20:55:16.167Z Reads: 55

```
Most people have the heat shrink on, me included. 
No issue. 
First time I heard a recommendation to remove it.
```

---
## \#20 Posted by: RedEagle Posted at: 2018-03-02T01:53:53.917Z Reads: 56

```
Well I'd rather be safe than sorry. There is a reason I've had no problems whatsoever with my maytechs..
```

---
## \#21 Posted by: biggdaddyhawk Posted at: 2018-03-02T04:02:31.098Z Reads: 48

```
If you have a good heatsink on the top and bottom of the FETS would you still need to remove the heatshrink?
```

---
## \#22 Posted by: RedEagle Posted at: 2018-03-02T14:23:02.565Z Reads: 46

```
I'd say no. You already solved a big part of the problem. I would be a little worried about the drv though. If it gets cooked you're dead. Then again.. I may be too cautious just because I run maytechs xD
```

---
## \#23 Posted by: biggdaddyhawk Posted at: 2018-03-02T19:15:47.112Z Reads: 47

```
So do I need to heatsink the drv as well? Seems like that's what everybody burns...not the mosfets.
```

---
## \#24 Posted by: RedEagle Posted at: 2018-03-03T00:29:01.209Z Reads: 49

```
AFAIK there is no way you can put a heatsink on the drv. Only on the fets
```

---
## \#25 Posted by: GrecoMan Posted at: 2018-03-03T00:32:23.704Z Reads: 45

```
WRONG. my heatsink cools the fets and the drv. it’s a bit ghetto but just find the thickest thermal pads you can find and stack until they contact the drv and heatsink. it helps a crazy amount

also about this heatshrink thing... i don’t think that’s true...
i rode both my vescs with heatshrink without an issue. why would the manufacturer spend the extra $$ if it negatively effected the performance? if you’re pushing your vescs so hard that heatshrink becomes a problem, you need to change your settings...
```

---
## \#26 Posted by: RedEagle Posted at: 2018-03-03T00:39:42.415Z Reads: 44

```
Well, that's one way to do it...

About that.. I'd rather take the heatshrink off and not be thrown off my board because of a piece of plastic than keeping it on and faceplanting thank you very much.

Maytech vescs make you paranoid(in every positive sense of the word).
```

---
## \#27 Posted by: GrecoMan Posted at: 2018-03-03T00:40:56.115Z Reads: 44

```
if the vesc overheats it doesn’t slam the brakes. i’ve experiences it. it thermal throttles just like a computer. it will not push itself to death, unless something in your setup is wrong.
```

---
## \#28 Posted by: RedEagle Posted at: 2018-03-03T00:46:24.662Z Reads: 42

```
Same here. I've had some weird moments when I had cutouts and such. But those issues were non vesc related. 
There is a common misconception that maytechs are so bad you should never go near them. I say it depends on the person himself. If you respect your hardware and treat it like you do there is no room for failure. Same goes for batteries. _Especially **lipo's**._
```

---
## \#29 Posted by: Daniel828 Posted at: 2018-03-05T01:59:22.447Z Reads: 38

```
I have a maytech vesc and it’s been working great. I had a problem in the beginning, I was having intermittent cut out problems. It powered up normally but after I was rolling it would start stuttering   The problem was that the receiver was too close to the vesc.  It’s now located as far as the receiver cable will allow.  It’s working great now, no probs. This is just my 2 cents
```

---
## \#30 Posted by: RedEagle Posted at: 2018-03-07T00:34:08.766Z Reads: 37

```
Same here. 

I've not used my board for about two weeks. Recently I started boarding again and was having cut outs. I moved the receiver around and it got a little better. Before this the receiver was in the same place and I had zero problems. After a few days no more jittering/stuttering at speed. Guess it was just a little rusty. :rofl:
```

---
## \#31 Posted by: cliofreak Posted at: 2018-03-10T00:41:46.158Z Reads: 30

```
So, yeah... this Maytech makes no sense. Acts like a loose connection. Intermittent issues of booting up correctly (blue and a green when signal detected) and not booting up and displaying blue and red light side by side. LED battery display works and shows % correctly. All voltages are good. Its like it just sometimes kicks in and sometimes won't.
Thing thats so weird is that when it finally works (after 15min of on/off, rotating it, moving it away from other stuff. restarting controller, lying it on its back, on its front...) when it works, it works for miles. No cut outs. No judders. No issues. Its like its totally a boot up software issue and when it finally boots ok, its perfect.

So, feck it. I need a Focbox. 
Why on earth are they sooooooo expensive!?
```

---
## \#32 Posted by: RedEagle Posted at: 2018-03-10T00:55:17.983Z Reads: 26

```
Does this also happen when you have no receiver connected?
```

---
## \#33 Posted by: cliofreak Posted at: 2018-03-10T00:55:59.324Z Reads: 27

```
yeah, same with no receiver
```

---
## \#34 Posted by: RedEagle Posted at: 2018-03-10T01:01:14.288Z Reads: 25

```
Hmm.. My vesc was having cutouts and jittering at high speed. Turned out to be a receiver problem. Seems to me you've got a bad batch of vesc. Maybe it's something that you did recently that triggered it? My jittering and cogging problem began when i disconnected the motor for service. 
My maytech has been running strong for about a year. Nothing major I can't fix. (I'm lucky I know hehe)
```

---
## \#35 Posted by: cliofreak Posted at: 2018-03-10T01:04:33.948Z Reads: 25

```
Yeah, id say this one is fecked. Its doesnt make any sense and intermittent stuff drives me mad. Lifes too short for this farting around.
```

---
## \#36 Posted by: RedEagle Posted at: 2018-03-10T01:05:55.288Z Reads: 26

```
[quote="cliofreak, post:35, topic:47513"]
Lifes too short for this farting around.
[/quote]

 You mean ''Foc'ing around''.
```

---
## \#37 Posted by: cliofreak Posted at: 2018-03-10T01:10:06.159Z Reads: 23

```
hahahahahaha yes indeed
```

---
