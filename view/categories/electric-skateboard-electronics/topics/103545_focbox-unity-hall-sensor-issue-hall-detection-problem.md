# FocBox Unity &#124; Hall sensor issue &#124; Hall detection problem

### Replies: 42 Views: 439

## \#1 Posted by: Buxzzix Posted at: 2019-11-02T20:22:42.295Z Reads: 72

```
Hello everyone!
I have a problem with my FocBox Unity. I'm trying to detect hall sensors in my motor but without any good results. I've checked the phase wires, checked hall wires, everything is okay. When I connect motors to normal FocBox, not to Unity, everything is fine. But when I connect motors to Unity it can't properly detect hall sensors. I'm using RacerStar 5065 motors. I have few of them and always is the same problem - it cannot properly detect hall sensors. I'm attaching screen to this topic.

Waiting for your reply and maybe for problem solution.

Best regards, Bartek

![73057735_416198729301961_7050820245295988736_n|243x500](upload://yVZHdOq0BI74ynThziMOIEqE5KY.jpeg)
```

---
## \#2 Posted by: CarlCollins Posted at: 2019-11-03T11:34:47.164Z Reads: 64

```
Looks like one of your motor is defective and might be cold solder joints on Unity phase wires, please double check the soldering.
```

---
## \#3 Posted by: Buxzzix Posted at: 2019-11-03T11:37:30.457Z Reads: 63

```
I've chcecked soldering on phase wires and on hall wires. As I said - everyting on motor side is okay. So what should I do? Check soldering on Unity's phase wires?
```

---
## \#4 Posted by: CarlCollins Posted at: 2019-11-04T12:14:58.713Z Reads: 54

```
Yeah! You have to check the Unity side of solders
```

---
## \#5 Posted by: Buxzzix Posted at: 2019-11-16T13:15:38.747Z Reads: 45

```
I checked soldering, everything is okay. I changed connectors nad issue is still the same. I have no idea what the f**k can be wrong....
```

---
## \#6 Posted by: Buxzzix Posted at: 2019-11-16T13:15:49.079Z Reads: 43

```
Any other ideas? :\
```

---
## \#7 Posted by: CarlCollins Posted at: 2019-11-16T13:52:41.863Z Reads: 43

```
I would like to check you Unity via remote connection, let me know when we can do it?
```

---
## \#8 Posted by: Buxzzix Posted at: 2019-11-16T16:48:39.659Z Reads: 40

```
When You only want. I'm totally always available
```

---
## \#9 Posted by: Tyler93245 Posted at: 2019-11-16T18:21:27.592Z Reads: 40

```
Try swapping your phase wires. I had this same issue, for some reason hall sensors were not detected in one configuration but when I swapped two all was well
```

---
## \#10 Posted by: Buxzzix Posted at: 2019-11-16T18:25:16.471Z Reads: 41

```
I've tried that. Please, this is not my first DIY build. I've made a lot of them. I'm not noob in this thread :smiley:
```

---
## \#11 Posted by: Tyler93245 Posted at: 2019-11-16T18:26:11.989Z Reads: 39

```
Just trying to help. I was dealing with this issue only 4 hours ago and that fixed it
```

---
## \#12 Posted by: Buxzzix Posted at: 2019-11-16T18:27:15.938Z Reads: 38

```
You have changed phase wires in only one motor or in both?
```

---
## \#13 Posted by: Tyler93245 Posted at: 2019-11-16T18:27:50.300Z Reads: 34

```
Up your duty cycle during detection, that might help also. Mine were default set to .05, I had to up them to .07 to work
```

---
## \#14 Posted by: Tyler93245 Posted at: 2019-11-16T18:28:06.201Z Reads: 33

```
Both
10char
```

---
## \#15 Posted by: Buxzzix Posted at: 2019-11-16T18:29:27.656Z Reads: 33

```
Wait a minute, I will try to increase duty cycle. You are using FocBoxTool or FocBoxUI ?
```

---
## \#16 Posted by: Tyler93245 Posted at: 2019-11-16T18:30:13.010Z Reads: 33

```
I am using VESC tool. You should have the ability to tweak duty cycle in the focboxtool though.
```

---
## \#17 Posted by: Buxzzix Posted at: 2019-11-16T18:34:05.048Z Reads: 32

```
Still same problem :\
```

---
## \#18 Posted by: Buxzzix Posted at: 2019-11-16T18:34:58.323Z Reads: 33

```
![Hall1|690x421](upload://h3dT8NmkLgh0xAZau9N8XCDkYOo.png)
```

---
## \#19 Posted by: Tyler93245 Posted at: 2019-11-16T18:46:20.618Z Reads: 31

```
I don't get it, your hall sensors seem to be populating fine on the bottom of the screen. Does it give you an error when you hit "apply"?
```

---
## \#20 Posted by: Buxzzix Posted at: 2019-11-16T18:47:06.890Z Reads: 32

```
Look at values, there are three 255 values. Should be only two.
```

---
## \#21 Posted by: Buxzzix Posted at: 2019-11-16T18:47:30.482Z Reads: 33

```
On single focbox it's working pretty well. No issues
```

---
## \#22 Posted by: Tyler93245 Posted at: 2019-11-16T19:24:01.845Z Reads: 33

```
It's possible the individual wires on the focbox sensor plug are swapped. For example, when I switched from a flipsky VESC to a MakerX VESC, I had to swap h1, h3, GND, and 5v. Maybe check the individual ports on the focbox vs. the unity to make sure the order is correct
```

---
## \#23 Posted by: Buxzzix Posted at: 2019-11-16T20:11:44.795Z Reads: 33

```
I checked that. Everything is fine. I've tried a lot of combinations with phase wires and with hall wires. No good results :\
```

---
## \#24 Posted by: Tyler93245 Posted at: 2019-11-16T20:14:10.421Z Reads: 34

```
Hm, maybe you should try BLDC first. That might help troubleshoot/ isolate some issues. If that doesn't work, it may be time to pull out a volt meter and start checking the VESC
```

---
## \#25 Posted by: Buxzzix Posted at: 2019-11-16T20:21:41.230Z Reads: 31

```
How to try BLDC in FocBox Tool?
```

---
## \#26 Posted by: Tyler93245 Posted at: 2019-11-16T20:23:33.494Z Reads: 31

```
Not too terribly sure actually. I tune exclusively with the VESC tool, which may be of use to try since this may be a software issue also
```

---
## \#27 Posted by: Buxzzix Posted at: 2019-11-16T20:24:57.934Z Reads: 30

```
I know that in the VESC Tool is position "BLDC", but I don't have it in FOCBOX Tool :sweat_smile:
```

---
## \#28 Posted by: Tyler93245 Posted at: 2019-11-17T00:42:47.100Z Reads: 29

```
Here is what I figured out today: 

In BLDC mode:
-In some configurations of the phase wires, hall detection will fail. If you swap wires and reconfigure, it should work. If it doesn't, mess with your duty cycle
-Once you have it working OK in BLDC, then take it over to FOC. 

Hope atleast some of that helps.
```

---
## \#29 Posted by: Buxzzix Posted at: 2019-11-17T10:07:25.741Z Reads: 29

```
Thank you so much for attention. Now Im gonna wait for @CarlCollins, maybe he can help me :>
```

---
## \#30 Posted by: CarlCollins Posted at: 2019-11-17T16:00:06.708Z Reads: 29

```
@Buxzzix  Are you available now?
```

---
## \#31 Posted by: Buxzzix Posted at: 2019-11-17T20:05:39.918Z Reads: 30

```
I am available in this week always after 17:00 Polish time. It's GMT +01:00.
```

---
## \#32 Posted by: Buxzzix Posted at: 2019-11-17T20:06:22.644Z Reads: 30

```
And of course right now :D
```

---
## \#33 Posted by: CarlCollins Posted at: 2019-11-18T15:46:57.745Z Reads: 29

```
I am available now, inbox me if you are ready to do this
```

---
## \#34 Posted by: Buxzzix Posted at: 2019-11-22T06:46:50.758Z Reads: 26

```
@CarlCollins is there possibility to help me today? :blush:
```

---
## \#35 Posted by: CarlCollins Posted at: 2019-11-22T15:26:05.275Z Reads: 20

```
@Buxzzix
I am available now, I was out for the funeral of my grandmother.
```

---
## \#36 Posted by: AlanZhou Posted at: 2019-11-22T16:17:48.084Z Reads: 20

```
[quote="CarlCollins, post:35, topic:103545"]
funeral of my grandmother.
[/quote]

Condolences
```

---
## \#37 Posted by: Buxzzix Posted at: 2019-11-22T17:06:48.849Z Reads: 22

```
[quote="CarlCollins, post:35, topic:103545, full:true"]
@Buxzzix I am available now, I was out for the funeral of my grandmother.
[/quote]

Oh my God, Im so sorry. Unfortunately, I know what you're going through.
```

---
## \#38 Posted by: Buxzzix Posted at: 2019-11-23T06:48:02.219Z Reads: 22

```
@CarlCollins maybe if everything is okay we can try today? But i need to know hour because I dont have notifications from this site, its complicated because of that :frowning:
```

---
## \#39 Posted by: Buxzzix Posted at: 2019-11-25T17:42:11.271Z Reads: 17

```
I tried something new - I install brand new bootloader via STLink, and then flash software... unfortunately it did not help :C
```

---
## \#40 Posted by: Buxzzix Posted at: 2019-12-01T15:24:30.042Z Reads: 17

```
@CarlCollins are you available today maybe? :slight_smile:
```

---
## \#41 Posted by: czerepsky Posted at: 2019-12-05T20:03:13.040Z Reads: 14

```
Hello everyone,

I have the same problem like You @Buxzzix. Each symptom which You described I have with my Unity :frowning: 
Have You guys found solution to resolve this issue ?
@CarlCollins could You help us?
```

---
## \#42 Posted by: Tyler93245 Posted at: 2020-02-03T11:33:36.015Z Reads: 8

```
Sorry for the late reply.

Months later, I now own a unity of my own, so I know what I'm talking about forsure compared to my earlier replies drawing experience from flipsky escs. I’ve experienced this issue a few times, two real solutions:

1. Keep switching phase wire configs until it works. I don't have 100% success with this

2. If that doesn’t work, running without sensors will fix the issues. The focbox is good at controlling motors without sensors anyways (better than a normal VESC) so this is fine
```

---
