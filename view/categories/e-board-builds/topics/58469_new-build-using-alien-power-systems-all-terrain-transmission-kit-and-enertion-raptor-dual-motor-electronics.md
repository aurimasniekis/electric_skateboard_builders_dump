# New build using Alien Power Systems all-terrain transmission kit and Enertion Raptor dual motor electronics

### Replies: 8 Views: 420

## \#1 Posted by: Atxraider Posted at: 2018-06-10T23:37:40.589Z Reads: 151

```
So, just like the title says, I’m trying to make a build using the enclosure from an Enertion Raptor 1 dual (including battery, 2 VESC-x, Nano remote and receiver, etc) and the Alien Power Systems all-terrain transmission kit with the 6-inch pneumatic wheels and 50mm dual motors https://alienpowersystem.com/shop/cnc-kit/aps-all-terrain-transmission-kit-6-wheels/  
What I am needing help with are the settings I should put into the VESC-x. They are currently using a can-bus connection. Any help would be appreciated. Thanks.
```

---
## \#2 Posted by: onepunchboard Posted at: 2018-06-11T00:34:26.018Z Reads: 130

```
it depends on what riding style u look for. i would put straight 100 motor amp since it is mtb, with 50mm motor, u will need some amp. and I heard canbus in pron to fail the vesc.
```

---
## \#3 Posted by: Atxraider Posted at: 2018-06-11T00:58:09.393Z Reads: 119

```
I thought it wasn’t recommended to put Motor Max above 60A in the VESC, even though it is for a dual motor setup? If the canbus is prone to fail, do you recommend me using a Y setup, where both VESCs go to single nano remote receiver? Pretty sure the Enertion’s Nano remote can’t pair to 2 separate receivers, correct?

[edit] Also, it is not going on a Mountainboard, it’s going on a longboard. The transmission kit isn’t meant for a mountainboard, rather the purpose is to put pneumatic tires on a longboard build.
```

---
## \#4 Posted by: onepunchboard Posted at: 2018-06-11T01:07:44.574Z Reads: 93

```
vescx or focbox is safe to use at 100amps. I'm doing that for a year now.  and yes u have to go with Y set up. nano cant do 2 receivers.
```

---
## \#5 Posted by: Atxraider Posted at: 2018-06-11T01:13:17.064Z Reads: 86

```
Okay, thanks. Is it possible to just solder the servo wires of one vesc to the corresponding servo wires of the other vesc (except the 5V wire) then have the main servo connect to the Nano receiver? 
[edit] That way I wouldn’t have to wait on getting a Y adapter?
```

---
## \#6 Posted by: onepunchboard Posted at: 2018-06-11T01:13:58.873Z Reads: 87

```
correct sir!
```

---
## \#7 Posted by: Atxraider Posted at: 2018-06-11T02:48:30.610Z Reads: 77

```
Would it be better if I switched out the 50mm motors the kit came with, with 2 Enertion R-Spec 6355 motors?
[edit] not sure the drive gear pulley or mounts will support the 6355 motors, but just thought I’d ask.
```

---
## \#8 Posted by: onepunchboard Posted at: 2018-06-11T11:34:57.484Z Reads: 55

```
Yeah def. bigger motor is mor efficient and has better torqu
```

---
