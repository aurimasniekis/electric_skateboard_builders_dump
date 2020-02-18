# Need confirmation for my Electronic schematic

### Replies: 4 Views: 290

## \#1 Posted by: Jammm Posted at: 2018-04-10T18:11:12.681Z Reads: 70

```
Hello,

I am building an electric mountainboard with two 6s lipo batteries. The goal is to be able to charge the batteries without taking off the enclosure.

I came up with this idea using three loop keys.

When the board is charging, the three loop keys are disconnected, and the charging ports are plugged in. Therefore, it's as if the two batteries weren't connected to anything.

When the board is rolling, the charging ports are disconnected and the loop keys are plugged in, and the schematic is like a regular electric skateboard. 

This is a rather intricate way to go, is my schematic correct ?
![scanner_20180410_192825[1]|353x500](upload://dUlfB2piFSxYSAq4FFfndwvuxe2.jpg)
```

---
## \#2 Posted by: FabianOdermatt Posted at: 2018-04-10T18:27:18.843Z Reads: 54

```
It looks good at all. But you don't need three loop keys. Two are enough. 
One for disconnecting the batteries from each other’s(in the middle) and one, you can decide which one, to disconnect the batteries from the ESC.(top or bottom)
```

---
## \#3 Posted by: Jammm Posted at: 2018-04-10T18:32:32.709Z Reads: 47

```
Do you know which is better between top and bottom ?
```

---
## \#4 Posted by: TheImmortalJew Posted at: 2018-04-10T18:42:54.026Z Reads: 44

```
You don't even need two, just use the one you have in the middle connecting the batteries in series. When connected, you're running 12S...when you disconnect, it becomes two independent 6S batteries that you can charge separately.
```

---
