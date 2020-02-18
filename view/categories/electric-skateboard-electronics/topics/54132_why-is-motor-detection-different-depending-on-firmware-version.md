# Why is motor detection different depending on firmware version?

### Replies: 9 Views: 333

## \#1 Posted by: TSG_AU Posted at: 2018-05-02T14:27:17.838Z Reads: 71

```
I was running v4.12 VESCS with v3.3x firmware, and was having trouble with my motors cogging too much at low-moderate speed and high throttle input. Thinking that it had something to do with the FOC parameters, I flashed the VESCs with v2.18 firmware, and re-ran motor detection. The values returned were different, which I then applied to VESCs after reflashing them with v3.3x firmware again- this resulted in a huge improvement in performance- some cogging still occurs, but I could probably just raise my sensorless minimum ERPM up to 8000 or so and live with it.

So why did detection return different values between the firmware versions? Some values stayed pretty much the same, but L for example changed by over x2

Comparing detected/calc'ed parameters between v3.3x and v2.18 firmware:
R from 220mOhm to 195mOhm
L from 60uH to 140uH
lambda stayed about the same
Observer gain from 6 to 7
Current Kp from 0.06 to 0.1415
Current Ki from 225 to 195
```

---
## \#2 Posted by: onepunchboard Posted at: 2018-05-02T16:09:48.246Z Reads: 51

```
perhaps they backed up the settin a bit, from agressive 2.18, in order to solve drv problem
```

---
## \#3 Posted by: TSG_AU Posted at: 2018-05-03T00:44:07.843Z Reads: 30

```
I see. Well here's to hoping my DRVs don't burn out, since I'm also running a 12S battery.
```

---
## \#4 Posted by: strattos Posted at: 2018-05-03T00:46:45.936Z Reads: 28

```
What Vesc is it/ have you had any issues running FOC?
```

---
## \#5 Posted by: TSG_AU Posted at: 2018-05-03T01:03:13.836Z Reads: 25

```
VESC 4.12, and they had no trouble running my 6S satellite setup (~250kv motors) on FOC
```

---
## \#6 Posted by: strattos Posted at: 2018-05-03T01:21:21.074Z Reads: 22

```
I was hoping for which I guess version of the 4.12 design I guess the better question would be what supplier did you get it from
```

---
## \#7 Posted by: TSG_AU Posted at: 2018-05-03T01:27:21.157Z Reads: 20

```
I bought them both damaged second hand from different people, but I believe they were both from  originally.
I replaced the DRV chip, the STM32 on one of them, and added in the missing cap (on C26 I think)
```

---
## \#8 Posted by: strattos Posted at: 2018-05-03T01:31:04.832Z Reads: 20

```
Ohh cool thanks for the info. As far as motor detection goes I guess it would make sense if they've adjusted the parameters to try to avoid blowing the drv, however I don't think you could get that confirmed by anyone but vedder himself.
```

---
## \#9 Posted by: district9prawn Posted at: 2018-05-03T02:58:30.241Z Reads: 15

```
I had a similar problem going from firmware 2.18 to 3.38 on focbox. On 3.38, inductance was usually way off, resulting in the motor running rough and throwing over current faults. I tried running detection over and over again at different rotor positions and found that sometimes it would return the same inductance as fw 2.18, which would run smoothly.
```

---
