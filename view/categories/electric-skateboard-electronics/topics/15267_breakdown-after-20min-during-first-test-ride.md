# Breakdown after 20min during first test ride

### Replies: 25 Views: 2074

## \#1 Posted by: Msk8 Posted at: 2016-12-28T01:30:46.818Z Reads: 183

```
Hello, 
I have been reading and learning a lot here over the past weeks as I ordered parts and got ready for this holiday project with my son. Great community, hope to give back soon. Right now unfortunately we are looking for help. 

So we just finished bench testing and took it out for the first test ride around the block. Wow were we so excited to feel that power under our feet. Really scary but so much fun. We took turns and rode it slowly around the block, no hills. 

After about 20min it suddenly stopped working with plenty of battery left. We can still connect to the VESC with the BLDC tool and read/write configurations. However the motor detection fails. There are no errors when running "faults" on the terminal. On the "Realtime Data" tab we cannot see the last line, so not sure if any errors are there.  The VESC has a red light blinking, double flash followed by a pause. We checked the wires and can't see any issues with the motor connection. Motor detection worked fine earlier today, we ran it several times to ensure we use the correct parameters. 

Any thoughts on what might have gone wrong and how to further investigate are much appreciated. At this point we don't know if it's the VESC or the motor or both. One other test we did was to run motor detection without the motor connected and it looks exactly the same. 

Here are our main components:
* VESC from 
* Motor SK3 6364 190kv 
* Battery 10S - 2x 5S 5000mAh Lipos

<img src="/uploads/db1493/original/3X/f/9/f92377e8eb61594e02cee4b9866f9e87506fecb6.PNG" width="459" height="266"><img src="/uploads/db1493/original/3X/9/2/92375feb58828b731fefacb5525e022dca3f911d.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/3/c/3c2f2ed09a34e77f9f2ff32f951bbfd9afba1165.jpg" width="375" height="500">
```

---
## \#2 Posted by: Shogu12 Posted at: 2016-12-28T02:04:04.448Z Reads: 168

```
Turn on active sampling and look for fault code. I'm saying you fried your DRV8302. You should see activity.[Uploading...]()
```

---
## \#3 Posted by: Msk8 Posted at: 2016-12-28T02:24:17.435Z Reads: 158

```
Thanks. I am having trouble to see the last line, I believe that's where the error code is displayed. I tried different display resolutions but the UI is cut off here. Is there any other way to get to that error code?

<img src="/uploads/db1493/original/3X/0/a/0a1ba2f13e3de0cebb875958b436741b6b3e029c.PNG" width="690" height="441">
```

---
## \#4 Posted by: Shogu12 Posted at: 2016-12-28T02:34:06.666Z Reads: 149

```
Go to terminal and type fault and hit enter as you pull the trigger or use the arrow keys.[Uploading...]()
```

---
## \#5 Posted by: Shogu12 Posted at: 2016-12-28T02:38:52.753Z Reads: 151

```
That being said I have had 2 diy vescs and have ordered 2 more. 1 I sent back because it wouldn't  detect a motor the other died while riding it last week. I've ordered 4 drv8302's and like 30 c26/c18 caps( to improve the vesc not having a c26 cap) and a hot air smd rework station with all tools necessary.
```

---
## \#6 Posted by: Msk8 Posted at: 2016-12-28T02:43:23.464Z Reads: 150

```

FAULT_CODE_UNDER_VOLTAGE

hmm... each of my packs is at 20.3V right now, so total 40.6V. My battery cutoff is set to 30V.
```

---
## \#7 Posted by: Msk8 Posted at: 2016-12-28T02:47:23.140Z Reads: 141

```
thanks, yes I read your posts. Cool to hear that you are about to build 50 boards for your Airforce team. Good luck with that project!
```

---
## \#8 Posted by: Shogu12 Posted at: 2016-12-28T02:47:52.458Z Reads: 142

```
What are your motor/batterie/breaking parameters (amps)?
```

---
## \#9 Posted by: Msk8 Posted at: 2016-12-28T03:01:50.347Z Reads: 142

```
Here are two screenshots with my settings:

<img src="/uploads/db1493/original/3X/a/2/a244c30c1932d58cfccf0cf5962fb70aacd5bb56.PNG" width="690" height="441"><img src="/uploads/db1493/original/3X/8/f/8f582abf8af0e7179769a8d4f4103aae51bb0eab.PNG" width="690" height="441">
```

---
## \#10 Posted by: treenutter Posted at: 2016-12-28T05:04:09.033Z Reads: 118

```
Can you check the battery voltage using your charger or a mutilmeter? Maybe you are under-volting.

Make sure that the motor leads are connected to the VESC. Tape them so they don't come loose while you're riding.
```

---
## \#11 Posted by: boards Posted at: 2016-12-28T05:16:37.399Z Reads: 119

```
One of your solder joints probably cracked and isn't making a good connection, causing high resistance.
```

---
## \#12 Posted by: Msk8 Posted at: 2016-12-28T05:22:21.856Z Reads: 118

```
My voltage was at 40.6W (10S) when returning from the street. All my bench tests this afternoon were done with that charge. I am recharging now to see if it makes any difference...almost there.

I also re-soldered the 4mm plugs I put on the VESC for the SK3 motor to double check on that after I read a post about  exactly that. 

I noticed that the shrink wrap in the VESC is more crumbled on one of the mosfets, see blue circle. 

<img src="/uploads/db1493/original/3X/6/2/628a892958a8dd83e740742a430d96b1f7e21468.jpg" width="666" height="499">
```

---
## \#13 Posted by: Msk8 Posted at: 2016-12-28T05:30:36.438Z Reads: 112

```
ok thanks, I will check the solder joints again. Also just tried with full battery charge, same thing
```

---
## \#14 Posted by: Eboosted Posted at: 2016-12-28T06:27:46.515Z Reads: 104

```
After seeing all these VESC failures I'm really worried for the faith of mine. 

What version of firmware are you using? I'd suggest to flash the Ackmaniac firmware
```

---
## \#15 Posted by: Eboosted Posted at: 2016-12-28T06:35:03.516Z Reads: 104

```
If your VESC firmware had the current ramp bug and you didn't update the firmware your VESC would be toasted.
```

---
## \#16 Posted by: Msk8 Posted at: 2016-12-28T06:42:14.984Z Reads: 105

```
Re-soldered motor connection for the 2nd time. Am pretty sure it's solid. Not sure what I should try or buy/replace. Motor or vesc? Thanks for all your help.
```

---
## \#17 Posted by: Msk8 Posted at: 2016-12-28T06:46:27.942Z Reads: 101

```
Firmware 2.18. Which one has the bug?
```

---
## \#18 Posted by: Eboosted Posted at: 2016-12-28T06:46:49.438Z Reads: 103

```
Check this 

http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262
```

---
## \#19 Posted by: Ackmaniac Posted at: 2016-12-28T12:29:43.810Z Reads: 98

```
For Lipos your cutoff is too low. You should set the cutoff start to 36V (3.6V a cell) and the end to 34V (3.4V a cell).
Because when the battery reached already 33V without load then the Lipo is already empty and the voltage collapses.
But it is strange that you say that the voltage for each pack is still at 20.3V.
So it still could be another fault. But you should correct the voltage cutoffs, otherwise you damage the battery. For a Li-ion battery it would be another story.
```

---
## \#20 Posted by: Msk8 Posted at: 2016-12-28T16:30:00.277Z Reads: 87

```
thanks @Ackmaniac will do. I had the cut-off set higher during the ride, I just played with the parameters during troubleshooting, that UNDER_VOLTAGE error triggered that thought in me... no change.  
Will check today if I have that firmware issue @Eboosted mentioned.
```

---
## \#21 Posted by: Msk8 Posted at: 2016-12-28T18:46:20.060Z Reads: 79

```
@Eboosted I checked and my firmware seems not to have the current ramp bug. It remains at 0.04 after write and re-read.

Any other ideas what could cause my FAULT_CODE_UNDER_VOLTAGE error? I measured the input voltage at the VESC at 41.7V. When I turn the motor by hand, the RPM graph plots my hand turning speed and direction on the realtime data tab. So things seem somewhat connected.  

I just disconnected the motor again and I am getting the exact same FAULT_CODE_UNDER_VOLTAGE. Does every VESC give that error without a motor?
```

---
## \#22 Posted by: Ackmaniac Posted at: 2016-12-28T18:56:04.602Z Reads: 77

```
Did you adjust your ppm pulse width settings. Because maybe you brake when the remote is in idle. And when the motor looses its connection it might cause that error. 
And please try on another computer with a bigger monitor to figure out which voltage the vesc reads.
```

---
## \#23 Posted by: JohnnyMeduse Posted at: 2016-12-28T19:00:12.166Z Reads: 77

```
I might be a broken resistor... If i remember correctly maybe R4 or R3
```

---
## \#24 Posted by: Msk8 Posted at: 2016-12-30T07:18:05.170Z Reads: 64

```
Quick update to close the loop. I got the warranty from DIYelectricskateboard, I sent it back yesterday and Dexter will send me a replacement. Thanks @torqueboards. Fingers crossed that I have more luck with the next one. Thanks for all your support.
```

---
## \#25 Posted by: Eboosted Posted at: 2016-12-30T19:21:55.287Z Reads: 62

```
That's great to hear! Great customer support Dexter @torqueboards
```

---
