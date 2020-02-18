# Motor temp fault VESC 6+

### Replies: 79 Views: 1304

## \#1 Posted by: Keevaan Posted at: 2019-05-11T21:08:33.208Z Reads: 187

```
I have a dual drive trampa with Vesc6+ and aps 6384 170kv. I’m getting a motor temp fault while riding. Motor temps are spiking from 60c to 80c in a matter of seconds. Even with no load on the board with it on my workbench. Any suggestions?

Motor max 80A
Motor brake -65
Batt max 70
Batt then -70
```

---
## \#2 Posted by: Santino Posted at: 2019-05-11T23:19:21.477Z Reads: 175

```
I would try 60 motor amp, -35 motor break, 60 bat and -35 . If you break too much at -65 motor amp, I think it is too much stress for the stators dealing for such high amps... Actually I would try lower amps than 60... I would not follow the motor brand suggestions, I would start from 50 amps and change the values until you reach the spot for a balanced ride. What Batts are you using?
```

---
## \#3 Posted by: Keevaan Posted at: 2019-05-11T23:44:53.076Z Reads: 169

```
12s5p Li ion. Board worked fine before the upgrade. Before it had Vesc6 and 6384 200kv at 80A. I’m not sure why these motors are getting so hot. What’s “normal” temperature for a motor like this?
```

---
## \#4 Posted by: Santino Posted at: 2019-05-13T04:06:43.266Z Reads: 155

```
When I use 130kv motors, I run them at lower amps, they are efficient and they get the stator saturated if you manage the amps that you would use with a 200kv motor. Also, if you full charge your batteries and then you go riding and breaking a lot, or just downhill with a full charge, all that energy has to go some where, creates heat, and your battery is saturated, therefore your motors will work as dissipators, and you will hit the red zone very fast...you could set up the limit at 100 C grades, but I would rather set it at 80 C, because magnets suffers a lot at continuous high temps....I suggest you to try lower amps 45 motor amp -25 break, and 45 batt and amps to start, obviously carefully because you are experimenting, and you will reach the perfect spot with patience. Wish you the best...
```

---
## \#5 Posted by: Keevaan Posted at: 2019-05-16T23:01:14.988Z Reads: 137

```
I tried lowering the settings today, it longer but eventually reached the thermal limit again.  Ive noticed the temperature jumps around alot at the higher temperatures (60C and above).  also when temperatures are 80C i can still touch the motors with my hand for a short time.  Wouldnt 80C give me an instant burn?
```

---
## \#6 Posted by: Santino Posted at: 2019-05-16T23:20:12.920Z Reads: 125

```
By touching the motor by hand, you mean the bell? I touch the lateral (sprocket and shaft) if that burn my hand immediately , there temps are too high. But the bell it is always dissipation heat, therefore they are not too accurate. Few questions, do you have belts? if they are ti tight motors heat up rapidly. Do you have motor cover? same problem, they need air. Do you loose power when motor heat up? thats the proof vescs are saving them from burning. How is the weather? Too hot will heat motor fast. How is your riding style? accelerating and a lot of breaking aggressively will heat your motors. Also, 80 C do not burn my fingers instantly. If there is no answer, best try to talk with Bruno from APS, maybe he can help you, also Frank from Trampa. PM them or email.
```

---
## \#7 Posted by: Sn4pz Posted at: 2019-05-17T02:14:31.627Z Reads: 121

```
[quote="Santino, post:6, topic:93512"]
also Frank from Trampa
[/quote]


I would try Frank first. Ive been told there havnt been many, if any, VESC 6s that go bad overtime.

Thats not to pin blame on you though, it sounds as though its the motor, and something within it thats wonky.
```

---
## \#8 Posted by: Keevaan Posted at: 2019-05-17T12:50:10.247Z Reads: 113

```
Hi, 
I really appreciate the helpful comments, I have an etoxx gear drive, so no belts. I have been in contact with APS, on my previous setup I had Vesc 6 and APS 6384s 200kv. I blew a Vesc 6 up last month and ordered two new Vesc 6+ along with two APS 6384s 170kv motors. The new 170kv motors have a completely closed bell while my old ones had a vented bell. I thought this might be a factor but APS assures me that the enclosed bell should be okay.  I am losing power when the motors get hot, Vesc’s are throwing a motor temp fault.  The weather here is mild for now(Arizona) it’s a high of about 80-85F here currently.  My riding style isn’t super aggressive but I definitely enjoy accelerating hard out of some corners🤘.  APS said it was likely due to my geartrain (which I don’t think because it ran fine before) or timing(which I assume means Vesc settings?) I have also emailed trampa, awaiting a reply.

I am currently using the same motor min and max as well as batt min and max that I used on my 200kv that ran flawlessly never overheating for the past year. Even when it was 110F+ outside.  Also my friend has the exact same setup running the 170kv motors only difference is he is using focbox.

It just doesn’t make just sense to me, it takes about a mile or two to reach the temp limit then severely cuts power to protect motors.
```

---
## \#9 Posted by: taz Posted at: 2019-05-17T14:13:39.848Z Reads: 102

```
What is your firmware version?
Also during motor detection what is the reported motor resistance?
```

---
## \#10 Posted by: Keevaan Posted at: 2019-05-17T14:16:18.273Z Reads: 100

```
I believe 3.54 I’m not home at the moment but just updated the 6+’s when I got them
```

---
## \#11 Posted by: taz Posted at: 2019-05-17T14:20:18.056Z Reads: 102

```
As long as it is not 3.52 you are good.
Check the resistance values and let me know.
```

---
## \#12 Posted by: Keevaan Posted at: 2019-05-17T15:06:08.159Z Reads: 103

```
Motor resistance? 11.2 and 11.5
```

---
## \#13 Posted by: taz Posted at: 2019-05-17T15:18:53.458Z Reads: 100

```
Are you sure? 

11mΩ seems a little low.
```

---
## \#14 Posted by: Keevaan Posted at: 2019-05-17T15:32:56.650Z Reads: 103

```
![image|375x500](upload://hZAqIOZoTwx1hm6LG323qlnnZQh.jpeg)  firmware is 3.54
```

---
## \#15 Posted by: taz Posted at: 2019-05-17T15:46:10.316Z Reads: 100

```
I read your thread and I can't see something standing out.

Lower kv motors normally can't handle the current higher kv handle due to more turns in the winding.
However your motors have a lower resistance than all of my 6374 motors and I don't have major overheating problems with mine.

The only thing I can suggest, is to make sure you redo you motor detection, make sure temperature compensation is off and recheck all your motor phase connections.
```

---
## \#16 Posted by: Keevaan Posted at: 2019-05-17T15:52:51.236Z Reads: 98

```
Where can I find temp compensation?
```

---
## \#17 Posted by: taz Posted at: 2019-05-17T15:56:59.931Z Reads: 99

```
![20|690x388](upload://daSVfETpa5kKlMmf0uMKSymWiEx.png) 

Fw 3.52 had temperature compensation on by default during detection and it caused a few problems with some motors.
If you have FW 3.54, unless you activated it yourself, it should not be on.
```

---
## \#18 Posted by: Keevaan Posted at: 2019-05-17T15:59:16.674Z Reads: 95

```
Mine is on false but wouldn’t that not matter because I have hall sensors?
```

---
## \#19 Posted by: taz Posted at: 2019-05-17T16:01:46.541Z Reads: 93

```
No, although it is on the sensorless tab, it applies in all cases.
```

---
## \#20 Posted by: taz Posted at: 2019-05-17T16:04:17.936Z Reads: 99

```
What is the sensorless erpm you have set? (FOC, Hall sensors tab)
```

---
## \#21 Posted by: Keevaan Posted at: 2019-05-17T16:04:33.470Z Reads: 95

```
Interesting, do you use the simple or advanced foc setup? I’m used to the old Vesc tool so this is a little different. I
```

---
## \#22 Posted by: taz Posted at: 2019-05-17T16:05:31.254Z Reads: 90

```
I haven't used the full version of the vesc tool in a long time. I do all my settings with the mobile vesc tool.
```

---
## \#23 Posted by: Surfer Posted at: 2019-05-17T16:09:02.006Z Reads: 91

```
Did you setup the beta value of your motor In vesc tool?
```

---
## \#24 Posted by: Keevaan Posted at: 2019-05-17T16:09:54.210Z Reads: 90

```
I’m not sure what that is, sooooo no. Could you tell me how to?
```

---
## \#25 Posted by: Keevaan Posted at: 2019-05-17T16:10:43.899Z Reads: 90

```
Just reran detection, look normalish?![image|374x500](upload://5n04eEXIRg7oOqVjoxWIynUqO8q.jpeg)
```

---
## \#26 Posted by: taz Posted at: 2019-05-17T16:11:37.763Z Reads: 90

```
Looks good.
```

---
## \#27 Posted by: taz Posted at: 2019-05-17T16:14:10.272Z Reads: 89

```
Normally you should not have to mess with it. It is basically a way of calibrating your temperature sensor.

![15|690x388](upload://4GlDzFMqJhuRXHckCenOf8KAoBI.png)
```

---
## \#28 Posted by: Keevaan Posted at: 2019-05-17T16:18:49.985Z Reads: 85

```
![image|375x500](upload://xBmuwFuqe7Fu6A9Snlnd4xbh7mR.jpeg) looks the same except for fault stop time
```

---
## \#29 Posted by: taz Posted at: 2019-05-17T16:21:17.262Z Reads: 82

```
These are not my settings. They are they standard settings of the vesc tool.
```

---
## \#30 Posted by: Keevaan Posted at: 2019-05-17T16:30:18.361Z Reads: 82

```
So am I supposed to adjust the beta value?
```

---
## \#31 Posted by: taz Posted at: 2019-05-17T16:33:44.720Z Reads: 86

```
The beta value is a constant that depends on the characteristics of the thermistor used.

I don't know if motor manufacturers use various NTC thermistors with values that are different to the standard value in the vesc tool, but if that is the case, then this means that the temperature reported differs from the actual one.

You would only need to adjust this value if the vesc tool reports eg 80C when the actual temperature is 60C.

Considering that your motor temperature climbs from 60C to 80C very fast, I don't think this is your problem.
```

---
## \#33 Posted by: Keevaan Posted at: 2019-05-17T16:46:59.137Z Reads: 84

```
Okay, where is the proper place to take a temperature rating?
```

---
## \#34 Posted by: taz Posted at: 2019-05-17T16:53:28.393Z Reads: 80

```
Normally on the base of the motor. I still don't think this is your problem though. Do both motors overheat?
```

---
## \#35 Posted by: Keevaan Posted at: 2019-05-17T21:46:45.533Z Reads: 81

```
Yes, both of them reach thermal max.  It seems like a VESC setting issue to me?
```

---
## \#36 Posted by: Pedrodemio Posted at: 2019-05-17T21:56:05.252Z Reads: 85

```
You definitely need to adjust the beta factor, since the function is logarithmic a small error produces a big error in the temperature reading 

Measure resistance and temperature and resistance at two different temperatures and put them in the calculator bellow

The best way I’ve found with built in temperature sensor is to use a hair dryer and let it heating the motor for at least half and hour or more to stabilize, just be careful that some hair dryers will get things way too hot and damage the motor

https://www.ametherm.com/thermistor/ntc-thermistor-beta
```

---
## \#37 Posted by: Keevaan Posted at: 2019-05-17T22:12:17.014Z Reads: 77

```
So do I do one at “room temp” and then another after a half hour on hairdryer?
```

---
## \#38 Posted by: Keevaan Posted at: 2019-05-17T22:34:57.305Z Reads: 77

```
With that calculator I’m getting a beta value of -267.64 that doesn’t seem right
```

---
## \#39 Posted by: Pedrodemio Posted at: 2019-05-17T23:43:41.035Z Reads: 80

```
Exactly 

How are you measuring the motor temperature at both cases?
```

---
## \#40 Posted by: Keevaan Posted at: 2019-05-18T00:43:51.327Z Reads: 80

```
I’m using the rt data in the Vesc tool. Should I get a laser or probe to measure
```

---
## \#41 Posted by: Pedrodemio Posted at: 2019-05-18T01:03:28.895Z Reads: 81

```
It needs to be external, we are trying to calibrate the VESC tool temperature, do you can’t use it. I personally use a IR thermometer, just be careful to no use it anywhere shiny or the readings will be wrong
```

---
## \#42 Posted by: trampa Posted at: 2019-05-18T10:10:53.172Z Reads: 77

```
Ask the vendor about the specification of the thermistor. Is it a NTC ? What is the value?
```

---
## \#43 Posted by: Keevaan Posted at: 2019-06-05T11:45:23.104Z Reads: 73

```
Hi sorry for long reply time, waited for vendor reply. The thermistor is a NTC, the value is SMD0805-103J-3950H.
```

---
## \#44 Posted by: trampa Posted at: 2019-06-05T11:56:36.783Z Reads: 73

```
It seams to be a NTC 10K, which is what you want. If temp spikes up that fast something is funny somewhere. Question is: is the motor really getting war that fast, or is it a measurement issue.
sure the Thermistor is connected to temp and GND?
```

---
## \#45 Posted by: Surfer Posted at: 2019-06-05T12:23:45.067Z Reads: 73

```
Probably 3950 is the beta value of your thermistor, adjust it in vesc tool and try, normally the thermistor is placed on the stator, the hottest part, it will be very different to the temperature of the motor can.
```

---
## \#46 Posted by: Keevaan Posted at: 2019-06-07T23:24:10.249Z Reads: 73

```
The motor takes about 2 miles of riding to reach motor temp fault, a little longer if I ride it gently and little sooner if I ride it hard. It appears the thermistor is attached properly.
```

---
## \#47 Posted by: taz Posted at: 2019-06-08T06:45:44.670Z Reads: 71

```
@trampa
Frank, what is  the beta value of your 6364 and 6374 motors?
```

---
## \#48 Posted by: trampa Posted at: 2019-06-08T11:22:28.265Z Reads: 71

```
For our motors the standard setting is good.
```

---
## \#49 Posted by: Keevaan Posted at: 2019-06-09T21:51:13.457Z Reads: 65

```
The motor seems to be getting hotter then I remember my other ones getting. I feel like it’s a Vesc setting issue though rather then a motor or physical Vesc issue
```

---
## \#50 Posted by: trampa Posted at: 2019-06-11T08:05:46.122Z Reads: 66

```
Try BLDC and do a test.
```

---
## \#51 Posted by: Xenon Posted at: 2019-06-16T07:33:52.416Z Reads: 66

```
Any news? 
I got my 6384 170kv closed bell next week and now I'm worried about the temp problem.
```

---
## \#52 Posted by: Keevaan Posted at: 2019-06-19T12:11:23.153Z Reads: 61

```
I am out of state till August, so I am unable to test. I wouldn’t be worried seems like I’m the only one with this issue
```

---
## \#53 Posted by: Xenon Posted at: 2019-06-19T15:17:19.692Z Reads: 58

```
ok thx i am testing my motors tomorrow and do a litle logging with metr.pro
```

---
## \#54 Posted by: Keevaan Posted at: 2019-06-20T01:17:32.170Z Reads: 56

```
What Vesc are you going to be using? Please let me know your results, might help me
```

---
## \#55 Posted by: Xenon Posted at: 2019-06-21T20:18:57.159Z Reads: 55

```
i am use two vesc6+ and the last 2 days i ride this setup about 40km in mountain terrain at 24°C tempurture and the motors run good at ~45°C.
Here a quick logging under hard conditions  I have a 90 kg heavy mtb driver a steep mountain pulled up about 800 meters.

https://metr.at/r/f0dKY
```

---
## \#56 Posted by: Keevaan Posted at: 2019-06-22T00:46:59.401Z Reads: 50

```
Thanks for the info :) yeah something is not right with mine. I am getting above 90C motor temps riding easy for about a mile on flat pavement. Before I changed to Vesc6+ and 170kv motors everything was fine. I wonder if it is Vesc or motors. I’ll troubleshoot more when I’m back with my board
```

---
## \#57 Posted by: Xenon Posted at: 2019-06-23T15:06:57.659Z Reads: 48

```
Now I'm surprised I had yesterday sometimes a abs over current so I have both vesc delete and set up again  now the error is gone but the Motors now are hot as Keevaan´s up to 80 ° C in Bldc and in Foc so to the limit :-( and the vesc are gone hot too
```

---
## \#58 Posted by: Keevaan Posted at: 2019-06-23T15:27:58.428Z Reads: 47

```
Oh jeez so maybe it’s no just me 😢
```

---
## \#59 Posted by: Xenon Posted at: 2019-06-23T15:31:30.421Z Reads: 48

```
So it's definitely an vesc Setting thing but which one?
```

---
## \#60 Posted by: McErono Posted at: 2019-06-23T20:16:17.186Z Reads: 48

```
[quote="Surfer, post:45, topic:93512"]
Probably 3950 is the beta value of your thermistor, adjust it in vesc tool and try
[/quote]

Have you tried changing the beta value guys? As long as you can touch and hold the motor cans things should be ok.
```

---
## \#61 Posted by: Xenon Posted at: 2019-06-24T03:05:07.947Z Reads: 45

```
The thermistor Reading is correct. The Motors and the vescs are going warm/hot after 15min. Slow driving 20km/h without hills Motors 60-80C and vescs 50C.
```

---
## \#62 Posted by: Keevaan Posted at: 2019-06-24T12:15:14.747Z Reads: 43

```
Did you change any settings between when it worked fine and now? The same thing happened to mine. All was good for a few days then heat issues. Never changed anything
```

---
## \#63 Posted by: Xenon Posted at: 2019-06-24T12:57:55.523Z Reads: 42

```
I did a complete reset and check / change the motor wire too the right direction (without software invert.)
and than the normal Motor / input wizard setup.
```

---
## \#64 Posted by: Surfer Posted at: 2019-06-24T13:02:56.758Z Reads: 41

```
Yesterday I went for a quick ride and my hubs where getting hotter a lot quicker than usually, buy yeah here the summer is hitting hard lately, I hope is not same reason of your temp headaches :)
```

---
## \#65 Posted by: Keevaan Posted at: 2019-06-24T23:56:57.177Z Reads: 41

```
Are you also using Alien Power motors? 6384s? I don’t want to blame the sealed can but my old 200kv 6384s from APS never overheated. I wonder if they are starving for fresh air
```

---
## \#66 Posted by: Xenon Posted at: 2019-06-25T04:05:26.971Z Reads: 41

```
I dont think it is a air problem because the temp curve is to steep and before i Reset the vescs i Had No temp issue. Now the temp rise 10C per km at a 5-10 AMP Draw.
```

---
## \#67 Posted by: Keevaan Posted at: 2019-06-25T12:08:20.386Z Reads: 41

```
@trampa any ideas on what could be causing this issue? I’m away from my board but it sounds like we are having the same issue so xenon might be able to try some fixes.
```

---
## \#68 Posted by: trampa Posted at: 2019-06-25T12:39:51.173Z Reads: 41

```
@XENON needs to send me his settings via mail. frank at trampaboard dot com
I can look into this.
```

---
## \#69 Posted by: Xenon Posted at: 2019-06-25T13:02:31.152Z Reads: 42

```
@trampa Thanks for help i send you an mail :slightly_smiling_face:
```

---
## \#70 Posted by: Keevaan Posted at: 2019-07-08T19:16:24.042Z Reads: 41

```
Any solution??
```

---
## \#71 Posted by: Xenon Posted at: 2019-07-08T20:25:29.067Z Reads: 42

```
Maybe a hard solution :innocent: testing it the next days![IMG_20190701_184711|375x500](upload://ks7kgmphbCccI1fuj4fkUSes81Y.jpeg) ![IMG_20190701_184726|375x500](upload://Ahgr8hYwfnxMZcESsjEhN4V6ua7.jpeg) ![IMG_20190701_194316|375x500](upload://4Z4JYyckqHKV4IHG4S3IK4c4A6Y.jpeg) ![IMG_20190701_204148|375x500](upload://iD4LexQE7AaHHWm7zBJVuLopwAo.jpeg) 

and i find some one on youtube it has the same motors i ask him in the comments he say: Try vesctool v.1.09 .

here are the video:

https://www.youtube.com/watch?v=HssSMae3k8I
```

---
## \#72 Posted by: Keevaan Posted at: 2019-07-09T00:16:57.244Z Reads: 39

```
Dang was really hoping it wouldn’t come to that...... ![image|230x500](upload://A44tOOYOJauP1m2EK35w2iTWis5.jpeg)

I think I have two of the old style “vented” cans laying around that I can try to switch over when I’m back with the board
```

---
## \#73 Posted by: Keevaan Posted at: 2019-07-23T01:42:28.335Z Reads: 38

```
How did testing go?
```

---
## \#74 Posted by: Xenon Posted at: 2019-07-23T14:01:21.622Z Reads: 37

```
a little bit better ~60-65°C after 10km Ride.
```

---
## \#75 Posted by: Keevaan Posted at: 2019-07-24T01:08:04.182Z Reads: 35

```
Is it still throwing motor temp fault?
```

---
## \#76 Posted by: Xenon Posted at: 2019-07-24T04:07:58.909Z Reads: 33

```
No over temp faults. but if I drive today at 38C I'll definitely get an fault.
```

---
## \#77 Posted by: Keevaan Posted at: 2019-07-24T12:14:35.216Z Reads: 32

```
Hmmm so most of the problem seems to be the motor not getting enough airflow..... I’ll have to try them with the old style vented rotor. My 200kv 6384s motors never overheated even in 45C weather! But they had the old style “vented rotor”
```

---
## \#78 Posted by: Keevaan Posted at: 2019-09-19T22:40:32.948Z Reads: 29

```
So I am back with the board and still having motor temp faults. APS was very nice to me and sent over two of the vented style rotors just like my old 200kv motors. I am getting about 6 miles of regular riding in now before motors hit temp limit. Which is much better then the closed style rotor but something is still not right. Does anyone have any suggestions? 

12s5p li ion
Vesc 6+
APS 6384S 170kv with vented style rotor
Etoxx 1:5 gear drive

Motor max: 70a
Motor brake: -70a

Bat max: 60a
Bat regen: -60a
```

---
## \#79 Posted by: sayekim Posted at: 2019-09-23T14:35:19.941Z Reads: 26

```
My sealed maytech 170kv motors hit soft cut off temp of 85C within 9km. 

https://metr.at/r/rh2V7

Seems pretty normal to me. 

![image|281x499](upload://iuH2VWpGcu4TZCUOTrOEUox4vqg.jpeg)
```

---
## \#80 Posted by: Keevaan Posted at: 2019-09-23T18:46:13.157Z Reads: 25

```
I never had this issue till I rebuilt my board with new motors and VESC’s.  I cannot find the issue and was hoping someone here might be able to help
```

---
