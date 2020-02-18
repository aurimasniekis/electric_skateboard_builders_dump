# Motor Grinding Gears? VESCx Fault. Motor doesn&rsquo;t move, makes horrible sound

### Replies: 27 Views: 1663

## \#1 Posted by: trigger4point7 Posted at: 2017-01-22T01:55:22.407Z Reads: 124

```
I attached a video of my motor not working. It makes this horrible grinding sound and doesn't move. After a few seconds the fault light (red light) blinks a few times.  I have no idea what the issue is. Any help would be appreciated. I just finished the build and still haven't rode it. 

https://youtu.be/dLZObhp7KiU

<iframe width="560" height="315" src="https://www.youtube.com/embed/dLZObhp7KiU" frameborder="0" allowfullscreen></iframe>
```

---
## \#2 Posted by: Pathaim Posted at: 2017-01-22T01:57:56.745Z Reads: 121

```
check all ur connections, especially phase wires, something similar happened to me due to a bad joint with the phase wire
```

---
## \#3 Posted by: trigger4point7 Posted at: 2017-01-22T01:58:38.026Z Reads: 117

```
Sorry, but what exactly is a phase wire or a "bad joint"?
```

---
## \#4 Posted by: Pathaim Posted at: 2017-01-22T01:59:15.979Z Reads: 114

```
Phase wires, the 3 wires that go to your motor from your vesc, bad joint, a bad solder joint/broken joint not allowing proper current flow
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2017-01-22T02:02:28.660Z Reads: 113

```
Have you setup your vesc before using it ???!

Also be sure to properly isolate you motor lead...
```

---
## \#6 Posted by: trigger4point7 Posted at: 2017-01-22T02:06:07.651Z Reads: 112

```
I've gotten it to spin properly before. I just tested the phase wires by pulling them stright so they weren't so tangled and it worked perfectly.... Not so sure what that means. Perhaps I should resoder the bullet connections on the VESC? @Pathaim
```

---
## \#7 Posted by: Pathaim Posted at: 2017-01-22T02:06:48.919Z Reads: 109

```
yes that might help, all i remeber is i had a similar problem and it was caused by a bad connection on a phase wire
```

---
## \#8 Posted by: trigger4point7 Posted at: 2017-01-22T02:15:04.015Z Reads: 108

```
To resolder them do you know if you cut off the current connectors and try again or do you melt the current solder and pull them off? I know you don't remember much but if you had to do it again?
```

---
## \#9 Posted by: zmoney Posted at: 2017-01-22T02:17:05.227Z Reads: 105

```
Try de-soldering them, then soldering them on again. Don't cut the connectors off.
```

---
## \#10 Posted by: barajabali Posted at: 2017-01-22T05:09:52.647Z Reads: 100

```
Also maybe bad fet?
```

---
## \#11 Posted by: Blasto Posted at: 2017-01-22T05:11:16.604Z Reads: 96

```
This is a bad lead connection
```

---
## \#12 Posted by: trigger4point7 Posted at: 2017-01-22T18:54:11.016Z Reads: 81

```
I have a feeling that I have soldered these on backwards. The male connectors aren't completely covered when attached to the female. Could that be it? I'm definitely resoldering. I just want to make sure I know why.<img src="/uploads/db1493/original/3X/1/9/1990440e9f7b20bd60b0715039aa6b0c84ce3e7e.jpg" width="375" height="500">
```

---
## \#13 Posted by: mmaner Posted at: 2017-01-22T18:58:49.434Z Reads: 80

```
[quote="trigger4point7, post:12, topic:16465"]
soldered these on backwards
[/quote]

Looks like it.  The sleeve of the connector should fully enclose the pin.
```

---
## \#14 Posted by: trigger4point7 Posted at: 2017-01-22T19:13:57.760Z Reads: 78

```
Dang. Any tips on resoldering or should I just go for it. Heat up the connectors until it falls off? Should I order new female connectors?
```

---
## \#15 Posted by: mmaner Posted at: 2017-01-22T19:16:14.618Z Reads: 74

```
I would use new connectors, I doubt you will ever get the inside sleeve of those bullets cleaned out enough to not be crazy hard to connect.  To unsolder, remove the heatshrink/tape and heat the edge of the connector by the wire or if you can slip the tip of the iron into the connector.
```

---
## \#16 Posted by: mortorojo Posted at: 2017-01-22T19:18:13.900Z Reads: 73

```
If you soldered the wires to the ends without the holes on the side there is nothing you can do but get some new connectors.
```

---
## \#17 Posted by: trigger4point7 Posted at: 2017-01-22T19:22:43.106Z Reads: 70

```
So I did use the side with the holes? Is that the correct side. It's still possible I did a bad job?
```

---
## \#18 Posted by: trigger4point7 Posted at: 2017-01-22T19:22:53.811Z Reads: 70

```
Awesome thank you.
```

---
## \#19 Posted by: mmaner Posted at: 2017-01-22T19:24:48.327Z Reads: 70

```
THe side of the connector that has the holes in it is the side you want to solder.  If you soldered that side, see if you can figure out why the pin side wont slide all the way in.
```

---
## \#20 Posted by: mortorojo Posted at: 2017-01-22T19:26:30.758Z Reads: 70

```
On all the bullet connectors I've used the side with two holes is the side to solder the wires on. Best way to be sure you have them right is to connect them to the phase wires male connectors and see if they fit snug and slide flush with no gaps. Then remove them knowing which is the correct end to solder too.
```

---
## \#21 Posted by: mortorojo Posted at: 2017-01-22T19:30:03.989Z Reads: 67

```
If your still no to sure take another picture as you did before of the connectors, but remove the electrical tape from one of the female bullet connectors so we can see how you soldered them. I'd also recommend you get some shrink tube.
```

---
## \#22 Posted by: SeanHacker Posted at: 2017-01-22T19:45:11.767Z Reads: 68

```
This is how your bullet connectors should look. 

<img src="/uploads/db1493/original/3X/6/5/65a7490bb6f451ff4fe4b273558acab9386d36b8.jpg" width="281" height="500">

<img src="/uploads/db1493/original/3X/6/e/6eb4482c50613ddff83cba6c80b945ada6e1e613.jpg" width="281" height="500">
```

---
## \#23 Posted by: trigger4point7 Posted at: 2017-01-23T03:37:18.616Z Reads: 60

```
So as you can see in the pictures, I've soldered on the female connectors on the side with the hole. I've double checked that I have plugged the motor connectors as far in as possible. There is some residual solder on the side of the connector and a small gap between the connector and the wire from the VESC. Perhaps I have used the wrong connectors, both are supposed to be 5.5mm? These are the ones I've ordered... https://www.amainhobbies.com/tekin-5.5mm-highefficiency-bullet-connector-3-tektt3055/p32318?utm_source=transactional_email&utm_medium=e-mail&utm_campaign=order_complete&utm_cid=1239004&utm_content=%2ftekin-5.5mm-highefficiency-bullet-connector-3-tektt3055%2fp32318<img src="/uploads/db1493/original/3X/c/8/c83484ea631a197b600305ac2d4c4a1c4e1daeca.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/a/9/a94438b3d1dcd711648056b81db4d1b217e935fb.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/0/a/0ac5713091264741983eb8629410999b35660fd5.jpg" width="666" height="500">
```

---
## \#24 Posted by: Blasto Posted at: 2017-01-23T04:00:52.306Z Reads: 59

```
Hard to tell, but your middle connection seems cold. Drop some flux where the wire meets the connector and reheat
```

---
## \#25 Posted by: trigger4point7 Posted at: 2017-01-23T05:13:18.483Z Reads: 58

```
Cold? Does the solder on the outside of the connector on the right interfere?
```

---
## \#26 Posted by: zmoney Posted at: 2017-01-23T13:50:54.163Z Reads: 54

```
What @Blasto means by cold is that your solder joint for the middle connection is not solid enough, in lame mans terms. Also, the solder on the third connector is fine. Make sure to wrap those up in heat shrink so that you don't short them afterwards.
```

---
## \#27 Posted by: trigger4point7 Posted at: 2017-01-23T21:54:35.677Z Reads: 36

```
So I've resoldered everything with the proper bullet connectors they are completely enclosed (they fit flush) as you can see in the image. I've switched the wires around and nothing works. Same issue. I don't know what else to do...<img src="/uploads/db1493/original/3X/6/f/6f809680dc4686013416dc3a41d499fed6e6178d.jpg" width="375" height="500">
```

---
