# Board broken large sparks Help!

### Replies: 23 Views: 300

## \#1 Posted by: spigelli Posted at: 2018-11-04T23:18:18.910Z Reads: 126

```
Ran the eboard through a puddle or two on a ride a while back and it stopped working mid ride. The motor would jump when I turned it on but other than that nothing.
Dried it and waited a couple of days and when I plugged everything back in and turned it on, it made large sparks melting the metal leads. I unplugged the motor and connected bldc tool to the focbox and I can read the config and see that the receiver on the board is working. However, when I try to connect with the motor plugged in, the focbox turns off after about 30 seconds and the motor won't drive in that time.
If I touch the three motor leads to my tongue and spin it I can feel the electricity, but I have no idea why it wouldn't be working.

Battery 12s4p DIYelectric
Motor 6374 190kv DIYelectric
ESC Focbox

Thanks for the help!!!
```

---
## \#2 Posted by: Mich21050 Posted at: 2018-11-04T23:27:46.802Z Reads: 117

```
First of all I would connect the focbox and type faults into the terminal. :smile:
```

---
## \#3 Posted by: spigelli Posted at: 2018-11-04T23:42:17.108Z Reads: 109

```
I already tried that it won't come up with anything
```

---
## \#4 Posted by: Mich21050 Posted at: 2018-11-04T23:45:29.490Z Reads: 105

```
Have you checked your battery with a voltmeter? :slight_smile:
Otherwise, a guy like @CarlCollins could help you with your focbox :smile:
```

---
## \#5 Posted by: BoostedBuilder Posted at: 2018-11-04T23:54:48.185Z Reads: 96

```
[quote="spigelli, post:1, topic:73458"]
If I touch the three motor leads to my tongue and spin it I can feel the electricity
[/quote]

Damn haha   ‍      ‍      ‍
```

---
## \#6 Posted by: Mich21050 Posted at: 2018-11-05T00:04:37.997Z Reads: 90

```
https://giphy.com/gifs/funny-fail-tK5JkmMAPveNO
```

---
## \#7 Posted by: dareno Posted at: 2018-11-05T00:06:09.505Z Reads: 88

```
:rofl::rofl::rofl:
no.  just no.
```

---
## \#8 Posted by: J0ker3366 Posted at: 2018-11-05T00:06:23.851Z Reads: 87

```
He is either a fucking genius or a fucking idiot lol. Either way, he is always an interesting watch.
```

---
## \#9 Posted by: dareno Posted at: 2018-11-05T00:08:19.282Z Reads: 81

```
Alright if I can type while giggling what metal leads did the melting?
```

---
## \#10 Posted by: Mich21050 Posted at: 2018-11-05T00:09:26.489Z Reads: 82

```
I'm assuming that he meant the xt90 connector :slight_smile:
```

---
## \#11 Posted by: J0ker3366 Posted at: 2018-11-05T00:22:14.384Z Reads: 77

```
@Hummie, did you graduate from grinding pcbs to licking electricity cables lol?
```

---
## \#12 Posted by: dareno Posted at: 2018-11-05T00:22:42.302Z Reads: 75

```
@Hummie  is this you? do you have two accounts?
```

---
## \#13 Posted by: lrdesigns Posted at: 2018-11-05T01:19:58.217Z Reads: 64

```
[quote="spigelli, post:1, topic:73458"]
I have no idea why it wouldn’t be working.
[/quote]

Water, big sparks, melted wires would be my guess why its not working. jk. :rofl: 

We need some photos to help figure out what is broken. Where do you think the sparks came from? Some photos of the melted stuff too. 

You probably need to remove the battery pack from the board, then remove all the shrink wrap from the battery and inspect all the cells and the BMS.

I would also open the focbox to see if any water got on the PCB.
```

---
## \#14 Posted by: CarlCollins Posted at: 2018-11-05T03:48:58.370Z Reads: 52

```
@spigelli
You have burnt your MCU chip on the FOCBOX(s).
Please let me know from where you purchase the FOCBOX(s)?
```

---
## \#15 Posted by: torqueboards Posted at: 2018-11-05T03:57:24.704Z Reads: 48

```
@spigelli Your battery is probably still wet. You can always send it in and we can check it out but it might need to be repaired.
```

---
## \#16 Posted by: spigelli Posted at: 2018-11-05T04:24:24.160Z Reads: 47

```
@CarlCollins @torqueboards The battery and Focbox seem to be acting normally aside from the focbox turning off when the motor is connected, so I think it has something to do with the motor, but I'll post a video soon.
```

---
## \#17 Posted by: lrdesigns Posted at: 2018-11-05T04:42:53.115Z Reads: 41

```
[quote="spigelli, post:1, topic:73458"]
melting the metal leads.
[/quote]

Which wires specifically, you didn't mention yet? That happened as you turned on the power switch?
```

---
## \#18 Posted by: psychotiller Posted at: 2018-11-05T04:58:05.606Z Reads: 38

```
![image|260x194](upload://eAN1hr59gJ9OGyN9qN6qGb4UXaw.jpeg)
```

---
## \#19 Posted by: psychotiller Posted at: 2018-11-05T04:58:36.093Z Reads: 39

```
![image|259x194](upload://9ECWsVmfvk954IHvwqVheeS04Dl.jpeg)
```

---
## \#20 Posted by: spigelli Posted at: 2018-11-05T05:01:30.598Z Reads: 38

```
the motor leads just melted enough to need to be filed down in order to fit and a bunch of charring on the ESC females that I cleaned up before testing again
```

---
## \#21 Posted by: lrdesigns Posted at: 2018-11-05T05:07:20.181Z Reads: 33

```
Weird, not heard of that before. Going to have to leave that to the experts. I do know that the esc and motor work together as system. A shorted motor can kill an esc and a broken esc can short a motor.
```

---
## \#22 Posted by: CarlCollins Posted at: 2018-11-05T06:20:46.619Z Reads: 25

```
@spigelli
Keep us updated :slight_smile:
```

---
## \#23 Posted by: lrdesigns Posted at: 2018-11-05T06:26:21.643Z Reads: 25

```
Can you read your battery voltage in vesc tool or with a multi meter? If it is too low the vesc will not  turn the motor. 

But the big sparks and melting suggest something is now broken. Sorry. Need to start to figure out if its battery / esc / motor / all of the above :cold_sweat:
```

---
