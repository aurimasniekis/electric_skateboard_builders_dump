# Hubmotor winding explanation

### Replies: 12 Views: 689

## \#1 Posted by: bevilacqua Posted at: 2018-01-20T19:28:25.437Z Reads: 102

```
Hi, I bought a cheap 72mm Hubmotor on Bangood or Gerarbest for something like 30$ inkl. shipping. 
After a successful motor recognition on FOC/Sensorless and completing the VESC Tool setup I got out to test it on the road. Everything was working fine till I hit the brakes for the first time. After hearing some weird noises the motor wouldn't spin un anymore. 

Today I've taken it apart to see what the reason for the motor failure could be . 

I've noticed that the motor wiring seems a bit odd for a normal BLDC motor (See the pictures below): 
Can someone with some BLDC-motor knowledge @Hummie @evoheyax help me figure out the problem?   
Thank you 

Regards, Mathias 

![IMG_1841|667x500](upload://imymLErJ0NAEtMQuMbZpiLLzKRK.jpg)![IMG_1838|374x500](upload://3ksWitmVacjA49WE8ZL4870pIAL.jpg)![IMG_1839|374x500](upload://4wOPwSD3msvKPpGR1qdGr98bZVQ.jpg)![IMG_1840|375x500](upload://4csxILazczIh7mTOFjNQ2WfmMLT.JPG)
```

---
## \#2 Posted by: Deckoz Posted at: 2018-01-20T20:35:09.252Z Reads: 81

```
The phase wires split to multiple poles is fine... As it's wye winding/termination.. would be off to see that on a delta winding/termination.. anyway

More then likely it's your vesc is dead..not the motor
```

---
## \#3 Posted by: bevilacqua Posted at: 2018-01-20T20:54:22.374Z Reads: 78

```
I can't see any visual damage on my VESC, but it seems like it... Thanks
```

---
## \#4 Posted by: Deckoz Posted at: 2018-01-20T21:06:18.998Z Reads: 75

```
When you push the throttle. What do the LEDs on the vesc do?
```

---
## \#5 Posted by: bevilacqua Posted at: 2018-01-20T21:19:30.302Z Reads: 68

```
After the incident I flashed the vesc and got stuck at the Motor recognition (FOC). Tomorrow I could try BLDC and see what happens. I'll report the results.
```

---
## \#6 Posted by: pat.speed Posted at: 2018-01-20T21:20:11.501Z Reads: 65

```
What Vesc are you using?
```

---
## \#7 Posted by: bevilacqua Posted at: 2018-01-20T21:21:53.532Z Reads: 61

```
Maytech HW 4.12 with C18 Mod, works fine on FOC after the modification (At least on my dual 5065 Setup)
```

---
## \#8 Posted by: pat.speed Posted at: 2018-01-20T21:28:49.393Z Reads: 61

```
If you can plug the Vesc into the Vesc tool and have a look if there are any fault codes
```

---
## \#9 Posted by: bevilacqua Posted at: 2018-01-20T21:45:04.989Z Reads: 55

```
how exactly? I’ve tried typing ‘faults’ on the Terminal tab. 

Nevermind, after flashing it it won’t have any logs left :(
```

---
## \#10 Posted by: GrecoMan Posted at: 2018-01-20T21:55:52.904Z Reads: 53

```
did you click send?
```

---
## \#11 Posted by: pat.speed Posted at: 2018-01-20T22:05:12.837Z Reads: 52

```
Try running the Vesc again if there is any faults it should happen again and then you will be able to use the terminal thing to find the fault codes. Idk if that will work but it makes sense that it would
```

---
## \#12 Posted by: Hummie Posted at: 2018-01-21T00:11:35.904Z Reads: 40

```
yea theres a wye bundle under the wrap and normal.  looks like you also have some of the wires broken.
```

---
