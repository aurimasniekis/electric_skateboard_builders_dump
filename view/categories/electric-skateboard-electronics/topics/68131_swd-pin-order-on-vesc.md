# SWD Pin Order on VESC

### Replies: 11 Views: 458

## \#1 Posted by: ElBandido Posted at: 2018-09-15T18:13:08.545Z Reads: 101

```
Hey all,

I was unfortunate enough to get a VESC without a bootloader, but after some research, I think I can flash it myself.  I'm pretty confident about the process, but there's one issue that I'm running into.  I've poured over all the threads and documentation I can find, but I can seem to find the **pin out information** so I can hook up my ST-Link correctly.  

Was wondering if any of you had that info on hand.

Much appreciated
```

---
## \#2 Posted by: rich Posted at: 2018-09-15T18:23:08.183Z Reads: 90

```
You don't need ST-Link anymore!
Go to Bootloader Tab in VESC-Tool and upload it, just choose the correct HW version. :sunglasses:
```

---
## \#3 Posted by: ElBandido Posted at: 2018-09-15T18:32:04.947Z Reads: 85

```
That's great news!  But unfortunately, I've tried that before with no success.

**Load Bootloader >> Update Firmware >>  Recconect**

And I always get this error message 

![image|502x135](upload://ilKgu6T6AtkCFdnnLcbxj36yubE.png)

Only the **blue** LED is on until I remove power from the VESC.

When I try again, I get this error message

![image|502x175](upload://6qLGhFZHBNXmi3YYwYWCN3Vt8Cd.png)


I'm at a loss  
🤷
```

---
## \#4 Posted by: ZmasteR Posted at: 2018-09-15T18:33:18.155Z Reads: 77

```
When you get the second one follow this

https://www.youtube.com/watch?v=v1glLDO-EjA&t=231s

or maybe I didn't get your problem correctly and this won't help
```

---
## \#5 Posted by: ElBandido Posted at: 2018-09-15T18:43:27.491Z Reads: 72

```
I'm trying to run a dual motor setup.  I got both my VESCs within the last month from TorqueBoards.  

The process that you suggested @ZmasteR worked seamlessly for one of my VESCs, but I can't get the 2nd VESC to take the firmware.  I thought that it might not have a bootloader, but I haven't had success using VESC tool to flash a bootloader to my problem VESC.
```

---
## \#6 Posted by: mmaner Posted at: 2018-09-15T21:12:29.356Z Reads: 62

```
If they are TB VESC's they have a bootloader. I've never known then not too. @torqueboards you wanna weigh in?
```

---
## \#7 Posted by: ElBandido Posted at: 2018-09-15T21:24:21.988Z Reads: 62

```
I know them to be super reputable.  Love their products, but I just can't seem to figure out the issue.
```

---
## \#8 Posted by: torqueboards Posted at: 2018-09-16T02:37:26.033Z Reads: 55

```
@ElBandido How many seconds do you wait before you reconnect after you update new firmware? I'd wait about 5-10 seconds. Usually, you're computer will make a sound and you'll be able to reconnect.
```

---
## \#9 Posted by: ElBandido Posted at: 2018-09-16T02:58:10.195Z Reads: 56

```
Thanks for the response @torqueboards

That worked great for one of the two VESCs that I have, but the other one hasn't been cooperating. 

If I'm not having any luck with Vesc tool, is it reasonable to think that if I reflash the bootloader with an ST-link, that I could get the update to the VESC?
```

---
## \#10 Posted by: torqueboards Posted at: 2018-09-16T21:38:31.565Z Reads: 47

```
@ElBandido Yeah, stlink would work. Email us and we can do it for you also. Just pay shipping.
```

---
## \#11 Posted by: ElBandido Posted at: 2018-09-17T05:07:18.259Z Reads: 32

```
I've had a hard time figuring out how the pin-out from the VESC correlates to the pins on the ST-link.  Other than that, the process seems pretty straightforward.  

Is there a data sheet you could point me to that I'm missing?
```

---
