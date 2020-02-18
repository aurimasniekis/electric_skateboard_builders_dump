# Can Bus Focbox throttle curve setup question?

### Replies: 9 Views: 386

## \#1 Posted by: ksfacinelli Posted at: 2018-06-18T22:50:38.583Z Reads: 124

```
When you setup dual Focbox over Can Bus does the master report throttle control or do you need to setup for both slave and master?
```

---
## \#2 Posted by: mmaner Posted at: 2018-06-19T01:24:37.757Z Reads: 115

```
I think you have to do both, but I'm not positive. 
I've always done with because when I first started using throttle curves it did not  it may  in later firmware revisions  Goodestion.
```

---
## \#3 Posted by: ksfacinelli Posted at: 2018-06-19T02:52:45.194Z Reads: 101

```
I guess I can set both up just was hoping to find an answer as it would be easier to setup master.  When setuping master would you suggest saving the file and uploading to slate?
```

---
## \#4 Posted by: Slak Posted at: 2018-06-19T12:08:30.975Z Reads: 83

```
If you are using CAN Bus, only one of your 2 ESC is connected to the receiver. So why would you set a curve up on both ESC (only one is getting the signal from the receiver) ?

I may be wrong but it seems just pure logic for me.
```

---
## \#5 Posted by: ksfacinelli Posted at: 2018-06-19T13:16:51.158Z Reads: 73

```
Thanks your logic makes complete sense....I originally had split PPM and switched to can bus.  Thanks for sharing what I should have seen as obvious.

Kevin
```

---
## \#6 Posted by: Eboosted Posted at: 2018-06-19T18:38:08.890Z Reads: 62

```
If using can bus, you only need to set throttle curve on the master
```

---
## \#7 Posted by: ksfacinelli Posted at: 2018-06-19T18:57:04.050Z Reads: 60

```
Thanks....I find that runnning can bus is a lot smoother than split ppm.  I think the difference was due to PPM calibration on both modules vs running through only master.  The motors are completely synchronized with can bus enabled.

Kevin
```

---
## \#8 Posted by: Eboosted Posted at: 2018-06-19T19:47:18.221Z Reads: 56

```
I'm running two receivers and both ESCs as master in case one receiver fails.
```

---
## \#9 Posted by: ksfacinelli Posted at: 2018-06-19T20:14:24.960Z Reads: 51

```
I noticed it was difficult to get both wheels synchronized but that may be how I setup PPM and throttle...I think if I would have writen down exact values and loaded both Focbox the same  it should be better.
```

---
