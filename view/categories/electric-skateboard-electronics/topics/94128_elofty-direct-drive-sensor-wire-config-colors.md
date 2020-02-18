# eLofty direct drive sensor wire config / colors

### Replies: 7 Views: 371

## \#1 Posted by: on1y Posted at: 2019-05-17T09:09:30.478Z Reads: 172

```
So I’ve had a bunch of DDs. Metasurfs, carvon speed drives, Carvon torque drives, raptor 2, my buddy has the torque board dd’s. I just recieved the lofty dd motors. I noticed that the sensor wire is 5 pin instead of 6. Which wire is missing? Is it temp? To plug into my , would it go, ground(black), next pin empty, h1, h2, h3, 5v(red)? The sensor wire coming out of the motors goes black blue green yellow red. Do I just connect it into a 6 pin in the same order, except leave the second pin blank and move the other ones over one? I tried and it doesnt show up on motor detection. My motor had trouble detecting also, first time I had to raise the current to get it to spin up. Any help would be appreciated. I’ve built numerous boards over the past three years, so spare the newb comments please. Its prolly something dumb I missed but dunno what. Lemme kno if u need pics. It’s all heat shrinked up atm.
```

---
## \#2 Posted by: Andy87 Posted at: 2019-05-17T09:15:28.973Z Reads: 163

```
you can check the pin out on the lable of the esc.
usually it´s 

5V,temp,h1,h2,h3,GND

if you have only 5pins than it´s likely the temp is missing. means the one next to 5V should be free.
```

---
## \#3 Posted by: b264 Posted at: 2019-05-17T09:42:00.907Z Reads: 145

```
Usually,
* black is ground  
* red is 5V  
* white is temperature, and may or may not be present  


and the other three are typically  
* orange, green, yellow  
or  
* blue, green, yellow  
or  
* brown, green, yellow

and those three can be in any order.  The hall sensor table will be found when you do motor detection.

Of course, some motors may not conform to this normality....
```

---
## \#4 Posted by: Halbj613 Posted at: 2019-05-17T10:49:05.412Z Reads: 115

```
you can buy a converter from a couple of websites including flipsky
```

---
## \#5 Posted by: mishrasubhransu Posted at: 2019-05-17T20:29:13.112Z Reads: 75

```
Like @b264 said. I did the same with my eLofty.
```

---
## \#6 Posted by: Jansen Posted at: 2019-05-17T21:31:57.664Z Reads: 65

```
You check the elofty thread B? I believe I remember seeing someone post a diagram of the wire diagram for it....
```

---
## \#7 Posted by: on1y Posted at: 2019-05-18T06:16:24.619Z Reads: 50

```
Boom got it. I will the pcb layout is diff than what's written on the case. I annoying. Ithe sensor wires I got from baggy boards is legit. It comes w a round plug that seperates. And is weatherproof. Thank y'all for the help!
```

---
