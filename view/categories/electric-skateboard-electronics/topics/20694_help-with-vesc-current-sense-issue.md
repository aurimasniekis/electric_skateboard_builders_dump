# Help with VESC current sense issue

### Replies: 5 Views: 590

## \#1 Posted by: emepror Posted at: 2017-04-10T02:08:49.374Z Reads: 68

```
I've been working on diagnosing the issues with one of my VESC's and have noticed that the VESC in question thinks that the motor is drawing 80A+ at idle, with no battery draw. Obviously this is an issue and I have gone through a list of things trying to fix/diagnose this issue. If anyone has any ideas on what could be wrong or if I seem to have missed something please let me know. Potentially relavent riding history, the last time I went for a ride I blew the DRV8302 (VESC errored out) but did replace the chip

Things I have tried:
1. reflashing firmware, both 2.18 and 2.53
2. Confirming motors have no shorts/issues
3. Replaced DRV8302 (from previous issue)
4. Reflowed both MCU and DRV8302 (noticed both were slightly off from my assembly previously)
5. cleaned up many solder points and confirmed that all resistors and caps are well connected
6. cleaned and tested mosfets ( anyone got a good guide that i can double check i was seeing the right things?)
7. made sure sense resistors are soldered well and reading correct resistance.


I'm honestly a bit at a loss here, I managed to get the VESC to work well and not report crazy current levels after going through task 4 and 5 most recently but then when i went to put the whole board back together it started to act up again. Probably going to assemble another VESC to start fresh but I figured i'd try and see if anyone has had issues like this before.

Also, picture of realtime current data from BLDC-Tool:
<img src="/uploads/db1493/original/3X/5/c/5c7b48fde8b2393c247497d7261e50a5a13ed037.PNG" width="690" height="494">
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2017-04-10T03:42:50.297Z Reads: 54

```
Ok... did you check the mosfet, the shunt (it might be badly solder) and resistor r48 to r51... Also, what happen when your try to run motor detection...... And I do recommend to use a low voltage power supply, or if don't have repair all the defective part you might just blow up the drv again. :cry:
```

---
## \#3 Posted by: emepror Posted at: 2017-04-10T13:18:17.004Z Reads: 37

```
I've gone through and checked the soldering on all mosfets, same with the resistors and shunts. I think I'm going to go over them all again later. Running the motor detection causes the motor to stutter at points, definitely not a good detection if it passes correctly, but also fails with a bad detection result. 

The board used to work for the most part, I would get overcurrent errors occasionally, which makes me wonder if this has always been a problem

No smaller power supply right now, will probably be on order soon, till then it's trial by fire with the main battery
```

---
## \#4 Posted by: Fungineers Posted at: 2019-10-13T13:33:55.689Z Reads: 12

```
Hey did u figure out what was the issue? I have a similar issue. My vesc is always at 100% duty.
```

---
## \#5 Posted by: itsrow Posted at: 2019-10-13T16:21:32.280Z Reads: 12

```
3 years later man, I don't think this thread was even talking about 4.12 VESC's...
```

---
