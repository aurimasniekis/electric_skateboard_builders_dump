# Which 2 3s bms connection is right?

### Replies: 9 Views: 759

## \#1 Posted by: pau Posted at: 2017-06-08T19:20:04.839Z Reads: 45

```
Hey
 im not pretty sure which bms connection is right.
i saw different schematic at esk8.builders.


the first picture described how the batterys connected to the BMS without balancer port. 
Battery 1 and Battery 2 seriell connected.
The + Lead of Battery 1 goes to the + charger connector.
The - Lead of Battery 1 goes to the + Lead of Battery 2.
The + Lead of Battery 2 goes to the B- connection. 

<img src="/uploads/db1493/original/3X/f/1/f19e9e92a59d4fbb10ccbeb3dce909ae0db6e516.jpg" width="690" height="424">






**1st Schematic.**
<img src="/uploads/db1493/original/3X/7/6/769e7680568213a05a16889441d4213c209775cb.jpg" width="690" height="388">
The negative wire of the 2nd battery balancer Lead is not connected.


**2nd Schematic**
<img src="/uploads/db1493/original/3X/2/5/257fbf2a1335e8a9f343fa4e8d68d8a11b092a72.jpg" width="690" height="388">
The negative balancer wire from the Battery 2 is connected with the red balacer wire from battery 1


**3rd Schematic**
<img src="/uploads/db1493/original/3X/c/4/c4c7f91d1982c3970f6f1d5362497fb2c326072d.JPG" width="690" height="388">
Both negative wires form the balancer are connected to the negative BMS pin. 


**4th Schemactic**
<img src="/uploads/db1493/original/3X/6/4/64995edd8d94a727e846159bd2254ab59fec7be6.jpg" width="690" height="388">
The negative balacer wire from the 1st battery is not connected.
The negative balacer wire from the 2st battery is  connected to the negative pin of bms.
```

---
## \#2 Posted by: lowGuido Posted at: 2017-06-08T19:21:44.369Z Reads: 38

```
what the shit?!

the first one.
are you even joking about trying any of the others?
```

---
## \#3 Posted by: pau Posted at: 2017-06-08T19:25:21.454Z Reads: 37

```
sorry but i saw all that schematic.
i think the 4th one is right.
beacause i will use the negative wire from the 2nd battery to connected it to the bms.
and from 1st battery on the positivs wires.

because the batteries are connected in seriell.
```

---
## \#4 Posted by: lowGuido Posted at: 2017-06-08T19:28:09.361Z Reads: 37

```
like I don't want to be rude. but if people cant work out the most basic rule of "don't short the battery" they shouldnt be doing electronics.

its the first one, even the second one is ok. but with what you have just told me I wouldnt want you to join ANY red and black wires just in case.
```

---
## \#5 Posted by: Challlsss Posted at: 2017-06-08T19:55:42.215Z Reads: 36

```
1 or 2... NOTHING ELSE
```

---
## \#6 Posted by: pau Posted at: 2017-06-08T20:01:16.376Z Reads: 34

```
okay:grimacing:

sorry one more question. 
do you think the battery 2 goes directly to the positiv power suplly port? does it have to?
```

---
## \#7 Posted by: lowGuido Posted at: 2017-06-08T20:11:21.401Z Reads: 36

```
yes so B2 main positive lead goes to the positive of your ESC. B1 negative connects to BMS. and B2 negative and B1 positive join together.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-06-08T22:03:15.537Z Reads: 31

```
**NOTE** This diagram does not bypass the bms during discharge and requires a high power bms.

<img src="/uploads/db1493/original/3X/4/9/4901f0a1440d384bd3db291288b936e34a45b648.png" width="690" height="361">
```

---
## \#9 Posted by: Namasaki Posted at: 2017-06-08T22:25:24.041Z Reads: 27

```
**NOTE** This diagram is for bypassing during discharge cycle. Use this for low power charge only bms.

<img src="/uploads/db1493/original/3X/d/9/d9e1b0670d703eba95765796cc83737df9610a56.png" width="690" height="371">
```

---
