# Motors moving by themselves

### Replies: 21 Views: 575

## \#1 Posted by: abctheing Posted at: 2018-07-17T10:16:07.739Z Reads: 180

```
I'm using a dual focbox 6374 setup. Running bldc 12s.
Also using the photon advanced remote, but have used diy's nano remote previously. Same problem.

if the vescs are on for 10 minutes or more, the motors start moving and jerking on their own. This can throw me off the board. They start moving really slowly at first, unnoticeable when riding. But then you notice it.
I often ride around and notice the board acting a tiny bit weird. Then i jump off and pick it up, and the motors are going backwards and forwards, by themselves.

When the motors have started jerking on their own they just jerk more and more, they never stop.
If i don't cut the power they would eventually spin with full throttle, then go full throttle reverse etc, never stopping. It would ruin my vescs. As i said, they start real slow, only jittering until they start spinning.
I have to reboot the system to get rid of it (yes i have to restart my eboard every 10 minutes when i ride)

I used Y split receiver setup before, now canbus, but the motors jerk independently, as always.

Any ideas?
```

---
## \#2 Posted by: Ishayc Posted at: 2018-07-17T10:36:44.438Z Reads: 166

```
Had the same issue with CAN bus and 2 separate receivers.
Try to re-calibrate the remote/receiver through the vesc tool under PPM and see if it helps.
```

---
## \#3 Posted by: Slak Posted at: 2018-07-17T10:46:43.270Z Reads: 155

```
Interferences somewhow... Do you have a ferrite on your PWM cable (the one from the receiver to the ESC) ? Does your problem occur everywhere or just around a specific place ? Is your receiver really close from the phase wires (the ones going from motors to ESC) ? Check if your cable are not too close from each others (signal cable VS power cable)

Did you just finish this build or did it work well before and just start going weird ?

Any pictures from your enclosure layout to help us ?
```

---
## \#4 Posted by: abctheing Posted at: 2018-07-17T10:49:50.628Z Reads: 135

```
Well I this build was "ridable" a year ago, but I haven't been able to trust it because of weird problems like this. So it has been on pause for a long time. I gave up on it.

So yes I have had this problem since the beginning. 
i tried moving the receiver as far away as possible, but to no help. The board is still acting really weird, sometimes. The problem can happen anywhere.


BTW: using UART now
```

---
## \#5 Posted by: Ishayc Posted at: 2018-07-17T11:13:11.388Z Reads: 116

```
I though it was an interference from the battery or so but this issue happened only in one motor so I switched between the receivers and it happened again on the other motor.
It happened inside and outside a carbon fiber enclosure.
A calibration helped in my case though.
```

---
## \#6 Posted by: abctheing Posted at: 2018-07-17T12:30:26.765Z Reads: 98

```
Well i just did a small test outside on my terrace. I throttled from standstill, then the board suddenly 
throttled by itself, continuing for a second even after i left go of the throttle stick.

I don't understand how that could be fixed with a calibration.

This is exactly the kind of problems i have, which no one has answers for, it seems.
The entire year i have had this board, i have not felt safe, even though i have had fun.
Please help me make this skateboard with expensive worthless electronics on it work, so it could be usable.
```

---
## \#7 Posted by: Ishayc Posted at: 2018-07-17T12:36:40.188Z Reads: 87

```
Don't worry and don't be bumped this issue will be solved.
That's the fun of DIY :slight_smile:

First of all don't ride the board like that.
Second, What FW are you using?
```

---
## \#8 Posted by: abctheing Posted at: 2018-07-17T12:37:48.597Z Reads: 84

```
I updated the vescs to the newest firmware last week, I can't remember the version. 2.54?
```

---
## \#9 Posted by: Ishayc Posted at: 2018-07-17T12:40:24.357Z Reads: 85

```
2.54 is an old one, there's 3.xx already.  
Find out what version.

What is your enclosure made of?
```

---
## \#10 Posted by: L3chef Posted at: 2018-07-17T12:49:31.277Z Reads: 80

```
Jumping in here. Sensor motors? 2 years ago this happened to me. It was either bad sensor cables or power wires. 
Also do yoj callibrate the nano remote every time.befor riding?
```

---
## \#11 Posted by: abctheing Posted at: 2018-07-17T12:52:27.698Z Reads: 78

```
Vescs are 3.38. It was 2.54 before I updated. Dual foc boxes.

Well this project has been on pause for a really long time so all I've used to keep everything together is duct tape. I received a really nice enclosure from eboosted yesterday though, which I will mount soon.

![IMG_9215|281x500](upload://n32vg4UNlHbaSJUXzNFk8vf8EJk.jpg)![IMG_9216|281x500](upload://hAuQowoUFFqZZhVI3WeYPrpTNLc.jpg)
```

---
## \#12 Posted by: abctheing Posted at: 2018-07-17T12:52:56.827Z Reads: 76

```
Yes I'm using sensors. I will try switch them off in vesc tool
```

---
## \#13 Posted by: Ishayc Posted at: 2018-07-17T12:55:39.080Z Reads: 77

```
It happened to me sensorless but try disconnecting the sensor cable from only one and see if only one of the motors is good now. 

well no enclosure then that's not the issue.

If you have access to the receiver while this happens, try moving the connector to it and see if it helps
```

---
## \#14 Posted by: L3chef Posted at: 2018-07-17T13:11:44.202Z Reads: 71

```
You need to remove the jst connector from the vesc. It won't help dissable them in bldc/vesc tool
Then detect motors again as "sensorless"
```

---
## \#15 Posted by: i2oadsweepei2 Posted at: 2018-07-18T02:15:17.529Z Reads: 57

```
[quote="Slak, post:3, topic:62087"]
Do you have a ferrite on your PWM cable (the one from the receiver to the ESC) ?
[/quote]

I hope I didn’t miss it somehwhere. Using the ferrite ring is important to clean up the signals running through the receiver wires. Do you have it? Hopefully you can get this problem figured out. 

Those enclosures look sweet btw 😎
```

---
## \#16 Posted by: thisguyhere Posted at: 2018-07-18T03:23:59.361Z Reads: 56

```
someone mentioned above but make sure ppm is properly calibrated, your remote can go out of spec over time 

at neutral throttle ppm signal should be 50%, at full throttle 100%, full brake 0%
```

---
## \#17 Posted by: SeanHacker Posted at: 2018-07-18T03:55:20.558Z Reads: 56

```
I had this sort of thing happen about a year ago with a bad ppm cable. Have you checked that? Mine looked good but wasn't in the end. 

https://youtu.be/c8BRI9ZJslo
```

---
## \#18 Posted by: abctheing Posted at: 2018-07-18T13:48:33.291Z Reads: 46

```
I'm not using PPM anymore. I'm using UART with the photon remote. I can't figure out how to calibrate UART in vesc tool.
```

---
## \#19 Posted by: Kug3lis Posted at: 2018-07-18T13:50:41.172Z Reads: 47

```
Then it's issue with photon mostly, as VESC just takes value of duty cycle in UART mode. Maybe Photon calibration got bad or etc ;)
```

---
## \#20 Posted by: PatRocks Posted at: 2018-07-18T15:38:14.782Z Reads: 36

```
@Namasaki wasn't your 6355 board doing something similar a while back? Is it still twitching?
```

---
## \#21 Posted by: Namasaki Posted at: 2018-07-18T16:21:46.926Z Reads: 34

```
Yes but only when I turn the remote off and only when I’m close to the coast which is close to the airport. Probably getting some interference. 
I don’t have this problem when I’m at home in east county.
```

---
