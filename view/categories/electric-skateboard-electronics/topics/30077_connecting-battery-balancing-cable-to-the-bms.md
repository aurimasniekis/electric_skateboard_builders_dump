# Connecting battery balancing cable to the bms

### Replies: 11 Views: 996

## \#1 Posted by: karosass1 Posted at: 2017-08-08T16:49:08.270Z Reads: 93

```
I guess I didn't specify this when describing battery requirements, but long story short, my battery has balancing cables designed for smart lipo balancing chargers. Here's the balancing cable with explanation:
http://i.imgur.com/900IPQe.jpg

Meanwhile BMS expects 10 wires:
http://i.imgur.com/6DQMdsw.jpg

How should I rewire it so that it would be compatible with the bms?
```

---
## \#2 Posted by: Jinra Posted at: 2017-08-08T17:18:18.853Z Reads: 87

```
Ignore 1 as it's pack negative. 2 will be 1, 3 will be 2, 4 will be 3, and so on.

However, even with any advice (including mine) you're given on here, please make sure you probe the header with a multimeter to verify voltage before plugging it in.
```

---
## \#3 Posted by: karosass1 Posted at: 2017-08-08T17:22:00.261Z Reads: 86

```
So red (last wire) is 10th balancing cable on the bms?
```

---
## \#4 Posted by: Jinra Posted at: 2017-08-08T17:23:50.877Z Reads: 81

```
Should be. Use a multimeter probe and hold the black (neg) to battery negative. Use the red probe to probe each wire on the header. It should go up by multiples of about 3.8v~ starting at 3.8v~
```

---
## \#5 Posted by: karosass1 Posted at: 2017-08-08T17:25:20.134Z Reads: 78

```
Ahh, that explains it, I was weirded out that all balancing cables are negative and the last one is positive. And yeah, first and last cables provide full pack voltage.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-08-08T17:58:35.816Z Reads: 74

```
Whoever made the battery just didn't bother to color code the cell wires. 
Either way, "Trust No one"
Do as Master Jinra said and test the voltage of each wire.
```

---
## \#7 Posted by: taycro Posted at: 2018-03-24T03:56:15.345Z Reads: 41

```
@Jinra @karosass1 I get what you guys are saying about forgetting about the 1st black wire, but I still don't see how it will plug in. If the balancing cable is "11" wide and the BMS port is only "10" wide, how will it fit? I am just curious because I am planning my first board right now and I think I will have the same problem and I just want to make sure that I understand it.
```

---
## \#8 Posted by: Jinra Posted at: 2018-03-24T05:02:06.988Z Reads: 39

```
you need to get a 10 pin header of of the correct JST variant/pitch and use a pint to take out the wires from the header to place into the new header.
```

---
## \#9 Posted by: taycro Posted at: 2018-03-24T15:34:15.977Z Reads: 34

```
Are you saying that he can use 10 of the 11 wires but has to get a new end that is 10 and not 11? So, wouldn't it have just been easier to get a JST that had 10 to begin with?
```

---
## \#10 Posted by: Jinra Posted at: 2018-03-25T02:06:22.634Z Reads: 31

```
yes, but if the battery comes with an 11 pin connector, it's easier to get a 10 pin connector.
```

---
## \#11 Posted by: GrecoMan Posted at: 2018-03-25T02:33:51.262Z Reads: 32

```
you can always pull a me (not recommended)

and cut the connector
```

---
