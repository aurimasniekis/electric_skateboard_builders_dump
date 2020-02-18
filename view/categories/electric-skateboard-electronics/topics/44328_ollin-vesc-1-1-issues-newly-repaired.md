# Ollin Vesc 1.1 Issues (newly repaired)

### Replies: 49 Views: 1814

## \#1 Posted by: rocka Posted at: 2018-01-22T06:21:38.104Z Reads: 205

```
I have an Ollin Vesc 1.1 that I just received back from being repaired for a month and a half and it's not providing power to the motor. Chaka said that I had shorted the PPM cables of the vesc when I sent it in. The vesc is controlled by a servo signal from an arduino nano that takes input from a thumb throttle. The vesc seems to be operating properly with lights turning on when the throttle is applied and throws no faults when checked in terminal. I measured if there was voltage on the output of the vesc and found that when throttle is not applied there is the same voltage between the center pin and the outside cables as the battery voltage. This voltage is unaffected by the throttle when measuring both DC and AC voltage. I tested my motor with another speed controller and it worked fine so a bad motor can't be the problem. I'd love some help guys!![20180121_181133|374x500](upload://tELvw5jtj9iB3tiRYdI5qXYIJl0.jpg)![20180121_181206|374x500](upload://eezx8xrormx1dAfG2BsQyFAS7UH.jpg)![20180121_181200|374x500](upload://vnkyUQBxp2HAe6LIoTazdWuz101.jpg)![20180121_181338|374x500](upload://jInDFshSOvFhgxsNZNVQrybob8a.jpg)![20180121_181400|374x500](upload://3TJEzlOKKuKatsgqD2pHctLueey.jpg)![20180121_181146|374x500](upload://cwd9uF5AFfI63BHQpNf2bSUTcy4.jpg)![20180121_181421|374x500](upload://eBoSds2Fxi6Y2nEEaAVgZNNwf1y.jpg)![20180121_181153|374x500](upload://lVzTmy07Lp5GB8m0oHeXE0PnNie.jpg)![Capture|690x370](upload://1rJ7h1osXI9tt4Nuw4HpnIPGmAi.JPG)![Capture2|690x370](upload://oZePRyZN3c2tybIDzbnT40pshQ4.JPG)![Capture4|690x371](upload://y2IyThsXIbiWrnG2f7XVt1Za7bd.JPG)![Capture3|690x370](upload://293ZEMtJ9VQchY7xUdJ6FWUYIOw.JPG)![Capture5|690x370](upload://bU0aLwQQswuV7JEMEb1gefq78Qn.JPG)![Capture6|690x370](upload://75bR5F79t7672mb6xLf2x5vsSUt.JPG)![Capture7|690x371](upload://y1VOtqivWMa3vIEbS8XTMR7YJlk.JPG)![Capture8|690x371](upload://8koMdoCn0Wxg2ZDgfEFewI9CtYJ.JPG)![Capture12|690x370](upload://fu2Ge7priDnZg4pQ80BteOuNRQI.JPG)![Capture9|690x370](upload://rclzj5l1G1LMs7sDH7qAfrpPoYk.JPG)![Capture11|690x370](upload://katg0VepzCjVKLAZICd3oRXgkvS.JPG)![Capture10|690x370](upload://bXSgmBhv0HUx2KqV8lJi7x1DFWV.JPG)
```

---
## \#2 Posted by: Namasaki Posted at: 2018-01-22T16:11:07.671Z Reads: 125

```
Have you tried to contact Ollin about the problem?
That would be the first step.

The Vesc does not increase voltage as throttle is increased. 
It allows more current as throttle is increased
```

---
## \#3 Posted by: Blasto Posted at: 2018-01-22T16:25:55.090Z Reads: 126

```
I feel that your batt max is way to high, basically you have no safety mechanism in place with settings this high (not the cause of your current problem)

![image|430x182](upload://3sXCgmgH8UymIks587woApwvBsE.jpg)

I'm not to familiar with the ppm setting "current no reverse", but according to your real time data, you seem to be braking (or is that full throttle?) and the motor is not moving

![image|317x173](upload://crH8bNPiyVbeALDBlMxT8DCYbpF.jpg)

I'm not sure if you PPM window needs to be centered, currently you have it offset. you could try 

min ppm: 0.32
max ppm: 2.60

that should center your window with your current ppm output from the arduino. (why do you need an arduino anyways?)
```

---
## \#4 Posted by: Namasaki Posted at: 2018-01-22T18:04:13.092Z Reads: 113

```
Good eye @Blasto 
@rocka your absolute max is also too high. 
Acceptable range according to Vedder is 130-150
Also you have settings for dual Vesc but it appears that your running a single Vesc.
```

---
## \#5 Posted by: rocka Posted at: 2018-01-23T01:24:49.332Z Reads: 106

```
I contacted ollin and this is the response I got. ![Screenshot_20180122-172216|281x500](upload://vyfIobl85Xs8DCxEICf0JLHNVHx.png)
It also took quite a while to get any response back last time I emailed for help so I posted here first.
```

---
## \#6 Posted by: Namasaki Posted at: 2018-01-23T01:46:36.090Z Reads: 100

```
your screenshot link isn't working.

First you need to correct your bldc tool settings.
1. reduce your batt max to 50a
2. reduce absolute max to 130a
3. Limit max and min erpm to 60k and -60k
4. set battery cutoff start and end  22v and 21v
5. uncheck "send status over can"
6. uncheck "multiple esc's over can"
7. uncheck " enable traction control"
8. You need to get a successful motor detection, then apply the values and write configuration.

I am not familiar with using an Arduino controller.
Most of us use a 2.4ghz  ppm controller.
```

---
## \#7 Posted by: rocka Posted at: 2018-01-23T02:35:57.933Z Reads: 94

```
Thank you so much, I'll try this and post the results here
```

---
## \#8 Posted by: Namasaki Posted at: 2018-01-23T03:15:40.008Z Reads: 97

```
Have a look though these threads and maybe you can find some help with the Arduino
http://www.electric-skateboard.builders/t/arduino-help-and-ideas-thread/11900
http://www.electric-skateboard.builders/t/arduino-vesc-uart-communication-problem/18915
http://www.electric-skateboard.builders/t/control-vesc-with-arduino/6876
http://www.electric-skateboard.builders/t/arduino-nunchuck-remote-help/29838
http://www.electric-skateboard.builders/t/power-control-vesc-arduino/1796
http://www.electric-skateboard.builders/t/calling-vesc-uart-arduino-experts/42673
```

---
## \#9 Posted by: rocka Posted at: 2018-01-23T19:34:12.096Z Reads: 69

```
I did everything you said and didn't get any change. the motor is till not spinning and i'm not getting a detection. The arduino should not have any effect on the system as it worked fine before the fault and only outputs a servo signal to the ppm port of the vesc, the signal is even registering on the bldc tool
```

---
## \#10 Posted by: rocka Posted at: 2018-01-23T19:50:53.189Z Reads: 70

```
i believe that is showing that throttle is at 100%. I don't think PPM should be centered because i'm using current no reverse as as my control type. i'm using an arduino because I wanted to add other functionality such as cruise control, different power modes, and light toggles.
```

---
## \#11 Posted by: Namasaki Posted at: 2018-01-23T20:12:22.977Z Reads: 65

```
You have to get a successful motor detection befor dealing with the controller. 
Is your motor disconnected from the drive train while performing motor detection?
```

---
## \#12 Posted by: longhairedboy Posted at: 2018-01-23T20:31:48.348Z Reads: 63

```
PPM should always be centered, even when you're not using reverse. That could be a large part of the problem here.
```

---
## \#13 Posted by: rocka Posted at: 2018-01-23T20:39:15.176Z Reads: 57

```
The motor is connected to the vesc but the output shaft is not connected a belt or any drive train when I'm doing the detection. The motor also isn't making any sound and I can't feel any movement.
```

---
## \#14 Posted by: rocka Posted at: 2018-01-23T20:41:14.329Z Reads: 56

```
I had this working fine before with the ppm set like that. but I will go ahead and change the setting so it is centered when throttle in its resting position to see if it works
```

---
## \#15 Posted by: Namasaki Posted at: 2018-01-24T01:50:52.199Z Reads: 55

```
Are you using a sensored motor?
If yes, try disconnecting the sensor cable and do detection without the sensors
```

---
## \#16 Posted by: scepterr Posted at: 2018-01-24T01:54:07.764Z Reads: 54

```
I would set to No App, reboot, try detection then
```

---
## \#17 Posted by: rocka Posted at: 2018-01-24T01:59:51.031Z Reads: 54

```
i'm running the sk3 sensorless
```

---
## \#18 Posted by: Namasaki Posted at: 2018-01-24T02:04:28.466Z Reads: 53

```
what size and KV and are you running 6s.
```

---
## \#19 Posted by: rocka Posted at: 2018-01-24T02:04:34.722Z Reads: 54

```
just tried it. motor doesn't spin and its saying that the detection failed. but the vesc did blink green for a second
```

---
## \#20 Posted by: Namasaki Posted at: 2018-01-24T02:05:15.382Z Reads: 53

```
Does the motor turn freely by hand
```

---
## \#21 Posted by: rocka Posted at: 2018-01-24T02:05:20.764Z Reads: 49

```
I believe its 120 kv and i'm running 6s
```

---
## \#22 Posted by: scepterr Posted at: 2018-01-24T02:05:34.051Z Reads: 49

```
Increase the current in detection
```

---
## \#23 Posted by: rocka Posted at: 2018-01-24T02:06:50.863Z Reads: 51

```
motor turns freely by hand when unplugged, plugged in, plugged in with vesc powered on, and plugged in with vesc powered on and throttle turned
```

---
## \#24 Posted by: rocka Posted at: 2018-01-24T02:07:21.022Z Reads: 50

```
im at 6 amps right now, ill bump it up
```

---
## \#25 Posted by: rocka Posted at: 2018-01-24T02:11:08.253Z Reads: 50

```
tried it up to 30 amps to no change
```

---
## \#26 Posted by: Namasaki Posted at: 2018-01-24T02:11:40.883Z Reads: 48

```
I never had a problem doing detection at 6a
```

---
## \#27 Posted by: scepterr Posted at: 2018-01-24T02:11:46.426Z Reads: 49

```
Uhm shoulda mentioned not to go above 10..think you're still ok

Are there any faults other than just failed detection?
```

---
## \#28 Posted by: rocka Posted at: 2018-01-24T02:13:46.460Z Reads: 47

```
not a single fault, i wish it would at least give me something. thanks for all your help guys, you dont know how much this means to me.
```

---
## \#29 Posted by: Namasaki Posted at: 2018-01-24T02:14:18.202Z Reads: 47

```
Unplug the motor from the Vesc and touch any 2 of the 3 phase wires together and see if there is noticeable resistance when turning the motor by hand
If yes, then try one of the first 2 wires with the 3rd wire and check for resistance.
```

---
## \#30 Posted by: scepterr Posted at: 2018-01-24T02:14:30.056Z Reads: 48

```
Try bumping min erpm in detection at 6a
Up to 1000
```

---
## \#31 Posted by: rocka Posted at: 2018-01-24T02:20:16.568Z Reads: 48

```
i tried connecting every motor phase wire together in every two wire configuration and there was significant resistance on every one. the motor spins freely when unplugged. when i have the motor plugged in to the vesc there is noticeably more resistance than when completely unplugged but less than when two phase wires are connected.
```

---
## \#32 Posted by: Namasaki Posted at: 2018-01-24T02:21:29.284Z Reads: 46

```
There should be no resistance when plugged into the Vesc unless your applying brakes
You may have a short on the vesc
Did you try motor detection without the controller connected
```

---
## \#33 Posted by: rocka Posted at: 2018-01-24T02:25:45.747Z Reads: 43

```
this is the same problem i had last time with resistance on the motor when plugged in. but i sent it into ollin to get fixed. i got it back a few days a go and they said they replaced the board.
```

---
## \#34 Posted by: rocka Posted at: 2018-01-24T02:26:27.398Z Reads: 43

```
tried it to no result
```

---
## \#35 Posted by: scepterr Posted at: 2018-01-24T02:27:56.678Z Reads: 42

```
Yeah if you're getting increased resistance by just having it plugged in, there's a short on the vesc
```

---
## \#36 Posted by: rocka Posted at: 2018-01-24T02:28:49.455Z Reads: 42

```
is there a fix? or am i going to have to wait another month and half for ollin to "repair" it?
```

---
## \#37 Posted by: scepterr Posted at: 2018-01-24T02:29:55.629Z Reads: 43

```
Well you can test some components like the mosfets yourself and see if you can narrow it down
```

---
## \#38 Posted by: rocka Posted at: 2018-01-24T02:30:47.315Z Reads: 44

```
the one i have has ollins aluminum heatsink stuck on, is it safe to remove?
```

---
## \#39 Posted by: scepterr Posted at: 2018-01-24T02:32:11.803Z Reads: 46

```
Yeah it's fine to remove, if there are pads underneath (not sure if there are) make sure not lose them and keep them clean, take some pics of both sides of the PCB, might be something easy to spot
```

---
## \#40 Posted by: rocka Posted at: 2018-01-24T02:35:07.552Z Reads: 48

```
ill try to get it apart tomorrow between my classes and get some pictures for you guys, thank you so much for your help
```

---
## \#41 Posted by: Namasaki Posted at: 2018-01-24T02:44:16.452Z Reads: 47

```
Maybe you should contact Ollin first and tell them specifically what is happening. Maybe your replacement board was defective.
If you mess with it yourself you will probably void the warranty.

first, is your Arduino controller connected to the vesc during motor detection and resistance test?

If yes, that could be the whole problem.
```

---
## \#42 Posted by: rocka Posted at: 2018-01-24T02:46:11.357Z Reads: 48

```
i'll try reaching out to them again. 
the arduino is not connected during either
```

---
## \#43 Posted by: Namasaki Posted at: 2018-01-24T02:54:49.398Z Reads: 47

```
Ok then, must be a short on the vesc.
You might take a close look and make sure the heat sink isn't touching the phase wires where they are soldered to the board.
That Idea might be a stretch but hey, "leave no stone unturned"
```

---
## \#44 Posted by: rocka Posted at: 2018-01-24T05:29:46.167Z Reads: 45

```
wouldn't a short like that have the same resistive force as when the wires are connected?
```

---
## \#45 Posted by: Namasaki Posted at: 2018-01-24T16:08:59.221Z Reads: 43

```
 Not necessarily would be my best guess.
 I have never had shorted Vesc  myself. 
 I only know that there should be no increase in resistance when the motor is plugged into the Vesc
```

---
## \#46 Posted by: rocka Posted at: 2018-02-06T02:18:52.464Z Reads: 40

```
![20180205_181602|374x500](upload://wM2enFgYsGx8FG0uLJAXzwrWB72.jpg) after customer support telling me they replaced it and I'll have to buy a while new board. I took it apart too look at it. Found this underneath, any thaughts?
```

---
## \#47 Posted by: GrecoMan Posted at: 2018-02-06T02:22:34.970Z Reads: 40

```
send him a dm on instagram, i just got done talking to him.

does that middle fet not have thermal paste on it? cause that’ll just short if it touches bare metal.
```

---
## \#48 Posted by: rocka Posted at: 2018-02-06T03:09:06.192Z Reads: 37

```
![1517886478555-29366298|374x500](upload://xh4yvyvGhztQr53r83hFKrEbqI2.jpg)I thaught it did, but looking closer it looks like it shorted through the paste.
```

---
## \#49 Posted by: cloudy Posted at: 2018-02-12T23:17:17.820Z Reads: 30

```
Similar issue with Ollin. Sent back an ESC for repair and was returned a dud. My problem is that the 5v rail for powering the transmitter isn't powering up. Outputting 0v. Haven't been able to test it because of it. Although it does connect fine via USB to the BLDC tool.

Called Ollin and talked to Jeremiah, he told me he's not honoring the warranty to get it checked again.
```

---
