# Help please&hellip;..motor spooling issue/cut out

### Replies: 21 Views: 240

## \#1 Posted by: Hatman30 Posted at: 2018-06-20T12:51:56.714Z Reads: 75

```
I’ve been running my skateboard for a month or two with no problems but I turned it on the other day and now occasionally one of the motors spools up with out the other. When it does the throttle doesn’t respond on either motor and it takes a couple of seconds to stop, by which point both motors are totally fine again.
Has anybody experienced a similar issue or has any advice? Thx
```

---
## \#2 Posted by: linsus Posted at: 2018-06-20T13:21:37.065Z Reads: 73

```
Guessing you mean spins?

Are you using ppm for remote?
```

---
## \#3 Posted by: Hatman30 Posted at: 2018-06-20T13:27:41.435Z Reads: 66

```
The vesc are running master and slave /dual can bus.
```

---
## \#4 Posted by: linsus Posted at: 2018-06-20T13:31:06.168Z Reads: 67

```
yes, but im guessing you dont whisper to the vesc to drive forward, but use some kind of handheld device?
If its a ppm remote and the connector is abit loose the motor can go haywire interpreting the missing signal as full throttle.
```

---
## \#5 Posted by: Hatman30 Posted at: 2018-06-20T13:34:35.945Z Reads: 57

```
Yes it’s a ppm controller . The receiver is hardwired to the master vesc.
```

---
## \#6 Posted by: Hatman30 Posted at: 2018-06-20T13:37:16.891Z Reads: 51

```
If I use full throttle on the remote and then turn it off the motors spin down as they should and don’t go full throttle so it shouldn’t be a connection issue with the remote.
```

---
## \#7 Posted by: linsus Posted at: 2018-06-20T13:38:04.244Z Reads: 47

```
Check the connector just in case, cant hurt. Does it only occour when turning on the board?
```

---
## \#8 Posted by: Hatman30 Posted at: 2018-06-20T13:41:34.356Z Reads: 46

```
Nope , it only happens like once every minute or so. 
I’ll video it when I get home.
```

---
## \#9 Posted by: linsus Posted at: 2018-06-20T13:46:52.402Z Reads: 46

```
Unless its the batteries in your remote starting to go bad.
PPM connector gone loose,
Or the reciever on your board picking up something.

I'd guess its software related. Never experienced something similiar other then with my ppm remote, which I dont use anymore due to safety reasons.
```

---
## \#10 Posted by: Hatman30 Posted at: 2018-06-20T13:55:30.103Z Reads: 44

```
Is an Ollin remote and vesc .
Never had a problem before. Very strange
```

---
## \#11 Posted by: Hatman30 Posted at: 2018-06-20T17:39:27.532Z Reads: 40

```
ok so it's the slave vesc and motor that are starting randomly. Also when it happens the red light on the master vesc flashes 2x3 times
```

---
## \#12 Posted by: trancejunkiexxl Posted at: 2018-06-20T17:48:05.679Z Reads: 39

```
Try calibrating the remote again.. get a vid of it or somfin
```

---
## \#13 Posted by: Hatman30 Posted at: 2018-06-20T17:53:24.100Z Reads: 38

```
getting a fault code DRV 8302 from the master vesc
```

---
## \#14 Posted by: trancejunkiexxl Posted at: 2018-06-20T17:54:54.426Z Reads: 37

```
Damn dude I'm sorry
```

---
## \#15 Posted by: Battosaii Posted at: 2018-06-20T18:19:43.719Z Reads: 35

```
Drv 8302 fault means your vesc needs to pay a visit to the DRV wizard, I have to send in 2 of my Focboxes too
```

---
## \#16 Posted by: Hatman30 Posted at: 2018-06-20T18:20:43.780Z Reads: 35

```
Do u know anybody Uk/ eu based?
```

---
## \#17 Posted by: CarlCollins Posted at: 2018-06-20T18:21:48.805Z Reads: 35

```
@Hatman30

Check the VESC PCB by removing the plastic casing, 
I think something is fried causing DRV error
Also check you setup and wires to avoid this kind of issue in the future
```

---
## \#18 Posted by: Hatman30 Posted at: 2018-06-20T19:11:45.742Z Reads: 28

```
I can’t check the pcb as it’s an old Ollin aluminium enclosed vesc and the heat sinks are glue to it . All my motor wires are sunk into the deck ala LHB style so there’s no chance of the phase wires touching
```

---
## \#19 Posted by: Sn4pz Posted at: 2018-06-20T20:29:27.016Z Reads: 25

```
just summon @chaka :slight_smile:
```

---
## \#20 Posted by: Hatman30 Posted at: 2018-06-20T20:43:35.728Z Reads: 22

```
He’s not on the forum anymore
```

---
## \#21 Posted by: Sn4pz Posted at: 2018-06-20T20:44:24.478Z Reads: 21

```
oh crud.... sorry :o
```

---
