# Motor acting weird

### Replies: 12 Views: 188

## \#1 Posted by: legend27 Posted at: 2018-11-11T16:58:20.080Z Reads: 71

```
Hi :slight_smile:

My motor started acting weird after I taped the wires from the motor really close to each other. I have tested the motor before and had no problems. Also after I did the sensor setup. Does anybody have an idea of what's going on?

I got the 6355 motor from TB and vesc from them as well.

 https://youtu.be/OGnRX71E2kE
```

---
## \#2 Posted by: brenternet Posted at: 2018-11-11T17:13:51.240Z Reads: 65

```
Check that there's no exposed bits of the bullet connectors, they might be touching and shorting the motor. Beware this can kill your esc.
```

---
## \#3 Posted by: Andy87 Posted at: 2018-11-11T17:21:02.059Z Reads: 61

```
So motor detection is running through without issues right?
If you spin your motor by hand it’s like before free spinning or is there some resistance?
Like @brenternet said check also that there no exposed parts on your bullets touching each other.
Check your screws which hold the motor to the motor mount. If they too long you can short the phase wires inside the motor as well
```

---
## \#4 Posted by: torqueboards Posted at: 2018-11-11T17:59:59.457Z Reads: 52

```
Sounds like a VESC programming issue. Nice Bell :grinning: If you ride in BLDC you can just throttle hard and people move away. Downside for FOC/Sensored.
```

---
## \#5 Posted by: legend27 Posted at: 2018-11-11T18:06:39.136Z Reads: 49

```
@brenternet all bullet connectors are protected.

@Andy87 I can try to run the motor detection again, but I'm afraid if the motor will start smoking. Motor spins freely like before. Screws are 10mm so shouldn't be an issue.   

@torqueboards Do you think I can run the sensor setup again without the motor starts smoking?

![IMG_3572|666x500](upload://dBGbMlTK31LTfQvfyVK82neguca.jpeg) 

![IMG_3573|666x500](upload://uX8lfsD4XvAuJYyY8lrVnu4Ft51.jpeg)
```

---
## \#6 Posted by: torqueboards Posted at: 2018-11-11T18:16:48.215Z Reads: 43

```
@legend27 Run it on BLDC first and confirm everything is good. Have you ridden on BLDC first?
```

---
## \#7 Posted by: legend27 Posted at: 2018-11-11T18:18:09.596Z Reads: 42

```
It's been on BLDC the whole time. Will run the setup now and give an update after
```

---
## \#8 Posted by: legend27 Posted at: 2018-11-11T18:26:17.485Z Reads: 42

```
Update. Did the sensor detection without any problems. The motor rans as normal. BUT now it only beeps. 

https://youtu.be/AxzhB14FQkU
```

---
## \#9 Posted by: legend27 Posted at: 2018-11-11T18:32:29.920Z Reads: 40

```
@torqueboards

Got the problem fixed. All I did was run the sensor setup again, change sensor mode to "Sensored" and "write motor configuration" and "write app configuration".

Thanks for the help everyone! Didn't know what to do without this forum!
```

---
## \#10 Posted by: legend27 Posted at: 2018-11-11T19:12:50.003Z Reads: 35

```
Unplugged everything and back to the same issue. Connected everything again, ran sensor setup and it worked again. After you do the sensor detection you cannot unplug the sensor cable else you have to do the detection again. Is that normal @torqueboards ?
```

---
## \#11 Posted by: torqueboards Posted at: 2018-11-11T19:30:14.027Z Reads: 33

```
I'm not 100% sure.. maybe someone else who runs sensored more can let us know. But for myself anytime I change any motor settings on FOC Sensored. I always run it again.
```

---
## \#12 Posted by: ARetardedPillow Posted at: 2018-11-11T20:38:30.255Z Reads: 19

```
You need to do detection everytime after you change the orientation of the phase wires
```

---
