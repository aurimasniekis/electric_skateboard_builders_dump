# Deans connector spark with 6s series jst connector

### Replies: 7 Views: 1330

## \#1 Posted by: Chris_KP Posted at: 2016-04-09T07:29:29.883Z Reads: 82

```
I just received my 2x3s to 6s jst adapter. I had both balance leads plugged
into the adapter and then put my series connector on to both battery terminals, a big spark came from the positive terminal on the last battery I plugged in. Any thoughts??




<img src="/uploads/db1493/original/2X/a/a0136ad9d806bc7177c785dc347e19124813a546.JPG" width="375" height="500">
```

---
## \#2 Posted by: lowGuido Posted at: 2016-04-09T08:02:38.164Z Reads: 80

```
did you have the polarity of the JST's correct? 
id guess you had them wrong way around.

as per this thread
http://www.electric-skateboard.builders/t/lipo-spark-when-plugging-into-balance-board/243
```

---
## \#3 Posted by: lox897 Posted at: 2016-04-09T08:32:28.007Z Reads: 78

```
Please categorise your post.
```

---
## \#4 Posted by: Chris_KP Posted at: 2016-04-09T08:36:14.992Z Reads: 76

```
the batteries were but the jst connector only let me plug in one way
```

---
## \#5 Posted by: lowGuido Posted at: 2016-04-09T08:37:18.905Z Reads: 74

```
yeah but there are 2 of them so you can get them ass about.
```

---
## \#6 Posted by: Chris_KP Posted at: 2016-04-09T10:00:13.694Z Reads: 70

```
ill explain again.. I wasnt charging them i just had a balance adapter for converting 2 3s batteries to 6s balance lead. I then pluged in my series connector and the second battery i plugged in sparked and melted the contacts.
```

---
## \#7 Posted by: laurnts Posted at: 2016-04-09T10:33:40.888Z Reads: 71

```
Yes it doesnt take a charger or while charging to short it out. And yes you are shorting them out with your harness.

To fix this, you need to pre determine which battery will be the positive side and the negative side. Make sure that the positive side of the 3s battery is the same side with the 6s positive balance wire.

So the simple solution for your problem would be:
1. Connect the balance lead in series.
2. Set the series harness only to 1 battery.
3. Mark the series harness connector, 1 for A and 1 for B.
4. Connect the last battery (mark it as X) with the series harness.
5. If shorts happen, swap the batteries around. X to A from X to B without swapping the balance lead.

Its easier and safe to use voltmeter to test if shorts is going to happen while connecting ports by setting voltmeter to measure volt. If you see a voltage reading solid plus or minus, thats a short and don' connect them.
```

---
