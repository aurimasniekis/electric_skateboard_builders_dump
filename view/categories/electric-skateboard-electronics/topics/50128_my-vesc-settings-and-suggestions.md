# My VESC settings and suggestions

### Replies: 9 Views: 551

## \#1 Posted by: Holyman92 Posted at: 2018-03-25T23:53:25.197Z Reads: 114

```
@GrecoMan here is the caps of my current settings

![image|690x387](upload://dAL2nBjTbGMKVfbMwp57Tej38je.png)
![image|690x387](upload://eBp5HBU8pBsC312PkOUuejvGXa7.png)
![image|690x387](upload://bly7m2CxsA9qQRG29je9ITzi1pa.png)
![image|690x387](upload://bly7m2CxsA9qQRG29je9ITzi1pa.png)

what do i need to change? I have a 10s5p made with samsung 30q cells. I also need the brakes to be a little stronger because it takes me 1/2-1/4 of my street block to slow down to a stop NOT at full speed and i keep rolling through stop signs, i weight 215-220 lbs
```

---
## \#2 Posted by: Sender Posted at: 2018-03-26T00:17:32.242Z Reads: 96

```
*Up min battery to -15 to gain brakes(or higher up to -20). 

*You could up your battery max amps if you want  speed/torque increase (assuming you are dual I didnt look into what you are working with, sorry) to 50 amps each vesc as with that 10s5p pack you should be good to 100 amps (5 X 20['max' discharge of a single 30q).

*Limit Max ERMP to 60,000

*Uncheck limit ERMP on negative torque.


Dont listen to me though, wait til someone more experienced confirms this or sees other shit.  I am just trying to learn also by helping.
```

---
## \#3 Posted by: Holyman92 Posted at: 2018-03-26T00:19:05.011Z Reads: 90

```
im looking into ackmaniacs program right now... looks different, more gui
```

---
## \#4 Posted by: Holyman92 Posted at: 2018-03-26T02:20:20.138Z Reads: 75

```
@chaka @Ackmaniac

okay so im about to upload my settings using Ack's tool and i noticed what u said in another post about the ramp up @chaka and i changed that but mine isnt when i floor it from a dead stop (i dont do that as a general rule of thumb) but whats going on is when i am cruising i have to keep throttle at 50% on my remote otherwise it will start shuddering, not like the motor losing sync but more like someone turning the power on and off and it only happns when my pack hits 50% or lower... its unridable past 50% charge on a 10s5p pack with samsung 30q cells
```

---
## \#5 Posted by: Holyman92 Posted at: 2018-03-26T02:22:19.645Z Reads: 67

```
and another thing, it only happens when im on the board, if i lift the board off the ground or turn it upside downa nd ramp it up to full throttle it can sustain it no problems
```

---
## \#6 Posted by: Holyman92 Posted at: 2018-03-26T02:24:21.035Z Reads: 65

```
![image|690x387](upload://j7IY4X1AjTb10q5KLkBm1rEODmd.png)
![image|690x387](upload://ovcP5hLLFdVqGOcVPqobfhRBEkk.png)
![image|690x387](upload://tMcRqKQiPJLqJkEbCmGZxlt53ct.png)
![image|690x387](upload://na4xctyP1aebvLZzxP6gCMG3LeZ.png)
```

---
## \#7 Posted by: Holyman92 Posted at: 2018-03-26T02:24:55.422Z Reads: 56

```
@GrecoMan forgot to tag u in the post above... here are the settings in ack's tool
```

---
## \#8 Posted by: Holyman92 Posted at: 2018-03-26T02:44:23.486Z Reads: 57

```
ok so i strapped my laptop to the board (its a little netbook) and did the real time data (not sure f this helps) but this is the readout from when it drops and then tries to ramp up again and then i hit the brakes.

![image|690x387](upload://mE06kIxDzMweDI97GDqEFky1hA2.png)
![image|690x387](upload://sQP38hnuXkPQhmzGMavoztpYrRe.png)
![image|690x387](upload://2avhIFTMPX0NQrsFVeNgIyHOigS.png)

its in BLDC mode sensored since i have 4.12 hardware (not upgraded) and this only happens when i hit 50% or lower charge... from 100%-51% its fine and i can cruise full throttle no issues

oh and my setup is a single 6374 motor (until i buy a new motor or repair the one i dented... need a bar magnet for the can)
```

---
## \#9 Posted by: Ackmaniac Posted at: 2018-03-26T18:13:36.914Z Reads: 47

```
Best guess I have is that you have a Bms in the cycle with the vesc which shuts down when the voltage becomes too low.
```

---
