# \[RESOLVED\] VESC DRV8302 Fault Code. Is my VESC dead?

### Replies: 17 Views: 3426

## \#1 Posted by: Alanhunt123 Posted at: 2016-10-05T13:57:40.538Z Reads: 394

```
Hi, I am having some issues with my VESC purchased from Enertion. It is running 2.18 firmware, and was working great with my setup for about a day. It is 8s, with a 245kv Turnigy motor, and a 14-40 belt ratio on 83mm wheels, nothing too taxing to run. Now, when I try to run the motor, the red led flashes 3 times, waits, and flashes another 3 times. Sometimes, I can get the motor to spin up, and the throttle responds fine, but once the motor stops again, it won't start again for at least a few minutes.

I opened up the bldc tool, and went to the terminal and typed "faults", and it threw me a "DRV8302 Error". Anybody know what this means?
```

---
## \#2 Posted by: TarzanHBK Posted at: 2016-10-05T14:10:58.117Z Reads: 379

```
that means your DRV chip is cooked and need to be replaced. this is the most common vesc failure and there only few people who can really figuring out why this happens. Could be due to a short or to some wrong configuration in your bdlc tool.
```

---
## \#3 Posted by: SORRENTINO Posted at: 2016-10-05T14:21:24.416Z Reads: 367

```
I think common four reasons why this happens. you have a short, bldc settings wrong, FOC settings wrong, Long power wires to vesc. Maybe post a screen shot of your vesc settings
```

---
## \#4 Posted by: Alanhunt123 Posted at: 2016-10-05T14:36:01.112Z Reads: 356

```
<img src="/uploads/db1493/original/3X/6/b/6b47c2cfbacb95b5dc5c64e0b0682e1984a5550f.PNG" width="690" height="407">
Here's a screenshot
```

---
## \#5 Posted by: Alanhunt123 Posted at: 2016-10-05T14:36:59.216Z Reads: 338

```
There are no burn marks around the DRV chip that I can see, it seems ridiculous that after 1 day of use the thing is toast
```

---
## \#6 Posted by: rpn314 Posted at: 2016-10-05T20:36:22.433Z Reads: 322

```
Those settings don't seem odd. What's in your advanced tab there?
```

---
## \#7 Posted by: Alanhunt123 Posted at: 2016-10-05T23:28:21.999Z Reads: 314

```
The issue is now being handled. After some troubleshooting with Charles from from Enertion, we determined something is wrong with the board. I am now sending the board to be fixed by him.
```

---
## \#8 Posted by: SvantePanter Posted at: 2016-10-09T18:32:06.755Z Reads: 298

```
Hi @Alanhunt123 !
I have the same error, although I´m on a v.4.12 VESC (v.2.18 firmware) from DIYelectriclongboard.com / @torqueboards . I'm out riding, everything works fine. And suddenly the throttle doesn´t work/the motor wount run. After a second or so it works again.

I can repeat the error at home when connected to BLDC Tools. Sometimes I get the DRV8302-code.

Did you recieve a new VESC? Any theories from Charles at Enertion?.
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2016-10-09T19:07:03.152Z Reads: 286

```
Are you ridding FOC or BLDC
```

---
## \#10 Posted by: Alanhunt123 Posted at: 2016-10-09T19:17:43.230Z Reads: 283

```
I was riding BLDC. Since I did not have their premium version, they were not able to replace it. However, I was able to send it in the mail to get the DRV chip replaced. Charles is going to check my settings once it arrives to see if anything was incorrectly set. I'm going to update the firmware as soon as I get it back, as I think I saw someone on this forum say that Enertion's boards need to be updated.
```

---
## \#11 Posted by: Alanhunt123 Posted at: 2017-02-22T04:25:51.320Z Reads: 249

```
Sorry for not updating this for a while. The VESC I got back also burned its DRV within 50 miles. So, I was able to get a different board that was used from Enertion. No problems with it whatsoever.
```

---
## \#12 Posted by: ARollNation Posted at: 2017-09-19T00:42:50.299Z Reads: 194

```
Is the enertion one still holding up well?
```

---
## \#13 Posted by: Alanhunt123 Posted at: 2017-09-19T04:24:24.791Z Reads: 188

```
Oh, that one is long gone. Kept burning DRVs. I now have FOCBOX from Enertion, and it is such a step up from the regular 4.12 hardware, there is no comparison!
```

---
## \#14 Posted by: zepton Posted at: 2018-04-27T20:41:16.891Z Reads: 120

```
I just got a DRV8302 fault when I switched my board to 9S (I just plugged in the batteries on the bench I didn’t ride it. It works perfectly fine with 6S, and when I switched back from 9S to 6S it worked as usual…anyone else have this issue?
```

---
## \#15 Posted by: Busk8 Posted at: 2018-04-29T06:39:20.631Z Reads: 109

```
yeah im having a similar issue my vesc only works on  3S set up and nothing more
```

---
## \#16 Posted by: zepton Posted at: 2018-04-30T13:52:01.765Z Reads: 95

```
Send your configuration screenshots. Do you also get a DRV fault? I’d like to try and troubleshoot my issue but I am worried of getting the fault again and actually breaking my vesc...
```

---
## \#17 Posted by: TarzanHBK Posted at: 2018-05-14T18:41:49.606Z Reads: 83

```
Whats the fault code?
```

---
