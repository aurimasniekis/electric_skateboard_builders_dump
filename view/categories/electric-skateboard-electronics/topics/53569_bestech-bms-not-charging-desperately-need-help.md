# Bestech BMS not charging! Desperately need help

### Replies: 13 Views: 669

## \#1 Posted by: sterlinggray4 Posted at: 2018-04-26T14:30:46.593Z Reads: 97

```
Okay I have already been talking about my issue on a pre-existing thread but I haven't gotten any responses and am feeling pretty desperate.

Here's my situation: I have assembled a 10s5p Board using LG-HG2, a Bestech BMS w/ E-switch rated to 80A and a 42v 5A xlr style charger. I didn't spot weld them together but instead made custom battery sleds which have been working great. I soldered everything together using the diagram from Bestech and a combination of information that I have learned from this forum. I have checked all the voltages from the balance leads as well as from the charger and everything seems to be in order. I even replaced my first BMS with the second one I got from Bestech and I'm still having the same issues. The only time I have ever gotten the board to charge is when I unplug/plug in the balance connector which allows the charger to begin charging for 10 seconds before stopping again. 

If anyone has any thoughts that would be WONDERFUL as I am extremely frustrated seeing my board run, but only when it is plugged in.

Here's some pictures of what I've done so far:

![IMG_1706|690x459](upload://8V53xpVGNGb1NaLfBinBLCB9gsB.JPG)
![IMG_1703|690x459](upload://uzAWlxN4hymLQgwth30YmGQ5DXQ.JPG)
![IMG_1705|690x459](upload://dLCSm8jaHOUk6Icw2Y37ovSCwSS.JPG)
![D528V1LI10S80A-02  BesTech Power datasheet|353x500](upload://25kTecmLCdGXSKuhSAjEx7GEJsw.png)
![D528V1LI10S80A-02  BesTech Power datasheet 1|353x500](upload://jJY5rt6BtUVi8uln1fzJvRVM8SH.png)
```

---
## \#2 Posted by: RedEagle Posted at: 2018-04-26T16:30:57.725Z Reads: 74

```
Try bypassing the bms i.e. wire it for charge only. See if it makes a difference.
```

---
## \#3 Posted by: dg798 Posted at: 2018-04-26T17:08:38.933Z Reads: 74

```
Is the pack already fully charged. The BMS won’t allow it to charge more than 4.2v per cell.
Check the cells and make sure they are all around the same voltage and then check the pack in total and see what u get.
```

---
## \#4 Posted by: sterlinggray4 Posted at: 2018-04-26T18:46:56.881Z Reads: 70

```
The pack is currently registering 35.79V and each cell is at 3.572

Oh that's an idea @RedEagle
```

---
## \#5 Posted by: sterlinggray4 Posted at: 2018-04-30T18:33:43.893Z Reads: 60

```
I now believe that my BMS is only charging at the 50mA balance current and not accepting the full 5A charge from the charger as the pack now reads 36V in total and each cell has increased as well. I believe that this means that my BMS is not broken as I was afraid of so again if anyone has any ideas on what I can do that would be super helpful!
```

---
## \#6 Posted by: SORRENTINO Posted at: 2018-04-30T18:42:29.641Z Reads: 60

```
The e-switch is on when you are charging correct?
```

---
## \#7 Posted by: sterlinggray4 Posted at: 2018-04-30T19:26:35.039Z Reads: 59

```
Yes and I have tried the reset method described by @Namasaki
```

---
## \#10 Posted by: sterlinggray4 Posted at: 2018-05-01T14:54:32.979Z Reads: 47

```
HAHA @SORRENTINO did I have it backwards or not?
```

---
## \#11 Posted by: SORRENTINO Posted at: 2018-05-01T15:08:19.780Z Reads: 46

```
No, I was completely wrong lol. You have it wired like the picture from bestech. There has to be something we are all missing. It is highly unlikely you received 2 defective BMS's.
```

---
## \#12 Posted by: SORRENTINO Posted at: 2018-05-01T15:11:23.280Z Reads: 46

```
The e-switch works correct? Just want to double check that. That seems to be the main issue with these bms's
```

---
## \#13 Posted by: SORRENTINO Posted at: 2018-05-01T15:14:35.630Z Reads: 44

```
Have you checked to make sure non of your "p's" are over 4.2v? Have you checked voltage of each balance wire to double verify?
```

---
## \#14 Posted by: SORRENTINO Posted at: 2018-05-01T15:23:08.035Z Reads: 44

```
How are your sleds connected in series?
```

---
## \#15 Posted by: sterlinggray4 Posted at: 2018-05-02T14:23:33.299Z Reads: 41

```
Yes all of the Balance leads and sleds are all registering the correct voltages. The sleds are connected by 30A fuse wires. I believe that my e-switch works, I've checked the voltage across the wires when they're disconnected and run it is series with a multi meter to check what Amps it's pulling when it's switched on.
```

---
