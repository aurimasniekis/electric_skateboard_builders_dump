# Balanced LiPo Battery Build for E-MTB

### Replies: 13 Views: 1440

## \#1 Posted by: TheCheat Posted at: 2017-02-03T21:25:24.730Z Reads: 148

```
While I'm trying to figure out how to fix my blown VESCs, I might as well kill some time and do a quick post on how I built my balanced LiPo battery for my E-MTB.

Materials:
1x Pelican 1200 case
3x 5000mah Hard Cased Lipo Battery
1x 48v 2.5ah scooter charger from Ebay
1x 40a 12S BMS from Ebay
1x Velcro with adhesive side


I started off with the LiPo batteries. I'm not going to bother taking them apart because I'm lazy. Instead I'm going to directly connect their balance wires to the BMS.

The Ebay BMS actually came with its own 12 pin balance cable, so the first thing to do is to liberate that 12 pin connector.
<img src="/uploads/db1493/original/3X/d/b/dbc947675150f3dc95982f225e34353d0c988c8d.JPG" width="666" height="500">


I do the same to the LiPo batteries, and begin transplanting the freed balance wires into the 12 pin connector. Balance leads are live, so it's best to do one at a time.
<img src="/uploads/db1493/original/3X/3/7/37b3905e02d1d98bb7f5d0ea3a741f212d781736.JPG" width="666" height="500">


Did this for all the batteries. Eventually ended up with this. Also note how I excluded all the black balance leads.
<img src="/uploads/db1493/original/3X/7/6/762cd9fe10e9c5247468880af7266aa02ac9b003.JPG" width="666" height="500">


Now time to connect the batteries. I cut off all the plugs and tried to make the connecting wires as short as possible.
<img src="/uploads/db1493/original/3X/4/0/406c2a86bc700a548d4985f6fd5b500e87fba190.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/0/a/0a93330805ec25b6359e8a855602163729d18da4.JPG" width="666" height="500">


The final result ended up looking like this.
<img src="/uploads/db1493/original/3X/1/0/101f8394a9e8144466bdaae48e0ad9a0e131b021.JPG" width="666" height="500">


Now to wire up the BMS power leads. Firstly I didn't take pictures of this part (my bad), but there are plenty of guides on exactly how to do this, so take a quick look around. However the important part that I have to stress is that my BMS has a 40a fuse. You CANNOT connect your ESC to the power out on the BMS, unless you want to blow that fuse. Instead, I wired the power out plug directly to the LiPo battery(s).

Here's the final result after I fitted everything into the Pelican 1200 case.
<img src="/uploads/db1493/original/3X/a/2/a25096a5e09d4d067d10ca8545e72cd543803f6c.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/a/a/aa2fa34b64ba7e47432c6723143a948ad5760e20.JPG" width="666" height="500">

Final Notes:
The bullet connectors that I cut off the batteries were later reused as charging connectors for the scooter charger and the BMS. 
The power out of the battery is an XT90 connector
Holes were drilled in the back (close to the bottom) of the Pelican 1200 case
Everything you see in the final product is either Velcro'd or Friction fitted
Charging is as simple as plugging this thing into a wall socket
I sneeze in order to detect the polite people in the room
```

---
## \#2 Posted by: Okami Posted at: 2017-02-03T21:28:18.628Z Reads: 130

```
Nice work! How many hours did you put into this?

The lipo ''solution'' looks really neat.. I assume it is rather easy to work with ''lipo bricks'' if you got plenty of space to fit them :)
```

---
## \#3 Posted by: TheCheat Posted at: 2017-02-03T21:34:02.877Z Reads: 128

```
More or less 2 hours. My dumb ass forgot I had flux paste among the contraband items I packed for my dorm. Even then, the entire idea of this build is to minimize on soldering and make the process as simple as possible.
```

---
## \#4 Posted by: Okami Posted at: 2017-02-03T21:38:41.237Z Reads: 122

```
[quote="TheCheat, post:3, topic:17165"]
contraband items
[/quote]

This does sound fun haha :D

So are you doing all of the stuff in the dorms?
```

---
## \#5 Posted by: TheCheat Posted at: 2017-02-03T21:41:59.859Z Reads: 114

```
Pretty much. There's a Maker Space on campus, but I don't feel like going to 'training' for 3 hours in order to use a soldering iron. Also the ME and EE departments won't help (i'm a CE major) so I'm on my own.

It's even more funny that my RA shares the same wall as me.
```

---
## \#6 Posted by: Okami Posted at: 2017-02-03T21:46:57.251Z Reads: 112

```
Mh Im not sure what ''RA'' stands for.. though sounds like you have landed in technology related uni ;)
```

---
## \#7 Posted by: TheCheat Posted at: 2017-02-03T21:48:29.521Z Reads: 104

```
The guy/gal that writes you up for being too noisy on a Saturday night.
```

---
## \#8 Posted by: Okami Posted at: 2017-02-03T21:51:27.254Z Reads: 106

```
What time zone you have? Sorry for going off topic but its related to building battery in a dorm, I assume..

I once got smoke detector activated.. because of the solder / flux fumes :D So couldnt say that it is fun building anything in dorms, where soldering is required :)
```

---
## \#9 Posted by: TheCheat Posted at: 2017-02-03T21:57:56.753Z Reads: 106

```
Pacific Time Zone, San Diego CA.

<img src="/uploads/db1493/original/3X/f/2/f259ca6939ed3f255e66e409848c79b1e6255e9e.JPG" width="666" height="500">
For many things including soldering
```

---
## \#10 Posted by: Okami Posted at: 2017-02-03T22:43:04.688Z Reads: 96

```
haha :D yeah I've heard from others to just disable it .. to be done with it :D
```

---
## \#11 Posted by: NNGG Posted at: 2017-02-04T07:59:39.181Z Reads: 79

```
Finally more people in San Diego.
```

---
## \#12 Posted by: TheCheat Posted at: 2017-02-04T08:45:52.421Z Reads: 79

```
You don't happen to be the kid ridding around on campus are you?
```

---
## \#13 Posted by: NNGG Posted at: 2017-02-04T09:28:33.747Z Reads: 79

```
Naw I'll post pics of a build for a nephew soon
```

---
