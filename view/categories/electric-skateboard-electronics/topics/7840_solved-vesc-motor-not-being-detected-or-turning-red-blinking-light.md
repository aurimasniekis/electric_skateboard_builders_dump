# \[SOLVED\] VESC motor not being detected or turning red blinking light

### Replies: 28 Views: 6174

## \#1 Posted by: Pyrax Posted at: 2016-08-18T16:19:46.589Z Reads: 433

```
After receiving my VESC I plugged it into my battery, connected my motor (enertion 6374) to the VESC, connected my receiver (from the enertion remote) to the VESC and turned on my battery. Lights on the VESC were turned on and I binded my remote to the receiver successfully. To test to see if the motor would spin I pushed forward on the remote however nothing happened. At this point in time I thought it was a problem with the remote so I connected the VESC to my computer to see if the VESC would work with the BLDC tool. My VESC came with the latest firmware 2.18. I was able to successfully connect to the vesc, read and write limit values to the VESC however when I tried to detect the motor the message "Detection failed is displayed". There is a pink flashing light on the VESC which im guessing is used to show errors. In the Terminal section of the BLDC tool no faults are displayed when faults are typed in. Is there anything I can do to fix or will I have to get a new VESC? Thanks for any help
```

---
## \#2 Posted by: ed713 Posted at: 2016-08-18T17:50:17.514Z Reads: 422

```
I'm not sure what you mean by the terminal section, but VESC error codes appear in the realtime data tab. Does the motor spin up at all when you run detection? If so, I would turn on realtime data, then run detection, and quickly switch over to the realtime data and see if any error comes up.
```

---
## \#3 Posted by: Lizardking0069 Posted at: 2016-08-18T17:58:07.192Z Reads: 412

```
Check the wires from the motor to the vesc are secure.
```

---
## \#4 Posted by: Pyrax Posted at: 2016-08-18T18:05:12.460Z Reads: 400

```
<img src="/uploads/db1493/original/2X/3/32d81accb44594b041d4b60760ed1e992b6e8e3a.png" width="690" height="403">
The bldc terminal I was talking about. The motor does not spin or move at all.
```

---
## \#5 Posted by: Blasto Posted at: 2016-08-18T18:07:12.625Z Reads: 385

```
type "faults"
```

---
## \#6 Posted by: Pyrax Posted at: 2016-08-18T18:09:37.254Z Reads: 383

```
When I enter that into the terminal the message "No faults registered since startup" is given
```

---
## \#7 Posted by: Blasto Posted at: 2016-08-18T18:13:12.110Z Reads: 377

```
take pictures of your setup
```

---
## \#8 Posted by: Pyrax Posted at: 2016-08-18T18:34:54.345Z Reads: 370

```
<img src="/uploads/db1493/original/2X/a/a23315ecb4e1900ad4c2eb5f9a59c2e693f2c725.JPG" width="375" height="500">
<img src="/uploads/db1493/original/2X/8/83587d7d4e5ab59d7e00568396a5f99a705b6ef2.JPG" width="375" height="500">
<img src="/uploads/db1493/original/2X/4/4ef61d8ca3772502dcf181d2efb23d6016ecd8ec.JPG" width="375" height="500">
<img src="/uploads/db1493/original/2X/3/357fe85d4a870c43abedd636fd1e4af4dc2f88f6.JPG" width="375" height="500">
I am running 2x6s 10,000Mah batteries in series, using a circuit breaker as an ON/OFF switch, connected to the VESC.
```

---
## \#9 Posted by: Lizardking0069 Posted at: 2016-08-18T18:37:17.708Z Reads: 343

```
That looks like it could easily short the motor phase wires.
```

---
## \#10 Posted by: Pyrax Posted at: 2016-08-18T18:40:53.066Z Reads: 341

```
Good point, I will add some heatshrink around the connections. Could this have potentially caused any issues?
```

---
## \#11 Posted by: Lizardking0069 Posted at: 2016-08-18T18:42:05.132Z Reads: 338

```
Shorting of the phase wires can blow the drv chip.
```

---
## \#12 Posted by: Pyrax Posted at: 2016-08-18T18:48:29.420Z Reads: 335

```
Is there anyway to tell if the chip is blown? From the exterior there seems to be no damage.
```

---
## \#13 Posted by: ikjahaa Posted at: 2016-08-18T18:50:06.856Z Reads: 332

```
the bldc tool should tell so.
```

---
## \#14 Posted by: ikjahaa Posted at: 2016-08-18T18:52:49.138Z Reads: 334

```
Does this say anything ?

<img src="/uploads/db1493/original/2X/2/26e3fc978184650da9bdd8fc040c81ffb6c12bb8.PNG" width="690" height="394">
```

---
## \#15 Posted by: Jinra Posted at: 2016-08-18T18:53:22.077Z Reads: 319

```
As @Lizardking0069 said, those phase wires are very close to shorting, make sure you insulate more. You can check for faults if you turn on active sampling under "real time data". 

Did you make sure you set your PPM settings and changed the control made to duty cycle/current/pid?
```

---
## \#16 Posted by: Pyrax Posted at: 2016-08-18T18:55:40.003Z Reads: 318

```
<img src="/uploads/db1493/original/2X/c/c9e7e3a2fd9e84aa79e018cd32a33e567e253283.png" width="690" height="406">Nothing shows for the fault code
```

---
## \#17 Posted by: ikjahaa Posted at: 2016-08-18T18:56:16.322Z Reads: 305

```
make sure you check "active sampling"
```

---
## \#18 Posted by: Pyrax Posted at: 2016-08-18T18:58:37.938Z Reads: 305

```
There is now a fault code saying OVER_VOLTAGE
```

---
## \#19 Posted by: Pyrax Posted at: 2016-08-18T19:01:01.665Z Reads: 299

```
I am not sure what the PPM settings are and I dont know where to change the controls to duty cycle/current/pid
```

---
## \#20 Posted by: Jinra Posted at: 2016-08-18T19:02:04.792Z Reads: 294

```
What's your max input voltage? you shouldn't change it from the default 57v
```

---
## \#21 Posted by: Pyrax Posted at: 2016-08-18T19:03:38.258Z Reads: 280

```
Its set at 44V, but when I press Red Default Configuration it says the default was 42V
```

---
## \#22 Posted by: Jinra Posted at: 2016-08-18T19:07:26.853Z Reads: 273

```
set it to 57 and leave it there. you can set ppm settings in "app config > ppm"
```

---
## \#23 Posted by: Pyrax Posted at: 2016-08-18T19:10:55.242Z Reads: 275

```
@Jinra    @Lizardking0069  @ikjahaa      Thank you very much for your help. The set up now works.
```

---
## \#24 Posted by: Pyrax Posted at: 2016-08-18T19:11:13.469Z Reads: 275

```
The error in the end was the voltage being set too low
```

---
## \#25 Posted by: Blasto Posted at: 2016-08-18T19:13:31.767Z Reads: 277

```
in the end, good thing you had the voltage set to low. It prevented the vesc from spinning the motor, if the motor would have spun and the phases were touching, no more vesc.

isolate those leads properly! :)

Edit the name of this thread and add a "Solved" to it, so people can use it for future reference
```

---
## \#26 Posted by: Jake2k17 Posted at: 2018-03-14T23:21:56.586Z Reads: 118

```
I have been trying to program my VESC for multiple days now, following all of the steps in I AM DELUXE'S vesc optimization video. At first I just soldered the motor wires to vesc, but the BLDC tool kept on saying bad detection result received. How can I fix this, because I have absolutely no idea how to fix this.
```

---
## \#27 Posted by: SkateYS Posted at: 2018-04-04T23:31:15.301Z Reads: 94

```
What motor are you using? Make sure the motor is OK, check the sensor wires connection. If all that s okay, read and write "default configuration" on all the tabs of BLDC tool, reboot VESC and retry. Also make sure you are using the right version of BLDC tool for that version of VESC.
 The same thing happened to me (I was using the Yuneec EGO motor with modified sensor wires) It kept saying bad detection results too. I figured out it was the motor after I tried a different one!
```

---
## \#28 Posted by: marco Posted at: 2019-12-10T23:59:19.665Z Reads: 7

```
hello, I  have a similar problem, I  bought two  new vesc with firmware 3.38. when I connected to my pc in BLDC tool, it showed a message saying that the firmware was too old. so I began to use VESC tool, I updated the firmware  to 3.62 and I was trying to connect the motors clicking in wizard >setup motors FOC, but when I clicked on run detection the light red in the vesc blinked 3 times and  appeared a window saying detection failed reason:-11 , so I went to the terminal and there appeared " fault: fault_code_drv", I tried this with and without the receiver conected to the vesc and it gives the same message, I don't know if this information is matter but I clarify that  when  I conect the receiver with my vesc it always remains blinking , I tried to push "bind" in the transmitter and turn on it and a red light  remained in the receiver and a green blinking light appeared in the transmitter however I tried again the whole process and it didn't work. so  I have not been able to use the motors, I am not a professional, this is the first time  I build a skate , I hope you can help me, thank you

I use two lipo bateries of 8Ah an 22.2 v, conected in serie
and two motors sk3  6374 of 149 kv
and one transmitter GT2B
```

---
