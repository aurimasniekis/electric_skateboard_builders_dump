# Remote input not registered by vesc after failure and subsequent DRV replacement

### Replies: 13 Views: 603

## \#1 Posted by: BigBoyToys Posted at: 2017-02-05T22:25:37.532Z Reads: 53

```
Looking for input and ideas as to what might be causing this issue. 

I burned a DRV after overheating a Jacob's hubs motor. I replaced the DRV and now there are no faults registering but I'm unable to control the VESC with the remote. 

When viewing the remote input under the ppm tab it just stays at 50%. I'm also unable to control it via the CAN bus where it says no response from hardware.

Any ideas?

I've noted that the motor detection works and I'm able to control the motor via the arrow keys, I just can't control it via the remote or the master VESC.

I've also verified the remote/receiver is working since when I  plug it into the other vesc it works just fine.

Thanks guys
```

---
## \#2 Posted by: BigBoyToys Posted at: 2017-02-06T19:43:01.387Z Reads: 40

```
@JohnnyMeduse

Have u seen this before my good sir?
```

---
## \#3 Posted by: Luke Posted at: 2017-02-06T19:58:45.087Z Reads: 39

```
Have you ensured that the remote is binded correctly? It's probably worth trying to rebind it if you haven't tried
```

---
## \#4 Posted by: BigBoyToys Posted at: 2017-02-06T20:22:54.841Z Reads: 37

```
Hi Luke,

Thanks for your response. I have tried rebinding the remote.  This is a dual VESC set up. The remote works just fine on the 1st vesc, but when I plug the receiver into the 2nd vesc it does nothing. I know it's not settings related as I've copied the settings on the 1st VESC to the 2nd. 

Pretty confident it's hardware or firmware related. 

I'm hoping one of the VESC gurus, maybe @chaka can point me in the right direction in terms of board components to test or replace.
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2017-02-06T20:28:45.190Z Reads: 34

```
Can you check if you have a 5v on the ppm pin ? Or if the tvs diode (d5) is still alive ?
```

---
## \#6 Posted by: Luke Posted at: 2017-02-06T20:40:41.745Z Reads: 33

```
Ah, are your ppm settings exactly the same on both vescs? 
I believe that on the master vesc (controller ID  assigned is usually 0) you're supposed to have "send status over can"  unticked 
And for the slave vesc, it is usually ticked. 
I may be going down the wrong path, but  I just want to help how I can :p
```

---
## \#7 Posted by: BigBoyToys Posted at: 2017-02-06T21:10:38.493Z Reads: 30

```
I do have 5V on the PPM pin and D5 checked out ok as well, any other ideas?
```

---
## \#8 Posted by: BigBoyToys Posted at: 2017-02-06T21:15:49.704Z Reads: 30

```
That's correct Luke, send status over can was checked for the slave and not for the master when I was trying to drive the VESC via CAN. I also tried to drive the VESC via PPM control and ensured the PPM was selected under the application tab as well.
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2017-02-06T21:18:27.760Z Reads: 30

```
Where you able to run a motor detection after you replace the drv
```

---
## \#10 Posted by: BigBoyToys Posted at: 2017-02-06T22:05:41.853Z Reads: 25

```
Yes, I was. Motor detection completed successfully.
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2017-02-06T22:29:51.463Z Reads: 25

```
Are you sensor or sesorless, and can you check if the motor is set properly?
```

---
## \#12 Posted by: pyttroll Posted at: 2017-02-06T22:41:42.109Z Reads: 25

```
I had a similar issue with my VESC, running in hybrid mode, one of the wires on the sensor cable was disconnected.
```

---
## \#13 Posted by: BigBoyToys Posted at: 2017-02-07T05:54:30.181Z Reads: 17

```
Smh, I didn't reboot the VESC after changing from no app to ppm on the App.configuration tab. 

Thank you both for your help.
```

---
