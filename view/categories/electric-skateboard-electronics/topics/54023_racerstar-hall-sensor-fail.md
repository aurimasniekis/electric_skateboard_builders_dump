# Racerstar hall Sensor fail

### Replies: 38 Views: 1508

## \#1 Posted by: briman05 Posted at: 2018-05-01T12:46:04.348Z Reads: 196

```
Hey guys I'm in the final stage of completing my board I started planning this board about 6 months ago and I finally got my motors configured.  I want to run in sensored mode so it has the smooth start without having to do a kick start.  After watching several video about set up the board in the bldc tool from Jacobby and talking to @Deckoz I felt confident in my ability to know how to set it up.  First motor config was fine hall sensor was picked right up and configured.  When I shut down my board and plugged in my second motor the motor was detected but the hall sensor detection failed.  

I'm using racerstar BRH motos from banggood.com.  I have already put in a claim with banggood but I highly doubt I will get anything back from them.  @Deckoz suggested I try to plug the motor with the failed hall sensor into the focbox that detected the first one.  I will have to try that when I get home.  I brought the motor in to work today so I could check the continuity on the leads to see if I can find the reason why.

https://www.banggood.com/Racerstar-5065-BRH5065-200KV-6-12S-Brushless-Motor-With-Gear-For-Balancing-Scooter-p-1117658.html?cur_warehouse=CN
```

---
## \#2 Posted by: rich Posted at: 2018-05-01T13:50:18.864Z Reads: 173

```
[quote="briman05, post:1, topic:54023"]
@Deckoz suggested I try to plug the motor with the failed hall sensor into the focbox that detected the first one.
[/quote]


Yeah, definitely try that.

Also did you try different phase wire combinations? That could help as well
```

---
## \#3 Posted by: briman05 Posted at: 2018-05-01T15:22:15.447Z Reads: 157

```
I’m I feel like if it works on one but not the other it’s the focbox. And then Enertion will say user error fault pay us to fix it.
```

---
## \#4 Posted by: Mikenopolis Posted at: 2018-05-01T19:45:41.402Z Reads: 149

```
I sent in my carvon motors to upgrade the adapters and when it came back the hall sensor detection failed on both motors.

After a lot of frustration, I talked to Jerry and sent them back to him to check. It's back again and I haven't tried again. But he said when he opened them up, the sensor wires were too close or touching the phase wires. I wonder if that's your problem.
```

---
## \#5 Posted by: briman05 Posted at: 2018-05-01T20:24:06.943Z Reads: 134

```
I’m not sure how I would open this motor it is basically like the old Olin board or the evolve motor.
```

---
## \#6 Posted by: Jebe Posted at: 2018-05-01T20:31:28.744Z Reads: 127

```
Hit that search button. Likely to be motor not vesc. Could even be the hall sensor cable. Have a close look at the plug and check connections. Careful pulling that motor apart not to pinch your hand. Those magnets are powerful and when you remove the shaft they pull the rotor up.
```

---
## \#7 Posted by: briman05 Posted at: 2018-05-01T22:06:21.527Z Reads: 126

```
Could you maybe post the link because I can’t find any for this motor
```

---
## \#8 Posted by: Benjamin899 Posted at: 2018-05-01T22:19:58.889Z Reads: 122

```
isnt racestar know for being a bit shitty?
```

---
## \#9 Posted by: briman05 Posted at: 2018-05-01T22:35:35.850Z Reads: 115

```
It’s actually what evolve uses and ollin used the same motors as well
```

---
## \#10 Posted by: Deckoz Posted at: 2018-05-01T23:34:42.791Z Reads: 120

```
Ok so I have another idea. 

[quote="rich, post:2, topic:54023"]
different phase wire combinations?
[/quote]

Because @rich reminded me with this. I believe these cheaper motors(I ordered some of the bh5045) do not use 120 degree hall sensors, but side by side Hall's. So the phase wires and sensors will only properly detect when plugged in a certain way. This may mean your plugging it in, and it is spinning the wrong direction.

To fix this due to hardware limitations you will need Ackmaniac ESC Tool 3.100. first because it's a focbox and stock vesc tool has an issue initializing, which acks firmware fixes. But this also puts you on 3.xx firmware which has built in motor direction switching, unlike bldc tool.

Plug the motor in the same way as the motor that detected and dectect it on 3.xx, then change motor direction on the motor tab.

If this doesn't solve it and both motors cannot detect sensors on that focbox I would consider a possible focbox fault.. however if you are dead set on running bldc tool, then you can swap the hall sensor wires to be in the correct order with the phases to detect.

I think @Blasto or @JohnnyMeduse may have dealt with 120° vs side by side hall detection difference, if you choose to repin on 2.XX bldc tool
```

---
## \#11 Posted by: rich Posted at: 2018-05-01T23:52:46.226Z Reads: 111

```
There are 6 possible phase wire combinations.... 
I also had troubles with hall sensor detection but in my case 3 of 4 vescs had broken hall sensor ports :laughing:
```

---
## \#12 Posted by: briman05 Posted at: 2018-05-02T01:53:30.885Z Reads: 108

```
Well I have a Mac and I’m not sure @Ackmaniac vesc tool would work on a mac
```

---
## \#13 Posted by: Deckoz Posted at: 2018-05-02T02:06:17.076Z Reads: 111

```
https://www.dropbox.com/sh/t7dl90owz5ccbyl/AAD7CSlrseqWVMTkxu5V7bT6a/Old/ACKMANIAC-ESC-Tool_3_100?dl=0&preview=ACKMANIAC-ESC-Tool_3_100.pkg.zip
```

---
## \#14 Posted by: Deckoz Posted at: 2018-05-02T02:49:16.356Z Reads: 101

```
Before you do this just try to change the phase wires and detect. If so and it spins backwards and you know it detects properly then do the firmware and void your warranty. Just making friendly suggestions. Just in case it is the focbox sensor port..
```

---
## \#15 Posted by: briman05 Posted at: 2018-05-02T03:01:35.317Z Reads: 98

```
Yeah I will try changing the phase wires. I have the motors mounted as rear wheel drive. I will try it on the focbox that picked up the hall sensor first then I will try different phase wire combinations. I tried to make sure that they were going in the same spots on both of boxes when I was configuring them last night.
```

---
## \#16 Posted by: Ebisane9 Posted at: 2018-05-02T03:29:23.213Z Reads: 98

```
waaaaaaaaittttaminnnuuuuute....the 3.1 firmware can change motor direction in the tool so you don't have to switch phase wires?!?
```

---
## \#17 Posted by: Ackmaniac Posted at: 2018-05-02T05:42:46.396Z Reads: 95

```
Vedders vesc tool can do that as well. It's a feature he implemented in the original firmware for all versions that start with a 3.
```

---
## \#18 Posted by: egzplicit Posted at: 2018-05-02T08:17:01.155Z Reads: 95

```
[quote="briman05, post:15, topic:54023"]
Yeah I will try changing the phase wires.
[/quote]

When I ran my build on 5065 140k racerstars I had no issue running sensor detection (focbox, 3.100 firmware).

This is the order I (randomly) used when soldering the jst adapter:

![image|667x500](upload://o4sc6FLgkgfGKyDvzdrhPNT6a2N.jpeg)

![image|666x500](upload://2L5wn4xjwArWmWi3JEJnfBx9evJ.jpeg)

I would try this and see if it works.
```

---
## \#19 Posted by: briman05 Posted at: 2018-05-02T13:09:35.514Z Reads: 94

```
So I tried every combination for the phase wires and none worked. I checked the motor on the other focbox and the hall sensor detection worked.  

One thing I noticed is that the bemf and integrator limit where very different on the 2 motors I guess that would be because sensor worked on one and not the other. I believe those settings were very different on the same motor but different focboxes. When I do a motor detection it does give me values to put in for the sensor is that normal?
![image|375x500](upload://5QutbiBixWaPsSzDDR6VptKvXGF.jpeg)
```

---
## \#20 Posted by: briman05 Posted at: 2018-05-03T11:53:54.649Z Reads: 86

```
So I updated the firmware to ackmaniacs firmware. First after updating the firmware it locked up my MacBook Pro and I had to force quit the program. Then started to configure the motors and the motor detection on both hall sensors are now failing how can this happen the one was detected by bldc tool and will not detect on ackmaniacs.
```

---
## \#21 Posted by: Blasto Posted at: 2018-05-03T12:28:22.906Z Reads: 84

```
Try running foc sensored.

There’s a hall table that appears, but seems to be off a bit
```

---
## \#22 Posted by: briman05 Posted at: 2018-05-03T12:33:36.614Z Reads: 84

```
I would rather run bldc be it is less chance of blowing my focboxes.  Plus I feel like bldc is a lot simpler of a set up and should pick it up.  That really has me pissed is that the sensor was detected on the bldc tool for enertion.
```

---
## \#23 Posted by: Blasto Posted at: 2018-05-03T12:58:44.424Z Reads: 82

```
Foc gives a bit more detailed hall sensor table, for that reason i’m asking.
```

---
## \#24 Posted by: JohnnyMeduse Posted at: 2018-05-03T13:01:27.333Z Reads: 83

```
![FOC STEP|690x365](upload://vqWMCIBGR5wwrhC1IT3m8aA5N2B.png)
```

---
## \#25 Posted by: briman05 Posted at: 2018-05-03T13:07:11.059Z Reads: 84

```
Ok I can try it tonight.  It is just mind boggling that one sensor was picked up in the enertion bldc tool and one wasnt ok half the battle won.  Then change it over to ackmaniac's esc tool and neither are detected.  Now that is in the BLDC tool and since everyone said the ack's esc tool was better i updated and switched to that.  So would it be the same process?
```

---
## \#26 Posted by: Blasto Posted at: 2018-05-03T14:32:20.234Z Reads: 81

```
I do not think changing FW will make a difference here. You are detecting a hall table, but it seems it is out of the boundaries for a "pass" in BLDC

![image|356x162](upload://5W4hijDOB7tgQhrg7BmsaJVrxz5.jpg)

FOC sensor detection is a little different and it's a little less sensitive to hall placement.

I have a feeling that the sensors may be a tad bit far away from the rotor magnets or that the whole assembly is crooked inside the motor making the readings oscillate.

stick with the current tool for now, try out FOC
```

---
## \#27 Posted by: briman05 Posted at: 2018-05-03T16:18:52.800Z Reads: 75

```
That was on the bldc tool and said detection failed.  I will have to try it on Foc I guess.  Atleast if I get it in Foc it will be nice a quite running
```

---
## \#29 Posted by: briman05 Posted at: 2018-05-04T00:32:41.688Z Reads: 74

```
Now I just restarted everything and it came back and read the firmware and connected.  Plus it detected the sensors in FOC on both motors
```

---
## \#30 Posted by: Deckoz Posted at: 2018-05-04T02:24:18.017Z Reads: 71

```
@briman05 nice

@Blasto @JohnnyMeduse  thanks for stepping in 🙌🙌🙌
```

---
## \#31 Posted by: briman05 Posted at: 2018-05-04T03:09:12.990Z Reads: 69

```
I want to thank everyone for there help especially @JohnnyMeduse @Blasto and @Deckoz. I just need to figure out how to ease it into going because the remote is very touchy.
```

---
## \#32 Posted by: JohnnyMeduse Posted at: 2018-05-04T03:18:24.749Z Reads: 69

```
What Remote do you have ?
```

---
## \#33 Posted by: briman05 Posted at: 2018-05-04T03:44:04.214Z Reads: 68

```
I have the Nano-x
```

---
## \#34 Posted by: Blasto Posted at: 2018-05-04T04:38:06.211Z Reads: 68

```
Need to calibrate the remote everytime you turn the remote on.

Turn on remote, board off
Push to max throttle, pull to min throttle. (Calibration done)
Turn on board.

You can still “calibrate” after the board is on, lift up your wheels, push-pull max-min and your done
```

---
## \#35 Posted by: JohnnyMeduse Posted at: 2018-05-04T04:56:00.638Z Reads: 69

```
Like That guy said... :arrow_up::arrow_up::arrow_up::arrow_up::arrow_up::arrow_up:
```

---
## \#36 Posted by: L3chef Posted at: 2018-05-04T05:00:08.867Z Reads: 73

```
[quote="Blasto, post:34, topic:54023"]
Need to calibrate the remote everytime you turn the remote on.
[/quote]

I did not know this. Thanks!
```

---
## \#37 Posted by: briman05 Posted at: 2018-05-05T03:51:52.616Z Reads: 61

```
Could you explain the calibration of the remote. I have a loop key anti spark so without it in there is no power to the receiver. So how would the remote calibrate with out the receiver being powered
```

---
## \#38 Posted by: Deckoz Posted at: 2018-05-05T03:57:04.909Z Reads: 60

```
Remote is in your hand, the pot for the throttle needs calibrated to send the proper PPM to the receiver. Turn on the remote... Push throttle full, then full brake. Then plug in your board.. 

Receiver not involved..
```

---
## \#39 Posted by: briman05 Posted at: 2018-05-05T13:05:31.243Z Reads: 55

```
Ok thanks.
```

---
