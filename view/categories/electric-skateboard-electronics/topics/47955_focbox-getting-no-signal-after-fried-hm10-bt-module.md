# Focbox getting no signal after fried HM10 BT Module

### Replies: 18 Views: 553

## \#1 Posted by: Acido Posted at: 2018-03-02T17:48:06.284Z Reads: 115

```
So I got a splash of water in my enclosure, only the module died,all else is okay.
But the fucking focbox is not getting any signal from the reciever, ppm tab is always at 50%
The remote pairs instantly like before, and guess what
this all happened 10meters away from the endpoint, and thats my house


What should i do?
There are no faults in the focbox and I have no other reciever to check if its the recievers fault
Also the reciever is turned on, theres the red light

Motor is spinning when i send the signal with pc with my keyboard... So I guess it should be the reciever?
```

---
## \#2 Posted by: ShutterShock Posted at: 2018-03-02T18:38:52.638Z Reads: 111

```
Yeah I agree it sounds like the receiver here.  What remote do you use?  I think the GT2b replacement receivers can be acquired quite easily.

My guess is that some of the water splashed on the receiver pins and shorted out the connection that goes to the focbox or something along those lines.  Do you have another controller/receiver that you could test it with?
```

---
## \#3 Posted by: Acido Posted at: 2018-03-02T18:53:15.788Z Reads: 98

```
I bought 2 enertion remotes, winning ones
First failed on the first connection it just sparked and died, and now the second is dead..
I will try to source an receiver somewhere...
Could there be a short on focboxes side of the reciever? Since the reciever lights up... Is there an way to connect the reciever to uart port?
```

---
## \#4 Posted by: Namasaki Posted at: 2018-03-02T19:37:29.940Z Reads: 87

```
The module and the receiver both run off of the same buck converter so my first thought was that when you shorted the module, it shorted the buck converter. 
But if the receiver is still turning on with the focbox, then the buck converter must be ok.
```

---
## \#5 Posted by: Acido Posted at: 2018-03-02T19:39:48.631Z Reads: 86

```
I will get the multimeter from my car tomorrow and check the pins if they shorted...
```

---
## \#6 Posted by: Namasaki Posted at: 2018-03-02T19:40:33.674Z Reads: 83

```
Is the receiver turning on with the focbox or not?
```

---
## \#7 Posted by: Acido Posted at: 2018-03-02T19:44:50.800Z Reads: 79

```
It is, the fucker even pairs with the remote and bind function is working...
```

---
## \#8 Posted by: Silverline Posted at: 2018-03-02T20:37:57.197Z Reads: 74

```
Do you by any change have a simple servo tester ?
```

---
## \#9 Posted by: Namasaki Posted at: 2018-03-02T21:16:05.412Z Reads: 68

```
Guess the buck converter is not fried then.
```

---
## \#10 Posted by: Acido Posted at: 2018-03-03T07:21:06.319Z Reads: 55

```
Nah, I dont..
```

---
## \#11 Posted by: Acido Posted at: 2018-03-03T07:22:09.520Z Reads: 53

```
Did you consider the burnt hm10 module on the uart port? Maybe something is dead there.. Would it affect the remote?
```

---
## \#12 Posted by: Namasaki Posted at: 2018-03-03T11:34:50.351Z Reads: 48

```
I don’t think so but I’m no electronics expert either
```

---
## \#13 Posted by: Acido Posted at: 2018-03-03T11:49:49.908Z Reads: 46

```
Could water splash damage the sensor pcb?
Since Im getting failed results on sensor detection in foc and bldc
```

---
## \#14 Posted by: stewii Posted at: 2018-03-03T13:13:32.016Z Reads: 41

```
You better chance is to clean the PCB and the contacts with isopropyl alcohol
```

---
## \#15 Posted by: Acido Posted at: 2018-03-03T14:45:49.095Z Reads: 36

```
Recievers problem solved, but the sensors dont work for some reason, lets see how its to ride without them...
Could water damage them?
```

---
## \#16 Posted by: Nordle Posted at: 2018-03-04T12:03:47.415Z Reads: 29

```
A short kills sensors almost everytime :(
```

---
## \#17 Posted by: Acido Posted at: 2018-03-04T12:11:56.746Z Reads: 31

```
For some reason i can start slowly motor is quieter, now i only hear my non aligned chain :smiley:
I also switched to foc and am riding with no problems
```

---
## \#18 Posted by: Acido Posted at: 2018-03-04T12:12:24.623Z Reads: 31

```
All problems solved, idk how to close this
```

---
