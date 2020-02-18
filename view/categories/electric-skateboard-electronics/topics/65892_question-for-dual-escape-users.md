# Question for dual ESCape users

### Replies: 9 Views: 317

## \#1 Posted by: Taliesin Posted at: 2018-08-23T22:47:14.523Z Reads: 114

```
I have individually set identical motor settings through vesc tool and I am about to configure my remote but I’m not sure if my ESCapes are connected to each other or not.

Do I need to connect this 4 prong can bus from one escape to the other? Or does the ppm y splitter I already have connected to both take care of that?

![image|374x500](upload://xr0fmqIQJoMuAvAOn5G33fRmLcm.jpeg)![image|666x500](upload://sSZiHw3HdXO5N17D31JUjv17yDX.jpeg)
```

---
## \#2 Posted by: mccloed Posted at: 2018-08-23T22:50:52.419Z Reads: 103

```
Looks like you have a split PPM. You would want to set them both up individually.
```

---
## \#3 Posted by: Taliesin Posted at: 2018-08-23T22:55:00.135Z Reads: 98

```
So click “my setup has a single vesc.” ??
```

---
## \#4 Posted by: danielz Posted at: 2018-08-23T22:56:20.011Z Reads: 96

```
If you arent using can yes.
```

---
## \#5 Posted by: Taliesin Posted at: 2018-08-24T01:14:13.406Z Reads: 75

```
Benefits of split PPM vs can bus?
```

---
## \#6 Posted by: dg798 Posted at: 2018-08-24T02:39:59.160Z Reads: 68

```
split ppm in my opinion is safer then canbus. there is more that can go wrong with can then ppm
```

---
## \#7 Posted by: Colson003 Posted at: 2018-08-24T02:43:47.778Z Reads: 64

```
Can’t remember what thread it was but trampa said don’t use split ppm on version 6 hardware. Just use can.
```

---
## \#8 Posted by: dareno Posted at: 2018-08-24T09:19:22.166Z Reads: 52

```
Thats to do with the can bus being safer on the 6 variant.  Split ppm is fine so long as the voltage is not duplicated across both vescs which his aren't.  Apparently all the problems with can bus on 4 are now not evident on 6   want to put that to the test?   Nah fxxk that!!:sweat_smile:
```

---
## \#9 Posted by: dareno Posted at: 2018-08-24T09:22:54.814Z Reads: 50

```
[quote="Colson003, post:7, topic:65892"]
but trampa
[/quote]

Vive la revolution!!
```

---
