# Phase wire length and desync

### Replies: 17 Views: 472

## \#1 Posted by: xilw3r Posted at: 2018-06-18T07:27:27.654Z Reads: 143

```
Hello smart peoples of the interwebz.

I am working silently on a really stupid thing, which involves me putting the vesc right next to the battery in a box in the middle of the board. Then I just route the phase wires to the motor mount, which is going to be around 400-500 mm of travel  (15-20 inches). 

I thought this should be relatively problem free, since i only knew about the battery wire length issue where induced voltage spikes fry the vesc. But then I read a post by @Deckoz which has me a bit worried, he mentioned a phenomenon I have not known about, where the back emf reading can get distorted over long phase wires and the motor can simply stall during riding. Scary.

Does anyone know a limit where this can start happening? I read that @GrecoMan has been running really long phase wires without issues, but I have no idea on what hardware.

I am using vesc 4.12
```

---
## \#2 Posted by: pat.speed Posted at: 2018-06-18T08:09:17.672Z Reads: 140

```
You should be relatively fine me thinks, just make sure to use large enough phase wires, probably 12-10awg to minimise resistance. 

Is this going to be on a mountain board? Or just a standard longboard with the gear in the middle? @Sirshaunsta might be able to help as I think he had his batteries and vescs in the middle of his board
```

---
## \#3 Posted by: xilw3r Posted at: 2018-06-18T08:13:10.624Z Reads: 137

```
[quote="pat.speed, post:2, topic:59251"]
and
[/quote]

200mm wheels, single drive, but meant for city riding.. just shitty pavements.


edit: I have 12awg on hand, I thought about doubling them up for the major strecth.
```

---
## \#4 Posted by: dareno Posted at: 2018-06-18T08:23:41.184Z Reads: 126

```
Its my understanding and I'm sure I will be corrected by far more knowledgeable people than me if I'm wrong but phase wires cause desync when they are different lengths.  Dual motor set ups with one side shorter than the other will experience problems and the three wires on a single set up need to be the same length.  As for length, as @pat.speed said  compensate the resistance with a bigger gauge wire and you should be ok.
```

---
## \#5 Posted by: rich Posted at: 2018-06-18T08:36:49.400Z Reads: 115

```
Never heard about desync but I had 85cm (33.5 inch) phase (12AWG) and sensor (22AWG) wires running on V4.12 without problems so I wouldn't worry.
```

---
## \#6 Posted by: koralle Posted at: 2018-06-18T08:46:14.796Z Reads: 114

```
I have never ever seen proof of _10-12awg phase or battery wires that are <1m lenght_ cause anything at all except for current to flow.
If they are proper copper, the resistance is negligible so I would be ultra surprised if different lengths of phase wires would give any problems. Electrons don't "take time to reach the other end" ...
```

---
## \#7 Posted by: pat.speed Posted at: 2018-06-18T08:52:37.606Z Reads: 108

```
Yeah I’m not sure your quite right there, as the vescs are separate hardwares meaning they do not care about each other’s motors postition, except for traction control. 

As for different lengths of leads on the same motor, I know that small variances (1/2” or so) do not make a difference.
```

---
## \#9 Posted by: dareno Posted at: 2018-06-18T09:05:57.531Z Reads: 105

```
Yeah I'm not entirely sure either but all I'm going on is a twin motor set up on an Rc I built.  Problems with my esc's until i paired the wiring.  As for separate, are they?  They are both controlled by one receiver and if one motor has more resistance than the other then surely they will be out of sync. ( I'm learning here please correct me)  :slight_smile:
```

---
## \#10 Posted by: koralle Posted at: 2018-06-18T09:10:46.938Z Reads: 99

```
your motors are synced by being both fixed to the same board and the wheels running on the same ground. You can use different motors, different cables etc. They might not always push with the same torque but if theres no huge difference, you will not notice. Mono drives work too.
```

---
## \#11 Posted by: Sirshaunsta Posted at: 2018-06-24T15:58:47.740Z Reads: 75

```
Never heard of this DESYNC but it would make sense as even with car stereos if you run a thin wire over a long distance the power and signal get weaker.
```

---
## \#12 Posted by: Sirshaunsta Posted at: 2018-06-24T16:01:36.373Z Reads: 74

```
I have 16  yes 1 and then a 6 (16) 5s 5ah lipos between my legs with between 12 and 18 inches going from battery to vesc to motor in all four corners. In testing I've found NO ISSUES at 10awg but I'm also using thicker cables because of my battery size and to utilize all power of FOUR 190kv brushless motors(sk3-6364)
```

---
## \#13 Posted by: Fatos Posted at: 2018-09-08T13:34:56.135Z Reads: 60

```
What dif you end up with? Did it work? im building a trampa board myself and was wondering if it is possible to have motor cables stretched to the middle of the board.
```

---
## \#14 Posted by: xilw3r Posted at: 2018-09-08T13:54:04.421Z Reads: 59

```
my phase wires are 70cm right now, no issues at all. Only issue is the esc being inside a 3d printed case- it gets too hot too fast

edit: oops replied to the wrong post. Its meant for @Fatos
```

---
## \#15 Posted by: Fatos Posted at: 2018-09-08T14:36:08.154Z Reads: 55

```
It's a trampa board you have right?What is the Awg for the wires you used? What about motor sensor?
A picture would be appreciated, if you have a trampa board. 
Sorry for so many questions.
```

---
## \#16 Posted by: Andy87 Posted at: 2018-09-08T14:38:27.586Z Reads: 54

```
The critical wire length is only from battery to vesc as there it’s direct current.
With the phase wires and 70cm you shouldn’t get any issues
```

---
## \#17 Posted by: xilw3r Posted at: 2018-09-08T15:05:48.676Z Reads: 50

```
Its not a trampa :/ I wish lol. I have just some lame crappy chinese longboard with sawed off ends.

I am using AWG 12 wire, could go for AWG 10 or 8, every bit helps. Especially since after going hard for a longer while like up hill, the wires get rather warm over a 10-15 cm distance from motor and the mosfets. More copper never hurts lol

Oh, and I am sensorless for now. If you use sensors, I would make sure the cable is shielded. Probably not entirely necessary, but would not hurt I think
```

---
## \#18 Posted by: Fatos Posted at: 2018-09-08T18:43:09.039Z Reads: 38

```
Thanks man. I'll take your tip and do it like that :).
```

---
