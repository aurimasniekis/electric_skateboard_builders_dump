# BLDC tool, Dual motor, what values should I input?

### Replies: 23 Views: 1194

## \#1 Posted by: Idobartal Posted at: 2017-10-14T00:51:26.345Z Reads: 148

```
Im building a dual motor setup and im wondering about the numbers i should input to the vesc via BLDC tool. - im talking about the first page on BLDC tool, the one with erpm and voltages (added the pic of the page im referring to)

Battery information:
10s4p 10A
Samsung r25 cells

2* Motors information:
Brand: L-Faster
Model: 6374
Voltage: 36V
Power: 3000W
RPM: 230KV ( RPM / V )
Max current: 150A
Shaft diamter: 10mm
​Weight: 0.8kg

Pls remember that im using 2 motors so if it changes something about the values pls tell me.
Also heard something about voltages shold be halved for dual setup?...

Any one dominating this page on BLDC tool ???
 i want to know what value on each parameter on the page.
pls help me out. (Don’t mind the numbers in the pic, its only so you know what page I’m talking about)

<img src="/uploads/db1493/original/3X/5/e/5effe3ee390f89cdc151675d8779f33b30ec6f6b.jpeg" width="375" height="500">
```

---
## \#2 Posted by: Namasaki Posted at: 2017-10-14T01:35:09.199Z Reads: 134

```
230kv at 10s is over 60k erpm  and there is a possibility that it could damage the vesc if you spin the wheels with no load.
So be careful.
Set the erpm limits to 60K and uncheck "limit by negative torque"
I'm Not sure what how much regen charging your battery can handle but I'm sure it can't handle -20a per vesc.
find out what your battery's max charge rate is and divide that by 2. the the Batt min setting. It will be a negative number.
set your battery cutoff start and end higher.  If your not discharging through a bms then you'll want to use conservative numbers like 34v start and 32v stop.
```

---
## \#3 Posted by: Idobartal Posted at: 2017-10-14T09:49:21.607Z Reads: 122

```
Hi bro, thanks for your help (on both threds !)
Pls can you elaborate on the divide part?
I already set the min and max erpm to -60k and 60k as you stated, and I !unchecked! the LIMIT ERPM WITH NEGATIVE TORQUE
I set the regen to -15.00A 

What avout motor max and battery max ?
And How do i find out the battery charge rate (its a 10s4p 10AH of samsung r25 cells, 36V, 360WH and it has an inner bms).

What should i write ? ? ?

Also:
-Can you explain the LIMIT ERPM WITH NEGATIVE TORQUE? What does it mean?
-im having problems with the ‘Over CAN’ control, is it ok to use a double wiring for the ppm and than not to configure CANBUS connection ? Is it safe ? I read that you loose the traction control option- whats that ? (and of cours i cant control both of them via one usb, but thats a minor inconvenience, i dont need to program the vescs after im done with the setup so i dont mind that, but i do want to know what are the pros and cons for Y cable for the ppm vs over canbus setup)

I know its a lot to ask but you’re making it sound simple so i got carried away with the QA
Thx 
Ido
```

---
## \#4 Posted by: Namasaki Posted at: 2017-10-14T13:31:32.890Z Reads: 104

```
I'm at work now, I'll get back to you when I get home
```

---
## \#5 Posted by: Namasaki Posted at: 2017-10-14T13:38:30.078Z Reads: 102

```
I'm on break and have time to answer one question. 
Limiting erpm with negative torque. 
I haven't actually tested this but the theory is that with this function enabled, the Vesc will apply brakes if you exceed the limit. 
This could cause a dangerous situation where you would be thrown off your board at high speed.
```

---
## \#6 Posted by: Idobartal Posted at: 2017-10-14T14:27:57.488Z Reads: 103

```
Thank you very much, im waiting patiently for the rest of you knowledge:)

Meanwhile i chose to use a Y cable for the ppm instead of ‘over can’ setting. I read some threads regarding to issues in the over can setup so i chose this method.
The only thing i saw that im loosing while driving is ‘traction control’, comments on this say it wont be missed..
Is it true ? Thx alot bro (pics are just for fun)

<img src="/uploads/db1493/original/3X/0/7/074cd40a44dcf207347b8f43f4f60b5321284405.jpeg" width="690" height="388"><img src="/uploads/db1493/original/3X/e/b/ebb9bc13e1f1f8a4ea7487944ee051834ac79721.jpeg" width="375" height="500">
```

---
## \#7 Posted by: Namasaki Posted at: 2017-10-14T15:34:00.515Z Reads: 96

```
I use Y ppm. Much more simple and safer than canbus. 
Important to clip the 5v wire from one of the Vescs. 
You can only send 5v to the receiver from one Vesc 
I don't miss traction control. 
I also run BLDC mode. 
Not as quite as as FOC but a lot safer and more speed.

Breaks over, back to work
```

---
## \#8 Posted by: Idobartal Posted at: 2017-10-14T19:37:49.126Z Reads: 96

```
Thx a lot !
I already clipped the 5v of one of them, the system works fine !
Do you have any suggestion about outputting 12 v from the vesc ? ? Does the vesc has this feature? 
Btw, i set the batt min to -7.50 on each vesc, making 15A regen, does it sound ok ? 

- on my last built with the same battery i set the bat min to -15.0 A so i figured i should half it on this dual set rught ?
```

---
## \#9 Posted by: Namasaki Posted at: 2017-10-14T23:09:48.349Z Reads: 93

```
I searched for charge specs on those batteries, what I found is standard charge 1.25a per cell and fast charge 4a per cell
Since you have 4p pack that would be max fast charge of 16a so -8a batt min per vesc.

As far as Batt max, it depends on your bms. Wether it has a fuse or if it is bypassed for discharge.
The battery pack itself should be able to handle 80a continuous. which would be 40a per vesc.

The motor max depends on your motors max amp ratings.
Some motors have max rating of 80a others only have max rating of 60a.
You can set each vesc to match the rating of each motor.
increasing motor max current increases torque giving better acceleration.
```

---
## \#10 Posted by: Idobartal Posted at: 2017-10-15T01:07:31.335Z Reads: 91

```
Thanks so much again for the explanation,
My regen is set to 7.50 each so 15A is probobly good (~16A)
And im not sure about my bms specs but i set the batt max to 30A each so according to your numbers im in the safe zone here too.
The motors though -according to specs (screen shot  attached)- are 150A max current each??!!wtf??
Im now set to -/60A motor max/min each so what am i missing on that ?

And now - HALL SENSOR, 
Both of my motors are the same exact model but i didnt buy them at the same time, the one I bought recently is an updated version - it arrived with hall sensor cable pre soldered to a tiny connector and with an adapter(cable) converting from the tiny plug to the VESC plug .
 The older motor came with hall sensor wires but they’re not soldered to a connector at all... and i dont know in which order to place them in the connector... 
So: 
I know hall sensor can upgrade the performance but is it something worth fighting for ? Because it means im gonna bomb you with another topic of hall sensor wire order :),
Or is it something i can let go calmly.  
  Thx bro
Ido
<img src="/uploads/db1493/original/3X/1/c/1c582dab799ad5ba7882d7ef977cc1850759b27a.jpg" width="281" height="500"> connection...
```

---
## \#11 Posted by: Nix Posted at: 2017-10-15T01:26:27.350Z Reads: 84

```
Why is there a possibility to damage the vesc if you spin the wheels with no load?
```

---
## \#12 Posted by: Namasaki Posted at: 2017-10-15T02:26:23.109Z Reads: 86

```
150a motor current does not sound right. Motors like this are usually rated for no more than 80a ea.

Running sensored is mostly so that you can stand on the board and start from a stand still.
Without sensored, you need to push the board manually to get it rolling and then hit the throttle.
I prefer pushing the board manually before giving throttle because I believe it is easier on the battery and motors and vescs.
So I dont run sensored.
I dont think it is worth the hassle and if the plug comes loose because of vibration while riding, It might cause an issue for the vesc.
```

---
## \#13 Posted by: Namasaki Posted at: 2017-10-15T02:30:15.596Z Reads: 85

```
[quote="Nix, post:11, topic:35484, full:true"]
Why is there a possibility to damage the vesc if you spin the wheels with no load?
[/quote]


If you run too high KV motor for your voltage and spin the motor with no load and no erpm limit, you could burn up the DRV chip on the vesc. 
I'm not even 100% sure that setting the erpm limit will avoid this. I haven't had a chance to actually test it with a high KV motor.
```

---
## \#14 Posted by: Nix Posted at: 2017-10-15T04:24:45.515Z Reads: 76

```
So spinning the wheel with no load runs the motor which runs up the erpm limit closer to the Max? Which could pass 60k?
```

---
## \#15 Posted by: Idobartal Posted at: 2017-10-15T08:04:24.368Z Reads: 78

```
Ok, no matter what the real max current of my motors, i set it to 60k/-60k 
About the hall sensor-  I'm glad that thats your opinion b/c I’d rather skip the wire fixing of the sensor and also to avoid any possible sensor issues in the future, 

-Also, my last built was a selsorless single motor 
And it managed to start driving without pushing with the leg for help (yes, i know that stresses the motor but with dual motor setup I assume it will start smoothly with or without the sensor connection...) right ?-

Just to be sure, my values FOR EACH VESC are set to:

MOTOR MAX: 60.00A
MOTOR MIN: -60.00A
BATT MAX: 30.00A
BATT MIN: -7.50A

MIN ERPM: -60000.00
MAX ERPM: 60000.00
MAX ERPM AT FULL BRAKE: 300.00
MAX ERPM WITHE FULL BRAKE in current control mode: 1500.00

MINIMUM INPUT VOLTAGE: 8.00 V
MAXIMUM INPUT VOLTAGE: 57.00 V
BATTERY CUTTOFF START: 33.00 V
BATTERY CUTOFF END: 30.00 V
*SLOW ABSOLUTE MAX is checked ✔️
*LIMIT erpm WITH NEGATIVE TORQUE is unchecked✖️

Is this ok bro ?


 And about 12v from the system,
 I want to connect tail and head lights but it supports only up to 12v
Do you know any simple method for this or i must add a some sort of PDB or a voltage limmiter ?
```

---
## \#16 Posted by: Namasaki Posted at: 2017-10-15T10:52:51.523Z Reads: 71

```
Because the Vesc delivers full voltage in current control mode, the wheels will spin up to full erpm when there is no load.
```

---
## \#17 Posted by: Namasaki Posted at: 2017-10-15T11:00:54.157Z Reads: 72

```
Your settings look good to me. 

About headlights, 
I don't have experience setting up lights. 
There are threads covering that. 
Just search for lights on this forum. 

Motors will usually cog when starting without sensors so pushing off is recommended
```

---
## \#18 Posted by: Idobartal Posted at: 2017-10-15T11:37:22.238Z Reads: 71

```
Thx so much for all the info, ill dig the forum for lights setup, thx!!!
```

---
## \#19 Posted by: Nix Posted at: 2017-10-15T13:30:21.187Z Reads: 68

```
Oh so they will spin up to there full erpm with no load? Does this mean without load there will be no sag which casues full voltage? And without load to you mean when it's upside down or what exactly do you mean? Thanks for helping me!
```

---
## \#20 Posted by: GrecoMan Posted at: 2017-10-15T13:54:04.002Z Reads: 66

```
[quote="Nix, post:19, topic:35484"]
without load
[/quote]

he means sitting on the bench or, yes, flipped upside down.
```

---
## \#21 Posted by: Acido Posted at: 2017-10-15T14:28:04.844Z Reads: 62

```
If you dont limit max erpm there is a possibility 

Fyi im not an expret im new with vescs
```

---
## \#22 Posted by: High-roller Posted at: 2017-10-15T15:46:29.774Z Reads: 59

```
Regarding the lights, you could try using a dc/dc step-down converter. Just make sure it has a decent sized heat-sink.
Since your setup is quite similar to mine I'm hoping someone can tell me what I need to change from your vesc settings.
My battery is a 10s5p- 36v, 12A.
Dual 6374s, 190kv.
Dual FOCboxes.
Everything else is about the same.
```

---
## \#23 Posted by: kptheinventor Posted at: 2017-10-15T22:31:28.603Z Reads: 57

```
What Vesc do you have?
```

---
