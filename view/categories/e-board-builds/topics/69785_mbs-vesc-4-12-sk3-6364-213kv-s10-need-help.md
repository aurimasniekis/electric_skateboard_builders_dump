# MBS &#124; VESC 4.12 &#124; SK3 6364 213KV &#124; s10 NEED HELP

### Replies: 25 Views: 517

## \#1 Posted by: Damian Posted at: 2018-10-01T21:51:08.007Z Reads: 132

```
Hi , first I would like to say hello to everyone. I need to ask you for help with my MBS setup.

I have already prototype of my skateboard.
Sk3 6364 213kv single 
2x s5 5800mah 30c lipo series
Vesc mayteh 4.12 
Drive chain with 68 to 12 teeth
200mm pneumatic wheel.

I know single motor is not good idea but for now I just want to try with single one, and after buy another motor and vesc.

Can someone help me with max current for motor and battery for that setup. 

Currently I have 60A for motor and 50A battery.
The only problem with is so far ( excluding power of course ) motor sometimes on flat road just turn off. But that was also happens before with my longboard with this same setup but on 70mm wheals and 36 to 12 tooth.

Once again my question is how to configure vesc for that setup.

Thanks Damian![20180929_182819|375x500](upload://1VeSKjZmXw5HfFPDp2c1MXnDGUE.jpeg) ![20180924_121126|375x500](upload://hECQmVM08oJWFEljXkLFa7hmljM.jpeg) ![20180925_205416|375x500](upload://qPZYAYkuTnB2iPLHxFrR9crLw9Q.jpeg)
```

---
## \#2 Posted by: pat.speed Posted at: 2018-10-01T22:05:03.229Z Reads: 111

```
So you have done motor detection and programmed the vesc already? When does this stoping happen? During braking, accelerating or just cruising. We need to know these things to help you.


Oh and I don’t mean to be rude but how stable is that motor mount? Having only 2 threaded rods supporting the whole thing might not be strong enough for off road use
```

---
## \#3 Posted by: Damian Posted at: 2018-10-02T06:37:35.682Z Reads: 105

```
You are not rude any suggestions are welcome.

I know two rods are not the best solution but this is only temporary. And I don't want to use board in off road for now , just only on normal flat road.

I did whole procedure with detection. This is happens during slow acceleration or even with 50% throttle and constant speed. 

I used this motor and batteries with my longboard and was exactly this same effect. My friend have similar setup and everything works fine. That's why I ask for help with vesc setup.

Can you tell me if I set 50A for battery and 60A for motor vesc cutt off power totally  when is going higher or just send lower power?

Thank you.
```

---
## \#4 Posted by: Andy87 Posted at: 2018-10-02T06:47:54.167Z Reads: 91

```
50a as bat max for a hw4.12 esc could be your problem.
if it happens only after 5-10min your vesc probably overheat and restrict your power.
that happens usually from 80degrees. 
if hit the 100degrees the esc completely stop working.
i had an overheating problem with single drive also once i had my bat amps set too high.

set your bat max to 35a and look if it still the case than.
```

---
## \#5 Posted by: Damian Posted at: 2018-10-02T07:30:46.024Z Reads: 93

```
Thanks for answer , I will try put down Battery to 35A and keep motor still on 60A? 

I'm not sure it is important but after this stops skateboard going properly straight away. It is happens on flat even when I climb it is fine. 

Andy87 what esc you use ??
```

---
## \#6 Posted by: Andy87 Posted at: 2018-10-02T07:47:54.818Z Reads: 88

```
yes motor max 60a is good.
the vesc with which the overheating happende was a esk.de vesc 4.12 with direct fets and heatsink.

if you don´t have a bluethooth modul to track your ride, you could also connect your pc to the vesc after it happened and look for faults.
just ride around your house till you get reproduced the fault, than don´t switch off the board, connect your pc and look if there some faults written in the vesc tool.
if you fast enoug, you could also check the temperature there.
if you have a bluetooth module just get it connected with any app for esk8 and check the faults and temp as soon as your board take away power.
```

---
## \#7 Posted by: Damian Posted at: 2018-10-02T08:10:25.999Z Reads: 82

```
I have bt module and I checked faults before , I had few faults but temperature was lower then 80deg. But always current was like 50.10A that's why I thought it could be a problem with low amp. But I will put lower Battery amp and I will track temperature on it. And we will see. 

What do you think my 10s 5800mah 30c will be enough for 2 vesc and two 6364 213kv motor ? I know range will be horrible but except that will be ok?
```

---
## \#8 Posted by: Andy87 Posted at: 2018-10-02T08:46:08.202Z Reads: 75

```
i get 7-12km with my 12s 5ah lipos.
i think you can expact someting the same with your 10s 5800mah.
the c rating th 30c is kinda low.
if i would be on your place i would just try it out and double check the voltage sag with your bluetooth module and the temperature of the lipos by termometer.
if the cells not getting too warm and the sag is not out off the world, i would say, go for it.
if you plan to go offroad a lot, than you probably will need to get some better packs.
```

---
## \#9 Posted by: Narnash Posted at: 2018-10-02T09:42:57.036Z Reads: 72

```
On my single drive board I had a similar cut out problem with 50A motor and 35A battery current.
For me it wasn't a sag of the battery or something like that, I had the drop outs caused by over Amp. limits on my motor even though it was cold (52°C motor temp).
Just quick ramp ups or quick deceleration caused to go beyond my 50A motor current resulting the VESC to cut the power.

I would suggest to try to up the motor max. amp. a bit (at least as long you can be sure your VESC and motor aren't overheating; sensor+VESC overtemp settings) and try again. 
The Amp ratings of electric motors (or electrical consumers in general basicly) aren't strict boundaries as long the cooling/temperature is appropriate. The rule of "thumb":smile: : for motors is: is if you can touch it should be below ~ 65°C which is perfectly safe for a motor, but actual sensors or IR thermometers are prefered). 

BTW please don't take this statement to violate the max. ratings of electrical component in general (like "air can pass, so it should be fine", or "A piece of aluminium on top and it's fine" :sweat_smile:) 
In my opinion  50A battery max. should be plenty but checking the sag doesn't hurt and undervoltage protection would cause a similar drop outs so it's worth a try.
```

---
## \#10 Posted by: Andy87 Posted at: 2018-10-02T10:01:41.123Z Reads: 71

```
50A very low for motor A settings.
Just don´t understand how it could happen with you.
My logic 
The vesc gives power to the motor, if you restrict your current to 50A, how it can exceed this value?
It´s because you gave full throttle and the vesc can´t regulate the amps so fast that it will be restricted to the values you set it? :thinking:
```

---
## \#11 Posted by: Narnash Posted at: 2018-10-02T10:09:20.926Z Reads: 69

```
I have actually no clue, but 70A from my first 50A nothing else changed on that single motor as max. and it's working fine I never had cut outs again.
I exceeded 50A only for a few seconds anyway, basicly full speed from the start up or an incline or full break. It was a 4.12 VESC from esk8.de, I think nothing updated, so it may be a software thing at least in my case.
But my point was that this could be an easy solution for Damian as long he doesn't run in temperature limits with the higher motor max. current.
```

---
## \#12 Posted by: Damian Posted at: 2018-10-02T15:11:34.137Z Reads: 58

```
Thank you all for help , I will try put 65A on motor and 35A battery and I will let know what's gonna happen. 

Thanks guys
```

---
## \#13 Posted by: Damian Posted at: 2018-10-04T18:18:01.784Z Reads: 61

```
Hi everyone. I just try set motor on 60A and battery 35A , and this didnt solve problem. 
Motor still sometimes just stop during slowly acceleration if speed is constant is fine. I cant go faster because motor just cut off. I checked temp and motor was not even warm.

This is faults list from VESC. Any suggestions very welcome.  

The following faults were registered since start:

Fault            : FAULT_CODE_DRV
Current          : 54.5
Current filtered : -0.7
Voltage          : 40.54
Duty             : 0.944
RPM              : 167.5
Tacho            : 325964
Cycles running   : 14760
TIM duty         : 4163
TIM val samp     : 2091
TIM current samp : 4296
TIM top          : 4411
Comm step        : 4
Temperature      : 40.32
 
Fault            : FAULT_CODE_DRV
Current          : 38.5
Current filtered : -5.7
Voltage          : 39.13
Duty             : 0.950
RPM              : 187.9
Tacho            : 1658936
Cycles running   : 20717
TIM duty         : 4181
TIM val samp     : 2091
TIM current samp : 4292
TIM top          : 4403
Comm step        : 4
Temperature      : 43.61
 
Fault            : FAULT_CODE_DRV
Current          : 31.8
Current filtered : -0.3
Voltage          : 37.71
Duty             : 0.949
RPM              : 183.1
Tacho            : 3275628
Cycles running   : 13439
TIM duty         : 4182
TIM val samp     : 2091
TIM current samp : 4295
TIM top          : 4408
Comm step        : 4
Temperature      : 43.58
 
Fault            : FAULT_CODE_DRV
Current          : 24.3
Current filtered : -0.6
Voltage          : 37.65
Duty             : 0.950
RPM              : 167.1
Tacho            : 3466180
Cycles running   : 9471
TIM duty         : 4182
TIM val samp     : 2091
TIM current samp : 4292
TIM top          : 4403
Comm step        : 4
Temperature      : 38.09
 
Fault            : FAULT_CODE_DRV
Current          : 28.5
Current filtered : -0.5
Voltage          : 37.23
Duty             : 0.950
RPM              : 199.2
Tacho            : 3951396
Cycles running   : 28243
TIM duty         : 4182
TIM val samp     : 2091
TIM current samp : 4292
TIM top          : 4403
Comm step        : 4
Temperature      : 43.74
 
Fault            : FAULT_CODE_DRV
Current          : 29.4
Current filtered : -0.5
Voltage          : 37.31
Duty             : 0.950
RPM              : 179.3
Tacho            : 3951702
Cycles running   : 88030
TIM duty         : 4182
TIM val samp     : 2091
TIM current samp : 4292
TIM top          : 4403
Comm step        : 4
Temperature      : 43.07
```

---
## \#14 Posted by: Damian Posted at: 2018-10-05T08:06:48.838Z Reads: 46

```
Hi mate , can you have a look on my vesc fault and tell me what do you think about it??
```

---
## \#15 Posted by: Andy87 Posted at: 2018-10-05T08:10:32.347Z Reads: 46

```
Looks like your DRV is fried and you need to replace it.
If you don´t have somebody close to you, you can have a look on @Martinsp website. He offer VESC repair service.
http://electricskateboard.repair/index.php?id_category=19&controller=category
```

---
## \#16 Posted by: Damian Posted at: 2018-10-05T11:37:24.920Z Reads: 49

```
Really ?? It was changed two weeks ago. But skateboard works. Just only cutt off power sometimes
```

---
## \#17 Posted by: Andy87 Posted at: 2018-10-05T11:54:37.442Z Reads: 51

```
the cut out comes from the DRV fault.
did you check that all components are fixed?
could be caused by a lose capacitor or so. 

you said you just got it repaired?
who repaired it, and what was broken before?
```

---
## \#18 Posted by: Martinsp Posted at: 2018-10-05T16:13:13.814Z Reads: 51

```
Hello,

the DRV faults in most cases mean that the DRV chip is damaged. However to make sure it is not something else please double check all of your connections. As I understand it, your board works but cuts out sometimes right? 

However, I found that in most cases when there is a connection issue that makes the VESC throw DRV faults it is at a fairly consistent amperage which seems not to be your case since you have 54A in first fault and below 35A in the others.

Thank you @Andy87 for mentioning me... again. :D :)
```

---
## \#19 Posted by: Damian Posted at: 2018-10-05T17:57:32.254Z Reads: 48

```
Thanks for feedback :). 

Drv was replaced for new because I damaged it on foc mode. The Problem is ,skateboard sometimes just during acceleration cutting off power. I fell off few times because it is like 100% brake. Engine is cold , and after 1 second works fine. If you ride with low constant speed it's fine. Yesterday during 2h motor stoped few times during acceleration. Through whole ride with low speed was fine.
```

---
## \#20 Posted by: mikedv Posted at: 2018-10-09T06:56:25.785Z Reads: 42

```
Hello, can you please reply to my mails and pm's ? I am getting a little worried because i've seent you my 2 focboxes and didn't get any feedback yet....The focboxes arrived yesterday morning by the way.
```

---
## \#21 Posted by: Martinsp Posted at: 2018-10-09T13:12:41.020Z Reads: 37

```
Hi, yes sorry I was not able to reply. Im on it.. :)
```

---
## \#22 Posted by: mikedv Posted at: 2018-10-09T13:37:02.452Z Reads: 35

```
No problem. Glad you replied.
```

---
## \#23 Posted by: Damian Posted at: 2018-10-13T10:55:08.690Z Reads: 34

```
Hello everyone ,

I just want to let know everyone I fixed my problem. I set Motor max to 65A and battery max to 35A.

I also change Motor min to -20 and Battery min to -10. After this nothing changed so I decided to flash my VESC to 2.54 Ackmaniac fw. After that I setup vesc 65A , 35A , -20 , -10 like above and there is no foults from vesc so far. 

Thanks anyone who gave me advises.
```

---
## \#24 Posted by: mynamesmatt Posted at: 2018-10-13T11:59:56.043Z Reads: 32

```
you may have been hitting your erpm limit. on 10s the Max you can hit is 204kv. did you have a limit on your erpm to 60k? it could have been blowing the drv
```

---
## \#25 Posted by: Damian Posted at: 2018-10-13T13:51:20.367Z Reads: 32

```
Before limit was 100.000. Right now I put 60.000.

I'm not to sure what solve my problem, but right now it's fine after reflash fw.
```

---
