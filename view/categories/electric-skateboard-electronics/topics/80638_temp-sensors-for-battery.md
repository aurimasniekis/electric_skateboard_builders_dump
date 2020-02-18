# Temp sensors for battery

### Replies: 13 Views: 328

## \#1 Posted by: Hummie Posted at: 2019-01-11T21:53:22.001Z Reads: 91

```
How hard or expensive would it be to put maybe 24 temp sensors on a battery hooked just to an alarm?

https://www.adafruit.com/product/1782?gclid=CjwKCAiA99vhBRBnEiwAwpk-uAH2h5yOSxL4ccYCtjz7AaSDc-TuzF8DStizUj0B5uBfQJeKAzCZLhoCZ1UQAvD_BwE

There’s so many options here and I don’t know what I’m doing
It wouldn’t need to be accurate just alarm if something went over maybe 100f.  Hoping to find a pcb that could use many sensor wires.  I’m not sure if the ones sold here do.
```

---
## \#2 Posted by: Andy87 Posted at: 2019-01-11T22:28:21.372Z Reads: 77

```
You could get something like this.
https://s.click.aliexpress.com/e/by2X84V8
It’s single sensor, but maybe it’s possible to connect more temp sensors in a loop in series or parallel.
If you don’t nee 24 sensors you could just get some of this
https://s.click.aliexpress.com/e/c7B1dXG
And 3D print a case for the displays.
```

---
## \#3 Posted by: Hummie Posted at: 2019-01-12T01:13:03.449Z Reads: 56

```
Could you connect multiple sensors off that first one you posted?  Anyone?
```

---
## \#4 Posted by: ZachTetra Posted at: 2019-01-12T05:16:08.401Z Reads: 47

```
If you pull apart a battery (say a 6s2p into 6 sets of 2p in parallel) would each pair need a sensor or just one of the pairs?  And do batteries usually have a sensor in them?
```

---
## \#5 Posted by: Andy87 Posted at: 2019-01-12T06:10:27.752Z Reads: 45

```
Most bms have one or two temp sensors you could use.
I took a lot of laptop packs out of each other and I never found more than 3 temp sensors.
I think one senser for each p-group is more than enogh.

@Hummie i know that @PXSS  does the battery stuff at work, maybe he knows some board/pcb which can hsndle multiple temp sensors and monitor or create an alarm if out of range.
```

---
## \#6 Posted by: Darkie02 Posted at: 2019-01-12T06:22:30.887Z Reads: 39

```
Could you use multiple thermal cut out in series connected to a relay coil to turn off a relay if exceeding a set temp? Or are you trying to do some thing a bit more fancy?
```

---
## \#7 Posted by: ZachTetra Posted at: 2019-01-12T06:37:40.718Z Reads: 35

```
If you put a bunch of thermistors in series and that in parallel with a potentiometer you can plug the whole thing back into the temp sensor and it will go off if the net temperature is to high...not as fancy but it will say if everything is unusually hot or one cell is excessively hot if the others are normal
```

---
## \#8 Posted by: Hummie Posted at: 2019-01-12T16:48:36.271Z Reads: 31

```
I’m not trying to be fancy, just get a buzzer on the board to go off if the temp gets too high.   I’ll call some places on Monday and see. But if anyone  knows of some parts that would enable this please post them.
```

---
## \#9 Posted by: Surfer Posted at: 2019-01-12T17:35:31.000Z Reads: 26

```
What I do is  stick a thermistor inside the pack with hot glue, wrap it all and then I connect to a vesc like it was a motor temp, and then I can see it in metr app 😋
```

---
## \#10 Posted by: Hummie Posted at: 2019-01-12T17:39:58.779Z Reads: 23

```
If a bunch of sensors or maybe one long sensor that could pick up heat from anywhere in the pack..that’d be a huge safety plus

Is it a problem to have the board on while charging?
```

---
## \#11 Posted by: ZachTetra Posted at: 2019-01-12T17:43:29.844Z Reads: 21

```
What hardware is needed for metr?
```

---
## \#12 Posted by: Hummie Posted at: 2019-01-12T17:45:09.961Z Reads: 22

```
If this could go off the vesc that’s even better. One long temp sensor wiggled through all the cells, and keeping the escs on while charging and I’ll be invincible
```

---
## \#13 Posted by: Andy87 Posted at: 2019-01-12T17:55:45.120Z Reads: 19

```
Metr Bluetooth modul
```

---
