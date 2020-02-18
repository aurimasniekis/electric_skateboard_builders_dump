# Need help wiring my BMS

### Replies: 9 Views: 1499

## \#1 Posted by: Brycehoosiers Posted at: 2017-07-19T21:53:06.759Z Reads: 110

```
I need help wiring my bms to my batteries for charging here is the pic of my bms ( https://drive.google.com/open?id=0B6WNH8Mxk1jyM2dQS0FQZDdJUEE ) and I'm trying to wire 2 3s batteries that are in series to create a 6s battery that goes to the bms, so I am using a balance cable that is 2 3s jst-xh to 1 6s jst-xh but the problem I'm having is the bms only has 5 wires on the balance cable but the battery has 6 and I don't know how to wire them, and which wire to leave out, I also don't know which order to solder them in cuz I don't wanna ruin the bms﻿
```

---
## \#2 Posted by: Martinsp Posted at: 2017-07-19T22:04:30.567Z Reads: 104

```
First of all you should not solder the batteries directly to the bms.. use JST connector to save you some time later when you want to check the voltages for example.

The way you should go about wiring the BMS is try measuring voltage between the negative lead of your battery and one of the balance connectors wires on your battery. if it is showing voltage of one cell (anywhere between 3.0 and 4.2) connect it to the bottom most (based on your photo) pin on the JST on the BMS. if it does not show the voltage of one cell try another one of the balance wires of the battery until it does. Once you find it you do pretty much the same but this time you will use instead of the negative lead the one you found in the step earlier and so on.

Hope I explained it well, if not just ask what you dont understand. :)
```

---
## \#3 Posted by: Brycehoosiers Posted at: 2017-07-19T22:21:19.318Z Reads: 94

```
[quote="Martinsp, post:2, topic:28061"]
Once you find it you do pretty much the same but this time you will use instead of the negative lead the one you found in the step earlier and so on.
[/quote]

This part didn't really make sense to me. And I wasn't going to solder the batteries directly to the BMS , I just need to solder the wires from the battery to the bms. Will the batteries need to be charged for this , because I don't have a lipo charger. And then what wire will needed to be left unwired because the bms only has 5 pins/wires and the battery has 6
```

---
## \#4 Posted by: Martinsp Posted at: 2017-07-19T22:44:43.407Z Reads: 85

```
<img src="/uploads/db1493/original/3X/6/7/67bc6269a8f75905156c7fdf3795ddb57cd032ad.jpg" width="640" height="480">
This is how a typical (in this case 3S) battery is wired to the balance connector. You have plus and minus that are thicker power wires and thinner wires that are the same part of the battery going to the connector for balancing with a charger or whatever else. You with your 6S have the same but with more cells and more wires. You did mention that you have 6 wires on balance connector so you have 5 wires coming from cells like you see in the picture there are blue and green. You have the same with more wires. You just need to find out which wire is the 6th one meaning if it is the "duplicate" of the positive or negative. Thats why you should measure voltage between power wire, for example black and the cable on one of the sides of your balance connector. so here on the picture you would measure between black power wire and say red balance wire. What you would get is some woltage between 9V and 12.6V so that is not the duplicate. So you would try the other side and again with black power wire, you would get 0V because that is the same point in the battery. So you found which wire is the one that is in the balance connector that you dont need. 

Please send a picture so I can tell you exactly with your colors what you need to do. More specifically.
```

---
## \#5 Posted by: Brycehoosiers Posted at: 2017-07-19T23:41:11.608Z Reads: 69

```
I will send a pic next week once I get my batteries. Will I need to charge them before I do this , because I don't have a lipo charger
```

---
## \#6 Posted by: Brycehoosiers Posted at: 2017-07-21T03:42:19.743Z Reads: 55

```
I know the batteries come with some charge is it enough to do this ?
```

---
## \#7 Posted by: Martinsp Posted at: 2017-07-21T20:21:54.794Z Reads: 50

```
The batteries should come with around 3.6V which is 50%. That is the common storage voltage.
```

---
## \#8 Posted by: Martinsp Posted at: 2017-07-21T20:22:57.548Z Reads: 49

```
And you would need to buy a balance charger if your cells would come unbalanced but otherwise you can get away with just a bms and a regular charger for your pack.
```

---
## \#9 Posted by: Brycehoosiers Posted at: 2017-07-25T00:28:20.646Z Reads: 43

```
<img src="/uploads/db1493/original/3X/8/9/891269bcbb3eb327c5c96f0800dd1b26bdb5dc8b.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/b/b/bba9f92d54517b77fd0963a66a83ee301956afce.JPG" width="375" height="500">

Here's are 2 pics 1 of the 5 wires coming from the bms and one of the 2 3s to 6s cable 

The 6s cable has a total of 8 wires with a red and black connected in the middle , how do I wire those up two the 5 on the bms and which ones do I leave out or connect together
```

---
