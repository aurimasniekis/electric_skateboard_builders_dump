# VESC and BLDC Tool without USB

### Replies: 9 Views: 1067

## \#1 Posted by: Stefan Posted at: 2017-03-17T18:16:00.751Z Reads: 116

```
Hey everyone,

the USB port of my VESC broke. I tried to repair it but with no success. Does anyone know if it is possible to communicate with the VESC in BLDC tool without using the USB port? I am running Ackmanics modded firmware on the VESC btw. and i plan on switching from single to a dual motor setup with new motors so i need to do a motor detection with that VESC soon...
```

---
## \#2 Posted by: Blasto Posted at: 2017-03-17T18:23:20.666Z Reads: 109

```
Can always drop @JohnnyMeduse a msg to get it repaired

 http://www.electric-skateboard.builders/t/johnny-vesc-repair-services-now-with-soldering-tips/11267?u=blasto
```

---
## \#3 Posted by: JLabs Posted at: 2017-03-17T18:23:35.848Z Reads: 106

```
Not really, only thing I can think of is to get a Bluetooth module and program it from there. Although it is limited to what exactly you can do it's better than nothing.

P.S. How did you manage to break the USB ok the VESC?
```

---
## \#4 Posted by: Stefan Posted at: 2017-03-17T18:45:01.092Z Reads: 98

```
Unfortunatly i live in Germany, that would be an expensive option..
```

---
## \#5 Posted by: Stefan Posted at: 2017-03-17T18:49:48.473Z Reads: 93

```
I do have a bluetooth module (i think it is a HM-10) that is also working with Ackmaniacs VESC Monitor app. But it does not support motor detection or changing between FOC and BLDC. I am not sure if other apps support these features but e.g. the VESC Connect app is not working with the current firmware installed on the VESC.

The VESC was not even old at all, the port just fell off after maybe 20x plugging and unplugging within the first maybe 20 days :confused:
```

---
## \#6 Posted by: Luke Posted at: 2017-03-18T01:27:55.731Z Reads: 79

```
This also happened to me after about 5-10 plugging ins
```

---
## \#7 Posted by: Montiey Posted at: 2017-03-18T02:30:50.881Z Reads: 73

```
The port fell off? Which pads? Thing's don't just fall off. And usually, USB mini and micro ports can often times be stronger than the PCB itself. I would blame cold solder, but that doesn't help you now… So, do you have a hot air station? USBs aren't hard to attach, but that also depends on the condition of the pads.
```

---
## \#8 Posted by: Nordle Posted at: 2017-03-18T07:29:48.047Z Reads: 58

```
I have the same problem with one of my Vesc's is it possible to program with I2C module?
```

---
## \#9 Posted by: Stefan Posted at: 2017-03-18T07:30:04.071Z Reads: 54

```
Well, maybe it was a cold solder, I don't know. Eitherway i tried to resolder it a few times with a lot of flux but the VESC will not connect to my computer.
```

---
