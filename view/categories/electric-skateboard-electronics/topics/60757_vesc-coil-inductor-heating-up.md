# VESC coil/inductor heating up

### Replies: 5 Views: 283

## \#1 Posted by: Brando Posted at: 2018-07-03T00:47:18.179Z Reads: 78

```
Hey all. I have a dual focbox setup and one of them started heating like crazy just by being turned on. the FET temp rose steadily past 60C degrees before I let it go further. The other focbox sits nicely at around 30C.
The coil/inductor that says 202 on it is the source of the heat. I believe this is the link to buy a replacement: [SDR0805-220ML](https://www.mouser.com/ProductDetail/Bourns/SDR0805-220ML/?qs=y9m3SKnhpLMnaY53wPhSdA%3d%3d&gclid=CjwKCAjwmufZBRBJEiwAPJ3LpmyKb03NJa8QR74xpZi3EbTDq-vj1nZPxqukJykEWO9HsJyB-WzkhxoCEEsQAvD_BwE)
The replacement is SUPER cheap but something tells me the source of the problem is somewhere else. There are no fault codes reported by the VESC Tool.
here is a picture of my focbox
![image|666x499](upload://eDYJX8HPexelU3j3mzIwnA1X0Db.jpg)
```

---
## \#2 Posted by: laurnts Posted at: 2018-07-03T02:12:57.300Z Reads: 59

```
Either buck converter or DRV issues, I had the same issues before and VESC not powering up.
```

---
## \#3 Posted by: Brando Posted at: 2018-07-03T03:12:27.578Z Reads: 53

```
The weird part is that the VESC still powers up.
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2018-07-03T05:22:23.133Z Reads: 45

```
Tvs diode that protect the 5V is probably heating up... are you using dual PPM or is the 5v or 3,3V use by something else?
```

---
## \#5 Posted by: Brando Posted at: 2018-07-04T14:18:16.732Z Reads: 19

```
I use ppm and canbus. The slave vesc is the one that has issues. All cables, including motor are disconnected now though.
Are there repair stores in the U.S. BTW?
```

---
