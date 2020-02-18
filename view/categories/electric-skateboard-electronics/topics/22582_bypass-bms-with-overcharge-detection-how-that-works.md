# Bypass bms with overcharge detection. how that works?

### Replies: 18 Views: 2381

## \#1 Posted by: pau Posted at: 2017-05-07T12:08:28.451Z Reads: 214

```
hey,
i can not image how works the overcharge protection, in this schematic?

link to [bms](https://hobbyking.com/media/file/845847974X4580138X47.pdf)

for exapmle: there are 2 3s lipo with each 5Ah
the charger has a current of 5Ah.

one more question: are the balance wires correct connectet to the bms?
what is with the two negative wires? should i connect them to the ground wire of the battery?

what will happen if the charger is 10 hours connect/charge<img src="/uploads/db1493/original/3X/a/f/afe415fe295b4ad0da5ac215e9597a07df07ebf0.png" width="690" height="424"> to the bms? i think the battery will get overcharge, beacause the batterie is parallel to the bms.
```

---
## \#2 Posted by: IsTalo Posted at: 2017-05-07T13:31:14.483Z Reads: 188

```
I think the battery won't overcharge if you use the voltage of the battery, like, you have a 6s battery, so a 25.2v charger will be good! And other, if you charge when the board is off, the Bms will work fine, the overcharge still useful, but measure the voltage after the first charge
```

---
## \#3 Posted by: pau Posted at: 2017-05-07T13:36:40.174Z Reads: 178

```
why should i measure the voltage after the first charge?
what is when there is to low or too much voltage?
```

---
## \#4 Posted by: IsTalo Posted at: 2017-05-07T13:38:13.428Z Reads: 175

```
No, just to see if it overcharged! It wouldn't be too low, but if it's too high you have to talk with someone that understands more of Bms than me
```

---
## \#5 Posted by: evoheyax Posted at: 2017-05-07T14:11:34.791Z Reads: 176

```
It depends honestly on the bms. No sure about that bms, but I had put 2 in parallel before like this to bypass for discharging. The problem with both was no balancing took place. I could charge it, but they never balanced. I have heard of others having more luck. I think it depends on the bms, and it's hit or miss.
```

---
## \#6 Posted by: chinzw Posted at: 2017-05-08T15:35:18.649Z Reads: 148

```
With that wiring you won't get any overcharge protection from the bms. All you would get is passive balancing.
EDIT: if you look at the hobby king wiring diagram, that's how you would get overcharge protection. You put the charger and the load between B+ and P
```

---
## \#7 Posted by: pau Posted at: 2017-05-08T17:31:07.935Z Reads: 142

```
hey, 
i misstake was to put the charger plug parrallel to the bms and battery.
i think now it is all right. is it?
 so the charger plug will be in serielle between bms and battery.

is there now a overload protection?

<img src="/uploads/db1493/original/3X/0/5/05c70e55c09aee841a2a5e462b1fddcda3e875f7.png" width="690" height="424">
```

---
## \#8 Posted by: Jinra Posted at: 2017-05-08T17:36:10.754Z Reads: 118

```
The reason the letters are labled (-) on the BMS is that they're designed to be plugged into the negative of your pack/esc. Positive wires should always go to the battery directly. Your P- should be going to your motor controller and charging negative, not the positive of your pack.
```

---
## \#9 Posted by: chinzw Posted at: 2017-05-08T17:43:59.413Z Reads: 110

```
There's a perfectly good wiring diagram on the first link you posted for the BMS, just use that wiring diagram.
```

---
## \#10 Posted by: pau Posted at: 2017-05-08T18:34:05.613Z Reads: 116

```
here i updated the diagram.
is it now right?<img src="/uploads/db1493/original/3X/c/c/cc79aa132864215f5274662e0df21d84676ec93e.png" width="494" height="500">


it looks like  there are only negativ leads/connectors (B- and P- ) on the schematic(just bms)
<img src="/uploads/db1493/original/3X/4/1/41049872be472aff9c0b1b8a5fad3a32d4e747c3.PNG" width="690" height="245">
```

---
## \#11 Posted by: Jinra Posted at: 2017-05-08T18:36:53.003Z Reads: 116

```
No, besides the balance leads no + wire should be going into the BMS. B- should be going to battery negative and P- should be going to VESC/charge port.

You need to have charge port go to P- and battery positive. B- should go to battery negative. You should also place the volt meter after the switch so it's not always on.
```

---
## \#12 Posted by: pau Posted at: 2017-05-09T12:28:18.685Z Reads: 114

```
at first i want to say. Thank you for all your help!!! :)

i updated the diagram again. 
but now i think the bms is not bypassed. so the bms has to handel all that current. but i think i will blew up the bms, because it only can handle 10A.
<img src="/uploads/db1493/original/3X/a/c/acccf8e4de28f7aa5e5a613d83fc1686ed2fad29.png" width="494" height="500">

one more question. what does "load" mean in the schematic from the bms?
```

---
## \#13 Posted by: Jinra Posted at: 2017-05-09T13:45:57.900Z Reads: 103

```
Almost, put your charger positive before the switch so you don't have to turn it on when you charge.

If you don't want to use bms for discharging put the negative straight to the pack. Load is whatever you're powering. In this case, your vescs.
```

---
## \#14 Posted by: pau Posted at: 2017-05-09T16:41:47.935Z Reads: 101

```
hmm. but when i put the negative wire(blue wire) from vesc directly to the the battery, i dont have a overload protection. or i can install a switch ion that blue wire.


<img src="/uploads/db1493/original/3X/4/2/425192c3d70caffcf40c1f5c1707551abef60bc9.png" width="494" height="500">
```

---
## \#15 Posted by: Jinra Posted at: 2017-05-09T17:39:35.257Z Reads: 86

```
You can use a fuse. If you're bypassing BMS you're giving up BMS load protections
```

---
## \#16 Posted by: pau Posted at: 2017-05-10T17:33:08.285Z Reads: 86

```
Thank you for you help and patient.
I think I will install a xt90s anti spark on that blue wire. 
So for charging i just can pull out the xt90 connector.
```

---
## \#17 Posted by: edoardo Posted at: 2017-05-26T12:58:48.719Z Reads: 79

```
Hi, what's the meaning of "V" ( at right ) in the diagram?
```

---
## \#18 Posted by: krloz Posted at: 2017-05-26T13:51:19.267Z Reads: 80

```
The v is probably a voltage meter.  Parallel to the batteries.  Though no switch so always on. Careful
You can bypass the bus by connecting the black of the escs directly to the batteries and the red of the escs to the red on the batteries through a spark switch  (xt90s) disabling discharge protection ( do be sure yours race have correct minimum voltage set) while still jabbing the charge red to the battery red and the charge black to the bms enabling overcharge protection and balancing.  This is assuming this bms hag all of this protection.  I don't know t this physicist model
Whenever I said black is negative and red positive
I'm not sure but I think you have the balance wires turned around in each battery
```

---
