# Flipsky Sensor to Foxbox issue&hellip;wiring?

### Replies: 16 Views: 432

## \#1 Posted by: J95hicks Posted at: 2018-12-20T22:16:54.908Z Reads: 104

```
Hey guys, i have a sensored Flipsky motor and as i have everything in front of me it seams i cannot connect the sensor. Flipsky sensor pins dont line up to foxbox, they are much closer together..... please help![1545344242448451429059|375x500](upload://i242qmRAWrXNWbWMWV3umT2kl7b.jpeg)
```

---
## \#2 Posted by: mmaner Posted at: 2018-12-20T22:26:22.676Z Reads: 96

```
https://www.electric-skateboard.builders/t/hall-sensor-wire-extension-cable/41370/2?u=mmaner
```

---
## \#3 Posted by: JonathanLau1983 Posted at: 2018-12-21T09:22:49.920Z Reads: 69

```
https://flipsky.net/collections/accessories/products/flipsky-esc-sensor-wires

Or make your own JST-ZH 1.5mm pitch to JST-PH 2.00mm pitch cable/adaptor
```

---
## \#4 Posted by: J95hicks Posted at: 2018-12-22T21:07:12.536Z Reads: 59

```
So i got the right connection now...but im not sure how to connect the wires.... should i match the color or the order???![20181222_150622|374x500](upload://cx4tjdAaYgqOmBJ60toYPlyGD1G.jpeg)
```

---
## \#5 Posted by: Andy87 Posted at: 2018-12-22T21:23:21.719Z Reads: 53

```
Is it a male/female adapter (two plugs)
Or is it just a 2mm jst?
```

---
## \#6 Posted by: mtuan293 Posted at: 2018-12-22T21:23:40.448Z Reads: 53

```
why you cut it like that? You can just plug the motor sensor in the adapter cable
```

---
## \#7 Posted by: J95hicks Posted at: 2018-12-22T21:34:40.749Z Reads: 47

```
I didnt buy the adapter...time issue. I bought![1545514421886956231346|375x500](upload://s17wouG2ek5zMDnsZ8h2L1CKNs6.jpeg) so i have to wire it myself
```

---
## \#8 Posted by: J95hicks Posted at: 2018-12-22T21:35:49.007Z Reads: 44

```
Its the 2mm jst, got connectors from amazon
```

---
## \#9 Posted by: Andy87 Posted at: 2018-12-22T21:40:50.499Z Reads: 44

```
Look on your focbox, there is written which wire need to go to which pin
```

---
## \#10 Posted by: J95hicks Posted at: 2018-12-22T21:46:41.141Z Reads: 44

```
Okay, i see that. From the top. Its Gnd, h3, h2, h1, temp, 5v... green is gnd, im assuming red is 5v(neg) and i hope everything else is right bc idk lol
```

---
## \#11 Posted by: Andy87 Posted at: 2018-12-22T21:49:59.706Z Reads: 41

```
Most important is that you get the 5V and the ground right.
The sensor order doesn’t really matter.
T should be the old white cable.
```

---
## \#12 Posted by: JonathanLau1983 Posted at: 2018-12-22T21:51:09.521Z Reads: 42

```
* Red = 5v
* Blue = A
* Yellow = C
* Green = B
* Black = GND

From their site on another motor and white is the temp sensor. I've added a 10k NTC thermistor to my motors to the temp sensor works
```

---
## \#13 Posted by: mtuan293 Posted at: 2018-12-22T21:55:35.331Z Reads: 38

```
h1, h2, h3 are the hall sensors and their order doesn't matter. Only the order of Gnd, 5v and temp matters
From flipsky website
![image|305x180](upload://2UImBJcNvIP1ga13l4lbwEnLAbh.png)
```

---
## \#14 Posted by: J95hicks Posted at: 2018-12-22T21:59:59.190Z Reads: 32

```
Okay..so Red=5v, black=gnd, BGY=sensor, white=temp.. sound right?
```

---
## \#15 Posted by: JonathanLau1983 Posted at: 2018-12-22T23:27:23.173Z Reads: 30

```
That's correct
```

---
## \#16 Posted by: J95hicks Posted at: 2018-12-23T02:48:04.181Z Reads: 28

```
Yep, got it wired up and tested on my board. Ran alright. Foc wasnt quite as great as i had hoped. Not all that smooth... but it programmed or whatever to Foc so thats good enough for now
```

---
