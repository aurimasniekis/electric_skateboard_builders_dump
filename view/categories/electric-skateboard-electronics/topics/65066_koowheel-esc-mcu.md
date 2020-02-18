# Koowheel esc MCU

### Replies: 8 Views: 692

## \#1 Posted by: decebal Posted at: 2018-08-16T13:26:54.435Z Reads: 112

```
I've been inspecting this esc and I noticed that it's run by a GD32F103 MCU that's compatible with STM32 and also Arduino compatible.
Anyone tried to dump the contents? I see space for a 4 pin header. Could be VCC/GND/Rx/Tx.
Theoretically it could support  custom firmware. Same chip package, it is supposed to be a STM32 clone.
I'm not sure of the pinout but with some mods, would it theoretically be possible to upload VESC firmware?
```

---
## \#2 Posted by: careyer Posted at: 2018-08-16T20:42:15.119Z Reads: 96

```
Hi decebal, have you made any progress on this? I am also investigating if there is a chance to update that damn thing =) What koowheel are you driving? d3m?
```

---
## \#3 Posted by: decebal Posted at: 2018-08-17T03:12:05.552Z Reads: 80

```
Not yet, but I'm going to have to trace out stuff on the pcb and it will be a pain. Hope I find some time soon as it should theoretically be possible, depending if there's extra hardware on the VESC, functionally.
Yes, I have D3M. Tho rear side plate on one motor is missing some pieces :slight_smile:
```

---
## \#4 Posted by: careyer Posted at: 2018-08-17T07:54:44.750Z Reads: 60

```
Awesome! It would be fantastic if that controller could be hacked. Many people are riding these things (d3m) and while it is a nice performing board for the money especially the ESC part has some nasty characteristics, e.g: too steep acceleration/braking curve, sudden lack of power/amperage constraint at 50% battery, calibration on the 4 LED power indicator waaaay off... and so forth. 
It would be a blast being able to flash VESC firmware to it or at least alter some settings!
Keep up the good work man! =) BTW: Do you have the potted or unpotted version of the  PCB? lemme know if I can assist somehow.
```

---
## \#5 Posted by: decebal Posted at: 2018-08-17T16:33:01.427Z Reads: 54

```
One observation is the fact that there's one MCU controlling both motors, so for sure there's differences in the code. There's no way to just upload VESC firmware directly. I mean you could but it wouldn't work after reflash.
```

---
## \#6 Posted by: decebal Posted at: 2018-08-17T20:46:24.670Z Reads: 44

```
I managed to trace some stuff. I think there's more stuff for monitoring that I didn't find, and I also need to remove the MCU from the PCB when my hot air station arrives as well as my adjustable power supply (which can go to 50V output) so I can power the board as it would be powered by the battery.
I'd love a broken PCB so I can safely experiment with it. A board with burnt mosfets would be great, with no blown/corroded traces. Mine will go back in the board and I won't play with powering it on the bench since I don't wanna break it.
Board uses IRS2003 half bridge drivers. For remote there's nRF24L01 so should be easy to interface.
On the schematic "a" represents one motor and "b" the other (as in L1a is LIN from 1st phase on "a" motor, and H2b is HIN on second phase on "b" motor.).
Found the hall sensors and temperature monitor on each motor, battery LEDs. But I have no idea what kind of signals are in use. I need to power the board first.
Theoretically this should be good to start a firmware dev.
I still don't know exactly how to upload to MCU. There's a 4 pin contact on the PCB, I presume 3.3V/GND/RX/TX but need to test it when I power it up on the bench.
![47|561x499](upload://dIzNh3G7ouERlS6xne6YbAvrETC.png)
```

---
## \#7 Posted by: decebal Posted at: 2018-08-18T18:51:45.969Z Reads: 35

```
Is there anyone interested in adapting code from VESC for this application? Someone that is able to do that. I'm not that great on software, especially at the level VESC is atm.
So I know if it's worth it to dig deeper and trace everything.
```

---
## \#8 Posted by: careyer Posted at: 2018-08-20T14:24:06.613Z Reads: 30

```
Wow! Great achievement decebal. Looks like you are a real electronics magican. You cleared a lot of the mystery dust that comes with that controller already. Hope you Powersupply and HotAir station arrives soon. I will search the internet for a broken PCB. Let's see... 
Maybe it is possible to dump the current firmware from the controller and just alter/hack it instead of writing a new one from scratch?

Cheers! Keep up the excellent work!
```

---
