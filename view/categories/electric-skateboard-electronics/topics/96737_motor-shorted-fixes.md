# Motor shorted, fixes?

### Replies: 4 Views: 193

## \#1 Posted by: JensSjogren Posted at: 2019-06-16T16:37:49.654Z Reads: 72

```
Hi builders, so i've been running 2x APS 8085 motors on my trampa for the last few weeks. Those things are a blast but yesterday during a ride one of the motor suddenly twitched and seemingly put on the brakes almost sent me flying. The motor got resistance even when turned of so i either thought a bearing was broke or that it was shorted.

I opened the motor up and noticed the red phase cables insulation was melted and one copper wire was cut of, this wire was in contact with another winding that belongs to the black phase cable, so it probably shorted that winding. I decided to put a shrinktube on the red cable to insulate the copper and try it again. I got rid of the constant resistance and the board worked fine for a couple of kilometers until it did the same thing as yesterday, this time however it doesnt have any resistance when spinning it by hand, if its shorted it should have resistance all the time right? I'm also able to max out the motor without any load and it seems fine, no fault codes in vesc tool app either. 

My guess so far is that the windings that had contact with the cut off wire got it's protective coating damaged and now the winding shorts itself changing the KV of the motor, when i slam the accelerator the traction control that is set to 3000 ERPM difference doesnt react in time since the KV of my motors are now different, causing my motor to break after some time. This is a wild guess since i really don't know much about this stuff.

I know this is messy written, i'm afraid that i'm unable to explain it in a better way in english though, any input is greatly appriciated! 

![20190616_100627|375x500](upload://aS023EKnagpt4vsIxNbgyly7wUs.jpeg)
![received_2517398781614757|259x500](upload://4KrLzk5k9ziqEqvEV5dTROIezg5.jpeg)
```

---
## \#2 Posted by: banjaxxed Posted at: 2019-06-17T14:41:29.382Z Reads: 43

```
Try Bruno @ALIENPOWERSYSTEM1 @AlienPowerSystem

Probably email using your order ID email to get a response tho

Failing that you are going to have to disassemble the stator from the baseplate to get at that   🙁

Apart from the epoxy it will more than likely be press fitted which means a freezer bag and time in the freezer before setting a heat gun on the outer part to separate, sorry no manual there it came up in discussions on  a couple of days ago

Alternatively try clipping that stray wire and sliding over some thick adhesive heatshrink over that phase, it’s not actually that obstructed

Then battle harden the windings to stop any reoccurrence
```

---
## \#3 Posted by: JensSjogren Posted at: 2019-06-17T17:57:23.945Z Reads: 34

```
As seen on the pictures i did dissasemble the motor, insulated the damaged wire with new heatshrink and put epoxy on everything. 

I went into vesc tool and ran new motor detections which doesnt give any fault indications but the motors has very different values, the upper one is the one that shorted.

![received_2835464559857085|259x500](upload://lj39UCD2BBMAhD8Kf5RVvYiOOgU.jpeg) 

I also turned off the traction control, the board runs okay now but i do smell a slight burned scent from the previous shorted motor. I really think that the protective coating got damaged on one of the windings making the current take shortcuts and therefore giving different values and also creating a "hotspot" which gets very warm
```

---
## \#4 Posted by: banjaxxed Posted at: 2019-06-17T18:05:40.760Z Reads: 28

```
I didn’t see the repair photo, you may have blown the sensors on the shorted motor

Bruno sells the pcbs with wiring, try him? Maybe a warranty
```

---
