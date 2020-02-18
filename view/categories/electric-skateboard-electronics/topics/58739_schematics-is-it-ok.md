# Schematics - is it ok?

### Replies: 14 Views: 340

## \#1 Posted by: cypa9904 Posted at: 2018-06-13T13:20:32.703Z Reads: 150

```
Hi. 
Will sb tell me if it will work? 
![20180613_151927|690x388](upload://dgF0QW7TaH34cmbECLxDpYtfxVr.jpg)
```

---
## \#2 Posted by: abenny Posted at: 2018-06-13T13:25:16.344Z Reads: 140

```
Looks good, in the ppm y splitter make sure you cut the 5v wire from one of the foc boxes, some also cut the extra ground wire but I haven't
```

---
## \#3 Posted by: solodros Posted at: 2018-06-13T15:09:58.916Z Reads: 115

```
Make sure that the voltage difference between the two battery packs is small, otherwise the battery pack with high voltage will charge the battery pack with low voltage, and the current is very high because the internal resistance of the battery pack is very small.
```

---
## \#4 Posted by: cypa9904 Posted at: 2018-06-13T15:14:06.560Z Reads: 102

```
I have got 4x 30C 8ah 5s li po packs.
```

---
## \#5 Posted by: solodros Posted at: 2018-06-13T15:29:57.806Z Reads: 93

```
Use a multimeter to test the voltage of the four battery packs to ensure that the voltage difference does not exceed 0.1v.
```

---
## \#6 Posted by: thisguyhere Posted at: 2018-06-13T16:25:05.775Z Reads: 77

```
your battery is in parallel, don't have time now but I'll try drawing it out later.
```

---
## \#7 Posted by: abenny Posted at: 2018-06-13T16:26:56.761Z Reads: 72

```
he has 2x 5s in series , then he has that in parallel with another  2x5s in series. looks fine
```

---
## \#8 Posted by: thisguyhere Posted at: 2018-06-13T16:32:26.166Z Reads: 71

```
oh I see didn't know what each pack S count was

proceed
```

---
## \#9 Posted by: thisguyhere Posted at: 2018-06-13T18:34:35.018Z Reads: 53

```
wait, are you going to balance charge each P group?  kind of a hassle...
```

---
## \#10 Posted by: cypa9904 Posted at: 2018-06-13T18:44:51.449Z Reads: 51

```
What do you mean?
```

---
## \#11 Posted by: willumpie82 Posted at: 2018-06-14T07:50:17.539Z Reads: 37

```
why do you split the ppm instead of using canbus?
```

---
## \#12 Posted by: cypa9904 Posted at: 2018-06-14T08:28:57.136Z Reads: 35

```
Because some people claim that it is simplier and less risky. Btw. using split "y" do I need to ground one of the wires? If so, how do I do it? By simply cutting (1) middle wire off or sth like that?
```

---
## \#13 Posted by: pat.speed Posted at: 2018-06-14T12:13:42.378Z Reads: 28

```
Connect all wires in parallel and then just cut the second 5v/ red wire from the focbox
```

---
## \#14 Posted by: cypa9904 Posted at: 2018-06-14T16:48:45.182Z Reads: 20

```
Just one last question. 

Would it be good if my batteries were separated?
I mean only vescs would be connected in a radio receiver but batteries would be only connected in series (2x separate sources of energy, one for each vesc, two anti-spark switches etc.)

Or maybe I shouldn't do it for some reason?

 I have got e-mtb 10s 2x 192 kv sensorless motors and 1:4.55 reduction.

Sth like that
![received_1698898983540022|281x500](upload://2l3OPvlf1YfwxT9DJRQaB8Ik5cE.jpeg)
```

---
