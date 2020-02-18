# VESC Electrical Issues

### Replies: 8 Views: 1447

## \#1 Posted by: Jack Posted at: 2016-01-03T11:09:14.210Z Reads: 79

```
Hi guys I have ordered my VESC boards and soldered all the components as per the bom but I think I may have a short somewhere. I powered on the board with a 12v supply and the board gets quite warm. Especially the USB Jack and none of the LEDs light up. Also when I plug in the st link v2 to program the micro the led on the st link goes out when I plug in the 3.3v I'm guessing this is the short. 

Any ideas would be much appreciated as I'm really exited to get the VESC up and running!
```

---
## \#2 Posted by: EnertionSupport Posted at: 2016-01-03T13:52:19.903Z Reads: 73

```
Post some close-up photos and I can have a look for you.
```

---
## \#3 Posted by: Jack Posted at: 2016-01-03T19:05:34.329Z Reads: 65

```
Thanks for that, here are the photos.

I haven't added the connectors yet as they are on order. 

Cheers, Jack<img src="/uploads/db1493/original/2X/9/99877a5537fbe993ebfc5d2855532c622c765d93.jpeg" width="375" height="500"><img src="/uploads/db1493/original/2X/8/865c8a780c00ac908abd2c493e5fdcbdb5c477c3.jpeg" width="375" height="500">
```

---
## \#4 Posted by: EnertionSupport Posted at: 2016-01-03T19:17:08.098Z Reads: 67

```
check this area again: 
<img src="/uploads/db1493/original/2X/b/b40fb4d135279481fe4fa7bc7c3907b61419909f.jpeg" width="375" height="500">
it looks like there might be some extra unwanted solder bridges. I would also thoroughly look over all of your solder joints for anything else that might be causing a problem.
```

---
## \#5 Posted by: Jack Posted at: 2016-01-03T19:51:13.999Z Reads: 66

```
Yeah It looks worse in the photo but I'm sure those pins are joined anyway? Ive added another photo of the DRV chip for clarity. 

I've checked the board for around 2 hours also probing pads to check for shorts. Just wondering if anyone else has had a similar issue. It seams strange that when I apply 12v the whole board seams to warm up, not sure if that could mean anything!

Thanks for your help :smile:<img src="/uploads/db1493/original/2X/b/bdf546c20cd9fabb1272da2f85e7f885d1f11db1.jpeg" width="666" height="500"><img src="/uploads/db1493/original/2X/5/58310c10be1dafb0df754d6b24a6f6cf80864ca4.jpeg" width="666" height="500">
```

---
## \#6 Posted by: Jack Posted at: 2016-01-03T20:09:59.677Z Reads: 66

```
Quick update, I've gone over most of the pads just reflowing the solder and now something makes a low pitch clicking noise I think it's the DRV but I'm not 100% and I'm not sure if that's progress or I've screwed it up haha!
```

---
## \#7 Posted by: Jack Posted at: 2016-01-03T21:48:07.573Z Reads: 66

```
Update No 2

Okay so that buzzing was coming from the 3.3v voltage regulator. After looking at this thread 

http://www.electric-skateboard.builders/t/failed-vesc-help/426

I have a short between the 3.3v and ground but can't find what's causing it. I've removed the voltage reg and the left pad and middle one (gnd) are connected. Not good :frowning: 

Is there any other components that I may have damaged from the 3.3v short? Cheers
```

---
## \#8 Posted by: makepeace Posted at: 2016-04-25T18:09:34.146Z Reads: 45

```
I'm having the same issue. I have a short between the 3.3 V plane and ground. I didn't actually solder the board, I'm testing it for someone. Not being able to program it is the first issue I'm having :P. Everything looks pretty good on the face of it, apart from the usual DRV bridges, which I've checked against the schematic and are okay. Did you get any luck?
```

---
