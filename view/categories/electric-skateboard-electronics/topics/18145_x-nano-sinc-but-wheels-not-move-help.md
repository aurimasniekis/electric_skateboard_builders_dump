# X-NANO sinc but wheels not move HELP!

### Replies: 22 Views: 1107

## \#1 Posted by: Kilian Posted at: 2017-02-23T16:06:23.403Z Reads: 83

```
Hello everyone ... I need some help ... I have my x-nano i sync it with the receiver that's ok ,,, my problem is when I press the trigger on the x-nano the wheels do not move .. Enter BLDC-TOOL and change it in App Configuration by PPM and still do nothing .. change and probe with all and the wheels do not move ,,, HELP please .. thank you in advance
```

---
## \#2 Posted by: Jebe Posted at: 2017-02-24T07:40:10.912Z Reads: 64

```
try swapping the channel
```

---
## \#3 Posted by: Deakbannok Posted at: 2017-02-24T08:26:34.247Z Reads: 63

```
1. Make sure to check your Tx and Rx are they binded? and wiring.

2. Check the voltage from VESC on your Rx connection and Motor.
 { If you have VESC-X, check if the green LED is active and responses to your controller when pressing it.}

If non of these work.
Do this once  > Reflash the firmware to stock and repeat step 1 to 2

If not, then the faulty on your vesc or controller
```

---
## \#4 Posted by: Jebe Posted at: 2017-02-24T08:53:02.293Z Reads: 60

```
reflash the vesc? Little extreme given how many issues there has been this the nano x.
I found I had to sync the damn thing on one channel, then swapped the connections and it worked.
There was also this [thread on binding issues](http://www.electric-skateboard.builders/t/enertion-nano-x-binding-issue-resolved/15740)
```

---
## \#5 Posted by: Kilian Posted at: 2017-02-24T11:01:08.046Z Reads: 49

```
Unfortunately I also tried it and it did not work, and then I put the post, but thanks anyway
```

---
## \#6 Posted by: Esrapp21 Posted at: 2017-08-15T01:48:54.568Z Reads: 27

```
Ok I’m having the exact same problem. The controller definitely binds, i can see it on both the rx and tx. But no matter what I do the wheel won’t move. Any luck here?
```

---
## \#7 Posted by: jammin Posted at: 2017-08-15T01:53:01.713Z Reads: 23

```
I'm 99% sure the nano-x communicates via PPM, not UART. Are you saying when you move the trigger, the PPM gauge moves? How about pressing the left/right buttons on your keyboard?
```

---
## \#8 Posted by: Esrapp21 Posted at: 2017-08-15T01:55:28.975Z Reads: 22

```
Yeah, it does move. I had to set it to uart for the iPhone connect app thing. Is this the probable cause?
```

---
## \#9 Posted by: SORRENTINO Posted at: 2017-08-15T01:56:54.592Z Reads: 21

```
Change it to ppm and uart then restart the vesc and see if that works. If you change the app config you need to restart the vesc. Could be your issue
```

---
## \#10 Posted by: jammin Posted at: 2017-08-15T02:04:24.244Z Reads: 21

```
yeah I'd stick just to PPM at the moment, it's more reliable than UART (especially in congested areas). Hope that fixes your problem!
```

---
## \#11 Posted by: Esrapp21 Posted at: 2017-08-15T02:10:20.561Z Reads: 20

```
None of this seems to be working. I’ll try some more tomorrow
```

---
## \#12 Posted by: Esrapp21 Posted at: 2017-08-15T02:12:43.239Z Reads: 18

```
The VESC is getting good voltage, the remote is connecting, it just seems that no power is going to the motor
```

---
## \#13 Posted by: jammin Posted at: 2017-08-15T02:13:58.047Z Reads: 19

```
does the motor move with the keyboard arrows? What's your battery voltage? I'm pretty sure the VESC will still be powered on (even if it's reached battery cutoff), but I'm not sure.
```

---
## \#14 Posted by: Esrapp21 Posted at: 2017-08-15T02:17:47.830Z Reads: 17

```
The motor moves with the keys, and the VESC is at the regular 41 volts. Is it possible I blew that DRV thing on the VESC?
```

---
## \#15 Posted by: jammin Posted at: 2017-08-15T02:20:12.542Z Reads: 17

```
uuuuhhhh unlikely. Go ahead and check out the DRV errors (keep in mind that the DRV errors reset when the VESC resets). VESC seems fine, you're running at 10s? What's the motor you're using?

It's hard to tell what's going on, but double check your BLDC settings (specifically app config). PPM should be checked and you should be getting the PPM gauge movin' around n stuff
```

---
## \#16 Posted by: SORRENTINO Posted at: 2017-08-15T02:24:55.540Z Reads: 16

```
Did you set up your control mode? As in current no reverse and write it to the vesc? Maybe the disabled box is checked.
```

---
## \#17 Posted by: Esrapp21 Posted at: 2017-08-15T11:50:43.675Z Reads: 15

```
The disabled box was checked, but when I changed it to current no reverse it still doesn’t work. And with current no reverse the arrow keys don’t work.
```

---
## \#18 Posted by: Esrapp21 Posted at: 2017-08-15T11:52:00.023Z Reads: 15

```
The ppm gauge is definetly moving perfectly. Just the motor won’t move with it.
```

---
## \#19 Posted by: Esrapp21 Posted at: 2017-08-15T11:58:31.168Z Reads: 15

```
I don’t know if this helps, but I’ll give you the whole backstory to how this started. I took off the enclosure to make some software upgrades; upgrading to FOC and adding the Perimetr software to change the settings over Bluetooth. After that the remote didn’t work.
```

---
## \#20 Posted by: Esrapp21 Posted at: 2017-08-15T22:59:34.422Z Reads: 16

```
So to bring all the symptoms together, the remote connects on both the rx and tx, and the ppm gauge moves. The voltage in the VESC is normal. When the disabled box is checked in control mode, the arrow keys can move the motor, but when current no reverse is checked, they can’t.
```

---
## \#21 Posted by: jammin Posted at: 2017-08-15T23:10:17.458Z Reads: 16

```
are you still connecting your phone to your VESC? So, no matter what, you can see the PPM gauge move? Just trying to get my bearings here...
```

---
## \#22 Posted by: Esrapp21 Posted at: 2017-08-15T23:15:47.226Z Reads: 17

```
It still connects to my phone, but I haven’t used the perimetr app, the one that I installed the firmware for, yet. I see the ppm gauge moving on the computer
```

---
