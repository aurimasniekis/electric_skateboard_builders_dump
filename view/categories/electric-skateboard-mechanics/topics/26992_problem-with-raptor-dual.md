# Problem with Raptor Dual

### Replies: 27 Views: 1023

## \#1 Posted by: Battosaii Posted at: 2017-07-07T16:17:41.120Z Reads: 93

```
i just go the board in today and decided to try out i went around the block a few times with no problems, just scary fast, then i decided to take a trip to a mcdonalds and i didnt make it, about a mile in i start getting random braking under acceleration then i lost all power. i had to push back home in 95degree heat it wasnt fun. I took the cover off and nothing is lose what could have caused this? here is the video i made when it happened.
https://www.youtube.com/watch?v=ED-DAbzPngk
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-07T16:19:57.841Z Reads: 94

```
[quote="Battosaii, post:1, topic:26992"]
95degree heat
[/quote]

That's probably issue, overheating
```

---
## \#3 Posted by: Battosaii Posted at: 2017-07-07T16:22:15.439Z Reads: 90

```
well the motors were cool to the touch, i wasnt riding hard at all. If it were overheating wouldnt it go away when theboard cools down?
```

---
## \#4 Posted by: Jinra Posted at: 2017-07-07T16:22:58.548Z Reads: 88

```
oh i can't watch the video right now, but the board doesn't turn on at all anymore?
```

---
## \#5 Posted by: Battosaii Posted at: 2017-07-07T16:25:28.280Z Reads: 88

```
yes, it never turned off i just lost power to the wheels. one motor dosnt turn at all and the other jutters and barely turns. i assumed something came loose but it may be a faulty component, could it be the dreaded winning remote thats giving me this issue?
```

---
## \#6 Posted by: Jinra Posted at: 2017-07-07T16:32:07.239Z Reads: 85

```
Best thing to do is plug it into BLDC tool on your computer and see if you have any faults. Don't apply too much throttle to a motor that refuses to turn or you may blow your VESC
```

---
## \#7 Posted by: Battosaii Posted at: 2017-07-07T16:41:28.105Z Reads: 80

```
im going to try that in a few minutes, i hope its something i can fix today i want to ride so bad.
```

---
## \#8 Posted by: Battosaii Posted at: 2017-07-07T17:17:16.661Z Reads: 75

```
so i have my Raptor hooked up to the bldc tool, sorry im a complete noob how do i check for faults?
```

---
## \#9 Posted by: Jinra Posted at: 2017-07-07T17:18:50.174Z Reads: 76

```
Get it to act up, then go to "terminal" and type "faults"
```

---
## \#10 Posted by: Battosaii Posted at: 2017-07-07T17:26:32.056Z Reads: 70

```
ok i checked both Vesc and no fault codes i also ran motor detection on both Vesc and found that the left motor revved and was fine it just didnt detect hall sensors and then i tested the right side motor and it would not spin it would just jutter like crazy and then fail to detect the motor. it looks like my motor has failed, it coggs pretty badly. are enertion motors still available? if not what else can i replace it with? and can i disconnect the second vesc and ride single motor for now?
```

---
## \#11 Posted by: Jinra Posted at: 2017-07-07T17:29:00.081Z Reads: 65

```
Plug the "bad" motor into the other VESC and run detection again to verify it's the motor and not the VESC that's gone bad.
```

---
## \#12 Posted by: Battosaii Posted at: 2017-07-07T17:33:32.482Z Reads: 65

```
Thank you @Jinra for all the help i found the problem i did as you said i went to swap over the vescs and when i pulled the right one out i saw this. <img src="/uploads/db1493/original/3X/e/5/e5f8991de0d93e17cb2753d50b844f11cffd2e99.jpg" width="666" height="500"> im pretty sure all i have to do is solder it back on and i should be good to go
```

---
## \#13 Posted by: Jinra Posted at: 2017-07-07T17:36:06.224Z Reads: 64

```
Yea, looks like broken solder joint. If I were you I would take them all off and resolder then onto wire. Connections where bullets are soldered straight to the PCB are known to fail.
```

---
## \#14 Posted by: Battosaii Posted at: 2017-07-07T17:42:16.841Z Reads: 62

```
yea im going to order good quality wire online and do that but for now im gona do a quick fix and actually ride this for a little bit, hopefully nothing else comes out to bit my ass lol. another concern i had was from another forum member, if i go full throttle( when the board was working) and turn off the remote it would continue full throttle for about 2 seconds then full brake, i feel thats super dangerous especially with a winning remote, what are the settings to fix that issue so that it just coast if signal is lost
```

---
## \#15 Posted by: Jinra Posted at: 2017-07-07T17:44:55.676Z Reads: 62

```
Make sure you insulate with some electrical tape or heatshrink, if it comes loose again and touches the other phase connectors, you'll street your face or worse.
```

---
## \#16 Posted by: Mikenopolis Posted at: 2017-07-07T17:53:56.492Z Reads: 61

```
[quote="Battosaii, post:14, topic:26992"]
and turn off the remote it would continue full throttle for about 2 seconds then full brake
[/quote]

Rebind the remote and for god sake don't ride the board until you fix that failsafe. If that LOSING remote disconnects like some of ours then you will eventually get hurt. Do the full throttle, turn off remote check to see it it coasts or brakes after any build.

https://www.electric-skateboard.builders/t/please-help-when-turning-off-my-controller-the-motor-goes-full-speed/17001/2
```

---
## \#17 Posted by: Battosaii Posted at: 2017-07-07T19:24:38.682Z Reads: 50

```
i ended up soldering all 6 bullet connectors to 10awg wire and soldering the wire to the vescs and i also re paired the remote and now all my issues are gone and the board is working properly.


 time to out and enjoy this bad boy, btw I am a heavy guy and this thing does not even notice my size lol! im going to post up a video later.
```

---
## \#18 Posted by: Battosaii Posted at: 2017-07-07T21:31:21.897Z Reads: 48

```
wow I can safely say the Raptor is Big Boy approved, it flew up a parking garage I cant believe it could do that. thanks for all the help after an hour of riding she has not had a single hiccup.
```

---
## \#19 Posted by: Battosaii Posted at: 2017-07-08T21:01:57.718Z Reads: 35

```
so i think my right vesc broke, i noticed a bit of a lack of power today and belt slipage at full throttle and light braking which has not happened before, i assumed that i may need to change to belts. i turn the board over and only the left motor is working and it stutters and does not accelerate in free spin but will work fine under load ( when im standing on the board.) i swapped the vesc's over and the right side vesc would not turn or detect either motor. when i push the throttle the vesc just blinks red. The left side vesc will turn both motors. The BLDC tool says no faults were found when i plug it in but it wont detect either motor. 

What are my options? i cant just replace one can i? both vesc's need to be the same? @onloop @Jinra
```

---
## \#20 Posted by: Jinra Posted at: 2017-07-08T21:03:17.242Z Reads: 33

```
might be a burnt DRV, go to terminal in bldc tool and type "faults".
```

---
## \#21 Posted by: Battosaii Posted at: 2017-07-08T21:08:00.157Z Reads: 32

```
i did and it said no faults found.
```

---
## \#22 Posted by: Jinra Posted at: 2017-07-08T21:09:23.331Z Reads: 32

```
keep in mind if you turn the vesc off and on, all faults get cleared, make sure you do it when it happens.
```

---
## \#23 Posted by: Battosaii Posted at: 2017-07-08T21:09:52.843Z Reads: 34

```
ok ill try it again and see what it says
```

---
## \#24 Posted by: Battosaii Posted at: 2017-07-08T21:13:38.630Z Reads: 33

```
yep DRV8302 darn it not even 2 days and the same vesc has broken twice lol
```

---
## \#25 Posted by: Jinra Posted at: 2017-07-08T21:15:07.413Z Reads: 33

```
One problem might have caused the other.
```

---
## \#26 Posted by: Battosaii Posted at: 2017-07-08T21:18:17.128Z Reads: 33

```
hmmm i want to replace both vesc with good quality vesc's im thinking ollins or focbox.
```

---
## \#27 Posted by: Jinra Posted at: 2017-07-08T21:20:15.882Z Reads: 32

```
Axle is also a cheap, quality alternative. Though not sure if they're taking new orders right now.
```

---
