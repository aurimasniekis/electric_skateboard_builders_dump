# VESC 4 BLDC motor twitching

### Replies: 29 Views: 1519

## \#1 Posted by: Ingvarjedi Posted at: 2018-03-08T08:22:30.932Z Reads: 141

```
Who can explain why the engine twitching when the BLDC mode on this video? It can be fixed?

https://www.youtube.com/watch?v=RFA9374i2pk
```

---
## \#2 Posted by: Manu39 Posted at: 2018-03-08T08:35:46.538Z Reads: 135

```
sensorless engine so cooking at the demarage ..
```

---
## \#3 Posted by: Ingvarjedi Posted at: 2018-03-08T08:40:07.294Z Reads: 129

```
Do not understand a little bit. What you mean?
```

---
## \#4 Posted by: Manu39 Posted at: 2018-03-08T08:43:28.633Z Reads: 129

```
if your engine does not have a sensor then it is normal that you are a twitching ...
```

---
## \#5 Posted by: Ingvarjedi Posted at: 2018-03-08T08:49:39.467Z Reads: 131

```
These twitches will not spoil the motor or VESC? 

The difference in the use of the sensor and the sensorless motor only in jerking?
The maximum torque, the maximum speed will be unchanged?
```

---
## \#6 Posted by: Der6FingerJo Posted at: 2018-03-08T09:11:07.800Z Reads: 124

```
Essentially yes. A VESC can run Motors in BLDC or FOC mode. BLDC is the regular mode every R/C ESC uses, FOC is a bit more sophisticated and reducing the jerking in sensorless mode quite abit, but it's hard to run on high-kv motors and 4.12 regular VESCs.

Sensors are only really implemented in FOC mode, a buddy of mine uses sensors, regular HW4.12 and BLDC on his mountainboard and it still isn't as smooth as my VESC 6 FOC Sensor setup.

If you want to run FOC successfully, go with low kv motors and at least a Focbox, esk8 controller or similar VESC that is abit upgraded. Also look into stewiis ESCape, bimmers B-Box or Trampas VESC6 for best performance.
```

---
## \#7 Posted by: Manu39 Posted at: 2018-03-08T09:41:12.617Z Reads: 113

```
Very good summary @Der6FingerJo , you said everything.
```

---
## \#8 Posted by: Ingvarjedi Posted at: 2018-03-08T10:00:13.225Z Reads: 107

```
I have 192kv and VESC 4.12 from DIY.
Is it safe to use FOC mod with 12s battery?
```

---
## \#9 Posted by: pat.speed Posted at: 2018-03-08T10:13:28.822Z Reads: 100

```
**NO**

That will cook your vescs
```

---
## \#10 Posted by: Ingvarjedi Posted at: 2018-03-08T10:17:37.320Z Reads: 98

```
If limit the voltage to 10s?
```

---
## \#11 Posted by: pat.speed Posted at: 2018-03-08T10:20:24.627Z Reads: 95

```
Still no, diys vescs can't handle foc
```

---
## \#12 Posted by: Der6FingerJo Posted at: 2018-03-08T10:22:40.238Z Reads: 91

```
As @pat.speed said, i wouldn't risk it either. 
Options that come to my mind are:
- switch motor from star to delta connection to reduce kv (i have never done this, you will have to read up on this)
- get lower kv motors, 130kv and less
- use a VESC6 based ESC, i don't think any 4.xx hardware would handle 192kv on 12S with FOC
- install sensors and have at least a bit better bldc until vedder implements it proper (again, never done this myself)
- switch to 10S but still need a lower kv motor

Personally i would go with a VESC 6 derivative right now (or the trampa one if you can afford that, lol) as it seems to be bulletproof so far.

Would also be interesting what kind of board you want to build, mountainboard like in @Rich's  video or something else?
```

---
## \#13 Posted by: pat.speed Posted at: 2018-03-08T10:24:31.446Z Reads: 85

```
Spot on. I've never personally heard about the kV needing to be low. All I know is focboxs can handle 12s and 190kv. Some even push to 13s but that is right on the limit
```

---
## \#14 Posted by: Der6FingerJo Posted at: 2018-03-08T10:27:33.228Z Reads: 79

```
I'm not 100% sure about the kv thing, i just know from @Rich that his 136kv motors from trampa worked ok with stock 4.12 VESC FOC on 10S so we thought kv (more eRPM) might play a role in it. 
Could also be that i underestimate the Focbox, never personally used one :smile:
```

---
## \#15 Posted by: pat.speed Posted at: 2018-03-08T10:28:41.787Z Reads: 74

```
Hmm that's interesting I have only ever heard of a small few people that have had foc work reliably on Vesc 4
```

---
## \#16 Posted by: Der6FingerJo Posted at: 2018-03-08T10:32:32.442Z Reads: 70

```
I can only tell that i fried my stock 4.12 esk8.de VESC DRV on FOC after maybe 5 kilometers and a hard bump (the electronic box never touched anything, just a semi high curb i didn't see coming). It was with 10S and 168kv motor, can't tell if it was because of FOC or because of the bump.

Seems to be a gamble with 4.xx hardware.

That's why i got VESC 6 for my mountainboard, no worries and awesome startup performance.
```

---
## \#17 Posted by: Ingvarjedi Posted at: 2018-03-08T10:43:53.221Z Reads: 71

```
I want MTB Trampa
```

---
## \#18 Posted by: Der6FingerJo Posted at: 2018-03-08T10:48:36.681Z Reads: 69

```
In this case i personally think that 192kv is a bit high on 12S, common gearing options range from 1:4 to 1:5 and even with 1:5 gearing your top speed would be ~40mph~60km/h, assuming you use 8" tires. 

Maybe think about changing motors to 150kv or less.
```

---
## \#19 Posted by: laurnts Posted at: 2018-03-08T10:49:39.161Z Reads: 69

```
Holla - holla wait, wait a second. This description have some right and wrong to it. Both BLDC and FOC mode can run sensored and sensorless. VESC doesn't prefer lower kv motor over higher kv motor and it works well for any of them despite what it's being used for (drone / rc / esk8) as long as it being used for brushless motor. FOC mode is known for silent and abit more torque compared to BLDC, thats correct, but doesn't necessarily means that BLDC is worst than FOC and or FOC is burning up VESC. This is untrue, otherwise why most of us runs FOC mode.

There are however some conceptions about bad VESC and bad VESC suppliers, but it doesnt mean it applies to all VESC. I have VESC 4.12 running FOC for 3 years already, works awesome. I got one fail VESC from enertion, one of the very first batch. It even burns from BLDC mode, so it have nothing to do with FOC / BLDC.
```

---
## \#20 Posted by: Ingvarjedi Posted at: 2018-03-08T10:52:23.826Z Reads: 66

```
I think we need to make the right setting and will not fry
```

---
## \#21 Posted by: Der6FingerJo Posted at: 2018-03-08T11:01:31.694Z Reads: 62

```
Good to have another perspective :sweat_smile:

Most people i have talked to about this had problems with FOC on 4.12 Hardware while BLDC was generally fine, maybe it's just the bubble i'm in. 
Sure some VESCs burned in BLDC mode, but FOC VESCs burning seemed to be more frequent.

And to clarify, i think FOC feels way better than BLDC on Long- and Mountainboards, be it with or without sensors. But i don't think it's absolutely necessary to ride, on the street it's definitely more of a nice extra.

[quote="laurnts, post:19, topic:48476"]
VESC doesn’t prefer lower kv motor over higher kv motor and it works well for any of them despite what it’s being used for (drone / rc / esk8) as long as it being used for brushless motor.
[/quote]

But eRPM definitely is a thing and depends on voltage and kv, so given his 12S voltage a lower kv motor would result in less eRPMs which in turn should result in an easier time for the VESC to compute it's output. 

I don't claim to know anything i said with absolut certainty, but it makes sense in my head.
```

---
## \#22 Posted by: laurnts Posted at: 2018-03-08T12:06:26.847Z Reads: 60

```
Yes there are some cases where VESC burned down because of too high erpm. I think focbox and new vesc with direct fets release dont have this issue anymore. Better ask the seller if the vesc is ok with 12s setup.

Anyway I prefer to ride 10s as I don't like stressing vesc with super high current and or voltage. Yet I still love the idea of running higher voltage to reduce current draw.

FOC mode enforces VESC to process more data which causes more heat to be produced.
```

---
## \#23 Posted by: rich Posted at: 2018-03-08T13:40:39.603Z Reads: 63

```
Funny to see my video in a thread, it reminds me of the annoying experience last year.

[quote="Ingvarjedi, post:1, topic:48476"]
Who can explain why the engine twitching when the BLDC mode on this video?
[/quote]

Like @Manu39 said, with unsensored motors this behaviour would be normal. With sensored motors in hybrid/sensored BLDC mode there is zero difference in startup but better control at low speed.

This is because the hall sensors are not properly working in BLDC but perfect in FOC. This is what Vedder told me in the vesc-project forum:

![1|690x141](upload://3SpJVicjyr710rnsB8FPbXTaMR5.PNG)
![2|690x144](upload://1e8EGHBhonUg7GXRegPRTlAA3i8.PNG)


You see (4th line) that he is working on that for future updates of the FW

![todo|690x314](upload://mxFIBxm8x65xovcQQl2zJp6TDpl.PNG)

[quote="Der6FingerJo, post:6, topic:48476"]
If you want to run FOC successfully, go with low kv motors and at least a Focbox, esk8 controller or similar VESC that is abit upgraded. Also look into stewiis ESCape, bimmers B-Box or Trampas VESC6 for best performance.
[/quote]

I totally agree

[quote="pat.speed, post:13, topic:48476"]
Spot on. I’ve never personally heard about the kV needing to be low.
[/quote]

This is what Benjamin told me. Also vendors like esk8.de  mention that it must be below 200kv. It seems like it is safer with less kv.

[quote="Der6FingerJo, post:14, topic:48476"]
I’m not 100% sure about the kv thing, i just know from @Rich that his 136kv motors from trampa worked ok with stock 4.12 VESC FOC on 10S so we thought kv (more eRPM) might play a role in it.
[/quote]

If you don't know this video, here we go 

https://www.youtube.com/watch?v=ptlHqK7kqCA

[quote="laurnts, post:19, topic:48476"]
Both BLDC and FOC mode can run sensored and sensorless
[/quote]

Yes but hybrid/sensored BLDC didn't work at all as you can see :wink:

[quote="Ingvarjedi, post:5, topic:48476"]
These twitches will not spoil the motor or VESC?
[/quote]

I'm not sure in long term but I can guarantee it spoils your mind and mood :laughing:.
It was a nightmare after spending that money and time!


I think you have 2 options:
wait until the hall sensors are better working in a new update of the FW or buy new controller (Vesc 6 or similar). Also 192kv is high kv for mountainboard but it should work for the beginning. If you want more torque and efficiency get lower kv motors.
```

---
## \#24 Posted by: laurnts Posted at: 2018-03-08T13:58:57.370Z Reads: 53

```
Very correct! Maybe I was still using old HW and old version of HW that works fine with me. I don't know how and or why it works, but it works fine with mine. However I totally agree that FOC hybrid mode runs very very smooth with low kv motor. As the creator of VESC him self stated, it's best to go with his recommendation. Thank you @rich for providing a very good reference!
```

---
## \#25 Posted by: Namasaki Posted at: 2018-03-09T06:06:25.171Z Reads: 49

```
great video!

Makes me want to try FOC now!
```

---
## \#26 Posted by: Juiced Posted at: 2018-03-09T07:20:14.694Z Reads: 50

```
I've used foc for months and no problem with diy vesc.
```

---
## \#27 Posted by: Namasaki Posted at: 2018-03-09T16:24:37.803Z Reads: 43

```
I’m using Ollin Vescs with heat sinks version 4.12 with 2.19 firmware setup on BLDC tool. 

What version hardware and firmware are you using?
```

---
## \#28 Posted by: Der6FingerJo Posted at: 2018-03-09T17:01:36.073Z Reads: 40

```
For FOC i would suggest updating the VESCs, Benjamin said that FW3.xx is much better at calculating FOC.
```

---
## \#29 Posted by: Juiced Posted at: 2018-03-10T05:03:25.885Z Reads: 35

```
Diy vesc 4.12 with 2.18 fw. I've switched from bldc to foc a couple times due to thinking I damaged my vesc but never once had a problem.   I also have a lot of wire because I made series connections for my batteries.  (Single tb 6374 btw).
```

---
