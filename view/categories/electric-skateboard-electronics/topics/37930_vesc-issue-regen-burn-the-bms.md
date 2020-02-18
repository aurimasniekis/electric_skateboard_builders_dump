# VESC Issue Regen burn the BMS

### Replies: 6 Views: 667

## \#1 Posted by: shaohad Posted at: 2017-11-10T15:53:30.282Z Reads: 127

```
hi everyone.
i have this setup
Chinese vesc.
10S4P battery made with Samsung 30Q cells. runing with 50A BMS (bms have electronic switch to turn on and off the system)
6365 170kv motor

i manage to burn the bms multiple time, im not sure why, but i think its something with the regen breaking since the problems start after i break and mostly when i brake hard.
my BLDC tools settings are
like in the picture.
<img src="/uploads/db1493/original/3X/f/d/fdafa72dfdbd3f459a49eae715b9ed33153531fb.jpg" width="690" height="411">
so the question is there is anyway i can change any settings in the BLDC tool to stop that from happening?
what parameters in the BLDC tool should i change? (i don't want the breaking to be weaker, i don't mind do not get regen if its possible)

is there a good bms in those dimensions in good price you can recommend? (it must have electronic switch i do not wan't power switch)
needed size (no more) 65*65*25

thanks in advanced
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-11-10T18:17:32.117Z Reads: 103

```
Use the bms only for charging with the power supply. Exclude it from the ESC circuit.
```

---
## \#3 Posted by: shaohad Posted at: 2017-11-10T20:11:27.604Z Reads: 92

```
then i can't use the bms electronic switch so thats solution is not accept able
```

---
## \#4 Posted by: Namasaki Posted at: 2017-11-10T21:30:42.641Z Reads: 83

```
I use this bms. 80a continuous and it has built in E-switch. 
Never any problem with regen braking. 

http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
```

---
## \#5 Posted by: shaohad Posted at: 2017-11-11T07:33:06.791Z Reads: 67

```
yea its too big for me i wrote the size i have for it
```

---
## \#6 Posted by: Namasaki Posted at: 2017-11-11T16:13:30.479Z Reads: 55

```
Check the specs of your bms to see what the max charge current is and set your vesc's batt min current accordingly. 
I see you have it set at -20. 
If your running dual drive, that setting is too high for any bms. 
If your running single drive, it might still be too high for the bms your using.
You also should consider the max charge current of your battery.

The max charge current for 30Q is 4 amps
4a x 4p = 16a
Your total regen current or batt min current can not exceed -16a for the battery's sake. 
The max might be even lower on a compact bms with 50a discharge.
```

---
