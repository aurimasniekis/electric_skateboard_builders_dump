# Fault LED (red) blinks on FOCBOX but

### Replies: 13 Views: 485

## \#1 Posted by: nordlicht Posted at: 2018-08-21T10:12:36.245Z Reads: 102

```
.. but when trying to read the fault code on the VESC tool under terminal -> print faults it just returns "no faults registered since startup".
You got clues?
```

---
## \#2 Posted by: DavidBanner Posted at: 2018-08-21T10:32:18.957Z Reads: 99

```
check your battery cutt off voltages
```

---
## \#3 Posted by: Martinsp Posted at: 2018-08-21T11:36:52.658Z Reads: 90

```
Post pictures of your settings. Also, how many times does it blink and does it stop or just blinks all the time?
```

---
## \#4 Posted by: nordlicht Posted at: 2018-08-21T11:37:44.708Z Reads: 84

```
3 blinks, pause, 3 blinks pause. I'll check battery voltage soon and give pictures
```

---
## \#5 Posted by: nordlicht Posted at: 2018-08-21T12:01:08.668Z Reads: 81

```
![current|690x487](upload://pLCyhaNq43C474Ej8jBCWzw70PZ.jpg)![advanced|690x487](upload://bMK8uauS04VxXgLdPVSybS5r0jv.jpg)![general|690x487](upload://hYCFm8SDWiMtmbYUUkNyRym4Gua.jpg)![voltage|690x487](upload://hgXjJkkdYakiJi9fMJ6mG2iS4Dv.jpg)![FOC|690x487](upload://69G2WdTG37ufahDsoXhYTgGsyGK.jpg)

Things is I never made it over the FOC config in the Wizard. I thought it's because of this fault code, but the values I'm getting are also really odd.
Current voltage is 49V, running 12S
```

---
## \#6 Posted by: Kug3lis Posted at: 2018-08-21T12:03:05.821Z Reads: 74

```
Open real time data panel it show error or etc I probably guess it's motor temp sensor or etc had same issues but it was related that older  focbox had wrong pinout label on the case... So fck motor sensor board...
```

---
## \#7 Posted by: nordlicht Posted at: 2018-08-21T12:08:17.811Z Reads: 77

```
![fault|690x487](upload://l8gECdaAJd57KaFSQlxNYsN63iW.jpg)
So it sais it has no fault. But the fault LED keeps blinking. What is happening?
Edit: NVM, why do I see no data?
```

---
## \#8 Posted by: Martinsp Posted at: 2018-08-21T12:11:30.452Z Reads: 74

```
You have to enable real time data on the right side of the window.
```

---
## \#9 Posted by: nordlicht Posted at: 2018-08-21T12:13:00.812Z Reads: 74

```
![drv|690x487](upload://1DS6HFrHF3P3LrTijEZ2espH7VQ.jpg)
Fuck. A broken DRV was the reason I switched from VESCs to FOC Boxes. My motors are Torque 130KV HUBs.
Chances are high my motor are somehow killing the controller right?
```

---
## \#10 Posted by: briman05 Posted at: 2018-08-21T12:46:38.213Z Reads: 71

```
Well you motor brake is very low and your battery regen is very high for li-ion.  I think I have my max duty cycle at 85% where your's is at 95%  I would say it has to do with the duty cycle because if you look just after 10 seconds they are off the charts you are probably throwing too many erpm's at it.
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2018-08-21T13:30:04.092Z Reads: 67

```
Disable you motor temps... the reading is completely wrong and could throw a false error.

![image|341x500](upload://kIoAAmCqBiy7QvETHyI8IwM9taI.jpeg)
```

---
## \#12 Posted by: nordlicht Posted at: 2018-08-22T11:42:18.369Z Reads: 55

```
Ok @JohnnyMeduse that sounds like a solid idea, but I dont know how to disable my motor temperature.
I tried:
* removing the cable (and he still reads the same value)
* realtime data -> Temperature -> untick "Motor", but he still reads the value (its flickering intense) for T Motor.

How to disable it?
```

---
## \#13 Posted by: nordlicht Posted at: 2018-08-23T07:30:21.974Z Reads: 47

```
Hey it might be that it sounds stupid, but I have no idea how to disable the motor temps.
Highly appreciate help here!
```

---
