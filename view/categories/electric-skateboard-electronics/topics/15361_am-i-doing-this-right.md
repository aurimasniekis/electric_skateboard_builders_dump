# Am I doing this right

### Replies: 19 Views: 1206

## \#1 Posted by: SyrusB Posted at: 2016-12-29T19:55:17.904Z Reads: 106

```
<img src="/uploads/db1493/original/3X/2/e/2ec2514a6fe1c56d1709b3564bbee5a3a45de3d4.jpg" width="690" height="388"> 

Is this wiring right? 
And what am I doing wrong
```

---
## \#2 Posted by: mmaner Posted at: 2016-12-29T19:56:16.205Z Reads: 104

```
Are the phase wires touching?
```

---
## \#3 Posted by: SyrusB Posted at: 2016-12-29T19:59:54.962Z Reads: 101

```

Yes the phase wires are partially soldered
```

---
## \#4 Posted by: mason Posted at: 2016-12-29T20:01:42.885Z Reads: 102

```
INSULATE THOSE DAMN PHASE WIRES!! please
```

---
## \#5 Posted by: SyrusB Posted at: 2016-12-29T20:03:09.870Z Reads: 99

```
What does that mean
```

---
## \#6 Posted by: SyrusB Posted at: 2016-12-29T20:03:29.986Z Reads: 99

```
This is my first build and I have no idea what I am doing
```

---
## \#7 Posted by: mmaner Posted at: 2016-12-29T20:05:14.946Z Reads: 98

```
The 3 wires coming from the VESC to the motor, those are the phase wires.  If they touch, while powered, your VESC is dead.  Please put some heat shrink on em.
```

---
## \#8 Posted by: SyrusB Posted at: 2016-12-29T20:08:17.982Z Reads: 96

```
Okil have done this
```

---
## \#9 Posted by: SyrusB Posted at: 2016-12-29T20:10:19.278Z Reads: 94

```
What else should I do
```

---
## \#10 Posted by: Alextech Posted at: 2016-12-29T20:13:00.842Z Reads: 93

```
You will need to configure the Vesc to your motor.  You will need a USB cable and a computer loaded with the bldc tool.  There is plenty posts about how to set it up, just use the search bar.  :smile:
```

---
## \#11 Posted by: TranxFu Posted at: 2016-12-29T20:15:10.625Z Reads: 93

```
Did you mount the motor and vesc to the truck already ? Just to check the distances and so on... Just asking because you are not using bullet connectors for the phase wires. It'll limit you when trying doing the layout on the deck.
```

---
## \#12 Posted by: SyrusB Posted at: 2016-12-29T20:16:12.716Z Reads: 90

```
I have and it fits perfectly
```

---
## \#13 Posted by: SyrusB Posted at: 2016-12-29T20:16:25.028Z Reads: 87

```
Thank you for all of the help
```

---
## \#14 Posted by: SyrusB Posted at: 2016-12-29T20:16:52.140Z Reads: 86

```
Ok thank you
```

---
## \#15 Posted by: SeanHacker Posted at: 2016-12-29T20:21:56.741Z Reads: 82

```
This is why I love this forum. Everyone helps! :smile:
```

---
## \#16 Posted by: LukeL Posted at: 2016-12-29T20:30:48.702Z Reads: 80

```
can't really tell how good the solder joints are but looks like you haven't tinned the motor wires which you should really but it might be ok

you need to program the vesc before using it

are you going to add an anti spark loop key to turn it off/on without sparking

is that the only battery you're using? can't see what size it is in picture

also as you're not using connectors between your motor and vesc you might find it spins the wrong way and will be a pain to unsolder and switch the phase wires round, you could buy some bullet connectors instead so you can unplug them
```

---
## \#17 Posted by: SyrusB Posted at: 2016-12-29T20:45:30.338Z Reads: 75

```
Ok I will try resolder them and tin them better so that this might help I have programed the vesc and thank you for all the help everyone has given this forum is amazing
```

---
## \#18 Posted by: TranxFu Posted at: 2016-12-29T21:21:17.138Z Reads: 68

```
Yea thats a good point actually. If they have the wrong order your motor turns the wrong way... So just get bullet connectors or you'll have to resolder them another time. Watch some youtube tutorials on soldering bullet connecters/soldering in general.
```

---
## \#19 Posted by: rwxr Posted at: 2016-12-30T06:29:55.495Z Reads: 39

```
Hehe, fortune favors the bold...
You should've added bullet connectors to the motor and the VESC. And if you're doing that later on, look into doing the SK3-mod where you replace the motor wires with flexible silicon wire at the same time. The stiff original cables will sooner or later break due to bending and general wear and tear.

There is a thread for this if you search for "Sk3 silicone mod" or similar.
```

---
