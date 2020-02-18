# \[Solved\] What is the Fault code meaning for HW6.X as 3 red flashes of dot, dot, dot

### Replies: 4 Views: 191

## \#1 Posted by: chuttney1 Posted at: 2018-06-17T04:43:26.419Z Reads: 71

```
I do not have a battery of 36V hooked up to my derivative yet, but manage to get the boot-loader and firmware uploaded using the 5V coming from the USB port, It somewhat supplies enough power to initialize the MCU giving me blue, red, and green flashes. What is the meaning of having 3 red flashes of dot, dot, dot with a 1 second pause between each sequence?
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2018-06-17T15:24:07.062Z Reads: 50

```
dvr  error usually....
```

---
## \#3 Posted by: deltazeta Posted at: 2018-06-17T16:02:49.104Z Reads: 41

```
If you don't have the battery connected this is pretty normal. The drv isn't being supplied enough power from the USB port so it thinks there's a fault. Should go away once you power it correctly.
```

---
## \#4 Posted by: chuttney1 Posted at: 2018-06-18T04:27:04.768Z Reads: 22

```
I connected a 12 V battery and the red led light sequences no longer shows up. I should mention it is really dim, but it does solve the issue as probably being too low of a voltage for the MCU.
```

---
