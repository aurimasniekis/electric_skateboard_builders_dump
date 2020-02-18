# Motor stutters, please help

### Replies: 24 Views: 581

## \#1 Posted by: Jake2k17 Posted at: 2018-08-07T22:53:18.906Z Reads: 156

```
So I just connected my 2x 5s lipos to a bms, charged up my board, and went for a ride. The minute I left my drive way and accelerated, the motor started to stutter, and it threw me off the board, giving me some pretty bad road rash. Like I said, I installed a new enclosure and bms, but the bms is only wired for charge, and I don’t touch the Vesc or motor phase wires at all. If anybody could shed some light on this topic that would be great. Thanks.
```

---
## \#2 Posted by: threebysix Posted at: 2018-08-08T01:04:20.628Z Reads: 149

```
screenshot of your vesc settings might help. Did you do a motor detection?
```

---
## \#3 Posted by: ElectricCoast Posted at: 2018-08-08T03:39:25.643Z Reads: 124

```
Check and see if one of your phases came lose on your motor.
```

---
## \#4 Posted by: Jake2k17 Posted at: 2018-08-09T20:04:53.358Z Reads: 106

```


![Screenshot%20(2)|690x388](upload://98EMJFUrpoa7TLApujyyCBRMxnX.png)

i also typed faults into the terminal but nothing came up, none of the phase wires are loose and I did a motor detection and nothing all seems well.

![Screenshot%20(3)|690x388](upload://8ivFvmoYECz9afFk4bIt4g4q6je.png)
```

---
## \#5 Posted by: mikedv Posted at: 2018-08-21T09:53:04.443Z Reads: 89

```
Hello, i have the same issue on my new build . Did you manage to find a solution? For me the issue only occurs above 15-20kmh and only when the board is loaded, when pulling the trigger it stutters a lot. So much in fact that i cannot ride it properly.I have more or less the same vesc settings as you and use dual 190kv 6355 unsensored aps motors with  10s5p battery.I will soon test with another battery ,canbus cable and new sensored 6364 motors.
```

---
## \#6 Posted by: Brdchris Posted at: 2018-08-21T10:09:58.675Z Reads: 87

```
Hybrid sensored?
```

---
## \#7 Posted by: mikedv Posted at: 2018-08-21T11:36:40.462Z Reads: 80

```
The motors i currently (try to) use are unsensored. Both motors are stuttering , itried every possible vesc config but the issue persists .Will try sensored hybrid once i receive my order. They should arrive thursday or friday. I will post more infor regarding my vesc settings once i am back home.
```

---
## \#8 Posted by: Brdchris Posted at: 2018-08-21T11:59:42.046Z Reads: 77

```
Have you tried increasing motor and battery current? Mine seems smoother with higher settings. Maybe it’s in my head though
```

---
## \#9 Posted by: mikedv Posted at: 2018-08-21T12:25:58.200Z Reads: 73

```
yes i tried but will retry this evening.I resetted the vesc settings to the default settings but it remains the same. I am thinking that my battery is the problem. I'll post an update this evening. Damn it sucks , i waited months to gather all the parts and i still cannot ride it...You also have a similar issue with your board?
```

---
## \#10 Posted by: Brdchris Posted at: 2018-08-21T12:28:48.334Z Reads: 72

```
Not exactly. I run in foc and it would stutter if I ran sensored at startup until I increased current now it’s buttery smooth. I think I was hitting motor current limit when my board tried to get my heavy self moving. But I’m no expert
```

---
## \#11 Posted by: Jake2k17 Posted at: 2018-08-21T13:36:35.451Z Reads: 62

```
hi, I am still having this problem, the same problem as @mikedv. I will also try to increase the current limit.
```

---
## \#12 Posted by: mikedv Posted at: 2018-08-21T14:11:15.240Z Reads: 59

```
I tried with another spare 10s5p battery and i still have the same problem...
changed motor max and battery max to:
motor max 55a
motor min -55a
bat max : 40a
bat min: -12a
not sure if it is related to the vesc settings . My motors initially had 5mm banana connectors those were replaced by 4mm (soldered by a profesional as i have 2 left hands) . I am waiting for my new motors with 4mm connectors for a test. Will let you know the results once i've received them.
```

---
## \#13 Posted by: Jake2k17 Posted at: 2018-08-21T14:28:41.877Z Reads: 59

```
Yeah so I soldered my own connectors onto my motor, but I’ve been riding this board for months with no issue, and then I connected a charge only bms and now it stutters. That was when it started happening. I’m using two 5s lipos with a Vesc.
```

---
## \#14 Posted by: mikedv Posted at: 2018-08-21T20:55:47.413Z Reads: 50

```
did you try with only one motor and vesc connected? I did so and at first i only had the issue with one motor the other one was working fine. Later on i tried again and both motors were stuttering . Motor detection is ok , i used the bldc tool terminal and no faults were detected...The next things i will try --> test with new sensored motors , change canbus cable and/or connect both vescs with an y cable . But i really dunno what to try next if that doesn't solve the stuttering issue.
Man , i hope we'll find a solution soon. This shit is driving me crazy...
```

---
## \#15 Posted by: threebysix Posted at: 2018-08-21T21:06:50.393Z Reads: 46

```
Try lowering your battery cutoff values to like defualt 10 and 8, they seem too high and could be the reason your motor is clogging.
```

---
## \#16 Posted by: mikedv Posted at: 2018-08-21T21:43:42.669Z Reads: 44

```
Problem solved!!!!!!!!!!! i changed my battery start and cuttof settings but as i use li ion and not lipos i tested with following values 
start cutoff 30V
end cutoff 28V

This is thanks to @threebysix , when reading his post i remembered that i changed those values when configuring the vescs for the 1st time and never tried other values, until now :slight_smile:
@threebysix , you saved my life mate!
```

---
## \#17 Posted by: threebysix Posted at: 2018-08-21T21:58:56.744Z Reads: 40

```
Np my dude.
```

---
## \#18 Posted by: Jake2k17 Posted at: 2018-08-21T22:01:29.728Z Reads: 40

```
Will be trying this when I get home from school,  fingers crossed!
```

---
## \#19 Posted by: mikedv Posted at: 2018-08-21T22:05:29.944Z Reads: 39

```
Thanks again man , going for a nightride now :) , finally
```

---
## \#20 Posted by: mikedv Posted at: 2018-08-21T22:06:02.736Z Reads: 39

```
I really hope this will solve your problem too, keep us posted!
```

---
## \#21 Posted by: Jake2k17 Posted at: 2018-08-23T22:37:58.440Z Reads: 37

```
Hey guys....

I finally got the time today to try changing the voltage settings, and it didn’t work. I changed the start to 30v and the end to 28v like @mikedv what else could be wrong?
```

---
## \#22 Posted by: mikedv Posted at: 2018-08-24T20:23:00.124Z Reads: 36

```
hello man,the other day it worked for me for a few hours and the issue reappeared afterwards. I tried every possible vesc setting again and the problem came back again. About an hour ago i paired the remote again and disabled traction control on both vescs...i just came back from a night ride and everything works fine now .
So please try to : 
do a pairing of your remote again and if you use a maytech remote (i use a maytech mtsksr1712) make sure the leds are steady and not flashing. When flashing the board will not function correctly.
disable traction control on both vescs
DO NOT KEEP YOUR START AND AND CUTOFF SETTINGS LIKE MINE IF YOU USE LIPO!! 
I use Lio ion and the start and cuttof settings are totally different. Very important or you might damage your lipos. Check for the start and end cuttof for lipos, you should find it on the forum.

The cogging is gone for me , i am pretty sure it's all done now as i must have done about 4miles without any stuttering. 
I really hope this will solve your problem as i know what you are going thru and it drove me crazy.
Keep us posted and don't give up mate!
```

---
## \#23 Posted by: Jake2k17 Posted at: 2018-08-24T21:11:04.034Z Reads: 34

```
Hey bro, thanks so much for the response. Luckily, I decided to look for any loose connections, and I found one on my Vesc xt90. I re soldered the wire, and now everything works fine. You may want to try the same.
```

---
## \#24 Posted by: mikedv Posted at: 2018-08-25T21:43:29.970Z Reads: 33

```
I am glad it worked for you , my problem is solved too now. Didn't have much time to test the full potential of the board because of the weather here in Belgium but the torque and speed are exactly what i was looking for. Have fun with your build man! Grtz
```

---
