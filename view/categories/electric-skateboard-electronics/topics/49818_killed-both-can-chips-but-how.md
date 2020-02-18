# Killed both CAN chips but how?

### Replies: 31 Views: 1021

## \#1 Posted by: TarzanHBK Posted at: 2018-03-22T09:01:29.682Z Reads: 140

```
So what happened:

Had a board sitting on the shelf for half of a year. I took everything apart and reassembled it new, checked battery and rewired most of the connections. Everything was ready, but i didn´t connect the motors to the vescs (4.12). To test the new lights i switched on the BMS to power the vescs which feed the leds through the receiver. Both Vescs are powered on the same time and are connected over CAN.
Plopp! Bit of magic smoke and no LEDs on on both Vescs. Reciever was still powered and Lights worked like they should.
After i closed my WTF-face a minute later i checked the Can cable. Everything good! Nothing loose and not a bad contact!

HOW did i kill them? Had a propper connection, both vescs were powered and firmware was configured the right way about half a year ago and can worked back then!
```

---
## \#2 Posted by: b264 Posted at: 2018-03-22T09:04:21.384Z Reads: 140

```
Do you have a photo of the wiring?
```

---
## \#3 Posted by: TarzanHBK Posted at: 2018-03-22T09:09:33.508Z Reads: 136

```
nah, i already took it apart again yesterday.
Wires were all good, tested everything.
Pretty sure it´s a vesc kind of problem, but im not sure why
```

---
## \#4 Posted by: bimmer Posted at: 2018-03-22T09:18:34.849Z Reads: 132

```
2 or 4 wire can cable?
```

---
## \#5 Posted by: TarzanHBK Posted at: 2018-03-22T09:26:10.932Z Reads: 131

```
two wires. Is a 4 wires-Can cable even a thing on the 4.12 to connect two? I don´t think so without killing it :face_with_monocle:
```

---
## \#6 Posted by: Acidfie Posted at: 2018-03-22T09:47:29.007Z Reads: 128

```
4 wires will mostly fry your vesc, because of a ground loop
```

---
## \#7 Posted by: TarzanHBK Posted at: 2018-03-22T09:51:32.944Z Reads: 127

```
Yah, that´s why i´m wondering where @bimmer has had 4 wires before.

If he´s just wondering if im stupid enough to did a 4 wire connection - nah mate, can´t be so drunk to do that over 2 years of working with vescs ;)
```

---
## \#8 Posted by: TarzanHBK Posted at: 2018-03-22T12:42:33.640Z Reads: 116

```
@JohnnyMeduse any idea how thats possible?
```

---
## \#9 Posted by: SimosMCmuffin Posted at: 2018-03-22T13:54:09.794Z Reads: 111

```
[quote="TarzanHBK, post:1, topic:49818"]
Bit of magic smoke and no LEDs on on both Vescs. Reciever was still powered and Lights worked like they should.
[/quote]

So did you kill the CAN chips or the 3V3 regulator, if no leds are lighting up?
```

---
## \#10 Posted by: TarzanHBK Posted at: 2018-03-22T15:20:58.752Z Reads: 104

```
Good question, last time i had something like this, the Can chip died.
Do you know how to check if its the regulator?
```

---
## \#11 Posted by: trampa Posted at: 2018-03-22T15:31:21.959Z Reads: 103

```
Both ESCs connected to the same battery I guess, one switch.
```

---
## \#12 Posted by: TarzanHBK Posted at: 2018-03-22T15:34:40.931Z Reads: 103

```
Yes for sure! 
(Is anyone running dual on two different batteries?)
```

---
## \#13 Posted by: trampa Posted at: 2018-03-22T15:39:27.815Z Reads: 103

```
CAN on HW 4 can handle +-12V only, while HW6 can handle +-60V. This is why HW 4 needs to be powered up at the same time. If for some reason there was a voltage difference above 12V, they would have blown because of that. And to me that sounds the most plausible explanation. The reason for the voltage difference has to be somewhere in the system or on one ESC.
It is always a good idea to test things on 11.1 V (3S) if you have a 3S to hands to avoid such issues.
```

---
## \#14 Posted by: trampa Posted at: 2018-03-22T15:44:07.752Z Reads: 102

```
[quote="TarzanHBK, post:12, topic:49818"]
(Is anyone running dual on two different batteries?)
[/quote]

(Is anyone running dual on two different batteries?)

YES we are.
```

---
## \#15 Posted by: Acidfie Posted at: 2018-03-22T15:47:52.648Z Reads: 97

```
can anyone confirm this?

i am currently setting up 2 esk8 VESC 1.1 and they're HW 4.12 afaik.

@esk8 maybe you can give us some answers 

(http://www.electric-skateboard.builders/t/new-esk8-controller-1-1-based-on-v-4-12-little-bit-smaller/27756/3) 

i never heard of this problem but this scares me of using CAN for 2 VESC on the same battery
```

---
## \#16 Posted by: TarzanHBK Posted at: 2018-03-22T15:50:55.867Z Reads: 93

```
good to know.
The thing is, the setup ran fine half a year ago, but now poof..
```

---
## \#17 Posted by: koralle Posted at: 2018-03-22T15:53:07.946Z Reads: 89

```
I know I am repeating myself but does anybody have a link or a quick explanation on best practices when connecting VESCs 4 and CAN bus? Especially when setting up the VESCs.

Whats important? Which order?

Threads like these give me goosebumps.

I get that both vescs need to be on the same power source and connected simultaneously. Is that all? CAN bus connected from the beginning?
```

---
## \#18 Posted by: Acidfie Posted at: 2018-03-22T15:56:27.780Z Reads: 91

```
yeah, i want this too. still afraid to connect the VESC together via CAN.
```

---
## \#19 Posted by: trampa Posted at: 2018-03-22T15:58:29.720Z Reads: 89

```
Yes, CAN connected, simultaneous start-up. 
At setup 3s is always a good idea and CAN save some $$.
```

---
## \#20 Posted by: trampa Posted at: 2018-03-22T16:03:16.095Z Reads: 89

```
This is how you should do it. Y-PPM causes ground loops, which can kill your voltage regulators, since they will always fight against each other.  CAN is the way to go and should work just fine.
```

---
## \#21 Posted by: Acidfie Posted at: 2018-03-22T16:07:05.264Z Reads: 85

```
wait..wait...wait.

i was not talking about Y-PPM, i was talking about CAN.

so you say, connecting two VESC via CAN is no problem, no matter how they're connected to the battery?

1. connect both VESC via CAN
2. power up both VESC via Loop key or switch or [...]
```

---
## \#22 Posted by: DeathCookies Posted at: 2018-03-22T16:08:30.438Z Reads: 86

```
[quote="trampa, post:20, topic:49818"]
CAN is the way to go and should work just fine
[/quote]

That is questionable because what happens with CAN if your master (ppm attached to master) is fired? you cannot drive home.

but what about split PPM? Well you can drive home....


It is like a coin: every side has pro and cons...
```

---
## \#23 Posted by: DeathCookies Posted at: 2018-03-22T16:10:05.701Z Reads: 81

```
[quote="TarzanHBK, post:16, topic:49818, full:true"]
good to know.

The thing is, the setup ran fine half a year ago, but now poof…
[/quote]

When i Setup a board i ALWAYS configure each vesc individual and then attach/Setup CAN. This way i will know if one VESC is faulty before running into CAN-IS-A-BITCH-PROBLEMS (preventing fried hw)
```

---
## \#24 Posted by: fedestanco Posted at: 2018-03-22T16:16:46.589Z Reads: 80

```
The thing is CAN is supposed to be 100 times more reliable than PPM since it was developed for communication between vital electronic components on vehicles.
It gained a bad reputation in this forum probably because of bad installations or obsolete chips.
```

---
## \#25 Posted by: trampa Posted at: 2018-03-22T16:18:57.183Z Reads: 81

```
[quote="DeathCookies, post:23, topic:49818"]
When i Setup a board i ALWAYS configure each vesc individual and then attach/Setup CAN.
[/quote]

This is a good advice! If you then use a 3S for configuration, nothing should happen.
```

---
## \#26 Posted by: Deckoz Posted at: 2018-03-22T18:16:38.259Z Reads: 73

```
[quote="trampa, post:13, topic:49818"]
This is why HW 4 needs to be powered up at the same time
[/quote]

This is why you only run canbus with tx and rx connected, and the ground and vcc depinned...

😑😑😑😑

Can't blow a can chip without a shared ground or vcc. I really don't understand why every vesc has 4 pins, Should only have two to prevent user errors..
```

---
## \#27 Posted by: Bjork3n Posted at: 2018-03-22T18:37:18.442Z Reads: 71

```
From what i know there are more people having issues with canbus than with split ppm. 
I never heard anyone destroy a vesc using split ppm.

Im staying with ppm...
```

---
## \#28 Posted by: esk8 Posted at: 2018-03-23T06:54:18.752Z Reads: 62

```
I don´t know why have Tarzan killed the CAN chip.
I ride al my boards in dual system, and al my controller 
was connected with the CAN kable with out problems.
On my HP was in the tutorials how you can connecting 
the dual system with CAN Bus cable.
I programmed the slave at first and then the master.
Then i controlling the spinning by the motor and at the 
last step i connecting the CAN cable.
When a customer buy by me two controller i al time ask
he wants making a dual system.
And when he say yes, then i programming for him the 
master and slave, so thats he don't have a problems with this.
```

---
## \#29 Posted by: trampa Posted at: 2018-03-23T07:39:03.434Z Reads: 59

```
The standard for CAN is 4 pins, since you could power up a secondary device via CAN GND and VCC.
In this case all CAN devices sit on one common, shared power line.
If all devices have their own power supply or the same, shared power supply (like two ESCs), you should not connect GND and VCC since this creates GND LOOPs in the system. VESC-based ESC are not always used in skateboarding and therefore 4 PINs are very useful. 

If you design your own HW, you could make the decision to use a 2 Pin connector and limit the use for coupling ESCs only, or split connectors for CAN L And CAN H and GND and VCC into two separate ports. This is up to the designer of the PCB.
```

---
## \#30 Posted by: Jebe Posted at: 2018-03-23T11:58:55.126Z Reads: 49

```
Have fried many canbus chips now. Going with a reciever for each vesc and bound to 1 transmitter.
```

---
## \#31 Posted by: Acidfie Posted at: 2018-03-23T12:15:09.535Z Reads: 46

```
why is that so?
```

---
