# Blown unity - What component is this?

### Replies: 9 Views: 403

## \#1 Posted by: wannagofast Posted at: 2019-06-30T21:45:51.876Z Reads: 181

```
After a charge (and powering it on to see the battery level) I found out that my board didn't turn on when I wanted to ride it. Opening it up I saw that a component on the Unity's PCB was toast and was wondering what it was so I can try to mitigate it happening in the future. I have the platinum warranty and currently have a ticket out so I'm not worried about replacement but I'd just like to know.  
![20190630_135441|281x500](upload://eoAGF4QESSDznIthWAuNPR8GFi5.jpeg) 

Thanks in advance!
```

---
## \#2 Posted by: Grozniy Posted at: 2019-06-30T22:58:29.077Z Reads: 169

```
That's Jason's pride burning
```

---
## \#3 Posted by: Blasto Posted at: 2019-07-01T00:05:26.765Z Reads: 157

```
According to the chip code it’s a lm5060 from ti, high side driver.
```

---
## \#4 Posted by: longhairedboy Posted at: 2019-07-01T00:27:22.905Z Reads: 150

```
oh shit you blew the master steeze controller. No more steeze now. Damn.
```

---
## \#5 Posted by: Airwolf Posted at: 2019-11-02T04:20:09.498Z Reads: 64

```
Hey Wannagofast,

I have 2 Focbox Unities with the same burnt Component on the PCB.
It has the marking SZAB, and appears to be a generic Component for a LM5060 from Texas Instruments. 

DID YOU FIGURE OUT A WAY TO KEEP THIS COMPONENT FROM BURNING OUT???

Also, Did You try replacing it with a TI LM5060 or another SZAB Component, and if so, did the Focbox Unity Controller start working again after replacing it???

Would really appreciate any insight You might have on this...
```

---
## \#6 Posted by: banjaxxed Posted at: 2019-11-03T20:15:34.672Z Reads: 47

```
Any idea which one from here?

https://ie.farnell.com/search?st=LM5060&aka_sh=1&aka_re=1
```

---
## \#7 Posted by: Deodand Posted at: 2019-11-03T20:49:53.591Z Reads: 43

```
any of those will work. well except the dev board :)
```

---
## \#8 Posted by: banjaxxed Posted at: 2019-11-03T21:17:38.195Z Reads: 42

```
Thanks Jeff, going to see if I can resuscitate this one, do you think this component needs replacing as well?
![image|281x500](upload://qBAvosOcttEH52NrTcdwvpLAeEX.png) 

I’m bench testing a Unity atm with a Photon remote, so far so good, impressive kit 👍
```

---
## \#9 Posted by: Deodand Posted at: 2019-11-03T21:38:21.233Z Reads: 41

```
That's the 3v3 linear regulator, it looks ok to me but if you aren't getting 3.3v then maybe? 

You should also check if any of the fets across the switch are shorted out, should measure open circuit across the front and back of switch fets.
```

---
