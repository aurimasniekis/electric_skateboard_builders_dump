# Hub motor with twin ESC set up help

### Replies: 16 Views: 2710

## \#1 Posted by: Sean Posted at: 2016-06-18T21:39:07.679Z Reads: 166

```
Hello everybody, it seems, that I couldn't find any existing topic on what I need. I would like to build a boatd with twin hub motors from jacob. With two motors, come two ESC's, but I was wondering how to set them up, I guess in parallel? Could anyone help me, maybe with a diagramm.

Thanks a lot, really appreciate it
```

---
## \#2 Posted by: Karmannghiagirl Posted at: 2016-06-18T21:41:43.436Z Reads: 166

```
Please search the forum. there are a ton of threads talking about this topic.
```

---
## \#3 Posted by: Pablo_702 Posted at: 2016-06-18T21:45:42.219Z Reads: 160

```
Ollin boards sell a wire to connect two ESC together
```

---
## \#4 Posted by: Sean Posted at: 2016-06-18T21:48:37.543Z Reads: 156

```
I think its just for vesc's...****
```

---
## \#5 Posted by: Pablo_702 Posted at: 2016-06-18T21:59:33.845Z Reads: 158

```
That im not 100%  sure, ask @chaka
```

---
## \#6 Posted by: lox897 Posted at: 2016-06-18T23:29:30.075Z Reads: 146

```
It is just for VESCs. It is called a CANBUS wire. If you want to connect two normal ESCs to one receiver and one battery you will need something to join the two positive wires into one wire and you will also need that for the negative. Also get a servo y connector but if your ESCs have BECs in them then you must cut one of the ESC's red wires.
```

---
## \#7 Posted by: Sean Posted at: 2016-06-19T11:03:19.353Z Reads: 145

```
<img src="/uploads/db1493/original/2X/6/60a7ecf4f500e11fe08bf2f631d0a19f8e780aac.JPG" width="375" height="500">

Something like that, The ESC will be set up in parallel to the in series configured Batteries...

Would this work thanks again
```

---
## \#8 Posted by: Luke Posted at: 2016-06-19T11:45:59.703Z Reads: 144

```
http://www.electric-skateboard.builders/t/vesc-faq-connect-two-vesc-via-canbus-for-dual-motors/142
This thread will show you how to connect two vescs via canbus. It's useful for controlling both vescs with a single remote reciever
```

---
## \#9 Posted by: Sean Posted at: 2016-06-19T14:12:50.695Z Reads: 135

```
I need to connect two ESC's not two VESC
```

---
## \#10 Posted by: lox897 Posted at: 2016-06-20T01:59:59.416Z Reads: 113

```
That diagram looks right. @lowGuido would you mind double checking the diagram?
```

---
## \#11 Posted by: lowGuido Posted at: 2016-06-20T04:32:22.644Z Reads: 105

```
looks good to me. be careful cutting the BEC wire though. some ESC's like it and Some do not.
```

---
## \#12 Posted by: lox897 Posted at: 2016-06-20T04:50:46.175Z Reads: 100

```
Thanks for double checking.
```

---
## \#13 Posted by: Mobutusan Posted at: 2016-06-20T05:37:50.257Z Reads: 94

```
Aren't you supposed to put the servo "y" connector on the receiver wire between the esc and receiver? To me, it looks like the diagram has the servo "y" connector on the battery balance wires which would be good for charging in series as 6s, but spent really have anything to do with connecting two ESC's together. 

Is that right, or am I missing something?
```

---
## \#14 Posted by: lowGuido Posted at: 2016-06-20T05:56:34.455Z Reads: 88

```
LOL! yeah true story! the diagram has the servo wires going to the batteries!
I saw the word servo and assumed that it was for the ESC, but yeah the drawing does show it going to the battery!
```

---
## \#15 Posted by: lox897 Posted at: 2016-06-20T06:11:39.468Z Reads: 87

```
That just went right over my head. Nice pick up. Lol
```

---
## \#16 Posted by: Sean Posted at: 2016-06-20T16:49:50.586Z Reads: 72

```
First of all thanks all of you for helping me out! Really helped me a lot amd gives me mote courage to make my board. 

Yeah haha was in a hurry it should be on the esc and not the battery, but there will be a 3s to 6s comverter cable
```

---
