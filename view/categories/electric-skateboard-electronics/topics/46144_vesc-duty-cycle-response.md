# VESC duty cycle response

### Replies: 27 Views: 1912

## \#1 Posted by: CsabyTech Posted at: 2018-02-11T22:01:23.648Z Reads: 142

```
Hi guys!

I have a problem, where if I have the motor running at some duty cycle (say 90%) and than I move the ppm control to the middle (current control, so middle means no input), the duty cycle will remain the same for about another second. 
This is extremely annoying and dangerous, and I can't seem to find a solution. I can see the transmitter signal setting back to the middle right when I move the controller, so the signal should be fine, but the duty cycle is just stuck there.
Does anyone know what the problem could be?

(maytech vesc, hw 4.10, fw 3.3
sensored 170kv motor)
```

---
## \#2 Posted by: CsabyTech Posted at: 2018-02-11T22:02:32.904Z Reads: 134

```
I'm using the motor in bldc mode, as this is hw 4.10 so FOC braking doesn't work for me
```

---
## \#3 Posted by: Martinsp Posted at: 2018-02-11T22:05:56.942Z Reads: 130

```
I have not come across this problem myself yet but for starters I would try to use 2.18 or 2.54 firmware just to see if there is not some problem with 4.10 and 3.3, there should not be AFAIK but just to make sure.
```

---
## \#4 Posted by: CsabyTech Posted at: 2018-02-11T22:09:53.560Z Reads: 126

```
thanks for the suggestion, I'll definitely try that, but I'll wait a little to see if someone has experience with this issue, so I don't have to keep flashing the firmwares if that is indeed not the problem.
```

---
## \#5 Posted by: Pedrodemio Posted at: 2018-02-11T22:22:26.602Z Reads: 118

```
Whats values do you have for ramping? most important negative ramping time, this is perhaps the most dangerous setting in the current version and i think it's on the list to be fixed

If you accidentally set the negative ramping to a high value, lets say 10 seconds, if you realease the throttle
```

---
## \#6 Posted by: CsabyTech Posted at: 2018-02-11T22:34:41.055Z Reads: 106

```
I have negative ramping at 3 sec, and I can see when the brakes kick in, and I don't think that's the problem. When it starts braking, I can see the ramping building up, and it looks fine, the problem is, that it only starts doing any braking or any response at all, after about 1 sec. During that 1 second, the motor duty is stuck at where it has been, so if I'm accelerating and I decide to cruise, it will actually keep accelerating for another second... Nearly had an accident with this earlier.
```

---
## \#7 Posted by: CsabyTech Posted at: 2018-02-11T22:36:34.884Z Reads: 95

```
It also remains stuck if I don't actually apply the brake, just go back to no input (middle position). Same thing if I actually do brake. Everything works eventually, it is just stuck for 1 second.
```

---
## \#8 Posted by: b264 Posted at: 2018-02-11T23:03:08.918Z Reads: 86

```
If you look at the real-time data does your PPM input actually go down the instant you release the throttle?

What remote & receiver are you using?
```

---
## \#9 Posted by: CsabyTech Posted at: 2018-02-11T23:07:35.461Z Reads: 81

```
I actually stated this in the original post, yes, the ppm input signal goes instantly where I want it to go. I had my board connected to the VESC tool for analyzing. I do not think the transmitter or receiver are the cause of this problem. I will make a video tomorrow if I can't fix the issue by then (it's 00:07 here)
```

---
## \#10 Posted by: GrecoMan Posted at: 2018-02-11T23:08:16.815Z Reads: 78

```
[quote="b264, post:8, topic:46144"]
What remote & receiver are you using?
[/quote]

this question still stands
```

---
## \#11 Posted by: CsabyTech Posted at: 2018-02-11T23:10:23.239Z Reads: 76

```
I didn't answer that question because I don't have a good answer. It's just a regular 2.4Ghz rc controller you can buy off aliexpress for 30$. I am aware of the poor quality of this, but as the data shows, that is not the issue here, as the incoming signals to the VESC are exactly what they should be
```

---
## \#12 Posted by: GrecoMan Posted at: 2018-02-11T23:12:38.706Z Reads: 72

```
there is still a good chance it could be your remote...

please link it here.
```

---
## \#13 Posted by: CsabyTech Posted at: 2018-02-11T23:17:24.587Z Reads: 70

```
Can you please explain how the remote could be the problem?
I am looking at realtime data from the VESC tool, and I can clearly see the ppm signal moving instantly where I set it, and it is only showing the data that the VESC receives, so I don't see how that could be the problem. It is clear that the duty cycle is stuck way after the ppm signal is already different, as I can see that in real time on the screen. 
https://www.aliexpress.com/item/2-4Ghz-Electric-Skateboard-Remote-Controller-with-Receiver-Universal-for-All-ESC-Longboard-Skate-Board-Scooter/32840986176.html?ws_ab_test=searchweb0_0,searchweb201602_2_10152_10151_10065_10344_10068_10345_10342_10343_51102_10340_10341_10609_10541_10084_10083_10304_10307_10302_5060020_5870020_5130020_10312_10059_10313_10314_10534_5000020_100031_10604_10103_10605_10594_10142_10107_5080020,searchweb201603_2,ppcSwitch_5&algo_expid=9ac9fd34-0e88-4ae1-a192-a55b8364f36f-20&algo_pvid=9ac9fd34-0e88-4ae1-a192-a55b8364f36f&rmStoreLevelAB=5
```

---
## \#14 Posted by: scepterr Posted at: 2018-02-11T23:28:33.897Z Reads: 65

```
A pic of the vesc would be nice, I'm betting it's missing C37
```

---
## \#15 Posted by: CsabyTech Posted at: 2018-02-11T23:31:56.539Z Reads: 65

```
Is that the capacitor that was added in hw 4.12? Mine is 4.10, so if that's the case, than it is indeed missing, which is exactly why it doesn't work in FOC mode, which is why I'm using it in BLDC mode. I can't easily take a picture, it is assembled in such a way, that getting a pick of that would be a 4 hour job... I don't see how that could be the problem, but do explain if you think that could cause this
```

---
## \#16 Posted by: scepterr Posted at: 2018-02-11T23:32:23.913Z Reads: 61

```
No it's on 4.10 as well, just I've seen plenty of maytechs missing that
```

---
## \#17 Posted by: b264 Posted at: 2018-02-11T23:33:54.783Z Reads: 61

```
I'm not sure how C37 missing could cause those symptoms
```

---
## \#18 Posted by: CsabyTech Posted at: 2018-02-11T23:35:05.621Z Reads: 59

```
I can't tell if it's missing it without taking everything apart, which I'd like to avoid, as I really don't see how that could cause this problem.
I still suspect something software related, I just don't know what it could be.
```

---
## \#19 Posted by: scepterr Posted at: 2018-02-11T23:38:22.030Z Reads: 59

```
It's a decoupling capacitor for the fets
I guess not having it could cause some delays?
```

---
## \#20 Posted by: b264 Posted at: 2018-02-11T23:40:31.314Z Reads: 57

```
No it sounds more software-related I think.  It has to be something simple that's been overlooked
```

---
## \#21 Posted by: scepterr Posted at: 2018-02-11T23:41:10.713Z Reads: 52

```
Well either way we need pics of all the settings pages atleast

For reference:
https://www.electric-skateboard.builders/t/help-please-my-board-has-a-speed-restriction/46018
```

---
## \#22 Posted by: CsabyTech Posted at: 2018-02-11T23:49:03.933Z Reads: 55

```
These are my current settings

![bldc1|690x388](upload://rApW04jchFKEJf5t0QvN7XbgdG8.png)![ppm1|690x388](upload://mIJw01GGnF0U39e1qQZSrG2SJ99.png)![general1|690x388](upload://eoPLPlgnijWxxLotiJ09faRDtgJ.png)![general2|690x388](upload://vxcoJ03IsMRUfSibQK20wCWXrpo.png)![bldc2|690x388](upload://b7kB1pcm4lldeRIEGBbezahXLpc.png)![ppm2|690x388](upload://aihqiEZGYbwmQ6w22IMgT8XraVx.png)![ppm3|690x388](upload://tqdAdyk1qkFwdxUiMYH1xWsR2rA.png)
```

---
## \#23 Posted by: scepterr Posted at: 2018-02-11T23:54:52.700Z Reads: 52

```
Settings look fine to me
I would try an earlier firmware first, I think that's the simplest variable to eliminate
```

---
## \#24 Posted by: CsabyTech Posted at: 2018-02-11T23:57:03.583Z Reads: 51

```
best guess for now... I'll try that first thing tomorrow
```

---
## \#25 Posted by: Jumpman Posted at: 2018-02-12T11:07:58.470Z Reads: 42

```

The vesc project manual suggests changing to 0.1 seconds negative ramping for quicker braking response.  So, 6 and 3 seconds, positive and negative ramping, seems a bit high?  

Are those the default settings?  Or, did you change them for some reason?
```

---
## \#26 Posted by: CsabyTech Posted at: 2018-02-12T13:52:41.597Z Reads: 36

```
Thanks man!
This actually fixed the issue!
```

---
## \#27 Posted by: CsabyTech Posted at: 2018-02-12T14:04:09.758Z Reads: 35

```
Thanks for your time!
```

---
