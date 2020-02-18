# VESC sparked, what does that mean?

### Replies: 44 Views: 2533

## \#1 Posted by: anoop54 Posted at: 2016-08-28T07:07:36.614Z Reads: 131

```
So i set everything up, did the config on my vsec with 3s lipo. Then when i connected my 12s supply the vsec sparked a little. why did this happen? And is my vsec gone??
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2016-08-28T07:18:12.135Z Reads: 131

```
if you mean the connectors sparked when you touched the two halves together then it's ok. High voltage systems do spark when they are plugged in. This is normal. It's not very likely that it damaged your vesc. You can always buy an anti spark connector like the XT-90 to solve the problem.
```

---
## \#3 Posted by: paul775 Posted at: 2016-08-28T07:18:23.027Z Reads: 129

```
First what battery are you using? LiPo, Space Cells, etc. Then do you have an Anti-Spark on the setup? If not then make/buy one to get rid of sparks.

What light is on the VESC? Blue is good
```

---
## \#4 Posted by: Pablo_702 Posted at: 2016-08-28T07:19:22.664Z Reads: 125

```
A little spark if u dont have an anti spark connector is normal the vesc should be good but it is highly recommended to use an ati spark since the sparks over time will eat up the metal in your connectors
```

---
## \#5 Posted by: anoop54 Posted at: 2016-08-28T07:20:07.905Z Reads: 118

```
I have an anti spark plug in the circuit! Something sparked on the vsec. the lights were still on the vsec after the spark. but i immediatley turned it off. I have a li-po setup.
```

---
## \#6 Posted by: anoop54 Posted at: 2016-08-28T07:20:33.736Z Reads: 113

```
I have an anti spark plug in the circuit! Something sparked on the vsec. the lights were still on the vsec after the spark.
```

---
## \#7 Posted by: lox897 Posted at: 2016-08-28T07:26:13.306Z Reads: 105

```
Changed the title so people understand the issue through the title. Also, it is VESC, not VSEC.
```

---
## \#8 Posted by: anoop54 Posted at: 2016-08-28T07:27:08.591Z Reads: 104

```
Thank You! Appreciate it
```

---
## \#9 Posted by: anoop54 Posted at: 2016-08-28T07:29:10.982Z Reads: 100

```
I have an antispark plug. It sparked when I hit the throttle !
```

---
## \#10 Posted by: makevoid Posted at: 2016-08-28T07:32:41.816Z Reads: 100

```
Even if you have the anti spark in your circuit, you need to be sure that the anti spark  is the last thing you connect, otherwise you'll get a spark :).
```

---
## \#11 Posted by: paul775 Posted at: 2016-08-28T07:33:11.355Z Reads: 99

```
So once you throttled the VESC sparked.

Can you post your VESC settings. And also picture of the VESC on the side it sparked at.
```

---
## \#12 Posted by: anoop54 Posted at: 2016-08-28T07:36:07.602Z Reads: 100

```
<img src="/uploads/db1493/original/2X/8/82d0dce75cf214fce43751932c22beddacef0641.png" width="690" height="360"><img src="/uploads/db1493/original/2X/a/ad2e3c643908ceeb1955d056b93049ee1a88ef97.png" width="690" height="344">
```

---
## \#13 Posted by: anoop54 Posted at: 2016-08-28T07:38:17.465Z Reads: 93

```
I Had configured it with a 3s suply, everything was fine. Then when i connected the 12s the motor would only budge when the throttle was hit. After i hit the throttle for the 3rd time the vsec sparked.
```

---
## \#14 Posted by: anoop54 Posted at: 2016-08-28T07:39:03.129Z Reads: 92

```
Hey Thanks for your reply. I use it as a switch so yes it's the last thing I connect.
```

---
## \#15 Posted by: anoop54 Posted at: 2016-08-28T07:42:11.571Z Reads: 92

```
Appreciate all the responses. I've been trying to build this for a year now. Like literally. Burned 2 esc's and then finally got the vesc. And now I can't get this to work either. Any help would be greatly appreciated. I am a little scared to connect the vsec again.
```

---
## \#16 Posted by: paul775 Posted at: 2016-08-28T07:43:09.323Z Reads: 88

```
Change your **Battery cutoff start and end** to a 12s system. So 42.0V for start and 39.6 for end for now.
Also change your Max Input Voltage to 57V to be safe.

Edit: Updated values. Was looking at 10s values.

<img src="/uploads/db1493/original/2X/1/1c6d6ee60203f31b853eef249cbd04eb7fb78e82.png" width="590" height="200">
```

---
## \#17 Posted by: anoop54 Posted at: 2016-08-28T07:44:54.729Z Reads: 84

```
Is it safe to connect the 12s? Or should I strpid it down again to 3s and then config the esc?
```

---
## \#18 Posted by: paul775 Posted at: 2016-08-28T07:47:19.043Z Reads: 86

```
No first fix your settings. Use 3s.
```

---
## \#19 Posted by: makevoid Posted at: 2016-08-28T07:48:24.591Z Reads: 84

```
can you take a screenshot of the advanced tab as well?  specifically the current ramp step value on the right column, that should be around 0.04

also if you fry 2 esc before, could it be that your motor is shorting? which motor are you using?
```

---
## \#20 Posted by: anoop54 Posted at: 2016-08-28T07:51:31.620Z Reads: 88

```
<img src="/uploads/db1493/original/2X/b/bfeee6e87866829cbaf016e28a156e49eb19b8b4.png" width="690" height="382">

AND THIS IS THE MOTOR I AM USING. diy-electric-skateboard-kits-parts/electric-skateboard-sensored-epower-motor-5065-170kv-2200w/
```

---
## \#21 Posted by: anoop54 Posted at: 2016-08-28T07:57:19.796Z Reads: 81

```
<img src="/uploads/db1493/original/2X/0/004d2279a2af9347e8bb48ae05dcc38c23f6fca1.jpg" width="690" height="388"><img src="/uploads/db1493/original/2X/a/a89a4707b752b9bb1794adcd08bb074692cb8dd5.jpg" width="690" height="388">
```

---
## \#22 Posted by: paul775 Posted at: 2016-08-28T07:58:20.420Z Reads: 78

```
Change the **Max Current Ramp Step**. Put in 0.004 and write it. Might need to do that every time you write to your Motor Settings.

Here's why: http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262?source_topic_id=7249
```

---
## \#23 Posted by: anoop54 Posted at: 2016-08-28T08:06:37.378Z Reads: 78

```
<img src="/uploads/db1493/original/2X/4/4758c2f7e5aed4a54a754f63337aa7ce21f5ac2b.png" width="690" height="372"><img src="/uploads/db1493/original/2X/7/7c3a4e6d1d5ffe264fb94421c001adb58ab70309.png" width="690" height="356">
```

---
## \#24 Posted by: anoop54 Posted at: 2016-08-28T08:07:14.312Z Reads: 70

```
IS that good? Now should I connect 12s again?? and try to throttle? I don't want to damage the vsec
```

---
## \#25 Posted by: paul775 Posted at: 2016-08-28T08:08:36.670Z Reads: 73

```
Real quick can you take a picture of the other side of the VESC. 

That Max Current Ramp Step should be at 0.04 not 40. 

You can also check for errors in the Realtime Data tab but I don't know how since I never had a problem with my VESC.
```

---
## \#26 Posted by: Jinra Posted at: 2016-08-28T08:12:18.870Z Reads: 71

```
Check your faults first. If there are none then you might be safe. You will want to flash latest version of firmware from vesc.net.au to avoid the max current ramp bug. But honestly, it's looking grim.
```

---
## \#27 Posted by: anoop54 Posted at: 2016-08-28T08:13:17.475Z Reads: 72

```
I changed it to 0.04, now should I connect 12s?
```

---
## \#28 Posted by: anoop54 Posted at: 2016-08-28T08:15:01.160Z Reads: 71

```
How do i check faults?
```

---
## \#29 Posted by: Jinra Posted at: 2016-08-28T08:16:33.470Z Reads: 73

```
Realtime Data > Activate sampling. Should show up on the bottom right. You can also go to Terminal and type "faults". Keep in mind a fault would have to happened while the VESC was on for it to display faults. If you turn it off and on it will reset the faults.
```

---
## \#30 Posted by: anoop54 Posted at: 2016-08-28T08:32:46.418Z Reads: 70

```
<img src="/uploads/db1493/original/2X/0/0bbbe4b2d6768a29e3123c68ce48192d0adc1f9e.jpg" width="281" height="500">
There's damage on the otherside That i can see. Guessing that means im fucked?
```

---
## \#31 Posted by: anoop54 Posted at: 2016-08-28T08:41:55.875Z Reads: 67

```
UPDATEE: When I try to hit throttle the blue light changes to white. But the motor does not budge.
```

---
## \#32 Posted by: Jinra Posted at: 2016-08-28T08:42:31.618Z Reads: 67

```
Looks like you burnt your DRV, did you confirm the fault in BLDC tool? This was probably due to the extremely high max current ramp step.
```

---
## \#33 Posted by: kaziupir Posted at: 2016-08-28T08:44:05.871Z Reads: 67

```
So bug in the bldc tool burned next vesc.
```

---
## \#34 Posted by: Jinra Posted at: 2016-08-28T08:44:35.535Z Reads: 65

```
Technically it's a bug in the firmware, not BLDC tool.
```

---
## \#35 Posted by: paul775 Posted at: 2016-08-28T08:46:06.464Z Reads: 67

```
<img src="/uploads/db1493/original/2X/7/72784729fb2cf2c96eeef3f0e8838829c05fa24d.png" width="418" height="260">

Need some light but yeah your DRV chip is blown. Have you done the fault check?
```

---
## \#36 Posted by: anoop54 Posted at: 2016-08-28T08:51:55.134Z Reads: 67

```
<img src="/uploads/db1493/original/2X/0/085e72877cd621450d0d24b71c5f4e06fd5fb205.png" width="690" height="380">
```

---
## \#37 Posted by: anoop54 Posted at: 2016-08-28T08:52:32.584Z Reads: 64

```
So my vsec is done? Idk if i can afford a 4th one.
```

---
## \#38 Posted by: Jinra Posted at: 2016-08-28T08:54:56.466Z Reads: 63

```
Move throttle and see if a fault code pops up on the bottom left. You could get VESC platinum if it's Enertion and get it replaced.
```

---
## \#39 Posted by: anoop54 Posted at: 2016-08-28T08:58:56.729Z Reads: 63

```
It is Enertion! So I should check out the 1yr vsec warranty ? Does this cover vsec replacements for a year? And Do i have to send the fauty ones back?
```

---
## \#40 Posted by: kaziupir Posted at: 2016-08-28T08:59:26.916Z Reads: 61

```
Or you can replace drv https://www.youtube.com/watch?v=qeWzP2YahNc
```

---
## \#41 Posted by: Jinra Posted at: 2016-08-28T08:59:44.470Z Reads: 61

```
Check with @onloop or Enertion support, I'm not sure if it's a one time replacement or not.
```

---
## \#42 Posted by: anoop54 Posted at: 2016-08-28T09:01:34.939Z Reads: 63

```
Thank you ! Will give it a try.
```

---
## \#43 Posted by: anoop54 Posted at: 2016-08-28T09:07:01.399Z Reads: 63

```
Could you tell me why this happened? So I know to make sure it doesnt happen next time. It worked perfectly fine on a 3s setup.
```

---
## \#44 Posted by: Jinra Posted at: 2016-08-28T09:09:17.306Z Reads: 62

```
Can't tell for **sure** what happened, but it looks to be because you're using a version of the VESC firmware with the max ramp current step bug. See more info here

http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc

The first thing you want to do is to re-flash your firmware from vesc.net.au on your new VESC to fix this bug and not worry about it.
```

---
