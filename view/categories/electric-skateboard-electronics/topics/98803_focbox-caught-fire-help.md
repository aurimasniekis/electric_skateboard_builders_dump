# Focbox caught fire. Help?

### Replies: 8 Views: 342

## \#1 Posted by: benha Posted at: 2019-07-20T16:50:11.534Z Reads: 162

```
Hello, folks.

I have a legacy focbox that I bought last year and finally got around to trying to set up this week.  Didn't go well.

I hooked up to a 30A lab power supply at 27V. I tried doing the motor detection stuff in the BLDC tool and it failed.  Upon doing some further research I realized that I shouldn’t have anything connected to the motor when I do that, so I powered down the power supply and removed it from where it was installed, positioning it on the bench to configure.

I then turned the power supply back on and plugged the USB cable in, and as I was reaching for the mouse to connect to the FocBox in the BLDC tool USB port on the FocBox caught fire. I’m not sure how extensive the damage is given the blue light still comes on and I can't see any visible damage to other components, but I’m not able to use the USB port anymore.  (Actually hosed that USB input on the PC too, which really sucks.)

Enertion doesn't have any more of these, so I'm SOL with them.

A few questions here:

Before I try to solder a new micro USB port to the board (which will be a challenge):  Is it possible to configure this thing without USB?

Anyone have thoughts on what might have caused this?  I'd prefer not to repeat the disaster if I get the board working again.


Thanks,

-Ben

PS - To the extent it matters, this isn't being installed in an eSk8 application, but this is clearly the land of experts when it comes to VESCs and BLDCs.  I hope you guys don't mind.
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-07-20T17:15:29.095Z Reads: 148

```
@JohnnyMeduse
```

---
## \#3 Posted by: banjaxxed Posted at: 2019-07-20T17:49:02.284Z Reads: 141

```
Did you use an anti-spark? Presumably just turned on the power supply.

Motors need to be connected beforehand
```

---
## \#4 Posted by: benha Posted at: 2019-07-20T18:12:34.288Z Reads: 132

```
The motor was connected.  No anti-spark but it was connected to the PS and then I turned on the PS.  Regardless, it's hard to imagine why a spark on the mains would cause the USB port to let the smoke out, no?
```

---
## \#5 Posted by: trampa Posted at: 2019-07-20T23:49:18.797Z Reads: 110

```
Probably PS on the same circuit as computer.
Ground loop via USB smoked up something.

Best Practice: Laptop without connection to the grid.
```

---
## \#6 Posted by: banjaxxed Posted at: 2019-07-21T07:43:39.613Z Reads: 83

```
You can test with a 3s lipo afaik
```

---
## \#7 Posted by: SimosMCmuffin Posted at: 2019-07-22T09:16:42.076Z Reads: 42

```
I suspect this as well.

Either use a battery to power the ESCs to isolate them from power ground and then connect the USB or if powering via PSU then use a laptop to isolate the other end.

Or get an isolation transformer and power the PSU through that to get a floating supply.
```

---
## \#8 Posted by: ShutterShock Posted at: 2019-07-22T16:01:04.588Z Reads: 26

```
huh I actually never thought about this,  I always just use a laptop because I end up doing configurations in the garage or somewhere besides my desk

Guess it is a good thing to remember that this could happen
```

---
