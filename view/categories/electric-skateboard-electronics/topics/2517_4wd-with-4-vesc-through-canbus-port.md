# 4wd with 4 vesc through canbus port?

### Replies: 7 Views: 1210

## \#1 Posted by: evoheyax Posted at: 2016-04-22T18:50:18.792Z Reads: 159

```
I was wondering if anyone has tried to use 4 vesc's connected through the canbus to create a 4wd?

Is it possible to have more than 1 slave vesc connected by the canbus port?

what would a wiring diagram for this look like?

Curious as I'm thinking to buy 4 hub motors next time @hummie or @jacobbloy does a batch, and make it happen.
```

---
## \#2 Posted by: chaka Posted at: 2016-04-22T19:11:18.361Z Reads: 152

```
I have a customer with 8 vesc linked through the canbus. It is for a university competition so I can't give any details other than it works very well!
```

---
## \#3 Posted by: evoheyax Posted at: 2016-04-22T19:14:22.751Z Reads: 153

```
Would you just daisy chain them?

Or should each be connected to the master's canbus?
```

---
## \#4 Posted by: chaka Posted at: 2016-04-22T19:15:33.901Z Reads: 149

```
Daisy chain or splitter, it is all the same.
```

---
## \#5 Posted by: laurnts Posted at: 2016-04-22T19:19:19.948Z Reads: 145

```
I think you should do master slave rear drive then use splitter for the front master slave combination.
```

---
## \#6 Posted by: trbt555 Posted at: 2016-04-22T20:03:03.746Z Reads: 139

```
One master, three slaves, doesn't matter how they're connected, it's a bus so as long as both wires are connected to the canbus pins on each vesc, it should work.
```

---
## \#7 Posted by: laurnts Posted at: 2016-04-22T20:07:12.812Z Reads: 135

```
Owhh yes right didnt think about that! Great to know Tom! As long as all of the slave id are different, they gona respond to one master :)
```

---
