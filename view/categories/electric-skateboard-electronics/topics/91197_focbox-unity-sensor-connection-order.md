# Focbox Unity Sensor Connection Order

### Replies: 13 Views: 459

## \#1 Posted by: ajplant96 Posted at: 2019-04-20T04:22:17.006Z Reads: 115

```
When connecting the 6 pin sensor cable from the motor to the unity, is there a specific order that everything needs to go in? I know the cables from the motor have to be in a specific order, just need to know if they need to be in a specific order as far as plugging it into the unity goes too.
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-04-20T04:24:11.929Z Reads: 114

```
E: I was wrong, read what @ Lee said below
```

---
## \#3 Posted by: ajplant96 Posted at: 2019-04-20T04:26:18.233Z Reads: 109

```
I just know that ground, etc need to be correct but that’s good to know. 5 sensor cables to a 6 pin adapter (racerstar motors) should be fine though?
```

---
## \#4 Posted by: Sn4pz Posted at: 2019-04-20T04:28:32.893Z Reads: 104

```
I was incorrect, below @ Lee has the right information :+1:
```

---
## \#5 Posted by: LEE Posted at: 2019-04-20T04:43:58.994Z Reads: 92

```
![image|230x500](upload://xZBccEKhH00wDICNv7A0yWRNqD3.jpeg) 
The positions of GND, TMP and 5V are fixed.
There is no problem if H1, H2 and H3 are replaced.
```

---
## \#6 Posted by: ajplant96 Posted at: 2019-04-20T04:58:16.773Z Reads: 81

```
So with my motors having 5 cables one of the H points being left empty should be fine?
```

---
## \#7 Posted by: LEE Posted at: 2019-04-20T05:08:20.535Z Reads: 80

```
If there are 5 cables, the space is TMP.
```

---
## \#8 Posted by: ajplant96 Posted at: 2019-04-20T05:16:07.142Z Reads: 80

```
TMP? Sorry, totally new to anything DIY/technical within esk8
```

---
## \#9 Posted by: LEE Posted at: 2019-04-20T05:32:44.035Z Reads: 77

```
In case of 5 cables, it is a pattern without TEMP.
GND,H3,H2,H1,5V.
```

---
## \#10 Posted by: ajplant96 Posted at: 2019-04-20T05:39:32.559Z Reads: 74

```
Oh okay, awesome. Thanks so much, haven’t had a working board for 3 months and this is the last thing to do to get it running now so appreciate your help immensely.
```

---
## \#11 Posted by: Andy87 Posted at: 2019-04-20T08:06:54.671Z Reads: 67

```
I thought @Deodand did write something up in the unity SW so that the order not really matter anymore? Or was it just a protection if somebody switch the 5V and ground Pin?
```

---
## \#12 Posted by: LEE Posted at: 2019-04-20T12:09:23.720Z Reads: 57

```
https://www.electric-skateboard.builders/t/hall-sensors-5-wires-vs-6-wires/31626

It is an answer according to this content.
```

---
## \#13 Posted by: Andy87 Posted at: 2019-04-20T12:19:18.309Z Reads: 58

```
Found this from the man himself

https://www.electric-skateboard.builders/t/focbox-unity-support-setup-troubleshooting/77861/923?u=andy87

Seems like even the unity need to get 5V and ground in the right order. Thought I read something else somewhere...
```

---
