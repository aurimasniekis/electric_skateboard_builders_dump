# Confirming vesc setting for 6s

### Replies: 8 Views: 772

## \#1 Posted by: Lutsivo5703 Posted at: 2017-04-21T22:01:25.982Z Reads: 107

```
I am running a 6374 230kv motor, 2x 6s 5000mah batteries in parallel for a total of 6s 10000mah. I just got a vesc and wanted some opinions on vesc setup. Here is what I got so far.

Motor max:     80a
Motor min(regen):   -30a
Batt max:  50a
Battery min(regen):    -6a

Are these good settings? I just don't want to fry anything.
```

---
## \#2 Posted by: Luke Posted at: 2017-04-21T22:40:04.515Z Reads: 99

```
I would see how that goes, however I would suggest settings such as : 

Motor max: 60a
Motor min(regen): -50a
Batt max: 45a
Battery min(regen): -5a 

Battery cutoff start: 22v
Battery cutoff  end: 21v

...or something along those lines
```

---
## \#3 Posted by: Lutsivo5703 Posted at: 2017-04-21T23:17:35.324Z Reads: 90

```
Ok thank you so much I will give it a try!
```

---
## \#4 Posted by: Lutsivo5703 Posted at: 2017-04-22T02:09:43.917Z Reads: 82

```
I'm not sure what is happening but on higher speed the motor cuts out for some reason? It doesn't  apply brakes it just cutts out. What could be the reason?
```

---
## \#5 Posted by: Evan97 Posted at: 2017-08-19T21:42:52.581Z Reads: 50

```
I have the same problem
```

---
## \#6 Posted by: onepunchboard Posted at: 2017-08-19T21:58:10.378Z Reads: 47

```
it might be cuz of the regeneration amp is too little.
```

---
## \#7 Posted by: EL_PAPI_CHULO Posted at: 2017-08-22T01:39:38.936Z Reads: 43

```
i have the same problem in one of my motors
i will see if i can fix it
```

---
## \#8 Posted by: Deckoz Posted at: 2017-08-24T16:46:52.534Z Reads: 36

```
If you motor is cutting out, it could be your cells sagging below the cuttoff voltage...

if you want to keep it from sagging, lower your battery max to a point that it doesn't sag. ie

Lets take lipos for example 

Lipos are rated in C ratings. so if your Lipo has a 10C discharge rating, You would multiply your total capacity times the C count. IE 10aH of capacity X 10 = 100amps of constant current capability - don't set it this high as its higher then the VESC can handle..but you get my point

If you are using Li-ions, and the cells have lets say at 20Amp constant current discharge,  you have 2X 20Amp constant current series packs in parallel, your max continuous would be 40amps. 

Throw up some more info on your battery and we can determine what your Battery max should be(in constant current numbers). I don't suggest setting your battery max higher then the constant current capabilities. As well if you are dual motor you will need to divide this constant current capability between two vesc's... ie if your battery max CC is 40amps, each vesc would have 20amps set as the battery max.
```

---
