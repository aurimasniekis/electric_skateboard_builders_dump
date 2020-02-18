# Raptor 1 Issue: Motor will not rotate, it only jiggles

### Replies: 11 Views: 223

## \#1 Posted by: kisum95 Posted at: 2019-04-17T15:24:20.385Z Reads: 55

```
Hi guys, 

I bought a Raptor 1 (dual motor) long time ago, and I have not had any issues with it .. until now.

I rode my board today on my way to school, while starting to go up a slight hill it suddenly **lost all power**. I tried to switch the power off and on again to see if a reboot did the trick. It worked, but only for a short time. After 1-2 minutes of riding, the motor stopped again. **Now one motor turns, while the other just kinda jiggles**.

I found this post from two years ago, where a guy had the same issue, but it did not look like any solution was posted. Here is the video he posted of the problem (which is identical to my problem): 
https://photos.google.com/share/AF1QipPgTuh0nB2osLZ5UKuoHmOr04MnudAFpsf3Tlk1NoN2o396qNyC_7cjBuBz5Cn94Q?key=bWQzMGVzRDdidERTNDJmaEtyTlctdEJOTGpkZEpR

I have tried to connect my VESC to the BDLC tool and typed faults in the terminal, but it did not detect any faults.. 

Do any of you have a solution or recommendations for what I should do??

Thanks!
```

---
## \#2 Posted by: Jinra Posted at: 2019-04-17T15:27:45.712Z Reads: 50

```
If a motor doesn't move, don't apply too much throttle or you're liable to burn some components. Do FOC detection on both motors and post their values.
```

---
## \#3 Posted by: Blasto Posted at: 2019-04-17T16:09:14.955Z Reads: 43

```
![image|178x142](upload://9VZugcs9SqErKLdTmy59SfS00ys.png) 

something is up with this guy, the reason why the other wheel is "slow-jittering" is because of the traction control.
```

---
## \#4 Posted by: Blasto Posted at: 2019-04-17T16:14:22.336Z Reads: 37

```
oh wait, didnt read the entire post.. you are saying one motor turns and the other jitters?

sorry, bit hard to see if the bottom wheel is turning or not
```

---
## \#5 Posted by: kisum95 Posted at: 2019-04-17T16:14:26.873Z Reads: 38

```
I have read the FOC configurations for both FOC's: 
![02|690x364](upload://xDHY3RLhxe4W9J4wdcqIBLWrQWX.png) ![28|690x362](upload://6V8g4HCzWFUUO0T1GZfrddwio9T.png) 

Then I did the foc_state in the Terminal:
![20|418x500](upload://pnOvGDp88kvXMRoFbg1A3kbXRSW.png) ![28|351x500](upload://sV96PwbepU4AVinotkDZASXXA9C.png)
```

---
## \#6 Posted by: Jinra Posted at: 2019-04-17T16:15:52.716Z Reads: 35

```
I didn't mean read, but actually do detection. Specifically "Measure R and L" and "Measure Lambda"
```

---
## \#7 Posted by: kisum95 Posted at: 2019-04-17T16:35:35.171Z Reads: 34

```
Okay, I found it now (I think). The left one rotated, and the right one only jiggled.

And thanks for the quick response BTW! :-) 

 ![16|690x81](upload://yqj8sqaunHCq0lboCbMCntodL4H.png) ![47|690x78](upload://zWSNzj0FftdMSA4yyZ7eQ0mYwJf.png)
```

---
## \#8 Posted by: Jinra Posted at: 2019-04-17T16:45:05.080Z Reads: 34

```
Looks like the Right vesc motor might be shorted. Try turning it by hand, is there resistance when you try to turn it vs the other motor?
```

---
## \#9 Posted by: kisum95 Posted at: 2019-04-17T16:48:14.319Z Reads: 33

```
 The resistance is clearly higher when turning the left vesc motor compared to the right one..
```

---
## \#10 Posted by: Jinra Posted at: 2019-04-17T16:49:14.902Z Reads: 31

```
ah, then yea the one with higher resistance is shorted. Now to determind if it's a short in the motor or the vesc. Disconnect the 3 phase wires from the Vesc and try turning again. If resistance disappears then the VESC is shorted, if it's still present, then the motor is shorted.
```

---
## \#11 Posted by: kisum95 Posted at: 2019-04-17T17:15:42.047Z Reads: 29

```
I disconnected the motor that did not rotate (which also had less resistance). 
It is the one I spin first. It still has less resistance. 

The belts are fairly equal tight. 

Thanks for all the help so far! 

https://photos.app.goo.gl/DYj7c5SAtihS5tyj9
```

---
