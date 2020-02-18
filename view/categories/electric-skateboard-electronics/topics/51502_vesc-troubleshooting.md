# VESC Troubleshooting

### Replies: 20 Views: 979

## \#1 Posted by: danielz Posted at: 2018-04-07T18:08:21.265Z Reads: 116

```
I am trying to narrow down the cause of my broken vesc, version 4.10

I assumed it first stopped working after braking at slow speed after only being powered on for 1 minute. The motor just started twitching, and it refused to connect via usb, but it may have happened earlier and i hadn't noticed.

I put it away for fews weeks came back It did briefly connect via USB. Whilst watching real time data, I ran motor detection, the motor twitched and i briefly saw the word 'drv' in the fault section, the vesc then disconnected and will no longer connect via USB. Now when powered on i just have a single solid blue light.

Motor confirmed fine as it operates perfectly with my other vesc.
No visible damage
Power to transmitter is normal at 5v
Resistance between all motor wires on the good vesc is 82k. However, Resistance between red and yellow wires in bad vesc is 82k, but is only 36k between blue and the other two motor wires.
Resistance from negative battery input to red yellow motor wires is 35k but only  1omh to the blue motor wire.

Does anyone know any other tests i can do to pin down the cause, before i blindly attempt to replace the drv. 

Thank you.
```

---
## \#2 Posted by: Acido Posted at: 2018-04-07T19:09:01.693Z Reads: 95

```
Go to the terminal tab and type "faults"
```

---
## \#3 Posted by: Martinsp Posted at: 2018-04-07T19:34:05.873Z Reads: 88

```
[quote="Acido, post:2, topic:51502, full:true"]
Go to the terminal tab and type “faults”
[/quote]

I dont think he is able to connect to PC.

What you describe with the phase wire resistance is most probably (if I understand correctly) a blown FET or more of them. And if you saw that the DRV error was displayed in the real time data, that will need to be replaced too. check your motor very carefully because this scenario (blown FET and DRV) usually means that the phase wires were shorted, in some cases maybe the connectors touched and in others the insulation on motor wires got pierced most probably against the motor chassis. So it seems like you will need to replace/have replaced the DRV, FET (maybe multiple) and maybe gate resistor (maybe multiple) because those in many cases fail with mosfets.

Check your motor, not only resistance between wires but also measure the resistance against the chassis, put one probe of your meter somewhere on the motor where there is no anodization or other insulation (stickers etc) like the shaft or bearing for example and measure the resistance to all the wires while bending and moving the wires to simulate the motor moving as you steer your board. If you find that there is a short, you will have to work on your motor too or replace it, also check the wires visually. There also may be something inside the motor like a rock for example that damaged it and shorted the phase wires, not very probable since the motor works with other VESC but worth checking/cleaning
```

---
## \#4 Posted by: danielz Posted at: 2018-04-08T14:06:12.687Z Reads: 65

```
Thank you Martin, yep i think you are right regarding at least a blown fet. Im just looking at the schematics and the pcb layout on osh park to get a better understanding on how it works. Ill start with the motors i think, no point trying to fix it to blown them again when testing. Then ill turn my attention to the fets.

Thanks again, ill be back :D
```

---
## \#5 Posted by: RedEagle Posted at: 2018-04-08T17:25:29.376Z Reads: 66

```
You also most likely got a blown mcu.
```

---
## \#6 Posted by: danielz Posted at: 2018-04-08T20:21:39.247Z Reads: 59

```
Isn't much i haven't blown by the sounds of it lol. Just the one fet stuck closed. Desoldered it, its knackered, the two gate resistors seem fine though. 4.7 reads 5, 39k reads 38.77
https://youtu.be/5eEdimf2Uf4
```

---
## \#7 Posted by: danielz Posted at: 2018-04-09T13:16:16.788Z Reads: 46

```
5v is fine, 
3.3v is fine. 
which makes sense as i read its walled off from the rest of the drv.

usb resistors to MCU all fine. 
All USB pins have continuity. 

MCU must be damaged unless a firmware/bootloader can be corrupted? might as well get an st link first, will need one if switch mcu out anyway.
```

---
## \#8 Posted by: Martinsp Posted at: 2018-04-09T20:21:58.100Z Reads: 43

```
I doubt t is going to be a bad resistor or other passive component, I would suggest trying to use stlink and replace the fet and possibly drv too
```

---
## \#9 Posted by: danielz Posted at: 2018-04-10T17:03:34.926Z Reads: 38

```
Well i never, flashed the firmware included in bldc tool with an stlink clone and bam! Its alive, usb works again!!! Connected with vesc tool and updated to latest firmware. No faults showing at the moment. However i cant test anything until the fet arrives.
```

---
## \#10 Posted by: Martinsp Posted at: 2018-04-10T18:16:10.356Z Reads: 35

```
Sounds like you got lucky :D
```

---
## \#11 Posted by: danielz Posted at: 2018-04-10T20:08:15.286Z Reads: 34

```
Something will go wrong again, always does for me. Ill prob bbq the fet again.
```

---
## \#12 Posted by: danielz Posted at: 2018-04-18T20:41:23.492Z Reads: 32

```
Fets finally arrived. Amazingly it all works fine :smiley::smiley::smiley::smiley: Marvelous
```

---
## \#13 Posted by: Martinsp Posted at: 2018-04-18T20:42:54.082Z Reads: 32

```
Thats great news! :) 
Have you located the reason why it happened originally?
```

---
## \#14 Posted by: danielz Posted at: 2018-04-18T21:06:45.699Z Reads: 29

```
No idea unfortunately
```

---
## \#15 Posted by: Martinsp Posted at: 2018-04-18T21:09:04.637Z Reads: 28

```
hmmm, just wires touching maybe? like only partially heat shrinked connectors? 
As long as it does not happen again it should be good! :D
```

---
## \#16 Posted by: danielz Posted at: 2018-04-18T21:15:58.601Z Reads: 28

```
Thats the thing, i took all necessary precautions. Extra active cooling fans and heatsinks, extra low esr caps, very secure inside enclosure, all wires heatshrinked and the bullets. 

No idea how the fet failed or how that can corrupt formware/bootloader either. Maybe a stray bit of solder did it.

Long test ride tomorrow and im going to upgrade the ceramic caps to 100v versions soon. Ill try make these last, whilst i build some vesc 6s
```

---
## \#17 Posted by: Martinsp Posted at: 2018-04-18T21:23:42.921Z Reads: 25

```
Yeah, solder balls may have caused this. Or maybe just some conductive crap that may have shorted the gate of the mosfet which may have caused some weird behavior and blow the fet possibly. I think that the max voltage of the gate is 20V but I am not 100% sure. If it was one of the FETs on the side where the DRV and MCU is this is possible. If it is on the other it is not this scenario because the gate would be connected to ground which would not destroyed anything (tested this, unintentionally soldered gate and battery negative together and it just did not work, after removing the solder everything was fine)
```

---
## \#18 Posted by: danielz Posted at: 2018-04-18T22:42:49.560Z Reads: 23

```
Its the power side where the wires are soldered :laughing:
```

---
## \#19 Posted by: Martinsp Posted at: 2018-04-18T22:53:56.255Z Reads: 23

```
Aha, than it has to be some other cause :D Well... I guess we will just have to wait and see... BTW, have you cleaned the VESC after soldering the FET? With alcohol or other flux removing chemical. Useful mainly for removing solder balls and other potentially conductive crap to prevent further damage.
```

---
## \#20 Posted by: danielz Posted at: 2018-04-19T00:01:08.611Z Reads: 21

```
I will do, after im completely finished messing with it tonight :slight_smile:
```

---
