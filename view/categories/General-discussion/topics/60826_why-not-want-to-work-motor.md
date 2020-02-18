# Why not want to work? (motor)

### Replies: 14 Views: 451

## \#1 Posted by: gacsger Posted at: 2018-07-03T19:24:46.820Z Reads: 114

```
Hello!

I bought my first electric skateboard build, but when i wanted start the skateboard it isnt worked...
Somebody can help me? :confused:
Video link: https://streamable.com/0jmps
```

---
## \#2 Posted by: telnoi Posted at: 2018-07-03T19:36:13.973Z Reads: 110

```
Read the documentation that came with the esc.
If there was none, get it from a secondary source. Describe here which steps you have taken based on the documentation. 
Describe the things you have tried to resolve the issue. 

Doesn't look like your remote is paired. I would start there. Good luck.
```

---
## \#3 Posted by: gacsger Posted at: 2018-07-03T19:49:29.668Z Reads: 94

```
I think its paired because when i pull back the remoter its stoped flashing (remoter & esc)
So i think its paired
```

---
## \#4 Posted by: telnoi Posted at: 2018-07-03T21:04:40.643Z Reads: 79

```
I'm not seeing the battery voltage reflected by the remote.
```

---
## \#5 Posted by: gacsger Posted at: 2018-07-03T21:31:19.755Z Reads: 73

```
[quote="telnoi, post:4, topic:60826, full:true"]
I’m not seeing the battery voltage reflected by the remote.
[/quote]

Its 10% but i think what is the problem, the parallel because when i connect 2pcs 3s battery its stay 11.3 but i already connect 2 battery so yes i think!![jpg%201|325x500](upload://jG45Ps8U8hrCdXGrdqXDNSmObWo.jpg)
```

---
## \#6 Posted by: telnoi Posted at: 2018-07-04T05:04:40.593Z Reads: 54

```
Yes, you need a series connector for 6s. Most likely does not work due to low voltage cutoff.
```

---
## \#7 Posted by: gacsger Posted at: 2018-07-04T13:53:20.228Z Reads: 52

```
Hm okay, i charge the batteries more voltages
```

---
## \#8 Posted by: abenny Posted at: 2018-07-04T13:59:33.695Z Reads: 51

```
thats not what he meant, right now you are running your batteries in parallel and will only be able to get maximum 12.6 volts which is still too low even if you charge the batteries. you need to connect them in series to double the  effective voltage since the ESC requires more voltage to run
```

---
## \#9 Posted by: telnoi Posted at: 2018-07-04T14:12:48.503Z Reads: 49

```
thanks for clarifying. Exactly that.

The ESC is soldered to allow for different voltage configurations. The minimum voltage for this ESC is 6S. Any voltage below the typical cutoff voltage for 6S will prevent the ESC from working correctly. It will power on, but it will not allow the motors to run.

From the manual:

6S 24V：connect those 2 dots on position 3 on the picture. disconnect those 2 dots on position 2 on the picture
7S 29.4V：connect those 2 dots on position 2 on the picture. disconnect those 2 dots on position 3 on the picture
10S 36V：disconnect those 2 dots on position 2 on the picture, disconnect those 2 dots on position 3 on the picture
```

---
## \#10 Posted by: gacsger Posted at: 2018-07-04T14:59:38.452Z Reads: 44

```
Yes I read this descripton but i didnt found the picture, so what is the correct 6s? :confused:
Is it good serial?!
https://hobbyking.com/en_us/xt60-series-adaptor-2pcs-per-bag.html
```

---
## \#11 Posted by: telnoi Posted at: 2018-07-04T15:37:19.630Z Reads: 36

```
6s/7s should be marked on the PCB.
![s-l400%20(1)|300x400](upload://ppwky1Yae9BosneufSjh9rHfpoo.jpg)
```

---
## \#12 Posted by: gacsger Posted at: 2018-07-04T17:48:14.299Z Reads: 28

```
So i have to to be soldered the 2 dots?
So connect the 2 dots with soldering?
```

---
## \#13 Posted by: telnoi Posted at: 2018-07-04T17:53:27.181Z Reads: 27

```
Bridge the two silver pads marked 6s (within the white square bracket) with solder.

If the 7s pads are already bridged, you need to unsolder that in addition to the first step described.
```

---
## \#14 Posted by: gacsger Posted at: 2018-07-06T12:01:17.147Z Reads: 15

```
Thanks the help, the problem solved!
```

---
