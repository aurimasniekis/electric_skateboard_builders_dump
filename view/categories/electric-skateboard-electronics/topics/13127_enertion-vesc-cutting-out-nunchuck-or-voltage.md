# Enertion VESC cutting out. Nunchuck or Voltage?

### Replies: 10 Views: 707

## \#1 Posted by: Humps428 Posted at: 2016-11-15T22:47:59.702Z Reads: 80

```
I am running the Enertion VESC, Ollin 200KV motor, two 5s Zippy flightmax 5000Mah 20c in series for a 10s set up. First I will also mention I am a total newbie. 
    What I am experiencing is, while accelerating every 2-3 seconds i experience a drop out. I see people claiming voltage dropout and are fixing that issue by adding capacitors. Then I see the others claiming it is the Nyko Kama. I will connect tonight and take screen shot of my BLDC seetings. I have heard some grumblings of the Enertion VESC
    What are were fixes that work for anyone else experiencing this issue?
<img src="/uploads/db1493/original/3X/4/a/4a9292174c56165986607cfe7105df965eeab2af.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/5/4/544b8b8235d050b7249b9292fa71ce39b850736e.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/2/e/2edb88de7b9dd88eb69df9adb7d436c60f1e8bd5.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/b/c/bcf1b36c6b844231eb20d6c150aeb8885bdc679a.JPG" width="666" height="500">
Thank you in advance!
```

---
## \#2 Posted by: chinzw Posted at: 2016-11-17T00:44:20.485Z Reads: 54

```
How long does the cut out last?
Also, when you get a cut out, dont turn off the VESC, keep it on and connect it to a computer, than check for faults, that way we can help you.
```

---
## \#3 Posted by: Humps428 Posted at: 2016-11-18T21:24:45.851Z Reads: 44

```
@chinzw Thank you! as soon as I get some dry weather I will do a another test ride and see what I come up with. Thanks again!!
```

---
## \#4 Posted by: Ackmaniac Posted at: 2016-11-18T21:41:21.159Z Reads: 44

```
Just make it easy for everybody and post Screenshots of your settings. And check your receiver in the enclosure and the connection to the vesc. Make sure it is not too close to the power cables and it doesn't touch any metal.
```

---
## \#5 Posted by: Humps428 Posted at: 2016-11-22T19:36:54.847Z Reads: 41

```
@Ackmaniac
     Posted screen shots and a pic of my kama receiver (which I assume is to close)!
Thank you!
```

---
## \#6 Posted by: Ackmaniac Posted at: 2016-11-22T19:41:54.055Z Reads: 38

```
Set your maximum input voltage on the first screen to 57. It doesn't matter which kind of battery you have. Always set it to this value. And raise your Motor min to -40 or higher like -60 to have better brakes.
```

---
## \#7 Posted by: Blasto Posted at: 2016-11-22T19:43:53.688Z Reads: 37

```
And set your absolute max current to 130A
```

---
## \#8 Posted by: raxell Posted at: 2016-11-22T22:25:27.616Z Reads: 33

```
I have the same issue when I accelerate from zero speed to max throttle. My VESC is from esk8.de and I use Nyko Kama too.
Now I don't accelerate at full throttle. I do it slowly but enough to get speed. I don't know if it is good for VESC.
Someone told me the problem is Nyko Kama.

I have to say that I experience drop out when i accelerate aggressively. I have never experienced drop out running normaly
```

---
## \#9 Posted by: Humps428 Posted at: 2016-11-28T16:29:33.713Z Reads: 24

```
The cut out  was a a pattern, about every 3 seconds it would cut and then almost instantly pick back up. I has been raining so I haven't been able to replicate it to hook up to the computer and check for errors. On another note it also seemed to be less apparent when I rode it in our warehouse.?
```

---
## \#10 Posted by: raxell Posted at: 2016-12-21T17:49:35.690Z Reads: 20

```
Ok, I don't know why, after 3 months of perfect working my nunchuck has become uncontrollable. Lot of random cutoff. BLDC says NO FAULT.
I have change all wires and conections from zero. I have isolated it too and still with the issues...
```

---
