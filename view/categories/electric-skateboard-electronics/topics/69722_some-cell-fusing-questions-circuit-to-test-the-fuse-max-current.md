# Some cell fusing questions : circuit to test the fuse max current?

### Replies: 9 Views: 373

## \#1 Posted by: akira Posted at: 2018-10-01T10:11:08.029Z Reads: 112

```
Hello.
I'd like to build a 10s3p with cell fusing. My 18650 are LG-HE4 which have a max continuous discharge current at 20A. I hesitate between 22 and 20 AWG wires for the fuses. Any advice on it ? 

Also I am tring to think of a setup to test the current capabilities of my wires. How could I setup a circuit to ramp up the current from 0 to 20-30A to test when the wire would blow and decide (experimentally) which one to use ?
```

---
## \#2 Posted by: akhlut Posted at: 2018-10-01T13:49:15.242Z Reads: 101

```
24awg has a fusing current of 29.2A, which is 146% of the continuous load.  with 3p i wouldn't move down to 22awg.  

20awg has a fusing current of 58.6A.  if 1 of 3 cells fail the remaining two cells can only deliver 40A, not the 58.6A needed to blow the fuse on the bad cell.
```

---
## \#3 Posted by: sztamas Posted at: 2018-10-01T14:09:31.664Z Reads: 94

```
I am not an expert, but here is a list what I found:
* in the datasheet the short amperage is 130A for a single cell. I think this is for a fully charged battery, but should be somewhere near for a drained one.
* 20awg will be more then 75 °C for 11 amper continous and will fuse less then 1 sec
* 22awg will 75°C at 7 amps will fuse less then half sec (but it is rare for draw 7 amps continously)
* Kaly uses 24 awg nickel strips
```

---
## \#4 Posted by: akira Posted at: 2018-10-01T14:17:41.338Z Reads: 88

```
Thanks guys for your inputs !

@sztamas  
I don't understand your explanations. the 75degrees and 11 or 7 amps are for normal operation, right ? It looks freaking hot to have a fuse at 75 degrees for 7A !!

How do you get the fusing time ? @akhlut mentionned that 20awh has a fusing current of 60A. How can it blow in 1 second with the two remaining cells ? It is because they will deliver 130A (and not the 20A continuous) ? 

@akhlut
Is there a risk of having the fuses get really hot under normal conditions when using only 24 awg ? @sztamas is talking about 75deg for 7A continuous ?
```

---
## \#5 Posted by: sztamas Posted at: 2018-10-01T14:35:19.210Z Reads: 86

```
[quote="akira, post:4, topic:69722"]
lly hot under normal conditions when using only 24 awg ? @sztamas is talking about 75deg for 7A continuous ?
[/quote]

https://en.wikipedia.org/wiki/American_wire_gauge

If you short the 3p, there will be 3*130A on the main wire, and 130A on each fuse (for the 30q, I am not sure about the LG).
If you go too low the fusing time will be too much, but if you go too high the shorted cell can be damaged.
You should build your battery to not be able to short itself by the parallel groups, but if 1 cell is faulty it can cause shortage, and the other 2 cell will pump 230A trough it. When the fuse blow, you pack should be safe. 
I was not able to run test by myself. but I went with 20.
```

---
## \#6 Posted by: akhlut Posted at: 2018-10-01T14:37:15.503Z Reads: 72

```
Yes, because your P-group is small you'll be pulling lots of amps through each fuse unless you cut back on your batt max in the VESC.  

Fusing is great, but there are downsides too.
```

---
## \#7 Posted by: sztamas Posted at: 2018-10-01T14:40:24.960Z Reads: 70

```
If you check a random metr tracking you will see there is not a lot of continous current, except maybe on hills
https://metr.at/r/5nWnZ
```

---
## \#8 Posted by: akira Posted at: 2018-10-02T10:04:34.657Z Reads: 59

```
@akhlut @sztamas
I guess you are using very different current values for the fusing event. @akhlut is using the continuous discharge and @sztamas is using the max discharge. 

If one uses the continuous to choose the fuse, the wire will be very thin and will run hot even under normal use. If one uses the max discharge, the fuse wire can be chosen larger and will run cooler ... but it will put more strain on the remaining 2 cells to fuse it in case of a short.
```

---
## \#9 Posted by: Blix Posted at: 2018-10-04T14:39:25.394Z Reads: 50

```
I have learned from [his tests](https://www.youtube.com/channel/UCwHeIzOoLgSXHwxTSNSaKXA) that the fusing depends a lot on the distance of the fuse wire and the heatsinks...
In [this](https://www.youtube.com/watch?v=QWZKIr5BcU0) test the 30ga remington industries wire is fusing at 19,6 burst
So everything below that should be good for 15a cells... like the 30q 28/26, maybe 26/24 for 20a...
```

---
