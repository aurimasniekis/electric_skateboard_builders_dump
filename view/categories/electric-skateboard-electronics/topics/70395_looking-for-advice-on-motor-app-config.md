# Looking for advice on motor/app config

### Replies: 5 Views: 336

## \#1 Posted by: Gdunn416 Posted at: 2018-10-07T01:10:07.364Z Reads: 97

```
I just completed this build here - [12s4p - dual focbox - dual 6374 190kv](https://www.electric-skateboard.builders/t/name-coming-soon-ly-evo-tb-218-dual-6374-190kv-12s4p-30q-dual-focbox-metr/)

It connects to the Ackmaniac ESC Tool via a Metr Pro module. I have configured it in FOC Sensored mode, and the motors are spinning perfectly. Does anyone have any recommended changes I should make to the motor and app configs below before I let this thing move me around the streets? Thanks to anybody that wants to help!

I realize this is a lot of screenshots to dump here. Please let me know if there is a simpler or cleaner way to do this!

**Motor / Additional Info**
![Motor%20Additional%20Info%20General|690x204](upload://q4nwWbuZt4az3GSSj9roZtyjtnI.png) 

**Motor / BLDC section** 
![Motor%20BLDC%20General|690x97](upload://n1tH4d4YvZtDfMfzm51Vrl6ESxd.png) ![Motor%20BLDC%20Sensorless|690x124](upload://9zMpMqURYC74GDjQsX7WG6BJ7SR.png) ![Motor%20BLDC%20Sensors|690x224](upload://3Ia16wETtWoC2PnTW912iEVAk5d.png) 
![Motor%20Sensors%20Advanced|690x224](upload://3F2WWhqfR56LWmDh9S9taZWMDkT.png) 

**Motor / DC section**
![Motor%20DC|690x113](upload://qZGGAgj1zzv6CzNjDag6idfQua.png) 

**Motor / FOC section**
![Motor%20FOC%20Encoder|690x126](upload://trKeC8ujsikqHGZz8Fo0aYb5bTp.png) ![Motor%20FOC%20Advanced|690x261](upload://cDPnwfPnYeyj6vZXWAmyxpybatR.png) ![Motor%20FOC%20General|690x167](upload://oyLpXmvPYMWSUcPwA5J9h47Ub3N.png) ![Motor%20FOC%20Hall%20Sensors|690x221](upload://9ui8yd8K9JRS1k7yF9t2PbR9N2z.png) ![Motor%20FOC%20Sensorless|690x157](upload://uqZVykHUwTq1zEkOwle19UX6re4.png) 

**Motor / General section**
![Motor%20general%20general|690x145](upload://tYu5cTcNgHWtC0OnuwGVPPePg9L.png) ![Motor%20General%20Advanced|690x180](upload://eV6e5GQqPvMjZxkC78cUz9Y5Z5T.png) ![Motor%20General%20RPM|690x114](upload://fRzFjSXFwCz4BknU1jo9nW0EZtU.png) ![Motor%20General%20Current|690x309](upload://yEtEJxxI0hvyUHG42FDQEVCzNce.png) ![Motor%20General%20Temperature|690x177](upload://esxczF2GDkixN9o3G9oxMYPZJol.png) ![motor%20general%20voltage|690x97](upload://a4DGoN7DHOdpfpKksGvBLMKpGsA.png) 

**Motor / PID section**
![Motor%20PID|690x243](upload://58m8veLs1hFbKqqLMCKL52E4AGT.png) 


**Here are screenshots under the "App" section**
![App%20General|690x176](upload://x386ZtlnUVGAvMeJ3XOnDwmtkLo.png) ![App%20PPM%20General|690x343](upload://k1qaiZ7YJrA9YHOZq4IgWy5PKJJ.png)
```

---
## \#2 Posted by: Gdunn416 Posted at: 2018-10-08T23:22:14.417Z Reads: 53

```
Does anybody see any obvious changes that should be made? I think it's all probably OK, but it would be cool is someone with more experience had a look at it too.
```

---
## \#3 Posted by: Andy87 Posted at: 2018-10-09T10:04:35.909Z Reads: 50

```
looks good so far.
you set the max erpm to 60000
the bat cut off is right
the motor and battery max min values seam ok too ( just don´t break down a 3km hill with -20a batt min ;) )
if motor detection was running well and your remote adjusted properly (inclusive fail save) than give it a go.
```

---
## \#4 Posted by: Gdunn416 Posted at: 2018-10-09T15:48:07.226Z Reads: 49

```
Thank you for looking over the settings. If I decide to head west toward the beach, I'll have to go down a hill for about a mile. The elevation is a couple hundred feet.  For those situations, should I change the battery to -10a?
```

---
## \#5 Posted by: Gdunn416 Posted at: 2018-10-19T16:36:02.123Z Reads: 49

```
So far everything is running great. Thanks again for looking it over.
```

---
