# Quick check my stuff thread!

### Replies: 10 Views: 824

## \#1 Posted by: Jack Posted at: 2016-06-21T21:01:44.206Z Reads: 98

```
So theres loads of info on this forum which is fab but sometimes takes a while to find info, I thought it would be cool to have a place to post a quick question or diagram on a dedicated thread for a quick answer or to double check if you've done something right. Even really experienced builders could do with a second opinion sometimes!

I'll kick off with a diagram of a 10s2p flat pack I'm building. Am i right?! ;) (Numbers correspond to BMS wires or balance)

<img src="/uploads/db1493/original/2X/1/15f07090c1799bf74ba427b18bff4b23f9f66a64.png" width="454" height="500">
```

---
## \#2 Posted by: Maxid Posted at: 2016-06-21T21:04:53.132Z Reads: 86

```
the balance cables are alway the series number + 1. So in your case you need 11 - starting with the common ground where you wrote "batt cathode"
```

---
## \#3 Posted by: Jinra Posted at: 2016-06-21T21:08:21.863Z Reads: 82

```
Depends on the BMS, battery supports has a great diagram to check with for their BMS's. There's 1 lead per series, though you can argue that the 11th one is the negative that goes to the BMS ground.

http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html
```

---
## \#4 Posted by: Jack Posted at: 2016-06-21T21:10:39.751Z Reads: 77

```
@Maxid yeah my BMS has a separate ground for the negative :D
```

---
## \#5 Posted by: Jinra Posted at: 2016-06-21T21:12:19.467Z Reads: 74

```
Your diagram looks good :)
```

---
## \#6 Posted by: Maxid Posted at: 2016-06-21T21:21:14.177Z Reads: 74

```
I would double check if your bms actually does not need the first one to be ground again. As far as i know the BMS takes a standard balancer plug from for example Lipo packs as well and they always have the first one as ground. A balancing plug always has the ground in it as well.
```

---
## \#7 Posted by: Jack Posted at: 2016-06-21T21:25:55.590Z Reads: 72

```
This is the diagram of my previous pack which worked fine. I just followed the diagram from Battery Supports haha
<img src="/uploads/db1493/original/2X/3/31d2730e72c99a332748c2bb227cc195f592d113.png" width="690" height="305">
```

---
## \#8 Posted by: Jinra Posted at: 2016-06-21T21:27:44.732Z Reads: 70

```
Just curious, why do you have an anti-spark loop as well as an anti-spark switch? Additional safety?
```

---
## \#9 Posted by: Maxid Posted at: 2016-06-21T21:28:26.742Z Reads: 69

```
Yeah I just checked their diagram and they indeed use the "wrong" balancer plug. This can be really dangerous when people just want to hook up their Lipo pack to a BMS. Also you will not be able to hook the "wrong" balancer plug into a balance charger.
```

---
## \#10 Posted by: Jack Posted at: 2016-06-21T21:30:47.414Z Reads: 64

```
@Jinra Yeah honestly I didn't 100% trust the anti-spark at first and preferred the fool proof disconnect method. Although now I'm just using the anti-spark haha 

@Maxid Yeah its strange I desoldered the connector from the BMS and soldered the balance wires straight into the PCB to stop that happening in the future :smiley:
```

---
