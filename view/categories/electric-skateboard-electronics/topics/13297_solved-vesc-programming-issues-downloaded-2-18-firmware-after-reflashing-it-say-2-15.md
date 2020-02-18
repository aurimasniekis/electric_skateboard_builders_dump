# \[SOLVED\] VESC programming issues_downloaded 2.18 firmware after reflashing it say 2.15

### Replies: 10 Views: 3283

## \#1 Posted by: ninja Posted at: 2016-11-19T01:13:26.959Z Reads: 218

```
Hi builders! Right now i'm programming VESC from enertion, it had 2.18 firmware. I uploaded  firmware from BLDC tool which said it's supported for 2.17 and 2.18 but now it's reading like it's 2.15 firmware. Now it's say:

 Connected vesc got too old firmware, since connected vesc has firmware with bootloader support, it can be updated from firmware tab. Until then limited communication mode will be used...

What does it mean, what i should do now?  I just don't know what to do next! Hope for same advice. I've tried to find answers in searching bar, found about 3-4 times when people had the same issue, but nobody had given good solution. 

Why all downloaded 2.18 BLDC tools for windows from different sources that i had have this thing, that after refreshing 2.18 actually make it 2.15?

Other thing are bugs, should i be worried about them in 2.15 firmware?
```

---
## \#2 Posted by: sl33py Posted at: 2016-11-19T01:24:12.854Z Reads: 211

```
Using Windows, Mac, or Linux BLDC tool?
```

---
## \#3 Posted by: ninja Posted at: 2016-11-19T01:25:16.252Z Reads: 204

```
Windows BLDC TOOL.
```

---
## \#4 Posted by: sl33py Posted at: 2016-11-19T01:26:23.063Z Reads: 194

```
OK - which version are you using and from where?

what version is your VESC specifically.  what does it say on the PCB of the board?
```

---
## \#5 Posted by: ninja Posted at: 2016-11-19T01:29:06.190Z Reads: 190

```
I'm using BLDC TOOL from this site http://www.esk8.de/tutorials-d-e-f/ 
On PCB say 4.12
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2016-11-19T02:17:42.378Z Reads: 181

```
maybe try Jacob BLDC TOOL http://vesc.net.au
```

---
## \#7 Posted by: sl33py Posted at: 2016-11-19T02:57:37.067Z Reads: 175

```
What Johnny said - make sure you are using hte correct version of the BLDC tool for your board v4.12 and firmware.
```

---
## \#8 Posted by: ninja Posted at: 2016-11-19T10:42:14.844Z Reads: 165

```
I downloaded BLDC tool for 2.15, so everything working now! But i want new version without bugs, like 2.18. How can i upload 2.18 if it allows only 2.15? How does it possible that my VESC has so old firmware 2.15, i bought it maybe just 3 months ago? So it means that they sold me some old VESC or something? O.K. i don't care if it's 2.15 or 2.18 as long as it's without firmware bugs. So how can i tell if my 2.15 version have bug or not?
```

---
## \#9 Posted by: yaca Posted at: 2016-11-19T11:02:58.191Z Reads: 153

```
Why don't you use the latest newest best BLDC Tool and firmware 2.51?

http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-and-individual-throttle-curve/12286
```

---
## \#10 Posted by: ninja Posted at: 2016-11-21T00:16:57.908Z Reads: 134

```
So topic issue is solved, big thanx to Jacobbloy! He told me to do this and this helped straight away:) - 

"i think the problem is that when you update bldc tool on windows it does not delete and replace the old files, so you have to delete the old firmware files then install again or just download the files again."
```

---
