# Problem programming VESC : Dual FOCBOX + 190KV 6355 TorqueBoards Motors + 12s4p battery

### Replies: 27 Views: 346

## \#1 Posted by: PI3RR3 Posted at: 2019-01-15T09:44:51.940Z Reads: 103

```
Hi everyone,

I have a problem with my (first) build : when I press the throttle on my remote, my motor makes a beep noize but it doesn't turn.

Here is my build:
* dual FOCBOX motor controller (split PPM, not master-slave through CAN)
* dual 190KV 6355 TorqueBoards motors (belt drive, not HUB)
* 12s4p battery

To configure the two focbox, I followed the enertion guide :[https://enertionboards.zendesk.com/hc/en-us/articles/115002858294-How-do-I-configure-my-Focbox-](https://enertionboards.zendesk.com/hc/en-us/articles/115002858294-How-do-I-configure-my-Focbox-)

I left all default values like recommanded, and the sensor cables of the motors is plugged in. Something that I noticed : when I do the "start detection" on each motor, it spins fine, then brakes making the beep noise. Sometimes it looks like it struggles to brake. as a consequence the BEMF coupling detected if very high (around 1500-2000) whereas when it doesn't struggle, it stands around 800 like the other motor.

My questions are:
* is my motor broken? 
* what can be wrong with my motors and how can check that?
* are default values good for my build ? or what should I change ? to what values ?
* any suggestions ?

Thanks for the help
```

---
## \#2 Posted by: Andy87 Posted at: 2019-01-15T10:08:05.644Z Reads: 89

```
some additional information would be good.
1. did you set up in BLDC or in FOC
2. what´s the standard settings (as min I don´t remember them) screenshot would be nice.
3. did you do motor detection with or without belts attached
4. did you set your motors up in sensored or unsensored mode
5. do you get any fault after motor detection.
6. is your battery charged and did you set the battery cut off limit right
7. is your remote charged

i think that´s all for now.
maybe one of the points already will fix your problem.
```

---
## \#3 Posted by: rojitor Posted at: 2019-01-15T11:44:26.923Z Reads: 72

```
Did you remove one of the 5v pins?
```

---
## \#4 Posted by: PI3RR3 Posted at: 2019-01-15T16:37:22.348Z Reads: 62

```
Thanks for the reply. Here are some precisions:
1. I use BLDC.
2. It's the one you get when you click "Read Default Configuration" (cf. screenshot)
3. I tried both.
4. I tried both (I actually don't know wether I should use sensored or sensorless, the sensor cable of my motor is always plugged to the vesc btw).
5. No fault after motor detection.
6. Battery at 89%. I don't know for the cut off limit... How to make sure I set it right ?
7. Remote 100% charged.

![screen1|690x409](upload://hCQLO0tvM6pPJUxAn5RoxiDvb87.png)
```

---
## \#5 Posted by: PI3RR3 Posted at: 2019-01-15T16:38:06.641Z Reads: 59

```
You mean for the split PPM? No. Should I?
```

---
## \#6 Posted by: MannyM0E Posted at: 2019-01-15T16:38:47.465Z Reads: 56

```
Try running it sensorless if your running sensor
```

---
## \#7 Posted by: PI3RR3 Posted at: 2019-01-15T16:39:21.364Z Reads: 53

```
Ok can you explain the difference really quick?
```

---
## \#8 Posted by: MannyM0E Posted at: 2019-01-15T16:40:39.337Z Reads: 52

```
I’ve always had trouble with motors spinning sensor(don’t know if I’m doing something wrong) but I’m always getting good result sensorless.
And if using ppm splitter you are suppose to cut one of the 5v off
```

---
## \#9 Posted by: PI3RR3 Posted at: 2019-01-15T16:43:48.692Z Reads: 50

```
That kinda makes sense for the 5v pin, but what can happen if I forgot that? (I actually forgot that)
```

---
## \#10 Posted by: Andy87 Posted at: 2019-01-15T16:45:18.111Z Reads: 48

```
Yes you should. Get the 5V only from one focbox.
Take away the tick at limit max erpm with negativ torque please. That means if you reach full speed your focbox would make a full break.
Something you don’t want!
Try this both first.
If it not work, try to set up in FOC sensored.
Should be no problem with focboxes.
```

---
## \#11 Posted by: Andy87 Posted at: 2019-01-15T16:46:54.519Z Reads: 44

```
There can be a potential difference which means one focbox would try to compensate the other and fry your ppm input or as min disturbe your signal
```

---
## \#12 Posted by: PI3RR3 Posted at: 2019-01-15T16:48:59.461Z Reads: 41

```
Ok thanks for the information.
I'll try what you say right now. Should I try BLDC sensored or sensorless?
Are all the default values ok?
```

---
## \#13 Posted by: Andy87 Posted at: 2019-01-15T16:50:53.844Z Reads: 40

```
First fix the 5V thing.
Don’t change anything else.
Try your luck and then continue one by one and look if one of the changes will help.

PS: the stock settings are ok for now if your pack is made out of Samsung 30q cells
```

---
## \#14 Posted by: Andy87 Posted at: 2019-01-15T16:51:40.076Z Reads: 37

```
Make please a screenshot of your battery cut off settings too.
```

---
## \#15 Posted by: PI3RR3 Posted at: 2019-01-15T16:58:24.370Z Reads: 39

```
I just tried with only one 5v pin and without the limit max erpm and I had the weird thing again: on the same motor,
* one start motor detection looked fine and gave a BEMF coupling of 730
* one looked weird with the motor struggling to brake and gave BEMF of 2000
What does it mean?

Battery cutt off start and end are on the screenshot (33 and 30 V)? is there other battery cutt off parameters?
```

---
## \#16 Posted by: Andy87 Posted at: 2019-01-15T17:02:05.906Z Reads: 40

```
They Already in your screen shot...
My fault. Didn’t use bldc tool long time.
The settings are for 10s.
They too low for 12s. That will not fix your motor problem but please set it up to 3.3v per cell start and 3v per cell end.
So 12x3.3 and 12x3
```

---
## \#17 Posted by: PI3RR3 Posted at: 2019-01-15T17:03:31.774Z Reads: 38

```
Ok thanks, should I also change the max and min input voltage too?
```

---
## \#18 Posted by: Andy87 Posted at: 2019-01-15T17:04:16.915Z Reads: 41

```
Motor detection should be done always without load, so no belt attached.
It is like this at the moment?
Can you spin the motor with your hand?
Do you hear any grinding noise or one motor turns worse than the other?
```

---
## \#19 Posted by: Andy87 Posted at: 2019-01-15T17:04:34.795Z Reads: 41

```
No, let that. That’s fine
```

---
## \#20 Posted by: Sn4pz Posted at: 2019-01-15T17:04:48.662Z Reads: 42

```
@Andy87 as youre active the thread right now, shouldnt the Limit ERPM with negative torque be unchecked?

Its likely not part of the problem OP but you dont want funky breaks at peak speeds
```

---
## \#21 Posted by: Andy87 Posted at: 2019-01-15T17:05:58.227Z Reads: 39

```
Thats what i said.
Don’t check the box. 
It’s standard set, but it’s not good. Uncheck for sure.
```

---
## \#22 Posted by: Sn4pz Posted at: 2019-01-15T17:07:12.511Z Reads: 38

```
[quote="Andy87, post:10, topic:80951"]
Take away the tick at limit max erpm with negativ torque please.
[/quote]


woops :P must have glanced over it, thanks!

Its been awhile since ive done anything in the BLDC tool, I want to re-familiarize myself before I even unbox my Unity :rofl:
```

---
## \#23 Posted by: PI3RR3 Posted at: 2019-01-15T17:07:36.008Z Reads: 40

```
The motor spins fine during the first step of motor detection, it is at the end of the process when it brakes that something weird is happening (not always though)
```

---
## \#24 Posted by: Andy87 Posted at: 2019-01-15T17:30:39.949Z Reads: 41

```
Honestly i‘m not a big expert.
But there some simple things you can do like I said you.
If all this not help you can maybe make a small video and upload it on Vimeo or similar and link it here.
The more information the better.

What I still don’t understand.
One motor is working fine and the other not? Or both have the same problem?
```

---
## \#25 Posted by: MannyM0E Posted at: 2019-01-15T20:20:42.991Z Reads: 32

```
Try sensorless
```

---
## \#26 Posted by: PI3RR3 Posted at: 2019-01-16T12:15:32.543Z Reads: 30

```
I tried your modifications and @MannyM0E I tried sensorless also. Both motors ran fine this morning... I will ride again longer later today and update you.

Thank you guy for your time and all the usefull information.
```

---
## \#27 Posted by: PI3RR3 Posted at: 2019-01-17T08:25:50.475Z Reads: 16

```
Ok it seems like it's working fine now. Let me introduce you guys to my healthy wife, a beautiful beast named Cali.

![49998704_10218956071872107_1469856461457719296_o|690x386](upload://vfNyOMiAJhXlJsUY3uzK3Y36ZxG.jpeg) ![50227010_10218956071792105_3505879179776229376_o|690x386](upload://sKut18i33T4k0uOVawO0x92ErnH.jpeg)
```

---
