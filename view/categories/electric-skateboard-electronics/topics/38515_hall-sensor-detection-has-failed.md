# Hall sensor detection has failed

### Replies: 7 Views: 2138

## \#1 Posted by: nordlicht Posted at: 2017-11-16T16:18:29.857Z Reads: 219

```
Hi,
this was the first time I tried the VESC.
Here is what I did:
Using a lab power supply, since I didn't finish the battery pack yet. Put the voltage to 34.4V.
Connected the vesc to power supply than connected the vesc to the PC.
I read the config and put the battery cutoff start to 33V, the end to 30V.
I wrote the config successful.
Went to BLDC tab and started detection. Motor spun really short and gave the following out:


----------

Int limit: 76.86
BEMF: 425.39

Hall sensor detection failed:
5, -1, 1, -1 , 4, -1, 2, -1


----------

I'm running 130kv torque HUBs.
Important to note is here that I (stupidly) didn't order the cable-adapter to connect the motor hallsensor to the VESC hall input.
I measured the voltage from the outer 2 pins and the outer one (the once next to the border) is the positive one.
Than I connected the red cable from motor hall with the outer pin on the board, the black one with the inner pin and the others in the original order (but the order of those actually doesnt even matter, right?).

I made sure there is no contact in between the pins. They are all isolated.

Any ideas?
I'm buying a JST XH pack on amazon asap.

If you could upload an actual picture of the wiring from your motor to the VESC board, I really would appreciate.

Cheers,
Nordlicht
```

---
## \#2 Posted by: E1Allen Posted at: 2017-11-16T18:58:56.668Z Reads: 194

```
One is signal as well. Next to red.<img src="/uploads/db1493/original/3X/4/9/49b81148871da84bec10ef6aa8e1da9ccb516a87.jpg" width="281" height="500">

I'm not 100% sure but I think it has to go there.  Sensor input at top of the picture.
```

---
## \#3 Posted by: Quezacotl Posted at: 2017-11-16T20:11:25.654Z Reads: 184

```
5V and GND to the respectful pins. Hall sensor order doesn't matter in VESC. And VESC has pull-ups(or was it down) already installed.

I have same problem. Can't get it to work. All i know that those i told are the facts.
My hall-sensors are working. I have measured.

Next thing would be to try fiddling with the settings. I think i have tried all i can think of. Next commenter can maybe help further :)
```

---
## \#4 Posted by: kylepls Posted at: 2017-11-17T05:40:23.276Z Reads: 175

```
Seems to be a common issue all the sudden. I posted the same thing a few days ago. http://www.electric-skateboard.builders/t/need-help-hall-sensor-detection-not-working-with-brand-new-motor-and-esc/37651
```

---
## \#5 Posted by: esk8 Posted at: 2017-11-17T06:02:56.894Z Reads: 176

```
<img src="/uploads/db1493/original/3X/4/1/41b95971eae654a02c4d51c596a24bf4b002f7c9.jpeg" width="281" height="500">
GND H3 H2 H1 Temp 5V on the PCB
Vesc  :  Motor
red -> black
blue->yellow 
green->blue
yellow->green
white->white
black->red

Thats was so by my Motor,
and that was wit out guarantee 
thats the same by another Motors
I have here one older Motor who 
was the yellow cable the positiv +
```

---
## \#6 Posted by: Quezacotl Posted at: 2017-11-20T15:05:35.064Z Reads: 142

```
I believe here's the solution to many people (With FOCBox). I just checked, and i indeed have the label wrong. Once i corrected the wiring, it started working and there were no problems with the software :smile:
I just swapped T and H3, since the hall sensor wire order doesn't matter.

Now the startup is very good and no stutter whatsoever :sunglasses:

 http://www.electric-skateboard.builders/t/new-improved-focbox-official-thread/11102/433?u=quezacotl
```

---
## \#7 Posted by: nordlicht Posted at: 2017-11-23T15:06:01.868Z Reads: 135

```
Hi again,
thanks for your pictures and reply. Glad u found a solution Quezacotl =)
One Motor is working properly, the other one not. I measured the Hallsignals with an oscilloscope, the working motor has nice clear signals, the other one not. Apparently I got no luck with the order...

Does anyone have information about how diyelectricskateboard returns products like that? The motor has never touched ground...

Cheers
```

---
