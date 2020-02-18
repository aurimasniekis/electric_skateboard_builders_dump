# Another DRV blown

### Replies: 10 Views: 724

## \#1 Posted by: FabianOdermatt Posted at: 2018-03-14T19:13:45.343Z Reads: 146

```
Hey

I tried out the FOC mode on my VESC 4.12. 
(Setup: 10S LiPo, 245kV 6364 (high ERPM, I know))
I just did a bench test and after a hard brake my DRV8302 started smoking. When I plug in the VESC nothing happens and so I can't connect to the BLDC Tool. 
I will replace the DRV next week, but is it possible that there is another thing broken? Maybe something with the power supply? The rest of the VESC looks good and I couldn’t find something burned. 

Pics of my VESC:

![20180314_193252|281x500](upload://oGPCHGTNHOEIRLfqzpIXcsEZPut.jpg)  ![20180314_193202|281x500](upload://x4jAi1d8RGOfSo9nn4q9GM7EVcz.jpg)


Thanks for helping, you guys are awesome!

greets from switzerland
```

---
## \#2 Posted by: Scoo_B_SK8 Posted at: 2018-03-14T19:30:27.270Z Reads: 138

```
Toss us a screen shot of your settings...

Dbl check brake setting?

You cooked it...
```

---
## \#3 Posted by: FabianOdermatt Posted at: 2018-03-14T19:54:57.002Z Reads: 128

```
![FOC|690x388](upload://y9D2Tyts7YZZB7bqUt8JHFYO01z.jpg)  ![Motor|690x388](upload://CLG5RvvHqYbnvtn3XB5DSC7yHz.jpg)
```

---
## \#4 Posted by: Scoo_B_SK8 Posted at: 2018-03-14T23:58:39.029Z Reads: 101

```
i would look up what "motor MIN (regen)" does.:thinking:
```

---
## \#5 Posted by: MannyM0E Posted at: 2018-03-15T00:18:34.918Z Reads: 96

```
If it's the vesc from TB from what I read here, there highly not recommended for FOC mode. Also I notice you put 60a on battery max, like I said if it's from TB then their vesc could only handle 50a and for battery reg you put -20a which I think not good. I put -08a on mine
```

---
## \#6 Posted by: ShutterShock Posted at: 2018-03-15T00:42:13.519Z Reads: 94

```
Your motor min is fine, that does not directly translate to what actually goes into the battery.  However, the chances are that it was only the drv that blew.  

You could probably get away with leaving the -20, but I would recommend trying something like -12.  

Also, as mentioned, the TB VESC is not really recommended on the forum as FOC capable, probably just stick to BLDC for now.  They seem to talk it up on their website, but it is probably risky, as you found out, especially if you draw near the erpm limit.
```

---
## \#7 Posted by: E1Allen Posted at: 2018-03-15T01:56:19.218Z Reads: 85

```
Your battery min should relate to your specific battery.  Personally I use 2c for the 30q. But it's somewhere between your min and Max charge rate.  Dual vesc you need to split between both vesc.
```

---
## \#8 Posted by: FabianOdermatt Posted at: 2018-03-15T18:57:11.561Z Reads: 52

```
What I really wanted to ask: 
When **only** the DRV is burned, the rest of the VESC should work, right? So there is maybe an other thing broken, otherwise the LEDs would light and I could connect to the BLDC Tool. But what could it be? :thinking:
```

---
## \#9 Posted by: FabianOdermatt Posted at: 2018-03-15T19:00:01.726Z Reads: 51

```
And yes, I got it from TB and I won't try FOC again.
```

---
## \#10 Posted by: SOICDIP Posted at: 2018-03-15T19:00:14.614Z Reads: 50

```
[quote="FabianOdermatt, post:8, topic:49114"]
When only the DRV is burned, the rest of the VESC should work, right? So there is maybe an other thing broken, otherwise the LEDs would light
[/quote]

The drv supplies 5v to the system, so if it's dead, you wouldn't get any LEDs either.
```

---
