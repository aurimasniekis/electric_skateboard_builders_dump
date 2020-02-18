# Works fine, then DRV error, then fine again

### Replies: 20 Views: 953

## \#1 Posted by: abctheing Posted at: 2017-10-13T14:50:49.118Z Reads: 136

```
As the title says, i have a DRV problem. 
This video says it all: https://www.dropbox.com/s/eakb0iyikyzlh7h/IMG_4495.MOV.mov?dl=0

I just recently got these two vescs, but one of them has been acting weird.
This is not my first build so i kinda know what i'm doing.

Anyway one of the vescs goes in to DRV error for a second. It has happend since i got it.
I have done a test ride and the board has worked really well, but as said, the vesc
acted weird even before that.

It don't know what's causing it. Any help?
```

---
## \#2 Posted by: Jinra Posted at: 2017-10-13T15:02:33.291Z Reads: 135

```
likely defective
```

---
## \#3 Posted by: MysticalDork Posted at: 2017-10-13T16:09:24.245Z Reads: 129

```
Like jinra said, probably defective. Either replace the DRV, or replace the vesc.
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2017-10-13T16:31:14.139Z Reads: 128

```
@abctheing could you post the setting on both of the FocBox, these issue are usually due a bad motor detect or a duplication of the motor detection parameter on the Focbox... I doubt it's a DRV issue, most likely to be a bad connection over the mosfet or a damage Capacitor, maybe you could post some picture of your setup connection (we are here to judge your skill but to help you) and some of the Focbox. 

Regards
JF
```

---
## \#5 Posted by: abctheing Posted at: 2017-10-13T17:05:59.924Z Reads: 114

```
<img src="/uploads/db1493/original/3X/0/d/0d4cdfcc3fd62ac12f91978f789086cf11d924be.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/7/6/76e39069eec7fbb1fab0c206c0ea4bddda3d4a1a.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/0/d/0d1a0ab50752a6156b05a4f5265b1ad1f7cd4b93.JPG" width="666" height="500">

here are some screenshots. tell me if you need more
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2017-10-13T17:12:01.290Z Reads: 111

```
I'm not really sure, but if you look at the second Image, it doesn't look like the sesors table as been properly apply 

<img src="/uploads/db1493/original/3X/0/8/0809f0dba27519eb1934965cf3f3fd55fd496b72.png" width="666" height="500">
```

---
## \#7 Posted by: abctheing Posted at: 2017-10-13T17:20:25.164Z Reads: 105

```
Ah the motor detection is from the second vesc. I reran detection for both vescs.
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2017-10-13T17:23:52.383Z Reads: 103

```
OK, but just make sure that the Parameter you've got from running a motor detection Sensors, integrated limits and coupling correspond to each motor in each vesc
```

---
## \#9 Posted by: abctheing Posted at: 2017-10-14T13:05:25.933Z Reads: 91

```
Nothing seems to work. It still cuts out with DRV error for a second then goes back to normal.
```

---
## \#10 Posted by: abctheing Posted at: 2017-10-18T14:27:32.327Z Reads: 87

```
Is there anybody (preferably close to norway) who could repair the vesc? <img src="/uploads/db1493/original/3X/e/c/ecdda6b21b8c58dfd883a140d37a8f3515cc9458.jpg" width="428" height="500">
```

---
## \#11 Posted by: barajabali Posted at: 2017-10-18T15:46:56.085Z Reads: 83

```
Are you running Via Can or split ppm. Try running can could be a connection issue
```

---
## \#12 Posted by: abctheing Posted at: 2017-10-26T22:33:32.788Z Reads: 67

```
I am running split ppm. i also borrowed an older focbox from a friend that has been working for months, but now it gives my ABS_current_overload. I was riding the board then it suddenly stopped by itself. this happened more and more often and now the motor won't spin, it just clicks.
```

---
## \#13 Posted by: Michael319 Posted at: 2017-10-26T23:19:55.666Z Reads: 64

```
Sounds like the motor was shorted and then fried. I would try to reset my VESC to default settings. Make sure nothing got screwed up. Also, check your phase wires.
```

---
## \#14 Posted by: abctheing Posted at: 2017-10-28T18:42:04.654Z Reads: 51

```
I took apart my motor and reassembled it, i think the board works fine now. I took a small test ride and it worked.
```

---
## \#15 Posted by: Michael319 Posted at: 2017-10-28T19:22:37.719Z Reads: 49

```
Nice, make sure all of your phase wires are insulated so you don't get a short from a bump or something
```

---
## \#16 Posted by: abctheing Posted at: 2017-10-28T22:01:57.581Z Reads: 47

```
Oh sorry, i actually mixed this up. I replaced the vesc with another one, and i have problems with this one as well. ABS_over_current. I managed to fix it but the problem is back again after a test ride.
```

---
## \#17 Posted by: scepterr Posted at: 2017-10-28T22:37:33.967Z Reads: 47

```
Can you post pics of all your wiring and connections,
Some error logs will help too
```

---
## \#18 Posted by: abctheing Posted at: 2017-10-29T09:08:00.567Z Reads: 39

```
After a week i finally think i found the problem. One of the motor wires are broken and loose connection sometimes. The motor is brand new so this is weird. I think i have to open the motor and solder on new motor wires. Btw i have dual 6374 motors
```

---
## \#19 Posted by: abctheing Posted at: 2017-10-31T21:57:29.596Z Reads: 34

```
Soo the focbox is still broken. DRV error but the motor still spins up. Now my second vesc shows the same error. It can't be the settings because when the first focbox broke i replaced it with a 6 month old focbox. The old focbox has been working for so long, but the new fails? I have two broken focboxes now 😭😭😭 i bought them in a group buy
```

---
## \#20 Posted by: abctheing Posted at: 2017-11-04T19:09:31.131Z Reads: 29

```
Does anyone know what could be the issue? I get DRV error but the motor is spinning? I am boardless right now.
```

---
