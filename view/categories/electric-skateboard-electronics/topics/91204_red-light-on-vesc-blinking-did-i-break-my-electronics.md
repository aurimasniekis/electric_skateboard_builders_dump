# Red light on VESC blinking (Did I break my electronics?)

### Replies: 9 Views: 240

## \#1 Posted by: iamking Posted at: 2019-04-20T05:29:59.950Z Reads: 65

```
I have a VESC from diyelectricskateboards.com but I'm not why it won't work. 

So I tried hooking up my VESC to a battery and an SK3 motor. For some reason, it just keeps flashing red. The first time I did it, I was able to control the motor with my keys but after holding on to the keys for a while, it stopped working. Did I permanently break it?

I tried changing the battery cutoff and start to suggested values on other forums but I can't even seem to "upload" the data onto the VESC.

When I read the configuration, this is what pops up.

![37%20PM|690x419](upload://2wKyv6qijiCBOXtBETX8vYwUEDY.png)
```

---
## \#2 Posted by: b264 Posted at: 2019-04-20T05:38:09.586Z Reads: 63

```
Type "faults" into the terminal and paste what you see here
```

---
## \#3 Posted by: bigben Posted at: 2019-04-20T06:00:17.348Z Reads: 61

```
Did you do the motor detection before you started pressing the keys to run the motor?
```

---
## \#5 Posted by: iamking Posted at: 2019-04-20T06:02:21.031Z Reads: 58

```
Yes! I did motor detection and then it started working then after pressing keys for a while to run the motor, suddenly it stopped working. I think I tried clicking apply and write configuration.
```

---
## \#6 Posted by: iamking Posted at: 2019-04-20T06:04:35.364Z Reads: 56

```
I found it. 

The following faults were registered since start:

Fault            : FAULT_CODE_DRV8302
Current          : -0.2
Current filtered : 0.3
Voltage          : 46.92
Duty             : 0.01
RPM              : 0.9
Tacho            : 7
Cycles running   : 3
TIM duty         : 618
TIM val samp     : 314
TIM current samp : 24500
TIM top          : 48373
Comm step        : 1
Temperature      : 25.37

Fault            : FAULT_CODE_DRV8302
Current          : -0.2
Current filtered : -0.1
Voltage          : 46.92
Duty             : 0.02
RPM              : 1.4
Tacho            : 8
Cycles running   : 4
TIM duty         : 991
TIM val samp     : 523
TIM current samp : 22415
TIM top          : 43784
Comm step        : 2
Temperature      : 25.44
```

---
## \#7 Posted by: iamking Posted at: 2019-04-20T06:14:00.755Z Reads: 52

```
![IMG_3024|375x500](upload://3NlhvTRLFuDhEZqWQZEzrP6II0D.jpeg) 

Here is a photo of my setup. It's a 12S2P battery. Would love to get advice for the parameters I should be putting in when I am able to do so though.
```

---
## \#9 Posted by: iamking Posted at: 2019-04-20T08:05:58.417Z Reads: 42

```
Oh no! Does that mean I need to buy a new VESC? How did I toast it? My bad. Would you all have tips on what parameters I should put on before I try running my VESC next time?
```

---
## \#10 Posted by: Sn4pz Posted at: 2019-04-20T11:54:09.435Z Reads: 36

```
I'm assuming you're a US based person, so I'll point you towards @JohnnyMeduse ( the OG wizard) and @ThermalM16 (another option in the states)

These guys both do vesc repair, and will get you up and running for less than a new ESC 👍(if it's repairable)
```

---
## \#11 Posted by: iamking Posted at: 2019-04-26T21:45:49.904Z Reads: 21

```
Thanks! I reached out to both of them.
```

---
