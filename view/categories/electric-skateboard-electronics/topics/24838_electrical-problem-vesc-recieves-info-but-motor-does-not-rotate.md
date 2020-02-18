# Electrical problem. Vesc recieves info but motor does not rotate

### Replies: 6 Views: 489

## \#1 Posted by: crucialhunter Posted at: 2017-06-07T20:39:17.817Z Reads: 61

```
Last week i was riding and sudenly my motor stoped answering correctly, it was acting exactly like once one of the 3 cables that go to the motor disconected, the motor did a 1 centimeter movement and stoped. each time i chose pressed the triger in the remote the motor would just do that. 

At home i tried to check if i saw any cable making a bad contact and i couldn't see any issue .

Now after testing the motor no longer moves or answers to anything. 
Anyone has an idea what the problem could be? Is it the vesc or the motor? It felt like either the vesc or the motor had a problem :frowning: 
<img src="/uploads/db1493/original/3X/6/5/656888ef21c21855479ce37017e532e7625d38f8.jpg" width="690" height="388">
```

---
## \#2 Posted by: rpn314 Posted at: 2017-06-07T23:23:52.068Z Reads: 53

```
Is the VESC giving any sort of blinking lights? Have you connected it to BLDC Tool?
```

---
## \#3 Posted by: crucialhunter Posted at: 2017-06-11T15:22:21.649Z Reads: 34

```
Hi @rpn314 ! Thanks for the answer, took my way longer to answer than i would have liked.

The board detects the signal from the remote. but a red light blinks and there is no movement.
 Here is a video of it. https://goo.gl/photos/Ngd2YR8TmkRzLVuG9
When i triger and it is connected to the BLDC i get fault code : DRV8302 which i couldn't find to understand what it means.

<img src="/uploads/db1493/original/3X/3/2/328aa267e4b705ee1781674af66799a02f90d06c.png" width="690" height="454">

<img src="/uploads/db1493/original/3X/3/5/35b93a3a72cac86738a25af5811126ec30654297.png" width="392" height="113">
Might it be the vesc?
```

---
## \#4 Posted by: Deakbannok Posted at: 2017-06-11T16:13:12.259Z Reads: 33

```
Reflash your vesc and reset to default.
```

---
## \#5 Posted by: crucialhunter Posted at: 2017-06-11T16:42:28.370Z Reads: 30

```
How could i make that? thanks!
```

---
## \#6 Posted by: Deakbannok Posted at: 2017-06-11T21:38:36.078Z Reads: 23

```
Depends on your hardware. What is your firmware version on vesc? 
Try to up reflash your firmware on vesc first. If it 
doesn't work..   then likely your vesc is fried.
```

---
