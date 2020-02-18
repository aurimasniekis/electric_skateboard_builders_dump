# Carvon Single v.2.5 max speed 22mph in FOC Mode. WHY?

### Replies: 8 Views: 629

## \#1 Posted by: NAF Posted at: 2017-06-25T21:58:26.562Z Reads: 122

```
Guys can any one take a look at my VESC settings for my CARVON Single v.2.5 with 10s4p battery (no fuse) 60amp bms. 
In general FOC MODE works really well. It's super silent, smooth acceleration and breaking. 
I am hitting max 22mph with these settings:

<img src="/uploads/db1493/original/3X/8/d/8d1614d3af57d6666f710a55f8da4eb7dd5987bd.png" width="690" height="360">

Is there anything I could tweak to get some more speed ? @makevoid @evoheyax ??
@Ackmaniac Can I use Max Watt set to 1000 ??
```

---
## \#2 Posted by: NAF Posted at: 2017-06-26T05:16:10.024Z Reads: 80

```
Anyone could help ?
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2017-06-26T05:19:50.721Z Reads: 80

```
I shall ping @Blasto
```

---
## \#4 Posted by: NAF Posted at: 2017-06-26T05:20:44.205Z Reads: 80

```
@Michaelinvegas btw what max speed do you hit on your 12s?
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2017-06-26T05:21:14.521Z Reads: 79

```
30 plus easy ... 33 was the fastest..not even trying
```

---
## \#6 Posted by: NAF Posted at: 2017-06-26T05:21:41.449Z Reads: 80

```
Yeee. that's what I thought.
```

---
## \#7 Posted by: NAF Posted at: 2017-06-26T05:32:16.834Z Reads: 80

```
I was thinking of setting Motor Max to : 80a and lowering Max ERPM value, but I have no fuse on my BMS and I am wondering if it's safe. The BMS has over-current protection and some short protection as well.
```

---
## \#8 Posted by: HTownBomber Posted at: 2017-06-26T12:09:18.297Z Reads: 54

```
IIRC, some of the carvon 2.5s were set at 85Kv (149Kv re-terminated to Wye = 149Kv/√[3]).

10s li-ion at 85Kv with 90mm wheels yields a weighted top speed of ~24mph:

http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":10,"motor-kv":85,"system-efficiency":75,"motor-pulley-teeth":1,"wheel-pulley-teeth":1,"wheel-size":90}|
```

---
