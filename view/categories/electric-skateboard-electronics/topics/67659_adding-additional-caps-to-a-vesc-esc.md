# Adding additional caps to a vesc/ESC

### Replies: 14 Views: 625

## \#1 Posted by: Sn4pz Posted at: 2018-09-10T21:33:28.109Z Reads: 107

```
The only reason Ive seen this is to either have long wires or maybe a higher series number in cell count, but when I opened my ownboard ESC today I only saw two little caps .... I was wondering what adding an additional one/two would do :thinking:

would it give me a little more ability to break when the battery is full? im not sure of how much energy is sent back when breaking in relation to the size of the capacitors
```

---
## \#2 Posted by: danielz Posted at: 2018-09-10T21:51:31.757Z Reads: 101

```
The energy stored in a capacitor is tiny. So it wouldnt help for braking, better off adding more batteries in parallel.
https://en.wikipedia.org/wiki/Decoupling_capacitor
```

---
## \#3 Posted by: Sn4pz Posted at: 2018-09-10T21:52:42.528Z Reads: 92

```
ah ok thank you :D 

a 10s2p should be safe to ride down a hill if i stop at 41v right? i weigh 160 and the hills arent steep
```

---
## \#4 Posted by: b264 Posted at: 2018-09-10T21:53:51.986Z Reads: 89

```
Additional capacitors will only give you a few extra milliseconds of braking

If you had a BMS that could bleed cells ("balance") at a few amps or more, you could in theory have unlimited braking but this power would be dissipated in the BMS which means it'd get REALLY hot

Most BMS balance at about 50mA or 0.05 A

You'd need a BMS that could balance at like 5 - 10 A
```

---
## \#5 Posted by: Sn4pz Posted at: 2018-09-10T21:55:03.185Z Reads: 85

```
I understand now :) 

I dont know much about electricity and the components.... might have slept through that unit in physics :relieved::sleeping:
```

---
## \#6 Posted by: pat.speed Posted at: 2018-09-10T21:56:38.386Z Reads: 82

```
The main reason for the caps on a vesc is to smooth out voltage spikes. On my 12s board I have an extra 6x 3300uf caps to protect the TB vescs I’ve heard of a few failures at 12s and so far so good
```

---
## \#7 Posted by: Sn4pz Posted at: 2018-09-10T21:57:36.401Z Reads: 81

```
you must have been the example i had seed previously :) cool board!
```

---
## \#8 Posted by: b264 Posted at: 2018-09-10T21:58:47.302Z Reads: 79

```
[quote="pat.speed, post:6, topic:67659"]
On my 12s board I have an extra 6x 3300uf caps to protect the TB vescs
[/quote]

They will do that but your antispark switch will fail quickly.  I'm assuming you're using a loopkey?
```

---
## \#9 Posted by: pat.speed Posted at: 2018-09-10T22:10:03.380Z Reads: 70

```
As150 bullet
```

---
## \#10 Posted by: danielz Posted at: 2018-09-10T22:27:36.458Z Reads: 70

```
[quote="pat.speed, post:9, topic:67659, full:true"]
As150 bullet
[/quote]

Didnt know they did them in pullet form.
```

---
## \#11 Posted by: ElectricCoast Posted at: 2018-09-11T06:24:50.664Z Reads: 52

```
How do you have six of them hooked up?  Have a picture handy?
```

---
## \#12 Posted by: pat.speed Posted at: 2018-09-11T07:52:27.531Z Reads: 49

```
I can’t seem to upload the picture at the moment, check out the build thread that details it below



https://www.electric-skateboard.builders/t/re-re-rebuild-my-boards-thread/50805?u=pat.speed
```

---
## \#13 Posted by: ElectricCoast Posted at: 2018-09-11T08:07:27.759Z Reads: 45

```
Are they 63v caps or 100v caps?
```

---
## \#14 Posted by: pat.speed Posted at: 2018-09-11T22:38:11.996Z Reads: 32

```
I’m pretty sure 63v I pulled them out of an old 2000w audio amp
```

---
