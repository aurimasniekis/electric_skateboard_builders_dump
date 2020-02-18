# Calling electronics experts to confirm something

### Replies: 14 Views: 268

## \#1 Posted by: 12meterkuk Posted at: 2018-09-08T19:00:29.240Z Reads: 117

```
Does this pcb look like it’s based on the vesc project?![image|281x500](upload://1zWAL3BE6uFOoxIY3DweRwYpbux.jpg)

I have a feeling it is
```

---
## \#2 Posted by: AlexBE Posted at: 2018-09-08T23:28:03.143Z Reads: 92

```
It's very difficult to tell. There are only so many ways to design an ESC for a BLDC motor. Any idea which microcontroller they put on the assembled board?
```

---
## \#3 Posted by: TowerCrisis Posted at: 2018-09-08T23:35:57.981Z Reads: 91

```
![Capturedrv|690x462](upload://mO9ct8xH0HYS2l4BpIUPfFbZ2If.PNG)

Hard to tell and nothing will be conclusive until the full pcb is visible.

But these pad layouts look like a DRV style pinout and MCU of the VESC
```

---
## \#4 Posted by: 12meterkuk Posted at: 2018-09-08T23:38:14.345Z Reads: 88

```
So if they end up being based on the vesc the company would be required to publish the changes? @Kug3lis @b264
```

---
## \#5 Posted by: AlexBE Posted at: 2018-09-08T23:40:44.918Z Reads: 85

```
I would go further and say it's actually impossible to tell which micro it is from the footprint alone. Using a DRV also makes complete sense, it was chosen for the VESC for good reasons. How much they might have copied from the VESC project will be shown in things like pinout and code (if they used the same micro).
```

---
## \#6 Posted by: TowerCrisis Posted at: 2018-09-08T23:41:15.266Z Reads: 84

```
It also appears that there are 4 current shunt resistors total (2 per motor) so if it is it's definitely 4.12 hardware based (if it is vesc based).
```

---
## \#7 Posted by: TowerCrisis Posted at: 2018-09-08T23:43:43.715Z Reads: 80

```
I agree, it is impossible to tell from the layout alone. I'm simply pointing out similarities. So far it looks like there isn't anything in the PCB that rules out any vesc derivativety. But it has been nailed down to 4.12 if it is.
```

---
## \#8 Posted by: AlexBE Posted at: 2018-09-08T23:47:26.582Z Reads: 78

```
Ahh yes absolutely. Agreed that nothing on the board shows that they are trying something different.
```

---
## \#9 Posted by: Kug3lis Posted at: 2018-09-09T02:08:14.815Z Reads: 68

```
Guys guys, why you attack instantly without even knowing what is going on :D Yes it is based on VESC and with many improvements for the schematics which will be published back when it will be released ;)

P.S. It can be any other esc, DRV is just gate driver it doesn't have anything much to do with VESC itself apart used in it ;) My ESC will also have some models with DRV based so, but its not VESC :)

I think @captainjez can explain a bit more in the detail but don't expect Enertion level ssss happening with them. (Stil waiting for a month ago promised published code and schematic within a week for Unity)  :D
```

---
## \#10 Posted by: AlexBE Posted at: 2018-09-09T02:25:56.535Z Reads: 65

```
Who is attacking? The post text is "Does this PCB look like it's based on the VESC project?"

Nobody is attacking anything, why do you assume people are attacking things when they aren't?
```

---
## \#11 Posted by: Kug3lis Posted at: 2018-09-09T02:41:57.250Z Reads: 60

```
Nah I read the topic because I was tagged here and from my side it looked like it looks like for everyone it looks like vesc but no one mentioned anything about it :) I didn't meant bad way :)
```

---
## \#12 Posted by: captainjez Posted at: 2018-09-09T02:46:55.408Z Reads: 54

```
Absolutely it is and we have stated this publicly many times. Files will be released for the changes made once we release our product.
```

---
## \#13 Posted by: Kug3lis Posted at: 2018-09-09T02:58:38.793Z Reads: 51

```
Also its a bit related to topic authors previous messages regarding Jed board ;)

https://www.reddit.com/r/ElectricSkateboarding/comments/7f4ung/the_truth_about_jed_boards/
```

---
## \#14 Posted by: Jc06505n Posted at: 2018-09-09T03:35:06.520Z Reads: 41

```
Also related 

https://www.reddit.com/r/ElectricSkateboarding/comments/7fc819/a_response_from_jed_boards/?st=JLUB1QDJ&sh=370d6557
```

---
