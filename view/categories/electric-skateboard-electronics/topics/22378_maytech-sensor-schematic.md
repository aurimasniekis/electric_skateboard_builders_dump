# Maytech Sensor Schematic

### Replies: 11 Views: 1863

## \#1 Posted by: TarzanHBK Posted at: 2017-05-04T13:40:37.284Z Reads: 210

```
Does someone have a schematic of maytech sensor cables?
I´m using Polar´s 6355 sensored motors with 6 sensor cables, but not sure how to connect them.
Not having a fuse atm, so I´d like to skip the trial and error and jump directly to the connect-and-working-part :slight_smile:
 <img src="/uploads/db1493/original/3X/e/4/e4fcb39a8c4f71b5eea19d358699351c90fde925.jpg" width="374" height="500">
```

---
## \#2 Posted by: longhairedboy Posted at: 2017-05-04T14:05:08.693Z Reads: 196

```
Zoom in on this image of two vescs. The pinouts are lebelled on the sticker for the sensor port, and you can see the orinetation of the connector so you should be able to define them from that. 

<img src="/uploads/db1493/original/3X/7/c/7ca5bc1986d4a125ae87b42f5c8ca019c077bdcc.jpeg" width="375" height="500">
```

---
## \#3 Posted by: TarzanHBK Posted at: 2017-05-04T14:13:04.059Z Reads: 193

```
Sure thx, but my problem is not the connection on the vesc, they are labled good :slight_smile:
I´m having trouble finding out the phases on the motors. I can´t tell which one is phase, ground, sensors 1-3 and temp.
```

---
## \#4 Posted by: Pimousse Posted at: 2017-05-04T14:21:41.009Z Reads: 193

```
Don't know if it's the same as Alien Power System motors, but I made a tutorial 9in french) for these motors :
http://e-sk8.fr/forum/viewtopic.php?f=8&t=1149

pin # VESC - Description - Motor sensor wire color

1 -  5V - Yellow
2 - Temp sensor - Green
3 - Sensor Hall 1 - Blue
4 - Sensor Hall 2 - White
5 - Sensor Hall 3 - Black
6 - GND - Red

Here is what Bruno (APS) sent me :
<img src="/uploads/db1493/original/3X/c/f/cfc57b7ac0fbad979ddb2f5ab4e3075a1158d44f.png" width="281" height="500">
```

---
## \#5 Posted by: TarzanHBK Posted at: 2017-05-04T14:24:12.190Z Reads: 173

```
Thx for that, but I think it´s a different one.
If you compare the colors, they don´t match.
```

---
## \#6 Posted by: TarzanHBK Posted at: 2017-05-04T14:31:50.415Z Reads: 173

```
And you can´t really tell from the outside, because the sensor pcb is blank and epoxied to the motor:
<img src="/uploads/db1493/original/3X/1/2/12ed42dc39afe7af9cada3b3e8cc3e6a1df5121d.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/7/9/79577ca74ed5628ffe645a0edaa53f148de86cc5.jpg" width="666" height="500">
```

---
## \#7 Posted by: mccloed Posted at: 2017-05-04T14:35:50.234Z Reads: 171

```
Colors of wire are irrelevant. They should be in this configuration:

<img src="/uploads/db1493/original/3X/e/5/e50a24bc0013b618102a347c22878ceac5057283.PNG" width="281" height="500">
```

---
## \#8 Posted by: Jinra Posted at: 2017-05-04T14:38:05.238Z Reads: 168

```
Check out my Carbonated build thread.
https://www.electric-skateboard.builders/t/carbonated-enertion-vescs-hi5ber-overtaker-custom-10s4p-25r-pack-with-cell-level-fusing-abec-flywheels/10879/10?u=jinra


TL;DR 
green/blue/yellow = sensors
red/black = 5v and GND
white = temp
```

---
## \#9 Posted by: TarzanHBK Posted at: 2017-05-04T14:40:26.274Z Reads: 163

```
Cool! So there is a norm for that, thats good :slight_smile:
```

---
## \#10 Posted by: TarzanHBK Posted at: 2017-05-04T14:42:20.187Z Reads: 165

```
Alright! Thx for that, makes sense now :)
```

---
## \#11 Posted by: Redfire1 Posted at: 2018-04-16T11:16:55.052Z Reads: 111

```
That’s my vesc ![image|679x500](upload://xNEWmDFUhUPqgQ8BG5Tptwt9UgN.jpeg)
```

---
