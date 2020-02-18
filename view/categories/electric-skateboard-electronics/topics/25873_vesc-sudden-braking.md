# VESC Sudden Braking

### Replies: 10 Views: 1003

## \#1 Posted by: vicciu Posted at: 2017-06-21T19:44:59.283Z Reads: 146

```
So I built my first electric longboard about 2 weeks ago and it was amazing. The acceleration and braking torque were really impressive and it was actually really fun considering I never drove a longboard before. That was until about 5 days ago, while riding at about 20-25km/h, the board suddenly braked for no reason and threw me off the board. Fortunately I got just some minor bruises, but that sudden braking kinda stopped me from riding for a few days. Now 2 days ago I decided to test the board while it was upside down(to see if the issue is with the remote or with the VESC) and after about 1 minute of testing one VESC stopped working and any attempt to accelerate would just give the purple blinking light. It turns out the DRV8302 is fried so I'm planning to replace it, but I'm still trying to find out what caused the sudden braking and consequently the death of one VESC. Could it be that the motor shorted? Maybe it's an issue with the VESC?

The parts used in my longboard are the following:
2x VESC
2x Turnigy SK3 5045 450kV
3x 6S 3000mah lipo batteries in parallel
The wheels are 83mm and the gearing is 14:36
The VESC is controlled via PPM from an NXP FRDM board(similar to arduino) that is connected to my mobile phone via bluetooth.
```

---
## \#2 Posted by: Pantologist Posted at: 2017-06-21T19:52:24.150Z Reads: 142

```
7 poles x 22V x 450kV = ~70k eRPM which is about 10k over the 60k limit. That is probably what fried it.
```

---
## \#3 Posted by: vicciu Posted at: 2017-06-21T19:59:49.325Z Reads: 135

```
it is true, spinning the wheels in the air does trigger the VESC 60K eRPM limit, however is this enough to fry an VESC? I would assume it has some sort of protection against this. Also do you have any possible causes for the sudden braking?
```

---
## \#4 Posted by: Vieo Posted at: 2017-06-21T21:40:01.363Z Reads: 115

```
Sudden Breaking: If you fried the DRV8302 while riding that could mean random (electronic) stuff happens with-in the VESC and cause weird (breaking) stuff? Just a guess though..
```

---
## \#5 Posted by: vicciu Posted at: 2017-06-21T21:53:59.436Z Reads: 105

```
Sorry if I wasn't clear, but it was the sudden braking that happened during driving. The DRV8302 got fried while testing it with the wheels in the air and hitting the max eRPM a few times.
```

---
## \#6 Posted by: Mattmccrary8 Posted at: 2017-06-21T22:06:45.627Z Reads: 99

```
That's your fail safe, rebind your remote. It happened to me at 24mph on my first ride lol
```

---
## \#7 Posted by: Alanhunt123 Posted at: 2017-06-22T01:07:52.068Z Reads: 88

```
This phenomenon of sudden braking followed by DRV error has happened to me several times. Every time was due to a short on my motor wires. Doh!

Makes perfect sense though, since when you short motor wires in the absence of any motor controller, the motor brakes as hard as it can. The first time it happened, I failed to properly insulate the bullet connectors by taping them individually with electrical tape. The second time, a sharp edge on my custom aluminum case ate through the wires and caused a short. Both times could have easily been avoided had I properly set up my motor wires in a way that they wouldn't be damaged!
```

---
## \#8 Posted by: pennyboard Posted at: 2017-06-22T02:01:17.589Z Reads: 78

```
I second what @Alanhunt123 said. I've fried a DRV chip through shorting the phase wires. It happened exactly as he described. 
I don't think it was the eRPM limit cause I run 12s on 192kv which is about 67,000 RPM and never had any problems.
```

---
## \#9 Posted by: vicciu Posted at: 2017-06-22T04:21:51.656Z Reads: 67

```
Thanks for the suggestion guys. Just checked and I might've made the same mistake as Alanhunt123, my motor wires weren't insulated too well(about 1mm of the gold connector is visible when connected). Now they are wrapped completely in heatshrink so I hope after the DRV replacement this won't happen again.
```

---
## \#10 Posted by: Alanhunt123 Posted at: 2017-06-22T12:43:59.663Z Reads: 60

```
That will definitely reduce your chances of frying your next DRV. Best of luck to you!
```

---
