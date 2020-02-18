# Vesc failed motor detection sk3 6364 245kv

### Replies: 26 Views: 2281

## \#1 Posted by: wowstudios Posted at: 2016-08-09T05:46:49.506Z Reads: 175

```
Hi.This is my first time posting here. I am deep into building my first eboard. It is a vesc powering an sk3 6364 245kv. I am into rc planes and have built several quadcopters and my own cnc machine, but i am totally new to eboards. It was all going well until i went to hook up my vesc to the pc. I powered my vesc with a small lipo. 1000mah 3s. upon plugging in the battery it instantly started smoking. I unplugged within a second. Upon farther investigation i found a short where the positive power connects to the vesc. The vesc never heated up or smoked at all. I resoldered the power wire and fixed the short quite easily. The vesc connected just fine after. All was going well until i tried to do motor detection. The motor jerks once and then a few seconds later it jerks again and the red lights flash several times. I have adjusted the motor detection parameters within the limits mentioned in the faq but no combination will allow for a successful detection. I am at a loss for what to try to solve this. Could shorting the battery have blown the capacitors? I have not yet reflashed the firmware.
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-09T05:49:14.645Z Reads: 175

```
Where was the smoke coming from the first time? You should check the real time data (turn on active sampling) and run motor detection again. See what the fault code is.
```

---
## \#3 Posted by: wowstudios Posted at: 2016-08-09T05:55:25.842Z Reads: 176

```
The smoke only came from the lipo. It was a 20c 1000 mah so it wouldnt be able to push an insane amount of amps. The fualt im getting is drv8302
```

---
## \#4 Posted by: Jinra Posted at: 2016-08-09T05:57:29.521Z Reads: 167

```
awww shoot, you might have a burned DRV, which is the most common part to die.

Could you take a look at or smell the DRV chip? It's the rectangular one here

http://www.electric-skateboard.builders/uploads/db1493/original/2X/d/d8fccff96bda7a90a3cffbce2fce5ae89d1566d1.JPG

It's likely it's busted and you need to replace it.
```

---
## \#5 Posted by: wowstudios Posted at: 2016-08-09T06:05:02.401Z Reads: 154

```
The vesc never got warm at any time. Correct me if im wrong but if there was a direct short from the power to ground would the allow the voltage to cause damage? it seems to me that that would "dam" the electricity. Im a bit of a newb when it comes to circuitry. Would enertion stand good for it since it was shorted on arrival?
```

---
## \#6 Posted by: Jinra Posted at: 2016-08-09T06:06:31.539Z Reads: 152

```
I'm sure Enertion will make it right, just contact their support. You should check out this thread as well.

http://www.electric-skateboard.builders/t/vesc-faq-negative-squared-cross-mark-warning-negative-squared-cross-mark-risk-of-short/6805
```

---
## \#7 Posted by: Jmak Posted at: 2016-08-09T06:13:31.785Z Reads: 147

```
I also have this problem with both my new VESCs. Do you think any of these are burned?

1:
<img src="/uploads/db1493/original/2X/a/a31516817bef49f4943deed8c31e2df44acb3564.jpg" width="375" height="500">
<img src="/uploads/db1493/original/2X/7/74486b521fb132a89c52cf71f507472237c8d428.jpg" width="375" height="500">

2:
<img src="/uploads/db1493/original/2X/0/0bb47738415066913465fa0a7c8dfcd979048b3a.jpg" width="375" height="500">
<img src="/uploads/db1493/original/2X/6/6f80335968a66a3c4ed61a8f5ea3719478794197.jpg" width="375" height="500">
```

---
## \#8 Posted by: Jinra Posted at: 2016-08-09T06:15:05.242Z Reads: 131

```
Both VESCs have a DRV8302 fault code? Did you check if the hall sensor pins are piercing the positive lead cable?
```

---
## \#9 Posted by: Jmak Posted at: 2016-08-09T06:17:04.762Z Reads: 131

```
Yes both of them have it. I hot glued the hall sensor pins before I powered the VESCs for the first time.
```

---
## \#10 Posted by: wowstudios Posted at: 2016-08-09T06:32:21.618Z Reads: 133

```
@Jmak what does your vesc do when you try detection. My motor just makes a violent jerk then several seconds later it jerk again. I did get my motor to spin up by pressing the arrow key on the keyboard on accident. I had to disconnect it in bldc in order to make it stop.
```

---
## \#11 Posted by: Jmak Posted at: 2016-08-09T06:37:12.415Z Reads: 130

```
Exactly the same thing. It jerks and then a few seconds later another jerk. But I can't even press the arrow keys without a DRV8302 fault.
```

---
## \#12 Posted by: onloop Posted at: 2016-08-09T07:26:02.945Z Reads: 119

```

Hi, can we see a picture of the other side & also a picture of the motor connection points
```

---
## \#13 Posted by: wowstudios Posted at: 2016-08-09T14:47:23.269Z Reads: 105

```
<img src="/uploads/db1493/original/2X/6/63ef8a1944ab06533478adedb2557f76976f92a5.jpg" width="690" height="388"><img src="/uploads/db1493/original/2X/0/0db9e158217d030adfb0634258dfc82ea3519b7b.jpg" width="690" height="388">
 Here is the pictures of the shorted power lead before and after I fixed it.

<img src="/uploads/db1493/original/2X/1/17ef1ff1208097f55c4c983bbc98edaf161e3428.jpg" width="281" height="500">
```

---
## \#14 Posted by: sprocket12 Posted at: 2016-08-09T15:09:00.535Z Reads: 92

```
You mentioned that you set the motor parameters according to the FAQ.  Did you also adjust your voltage cutoff limits for your battery size?
```

---
## \#15 Posted by: wowstudios Posted at: 2016-08-09T15:17:27.132Z Reads: 92

```
I set the minumum and cut off to 6 volts so that it would not be a problem with the 3s battery that I'm using to configure.
```

---
## \#16 Posted by: Blasto Posted at: 2016-08-09T15:25:32.008Z Reads: 92

```
If your running 3s for testing, try to increase your erpm to 800 and your current to 8A in the detect parameters
```

---
## \#17 Posted by: wowstudios Posted at: 2016-08-09T15:40:28.039Z Reads: 88

```
If the motor spins up when I press the right arrow key in bldc it would seem to me that it's not hardware. I wouldn't say that it totally eliminates the chance of a hardware issue tho. How is it supposed to act when I press the arrow key? My motor spun up to full and stay that way. I had to disconnect in bldc to make it stop. I did try detection with a 4s battery with similar results. I am now running a fuse in line. It is quite a violent jerk when I try detection.
```

---
## \#18 Posted by: Jinra Posted at: 2016-08-09T15:45:00.358Z Reads: 86

```
it shouldn't run continuously when you press the arrows, it should only spin for as long as you good it.
```

---
## \#19 Posted by: wowstudios Posted at: 2016-08-09T16:22:50.290Z Reads: 86

```
I'm quite suprised that such an obvious short made it through quality control. Mabe before I "try it till it breaks" I should just contact enertion and see what their solution is.
```

---
## \#20 Posted by: Pimplaren Posted at: 2016-08-10T07:45:03.671Z Reads: 80

```
My vesc failed to motordetect with a uncharged 5s, tryd with 10s and its worked out just fine!
```

---
## \#21 Posted by: wowstudios Posted at: 2016-08-10T15:16:50.917Z Reads: 73

```
Ok. I thought I read the 12 volts was enough. Did you get a "drv fault" with the 5s? I don't want to smoke it and ruin my chance of returning it to enertion.
```

---
## \#22 Posted by: Pimplaren Posted at: 2016-08-10T19:50:29.466Z Reads: 66

```
I had like 19.2v, i did charge the battery for a testrun after the motordetection! 

Nope just failed, put the other battery in serie and tryd again with success. :)
```

---
## \#23 Posted by: Jinra Posted at: 2016-08-10T19:54:11.064Z Reads: 67

```
You probably have increase the detection current/duty/erpm to detect on a lower voltage.
```

---
## \#24 Posted by: sl33py Posted at: 2016-08-10T20:09:33.214Z Reads: 67

```
@wowstudios a bit remedial compared to the other suggestions here, but also try a different USB cable - especially a shorter cable if you have a super long USB cable currently.  Waaay back Vedder mentioned this for motor detection and basic connection issues being potentially problematic.

GL!
```

---
## \#25 Posted by: wowstudios Posted at: 2016-08-10T21:04:14.496Z Reads: 63

```
I did try a different cable. I have tried it with the current between 1 to 6 amps and erpm between 300 and 1200. Thanks for all the suggestions. I will try again tonight with 6s
```

---
## \#26 Posted by: Jinra Posted at: 2016-08-10T21:06:33.427Z Reads: 61

```
try a higher duty since the voltage is lower.
```

---
