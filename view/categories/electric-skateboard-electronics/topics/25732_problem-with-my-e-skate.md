# Problem with my e-skate

### Replies: 32 Views: 1347

## \#1 Posted by: Koto Posted at: 2017-06-20T01:03:32.357Z Reads: 209

```
at the start of the year a made an esk8 that broke on its third run. I have another thread on this, and people said it was my drv. i got a new diy's vesc, but when i press the trigger, the vesc flashes red three times, the motor kind of started and stopped a few times but now it doesnt work. what have i done/how do i fix this
```

---
## \#2 Posted by: JLabs Posted at: 2017-06-20T01:24:59.087Z Reads: 206

```
Did you run motor detection? Please post pictures of your build and VESC screenshots. It helps us help you.
```

---
## \#3 Posted by: Koto Posted at: 2017-06-20T04:11:40.582Z Reads: 191

```
when i press connect on bldc it says no firmware read response
```

---
## \#4 Posted by: Koto Posted at: 2017-06-20T04:43:38.048Z Reads: 181

```
I feel like i have the same problem to @kaiser
```

---
## \#5 Posted by: Alanhunt123 Posted at: 2017-06-20T04:54:59.062Z Reads: 175

```
I hate to say it, but that red flashing usually means the DRV chip is blown.

You may have had a short in your motor leads. It may surprise you (certainly surprised me), but plugging the bullet connectors in and not taping them individually can result in a short, as happened to one of my VESCs. It shared similar symptoms of sort of working for a little bit, then dying completely.

Depending on where you got it, you might be able to get it repaired for very low cost. Mine from Enertion has been repaired for free given that I payed for shipping. 

Best of luck!
```

---
## \#6 Posted by: Alanhunt123 Posted at: 2017-06-20T04:56:27.622Z Reads: 162

```
Of course, some screenshots of settings would also help, as well as a picture of your hardware setup.
```

---
## \#7 Posted by: Koto Posted at: 2017-06-20T06:00:11.637Z Reads: 155

```
but i got a brand new vesc because 'apparently' the drv was blown on my last one so i think its the motor
```

---
## \#8 Posted by: Koto Posted at: 2017-06-20T06:27:55.901Z Reads: 154

```
hi i found my fault, is it my drv?Fault            : FAULT_CODE_DRV8302
Current          : 0.5
Current filtered : -0.0
Voltage          : 30.76
Duty             : 0.37
RPM              : 0.0
Tacho            : 1
Cycles running   : 3
TIM duty         : 3724
TIM val samp     : 1866
TIM current samp : 6895
TIM top          : 10057
Comm step        : 2
Temperature      : 24.48

Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 68.9
Current filtered : 130.7
Voltage          : 30.77
Duty             : 0.01
RPM              : 1.1
Tacho            : 2
Cycles running   : 26
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 3
Temperature      : 24.56

Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 56.6
Current filtered : 132.6
Voltage          : 30.77
Duty             : 0.01
RPM              : 3.2
Tacho            : 5
Cycles running   : 20
TIM duty         : 554
TIM val samp     : 297
TIM current samp : 24879
TIM top          : 49165
Comm step        : 6
Temperature      : 24.66

Fault            : FAULT_CODE_DRV8302
Current          : 0.4
Current filtered : -0.4
Voltage          : 30.76
Duty             : 0.39
RPM              : 1.3
Tacho            : 6
Cycles running   : 17
TIM duty         : 3752
TIM val samp     : 1880
TIM current samp : 6740
TIM top          : 9719
Comm step        : 1
Temperature      : 24.89

Fault            : FAULT_CODE_DRV8302
Current          : 0.4
Current filtered : -0.2
Voltage          : 30.73
Duty             : 0.35
RPM              : 1.0
Tacho            : 7
Cycles running   : 17
TIM duty         : 3682
TIM val samp     : 1835
TIM current samp : 7129
TIM top          : 10588
Comm step        : 2
Temperature      : 25.06

Fault            : FAULT_CODE_ABS_OVER_CURRENT
Current          : 41.7
Current filtered : 139.3
Voltage          : 30.86
Duty             : 0.02
RPM              : 2.4
Tacho            : 11
Cycles running   : 20
TIM duty         : 792
TIM val samp     : 421
TIM current samp : 23542
TIM top          : 46242
Comm step        : 6
Temperature      : 24.21
```

---
## \#9 Posted by: Koto Posted at: 2017-06-20T06:47:59.803Z Reads: 138

```
<img src="/uploads/db1493/original/3X/4/6/4676243f303fb9533e00a039affcdc5d4cce8703.PNG" width="690" height="355">
```

---
## \#10 Posted by: Koto Posted at: 2017-06-20T06:51:21.937Z Reads: 138

```
<img src="/uploads/db1493/original/3X/4/7/476719ed78cddbd1522c7d844d0203c108e83917.PNG" width="690" height="358">
```

---
## \#11 Posted by: Koto Posted at: 2017-06-20T06:54:56.136Z Reads: 132

```
<img src="/uploads/db1493/original/3X/c/c/cc0d3903bd07d28804879f55a39cdce28355c366.PNG" width="690" height="354">
```

---
## \#12 Posted by: TarzanHBK Posted at: 2017-06-20T08:56:41.886Z Reads: 122

```
what battery are you using?
Your cutoff start and end are normaly too low.
Also that Error is due to overcurrent. Vesc max is 130A and you´re getting almost 140A, so the vesc shuts down and maybe blow its DRV.
```

---
## \#13 Posted by: Alanhunt123 Posted at: 2017-06-20T12:11:52.049Z Reads: 124

```
Yup that error code most likely means the DRV is blown. Try testing the motor leads for shorts with a multimeter.
```

---
## \#14 Posted by: Tuomalar Posted at: 2017-06-20T13:12:47.641Z Reads: 125

```
At first tell us what battery and motor you use?  Are you sure that you soldered all correctly? No cold joints. There is clearly something wrong in your set up if it blows drv that easy.
```

---
## \#15 Posted by: Koto Posted at: 2017-06-29T00:40:18.991Z Reads: 111

```
Your fucking kidding me, I just got a new vesc because the last blew. I think there is a problem with the motor that keeps blowing the drv
```

---
## \#16 Posted by: oldguy Posted at: 2017-06-29T00:59:42.013Z Reads: 107

```
 I am no expert but I believe what the people who responded here are saying is that if there is a problem or short in the motor leads, or even the battery leads for that matter, it is what is blowing your the DRV. No matter how many new controllers you get until  The original problem is rectified you will continue to blow all of them. You might inquire as to getting the DRV replaced which might be cheaper than buying yet another controller. But before you plug anything else in you should go over all of your connections to find out what  is causing these failures. It seems like you're VESC is the victim of a problem that has not yet been found or rectified.  I suppose it could be your motor, I am not discounting that, but there are many other more likely suspects. Just my .02
```

---
## \#17 Posted by: Koto Posted at: 2017-08-14T07:29:16.213Z Reads: 95

```
hey,
thank you so much for this, ive been really busy and just getting back in to the game. I'll look over everything but i also need a new drv, can u link me one i can buy?
```

---
## \#18 Posted by: lrdesigns Posted at: 2017-08-14T07:49:14.220Z Reads: 91

```
Take several close up pictures of all your wires. motor esc battery etc. Then the community here will try to help. Without seeing the setup we will just be guessing which is not that helpful to you. 

I agree with @oldguy that we need to find the source of the issue.

Edit, also where are you located? So we can suggest someone for repairs.
```

---
## \#19 Posted by: psychotiller Posted at: 2017-08-14T15:04:44.799Z Reads: 87

```
I can't see anywhere in this thread that you answered the question:

What motor and battery are you using?

First step in fixing your rig is answering the questions. Or, just keep blowing DRV's
```

---
## \#20 Posted by: Koto Posted at: 2017-08-26T03:27:47.529Z Reads: 73

```
Turnigy Aerodrive SK3 - 6364-245kv Brushless Outrunner Motor and Turnigy 5000mAh 3S 25C Lipo Pack. I think i might resolder all connections and see how it goes. Can u link a place in eBay with the drv I need
```

---
## \#21 Posted by: rich Posted at: 2017-08-26T11:02:41.452Z Reads: 67

```
[quote="Koto, post:20, topic:25732"]
Turnigy 5000mAh 3S 25C Lipo Pack
[/quote]

do you mean 2 lipo packs in series to get 6s?
```

---
## \#22 Posted by: Koto Posted at: 2017-08-29T08:20:20.331Z Reads: 65

```
yes that is coorect
```

---
## \#23 Posted by: Koto Posted at: 2017-09-23T03:07:44.704Z Reads: 57

```
@psychotiller @oldguy @rich 
sorry been busy but am hyped to be on holidays to fix this. im going to re solder each connection and cover all wires with tape or heat shrink. Sorry for inconsistent replies. wondering what type of drv I need so that i can replace my blown one. im using a Turnigy Aerodrive SK3 - 6364-245kv Brushless Outrunner Motor and Turnigy 5000mAh 3S 25C Lipo Pack (in series to get 6s). Thank you
```

---
## \#24 Posted by: Koto Posted at: 2017-09-23T03:08:31.523Z Reads: 55

```
oh and btw im in Melbourne australia
```

---
## \#25 Posted by: psychotiller Posted at: 2017-09-23T03:30:42.122Z Reads: 53

```
DRV8302 Not sure you'll have a supplier there. I'm sure somebody could send you one cheap though!
```

---
## \#26 Posted by: Koto Posted at: 2017-09-23T04:08:10.144Z Reads: 50

```
[quote="psychotiller, post:25, topic:25732"]
DRV8302
[/quote]

any recomended types like digi key or verical http://www.findchips.com/search/drv8302
```

---
## \#27 Posted by: psychotiller Posted at: 2017-09-23T04:08:53.216Z Reads: 47

```
Hmmm...Not sure on that aspect.
```

---
## \#28 Posted by: Koto Posted at: 2017-09-23T04:09:27.464Z Reads: 46

```
probs all the same... hopefully
```

---
## \#29 Posted by: Koto Posted at: 2017-09-23T04:09:47.011Z Reads: 48

```
oh actually just found a thread about this
thanks!!
```

---
## \#30 Posted by: Koto Posted at: 2017-10-02T07:40:57.618Z Reads: 37

```
Hi, resoldered everything, so i know its not the connection. it still says bad detection. is this normal<img src="/uploads/db1493/original/3X/2/0/204f3fa70cceed5ad21ef9acb7b5cce8125f00f1.PNG" width="690" height="450">
```

---
## \#31 Posted by: Koto Posted at: 2017-10-02T08:35:14.383Z Reads: 33

```
does this support that<img src="/uploads/db1493/original/3X/c/6/c66a00585f57d5234e67f8406cd52da9500d074c.PNG" width="690" height="439">
```

---
## \#32 Posted by: Koto Posted at: 2017-10-02T09:29:13.773Z Reads: 30

```
HERE IS A VIDEO https://youtu.be/fJBKZZLvTr0
```

---
