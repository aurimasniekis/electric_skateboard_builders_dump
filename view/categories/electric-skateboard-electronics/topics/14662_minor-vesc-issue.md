# Minor VESC issue

### Replies: 8 Views: 880

## \#1 Posted by: Schulerbible Posted at: 2016-12-14T13:53:07.241Z Reads: 101

```
Hi guys, 

I am using two (most likely identical) Enertion 4.12 VESC's in my dual motor setup. I have set up the VESC's according to the recommendations given for a setup identical to mine. All works brilliant and I have already used the board for a couple of km's.  

Here is the thing. Both VESC's coming out of the same batch, one of them lights up a blue LED after that three red flashes and the other one lights up a red LED. Not sure why the VESC's behave different??? Should I worry that the red LED VESC will sooner or later fall apart??? 

Thanks
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2016-12-14T17:24:59.803Z Reads: 83

```
Can you post some picture? Is the blue and the red on the same position on each vesc?
```

---
## \#3 Posted by: lox897 Posted at: 2016-12-14T20:26:03.726Z Reads: 70

```
I'm taking a guess but could it be because one is master and the other is slave?
```

---
## \#4 Posted by: Schulerbible Posted at: 2016-12-14T20:46:02.285Z Reads: 63

```
Will post some picture this afternoon. I have never changed the configuration and both are not connected via canbus.
```

---
## \#5 Posted by: lox897 Posted at: 2016-12-14T23:29:08.970Z Reads: 48

```
How are they connected? PPM?
```

---
## \#6 Posted by: Schulerbible Posted at: 2016-12-15T10:14:52.545Z Reads: 38

```
Here we go. Bit hard to see but VESC 1 only lights up just the blue LED and VESC 2 lights up both.
I set up the VESCs individually and had this issue since they came out of the package. In the dual setup I split the RX signal. <img src="/uploads/db1493/original/3X/1/5/1571f7581a4f458b566e9b055324de5d1dc5dcd2.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/1/e/1eb9874dcf4f88de6a9f84380332d1ee0c7a311c.jpg" width="690" height="388">
```

---
## \#7 Posted by: Pimousse Posted at: 2016-12-15T10:20:37.630Z Reads: 37

```
You should use CAN communication between your VESC instead of Y RX cable. ;)

Anyway, connect the VESC which has the red led to BLDC Tool, go to Terminal tab and type FAULT.
You'll see if there is something going wrong.
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2016-12-15T13:54:14.728Z Reads: 29

```
Can you take a more clear picture (specially), but it seem like it just a mistake in the LED placement from the manufacturer, nothing to worry about.
```

---
