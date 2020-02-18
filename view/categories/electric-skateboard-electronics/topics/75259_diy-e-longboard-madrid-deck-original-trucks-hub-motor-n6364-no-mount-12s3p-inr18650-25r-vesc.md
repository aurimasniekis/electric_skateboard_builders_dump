# DIY E-Longboard &#124; Madrid Deck &#124; Original Trucks &#124; Hub Motor N6364 &#124; no Mount &#124; 12S3P (INR18650 25R) &#124; VESC

### Replies: 13 Views: 436

## \#1 Posted by: Nikolai2111 Posted at: 2018-11-19T19:46:51.258Z Reads: 113

```
Hello There

I'm building an e-longboard for my graduation work. The construction progressed very well and I was able to do the first tests. So far so well there were only small problems, the idle tests worked great.
Now the problem occurred when I wanted to test the board under load. The engines shook and vibrated, but didn't turn a bit.
But as soon as I pushed myself off and started to roll, they started to build up torque and it almost threw me off the board.
I'm assuming there's something wrong with the rotating field. Or that the rotating field rotates too fast, that the wheel cannot build up any torque.
I would be glad if the community could help me with this problem, because there is a lot of know-how in this forum.
In my board are VESC, a hub motor N6364 from China and a self-made battery pack 12S3P made of INR18650 25R cells. My remote control is a typical china model.

This are my wheels and the VESC I use one for two motors.
![IMG_20181117_175012|666x500](upload://tKyefZ74IJfSKKhQbvl3FzXKFW3.jpeg) 
![Wheels|690x292](upload://z9T1xmOlWNIVRWvizlH5Dq5XVUi.jpeg) 
This is my RC.
![IMG_20181117_175021|666x500](upload://d4g0KVPBmOw3tEEN02pHDNpbAnn.jpeg) 
This is my battery pack with the BMS.
![IMG_20181110_174026|666x500](upload://zHCRjOVOBjc9bs7JloP8wp2pjIK.jpeg) 
My BMS Settings
![BMS_Info|690x422](upload://6AxJkYHSXwsVAaJhdz05t4Ghryj.png) ![BMS_Settings|690x420](upload://iDQ0wOow0o0CONO15vZO7qCF81b.png) 
My VESC settings.
Motor Settings
General
![VESC_Motor_General-General|690x388](upload://wBQVIAjzYBFm8Be7R6t14YNNivM.png) 
Current
![VESC_Motor_General-Current|690x388](upload://oYBqi9e9Xy2khORgra78DxLx1CX.png) 
Voltage
![VESC_Motor_General-Voltage|690x388](upload://3qPrYtChKlMKAT6Rl12PekwlKIE.png) 
RPM
![VESC_Motor_General-RPM|690x388](upload://ngVmhWELNtlSdpuZioEiIqAq4EM.png) 
Wattage
![VESC_Motor_General-Wattage|690x388](upload://wJ84kR7ZaWsPKpO1ivhcQtohlVE.png) 
Temperature
![VESC_Motor_General-Temperature|690x388](upload://biIuScMo1WvnLgurPzBVKMiHY5f.png) 
Advanced
![VESC_Motor_General-Advanced|690x388](upload://kVv1vVhXvdknNyyDrrWVQU3MoaQ.png) 

BLDC Settings
General
![VESC_Motor_BLDC-General|690x388](upload://9KmJ3JTarrG0hF7Y4UpSu8rn6cF.png) 
Sensorless
![VESC_Motor_BLDC-Sensorless|690x388](upload://zOvGZ8kTAuGIvZ0xlkxedqi1f1T.png) 
Sensors
![VESC_Motor_BLDC-Sensor|690x388](upload://tj17flREfUeeKqQQevA7fSSNp6Y.png) 
Advanced
![VESC_Motor_BLDC-Advanced|690x388](upload://yfc3yeXE6SoBcROaKWBkrVCfwHC.png) 

APP Settings (However, I still think the problem is with the remote control.)
General
![VESC_APP-General|690x388](upload://6tqVPcHmPlAiZfjbNetkQLrMPRR.png) 
PPM
![VESC_APP_PPM-Throttle|690x388](upload://hbgMghRZ2B8bJiNORt8eJngClxJ.png) 
Mapping
![VESC_APP_PPM-Mapping|690x388](upload://z3OHwh4ivMYIpJBaqp05Cdp9p5N.png) 
Throttle Curve
![VESC_APP_PPM-Throttle|690x388](upload://hbgMghRZ2B8bJiNORt8eJngClxJ.png) 
Here are the RealTime Data
This shows the Current with no load attached.
![VESC_RT-DATA_with-no-Load|690x388](upload://zjpGdBcYjLpTWgTtTZ40ffQigGn.png) 
This shows the Current with load attached. The Current is only 2 or 3 Amps for a motor under Load?!
![VESC_RT-DATA_with-Load|690x388](upload://4R0RFdbxO7wCGY5tGaWsQbFpt7i.png) 

Hera are the videos.
This is with no load attached.
https://youtu.be/dTbel_uf9Cg
This is with load attached. 
https://youtu.be/6cpLV8g438A

I hope I have written all the necessary information and you can help me so that I can do my first manned test drives soon.
I thank you in advance for your helpfulness.
Thank you very much!

Nikolai2111
```

---
## \#2 Posted by: Grozniy Posted at: 2018-11-19T19:50:56.697Z Reads: 85

```
I think the problem is here

[quote="Nikolai2111, post:1, topic:75259"]
This are my wheels and the VESC I use one for two motors
[/quote]
```

---
## \#3 Posted by: pat.speed Posted at: 2018-11-19T19:52:10.952Z Reads: 85

```
Oh shit, never seen this before. I really don’t think it will work. You need to have 1 vesc per motor
```

---
## \#4 Posted by: Nikolai2111 Posted at: 2018-11-19T19:53:03.061Z Reads: 89

```
Thank you for your very fast answer.

I had already thought about that and did the same test as in the Viedos. Only that this time only one hub motor was plugged in.
```

---
## \#5 Posted by: Nikolai2111 Posted at: 2018-11-19T19:56:09.865Z Reads: 87

```
[quote="pat.speed, post:3, topic:75259, full:true"]
Oh shit, never seen this before. I really don’t think it will work. You need to have 1 vesc per motor
[/quote]

But why?
I've seen a lot of people do that. the maximum current per motor is 30A which is fused to a maximum of 60A in the VESC.
```

---
## \#6 Posted by: pat.speed Posted at: 2018-11-19T19:57:29.789Z Reads: 84

```
I think you have seen people using dual vescs. There are vescs our now that allow you to use to motors. They are basically just two vesc connected together
```

---
## \#7 Posted by: Nikolai2111 Posted at: 2018-11-19T20:14:59.015Z Reads: 78

```
But why shouldn't this working?

In this video and with out Load on my board it runs fine.
https://www.youtube.com/watch?v=GZkbB82-YBM

Here is also a link.
https://www.electric-skateboard.builders/t/dual-bldc-single-vesc-works/15193
```

---
## \#8 Posted by: JTAG Posted at: 2018-11-19T23:12:19.510Z Reads: 65

```
For two motors to work on a single controller you need to mechanically sync both motors such that they produce the same back emf ALL the time. 

With a motor per wheel without mechanical coupling and synchronisation setup you will burn either your motor or your esc.
```

---
## \#9 Posted by: pat.speed Posted at: 2018-11-20T04:58:25.602Z Reads: 49

```
Which would then lead to possible turning problems due to the inner wheel not being able to spin slower
```

---
## \#10 Posted by: Nikolai2111 Posted at: 2018-12-10T21:08:23.736Z Reads: 35

```
Thank you very much for the quick answers.

And sorry for the very late reply. I could only check the problem last weekend.

To do this I disconnected a motor and ran a new motor detection and blocked the motor again. I found the exact same problem.
Unfortunately I didn't pay enough attention and short-circuited the phases, which destroyed the driver.

Now someone can tell me what and where the problem is, because now only one motor is connected via the VESC and the problem still exists. 
The parameters have not been changed except for the parameters that are changed during motor detection
```

---
## \#11 Posted by: pat.speed Posted at: 2018-12-10T21:14:02.094Z Reads: 33

```
You probably fried the vesc. Plug it in try to run a detection then after it fails go to the terminal tab and type faults
```

---
## \#12 Posted by: Nikolai2111 Posted at: 2018-12-10T21:35:22.418Z Reads: 33

```
Yes, I burned the VESC. But by the short circuit of the phases. The driver broke.
But before that everything was OK or do you think that vesc was already broken?
Yes I did a motor detection before it burned, but it still didn't work. The motor was shaking like in the video.
```

---
## \#13 Posted by: bartroosen12 Posted at: 2018-12-10T21:46:43.379Z Reads: 31

```
You really scared me
![gallery|281x500](upload://d3PdJF0N4djVolxEmBLftcDQy07.jpeg) 

Maybe the problem is that the motors have no sensor wires and the vesc doesn't like it?
I see they are suggesting the chinese dual hubmotor controllers but you already got a 12S battery and the chinese esc's will work up to 50V.
So if you buy this: 
http://www.diyeboard.com/v20-dual-hub-motors-sine-wave-foc-esc-speed-controller-p-674.html
You need to make sure you charge your batteries only up to around 4.15V per cell which is totally fine.
```

---
