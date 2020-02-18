# How to wire this bms

### Replies: 20 Views: 1041

## \#1 Posted by: Brycehoosiers Posted at: 2017-07-25T18:06:16.074Z Reads: 99

```
<img src="/uploads/db1493/original/3X/8/9/891269bcbb3eb327c5c96f0800dd1b26bdb5dc8b.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/b/b/bba9f92d54517b77fd0963a66a83ee301956afce.JPG" width="375" height="500">

re's are 2 pics, 1 of the 5 wires coming from the bms and one of the 2x 3s to 6s cable.

The 6s cable has a total of 8 wires with a red and black connected in the middle , how do I wire those up two the 5 on the bms and which ones do I leave out or connect together. I will be cutting the end off the 6s jst cable just need to know how to wire the 8 wires to the 5 on the bms
```

---
## \#2 Posted by: darkkevind Posted at: 2017-07-25T18:09:24.786Z Reads: 90

```
Red and black are basically each end of the connector, the others are in the middle but you'll have to see which numbers the colours correspond to on the BMS. If it were in shot I'd be able to tell you...
```

---
## \#3 Posted by: Brycehoosiers Posted at: 2017-07-25T18:20:20.462Z Reads: 93

```
<img src="/uploads/db1493/original/3X/b/3/b392b818bf2aadd4d7ae8c6edd084a23783362e9.jpg" width="375" height="500">

Is this what you need?
```

---
## \#4 Posted by: darkkevind Posted at: 2017-07-25T18:21:47.833Z Reads: 90

```
Ah! They're not labelled! You get any documentation with it?

Looks like red and black may not be the main + and - for the pack...

Are you using the BMS for discharge as well as charge?
```

---
## \#5 Posted by: Brycehoosiers Posted at: 2017-07-25T18:22:45.092Z Reads: 88

```
Just charge
```

---
## \#6 Posted by: darkkevind Posted at: 2017-07-25T18:25:37.687Z Reads: 85

```
OK, any documentation?
```

---
## \#7 Posted by: Brycehoosiers Posted at: 2017-07-25T18:25:58.097Z Reads: 86

```
<img src="/uploads/db1493/original/3X/f/b/fbb4725dd19a56927319e97d28e8527e47431ed1.jpg" width="281" height="500">
```

---
## \#8 Posted by: Brycehoosiers Posted at: 2017-07-25T18:35:58.678Z Reads: 77

```
That's all I could find
```

---
## \#9 Posted by: darkkevind Posted at: 2017-07-25T18:38:59.693Z Reads: 76

```
OK here goes....

<img src="/uploads/db1493/original/3X/4/0/40b55c4a02a76c4c1b912e3ffade8761d8763d3f.jpg" width="374" height="500">
```

---
## \#10 Posted by: Brycehoosiers Posted at: 2017-07-25T18:42:21.067Z Reads: 72

```
Thank you so much I would have had no idea
```

---
## \#11 Posted by: Brycehoosiers Posted at: 2017-07-26T02:11:55.727Z Reads: 58

```
I wired up and plugged it in and left for a while then checked lipo and still same % , how do I check if power is going to the bms?
```

---
## \#12 Posted by: Namasaki Posted at: 2017-07-26T02:18:32.489Z Reads: 59

```
that's a very strange bms. I wouldn't trust my Lipos to that bms. Good Luck to you.
```

---
## \#13 Posted by: Brycehoosiers Posted at: 2017-07-26T02:20:59.512Z Reads: 57

```
What would you trust then?
```

---
## \#14 Posted by: Namasaki Posted at: 2017-07-26T02:22:13.775Z Reads: 56

```
Bestech or Battery Supports.
As far as I'm concerned those are the only suitable brands for this application.
```

---
## \#15 Posted by: Brycehoosiers Posted at: 2017-07-26T02:23:06.574Z Reads: 58

```
Ok I've seen people make them with this bms I just don't know how to use it
```

---
## \#16 Posted by: Namasaki Posted at: 2017-07-26T02:23:44.011Z Reads: 56

```
Do you know what its max discharge rate is?
```

---
## \#17 Posted by: Brycehoosiers Posted at: 2017-07-26T02:24:05.937Z Reads: 55

```
I'm not using it for discharging
```

---
## \#18 Posted by: Namasaki Posted at: 2017-07-26T02:24:53.338Z Reads: 55

```
http://www.batterysupports.com/22v-24v-6s-60a-6x-36v-lithium-ion-lipo-battery-bms-pcm-pcb-p-478.html
http://bestechpower.com/222v6spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
```

---
## \#19 Posted by: Brycehoosiers Posted at: 2017-07-26T02:26:05.006Z Reads: 51

```
Thanks I will see if this one will work and if not I will get one of those
```

---
## \#20 Posted by: Namasaki Posted at: 2017-07-26T02:26:06.216Z Reads: 53

```
you will be if you wire according to the instructions and it looks like it doesn't give you an option since you have to run the main power lead through it because it has not balance pin for cell 6

This is the first bms I've seen that has you running the battery main positive through the bms.

The thing is, if this bms is low power like I think it is, you could wind up with a melt down of the bms and since both your positive and negative battery mains are connected to it, it might possibly short your battery and  your whole board could go up in flames
```

---
