# Upgrade Vestarboard V2 ESC with Flipsky 4.20 plus

### Replies: 4 Views: 78

## \#1 Posted by: MarcoTeo Posted at: 2020-02-06T03:45:28.012Z Reads: 25

```
Hi Guys,
I fried my V2 Esc and I am trying to replace it with the Flipsky 4.20 plus but without good result so far.
After the setup with Vesc Tool the board is very slow with an awful start, basically no power, no torque ...very slow start and I can't understand why.... The motor are the cheap chinese 5055 sensorless but It should work better with a Vesc rather  than the original esc.
Thanks for any help
Cheers
Marco
```

---
## \#2 Posted by: ZachTetra Posted at: 2020-02-06T03:48:42.264Z Reads: 24

```
Make sure you run detection correctly and have the right settings for the remote

Can you show us the current settings and verify the remote takes it to 100% signal at full throttle?

Also make sure you are actually applying the settings, not just typing them in

If you think the drive train is at fault I have a dual PropDrive 5060 set up for sale
```

---
## \#3 Posted by: MarcoTeo Posted at: 2020-02-06T04:55:46.905Z Reads: 22

```
Hi Zach,
I tried the wizard detection but in Foc is even worse then I did manually in BLDC, but it is struggling to start, no torque,  It run smoothly on air but not on the ground.  The throttle is 100% and I applyed all the setting...like you said sometimes It can happen to write the values but not to  actually write on the Vesc.
I start to play with this values and it seems affect the run but I did not get any good result.
![20200206_125136|690x388](upload://9BQbq0iwX12Hrd33VJOGVog9bzJ.jpeg)
```

---
## \#4 Posted by: ZachTetra Posted at: 2020-02-06T05:16:04.648Z Reads: 19

```
Hmm that's strange, I've almost always had good luck with getting FOC running on everything.  So the no load behavior is fine but it struggles on the ground?  Can you show me the Motor Settings > General > Current tab?

You might be able to find help from someone much smarter than me on the eskate news forum instead of here
```

---
