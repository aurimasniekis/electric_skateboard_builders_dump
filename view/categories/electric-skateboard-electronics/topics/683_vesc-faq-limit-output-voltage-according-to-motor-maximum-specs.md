# VESC FAQ &#124; Limit output voltage according to motor maximum specs

### Replies: 29 Views: 12851

## \#1 Posted by: arsenic Posted at: 2015-12-08T21:37:18.630Z Reads: 1169

```
Hi,

I'm new in VESC utilisation. I was wondering if it's possible to limit the VESC output voltage according to the max motor voltage.

Why ?
Simply because my actual motor is 10S max (Aerodrive SK3 215kv), with a 6S max HobbyKing ESC. I'll upgrade to VESC, with 2x 6S attery and I 'would not change my motor ...

Is it possible with this device ?
I already found there is an option for rpm limitation, but i'm not sure it will be enought to avoid firing my motor ...
```

---
## \#2 Posted by: onloop Posted at: 2015-12-08T22:13:34.618Z Reads: 1151

```
YES, you can do it.

In BLDC tool / Motor Configuration / Motor

**This is recommended for anyone with 12S Battery & Motor over 200KV**

<img src="/uploads/db1493/original/2X/a/a23f57b9a3a388adaf0ff3e03b5587dee02697dc.png" width="690" height="401">
```

---
## \#3 Posted by: evoheyax Posted at: 2015-12-10T21:43:16.413Z Reads: 1081

```
@onloop could you elaborate as you why? I was planning on using 2 6s in series to make a 8000 mAh 12s to run 2 VESCs and a dual drive carvON. I don't want to damage the VESC, but by my math, a 12s can max out at 50.4 volts (4.2 per cell X 12 cells), which is well under the 60 volt max limit for the VESC.

The enertion shop page says up to 60 volts or 12s, but 60 volts would be a 14s, so can the VESC run on a 14s battery?
```

---
## \#4 Posted by: onloop Posted at: 2015-12-11T05:48:46.244Z Reads: 1043

```
this reason.............
[quote="onloop, post:2, topic:683"]
This is recommended for anyone with 12S Battery & Motor over 200KV
[/quote]
```

---
## \#5 Posted by: evoheyax Posted at: 2015-12-11T06:00:53.219Z Reads: 997

```
I get that but what's the science behind it?
```

---
## \#6 Posted by: trbt555 Posted at: 2015-12-11T06:34:50.695Z Reads: 976

```
Voltage rating of the components in the VESC.
```

---
## \#7 Posted by: akira Posted at: 2015-12-11T07:13:43.211Z Reads: 960

```
Is that true ?
I thought that VESC was not recommended when used with 12S voltage and motors over 200KV.
```

---
## \#8 Posted by: trbt555 Posted at: 2015-12-11T09:06:27.520Z Reads: 941

```
Sorry, I misinterpreted the question.
Some [interesting reading material][1] that might shef light on the subject.


  [1]: http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/
```

---
## \#9 Posted by: treenutter Posted at: 2016-01-09T01:47:15.565Z Reads: 923

```
@onloop @trbt555 Could either of you elaborate on how to properly set the voltage and current limits on VESC? What you base the values on? The motor's limit, or the battery's potential output, or some combination of those? I've not found a place where anyone describes how to derive the right values. @trbt555 I know you've written at least once about exceed VESC's threshold and have your power cut off. How do you avoid that now?
```

---
## \#10 Posted by: trbt555 Posted at: 2016-01-09T06:13:06.594Z Reads: 907

```
@treenutter I'm by no means experienced after only 4 rides but I'll share nonetheless, for what It's worth.
I posted about voltage cutoff in my build thread. If you look at my discharge curves (or any lipo curves on the net for that matter) you'll see the voltage drop steeply past 3.6V per cell.
So on my last ride I had the voltage cutoff set to 3.6V x 12 and I quit riding as soon as I felt the power drop. Worked pefectly, my charger told me all cells were perfectly at 3.6V and the 5000mAh Zippy's soaked up about 5200mAh on my charger to get back to 4.2V.

Unfortunately discharge curves don't tell you how much the cell voltage sags under heavy load. Because I had my cutoff set too high initially, I was hitting it even with charged Lipo's just by accelerating fast, just because my lipo's couldn't keep up. I think.

There are settings for both motor and battery current limits. As I'm using the R-SPEC's I left the default motor settings alone, and set the battery current limit to match what people were telling me my lipo's would be capable of and just above the max current my wattmeter was reading.

Hope this helps.
```

---
## \#11 Posted by: elkick Posted at: 2016-01-09T18:01:10.318Z Reads: 847

```
Just to give you some indications, you should adjust it to your experiences: 

"min. Input Voltage" = you can leave that at 8V
"max. Input Voltage" = you can leave that at 50V, except for 12s = 57V
"Battery cut-off start" = number of cells x 3,5V
"Battery cutoff end" = number of cells x 3,3V 

Table:
<img src="/uploads/db1493/original/2X/f/fb95302d91aa992329d1d0ccb21f626ae71fc139.png" width="586" height="196">
```

---
## \#12 Posted by: cmatson Posted at: 2016-01-09T19:47:54.015Z Reads: 805

```
[quote="elkick, post:11, topic:683"]
"Battery cut-off start" = number of cells x 3,5V
"Battery cutoff end" = number of cells x 3,3V
[/quote]

so would your VESC cut out at 3.5v, or 3.3v with these settings?
```

---
## \#13 Posted by: elkick Posted at: 2016-01-09T20:02:49.264Z Reads: 759

```
It would start slowing down at 3.5 and cut out at 3,3 (or 3,2 which is also ok). Advantage: the VESC will not just shut down at one point but indicate that you're reaching the end of capacity so that there's time to get acquainted to the fact that you have to stop skating. :grin:
```

---
## \#14 Posted by: cmatson Posted at: 2016-01-09T20:16:58.673Z Reads: 742

```
awesome, that's exactly what I was looking for.

Thanks!
```

---
## \#15 Posted by: arsenic Posted at: 2016-01-09T20:41:12.962Z Reads: 716

```
And what about these parameters ?

[quote="elkick, post:11, topic:683, full:true"]

"min. Input Voltage" = you can leave that at 8V
"max. Input Voltage" = you can leave that at 50V, except for 12s = 57V
[/quote]

Does the VESC will limit output voltage according to the "max. Input Voltage" value ?
For exemple, if I ride with a 12s battery (=57v), but this parameter is set to 50 (= 10s), does the output will be limited/regulated to 50v ?

I ask this because my motor is limited to 10s, but I plan to ride in futur with two 6s battery, so I'm looking in a way to limit the max motor voltage.
```

---
## \#16 Posted by: elkick Posted at: 2016-01-09T21:20:34.533Z Reads: 681

```
[quote="arsenic, post:15, topic:683"]
Does the VESC will limit output voltage according to the "max. Input Voltage" value ?For exemple, if I ride with a 12s battery (=57v), but this parameter is set to 50 (= 10s), does the output will be limited/regulated to 50v ?
[/quote]
It would limit the input voltage to 50V, yes. But my experience of limiting the Voltage that way wasn't very exciting, the motors behaved strange (stuttering when going fast). You could give it a try though.
```

---
## \#17 Posted by: arsenic Posted at: 2016-01-09T21:36:27.997Z Reads: 663

```
I don't want to fire my motor !
Do you know a better way to limit the motor violtage ?

(but I will did a try when I'll receive my VESC, with a 6s battery associate to a "software limitation" of 3s  ...)
```

---
## \#18 Posted by: trbt555 Posted at: 2016-01-10T08:30:47.122Z Reads: 645

```
12S = 57V ?
Please elaborate.
```

---
## \#19 Posted by: elkick Posted at: 2016-01-10T09:04:58.389Z Reads: 633

```
It was suggested by Benjamin, but I don't know the reason behind it except maybe to stay within the 60V limit.
```

---
## \#20 Posted by: arsenic Posted at: 2016-01-10T09:18:03.104Z Reads: 630

```
Sorry I did a mistake : 
10S = 42v
12S = 50v

Shame on me...
```

---
## \#21 Posted by: treenutter Posted at: 2016-03-17T20:34:41.857Z Reads: 605

```
@trbt555 @elkick FWIW the default Max input voltage in 2.16 is 57.00.
```

---
## \#22 Posted by: ayospringroll Posted at: 2016-11-17T08:09:27.297Z Reads: 447

```
So if I had a 6s battery set up I would use 25.2 for max input voltage?
```

---
## \#23 Posted by: yaca Posted at: 2016-11-17T10:48:31.983Z Reads: 438

```
No, just let it at default value 57V. I can not explain the reason but I red this many times and has to do with spikes maybe.
```

---
## \#24 Posted by: ayospringroll Posted at: 2016-11-17T11:30:40.076Z Reads: 435

```
Interesting... Well then.. Thank you! This helps me alot!
```

---
## \#25 Posted by: Ackmaniac Posted at: 2016-11-17T11:40:53.490Z Reads: 421

```
You could achieve that by limiting the maximum duty cycle. At the moment it is 0.95. That meansif you have 40V and want to reduce it to 20V which should go in maximum to the motor then set it max to 0.50. But I never tried that. But it should do the trick.
```

---
## \#26 Posted by: Rafeh1 Posted at: 2018-11-25T02:45:00.022Z Reads: 84

```
unable to use vesc parameter editor
need to set max vin to 58.6 v
this worked in old vers of vesc but not in new version. tried doing developer -> parameter editor
rafe
```

---
## \#27 Posted by: lrdesigns Posted at: 2018-11-25T02:48:04.719Z Reads: 81

```
If you want to do that you have to load the firmware “no hardware limits”
```

---
## \#28 Posted by: Rafeh1 Posted at: 2018-11-25T02:50:42.884Z Reads: 79

```
how to get this firmware?
```

---
## \#29 Posted by: Rafeh1 Posted at: 2018-11-25T04:32:39.174Z Reads: 79

```
[quote="lrdesigns, post:27, topic:683"]
firmware “no hardware limits”
[/quote]

i found it in the fw option
![vesc_nolimits|690x370](upload://zUEPr3ZcJ07DmcFfSEcWs6S7J1u.jpeg)
```

---
