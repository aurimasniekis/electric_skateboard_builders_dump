# Dual VESC 6 over CAN Problem - Big RPM difference between master and slave

### Replies: 10 Views: 811

## \#1 Posted by: Pedrodemio Posted at: 2018-02-24T18:40:05.096Z Reads: 151

```
Well, i may have find a bug, because after two hours testing everything i could imagine I can't make this work properly

I'm in the final stages of setting up my new board, I've always limited ERPM to prevent killing myself, but I can't get it working on dual VESC 6 over CAN on FW 3.34

The problem is that if i apply a RPM limit the slave VESC spins less than half of the speed of the master. The current limits are not being reached, this is the cases I tried

* **ERPM limits on both VESC'S at +100K and -100K erpm traction control off**
everything works, both motors reach the top speed of about 43K erpm

* **Master VESC with a +20K and -20K, slave +100K and -100K traction control off**
Master works and reaches the set 20K erpm limit, slave rises to about 6K erpm and stays there. If I hold the master wheel the slave increases speed to full, i guess it shouldn't do that since traction control is off

* **Master VESC with a +20K and -20K, slave +20K and -20K traction control off**
Master works and reaches the set 20K erpm limit, slave rises to about 6K erpm and stays there. If I hold the master wheel the **slave increases speed to the 20K limit**

* **Traction control**
On or off doesn't change the behaviour

Thanks for any help

Master settings

![image|690x138](upload://v9LZrz28tmrqbhrnCRQfvnePlwA.png)

![image|690x42](upload://wEc9kZE8c11duSESwLcsOWmmTmZ.png)

![image|690x82](upload://djy4jBobioM03MFQTLi9IjOol9G.png)

![image|690x147](upload://nbxmNyStjbhQrONPAInIR7wG36V.png)

![image|690x91](upload://tiqPWG3jDywSxbTlx7KNMqdCbqK.png)

![image|690x115](upload://reKimQUohUQgItrBxKwIbnY4oMx.png)

RPM behavior

![image|690x314](upload://hNTBGbf177aotgrK3qjxyNxiAa6.png)
```

---
## \#2 Posted by: Pedrodemio Posted at: 2018-02-24T18:46:47.098Z Reads: 129

```
*  **Slave settings**

![image|690x137](upload://lr1iu2GbgoQ3h6Znli3vMI5BINt.png)

![image|690x42](upload://szQCovRMYLiHjGrCAEB9MGBAvK2.png)

![image|690x86](upload://bLzF2ei49400EoKRCXhCbNX0MPc.png)

![image|690x147](upload://tNVmE0EBKz6tUahAqp4Gszx2NrD.png)

![image|690x94](upload://3PSQEVkw9yZZMSD26SOFQz5TWyO.png)

**RPM behavior** 
at first both motors are spinning, the master it at its erpm limits of 20K, the slave stays at about 12k, if i let spinning for a while the speed continuously drops. When the speed peaks is because I stop the master wheels

![image|690x317](upload://9uMPsd9MFnWxrvI7HT4VOSDEdYM.png)
```

---
## \#3 Posted by: bevilacqua Posted at: 2018-02-24T19:57:13.054Z Reads: 114

```
does it happen also under load (riding)? 
Maybe you can flash them again... 

Im sorry if it sounds like: „did you try turning it on and off“ ;) 
Good luck!
```

---
## \#4 Posted by: Pedrodemio Posted at: 2018-02-24T20:18:44.436Z Reads: 114

```
Thanks, I’m a few minutes from riding if stops raining, my gear is that with this behavior one motor will be driving and the other regenerating all the time

If all fails I will try a clean install, but this is already a clean install since I’ve updated the firmware

EDIT:

Yeah, there is definitely something wrong, the slave motor has almost no power, this with the same current settings on both VESC's, I can stop it just touching my hand on the wheel

On the bright side, just rode it in my living room, FOC is amazing, way smoother than BLDC and dead quiet
```

---
## \#5 Posted by: Pedrodemio Posted at: 2018-02-24T23:38:22.850Z Reads: 92

```
I took it for a spin, apparently it is behaving ok since the consumption of master and slave is almost the same, for some reason with no load its engaging a speed loop that shouldn't be happening

Master

![image|324x122](upload://zEcC5TtzHqibBMfnsLyb65jWGc4.png)

Slave

![image|324x121](upload://iIgWEJ0ZrVmEKqcfSsu75co4a7J.png)

https://metr.at/r/OqmDE?zoom_start=0&zoom_end=1971
```

---
## \#6 Posted by: rpasichnyk Posted at: 2018-06-13T15:31:30.150Z Reads: 68

```
@Pedrodemio is this still an issue in FW3.38?
```

---
## \#7 Posted by: Deodand Posted at: 2018-06-13T15:49:36.370Z Reads: 64

```
This is a FW bug @Blasto and  I found but haven't documented yet. The bug is inside the ppm app. Essentially the ppm current command is generated via a percent of the maximum current. Problem is it is scaled with maximum current NOW and this value changes according to limit scaling as you approach hardware limits. So maybe for motor 1 0.6 amps is enough current to generate 20k rpm but motor 2 might need 0.75 amps because of slightly more friction in the motor etc. When riding it wont matter because under load two motors will need roughly the same current to generate same speed but without a load the bug shows up. Unless you use two very different motors on the same board it shouldn't really be a big concern and wont effect your ride too much, but probably should be addresses in the can fwding section of the ppm app to instead send proper current command through.
```

---
## \#8 Posted by: Deodand Posted at: 2018-06-13T15:53:54.092Z Reads: 61

```
Another time this might cause issues is if the master motor driver was overheating but the slave motor drivers temp was still managable. You will throttle the slave motor driver according to the overheating conditions in the master.
```

---
## \#9 Posted by: Pedrodemio Posted at: 2018-06-13T15:59:39.176Z Reads: 56

```
I’m still on 3.34, but what @Deodand says make sense
```

---
## \#10 Posted by: Deodand Posted at: 2018-06-13T16:00:04.862Z Reads: 55

```
https://github.com/vedderb/bldc/blob/master/applications/app_ppm.c

Interested persons see lines 204 and 304 in the above code.
```

---
