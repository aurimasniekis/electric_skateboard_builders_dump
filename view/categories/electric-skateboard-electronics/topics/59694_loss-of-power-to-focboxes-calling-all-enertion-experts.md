# Loss of power to focboxes calling all enertion experts

### Replies: 28 Views: 557

## \#1 Posted by: dareno Posted at: 2018-06-22T03:28:29.231Z Reads: 187

```
Has anyone experienced a loss of output from a dual focbox set up?
I have bec power but no phase.  They were working fine and then just stopped no lights on or anything.  I can't access them either with the vesc tool.  They are 2 weeks old and have run a dual 6374 10s set up with bms for approx 20km  
Vesc settings are 60 amp motor max, 25 battery max, both are behaving exactly the same way so I'm hoping its something simple. :(
```

---
## \#2 Posted by: Jebe Posted at: 2018-06-22T03:57:08.264Z Reads: 171

```
canbus setup? Was one powered off while connected via canbus to a live unit?
```

---
## \#3 Posted by: dareno Posted at: 2018-06-22T04:00:06.213Z Reads: 167

```
Yeah it was.  How you doing?
```

---
## \#4 Posted by: Eboosted Posted at: 2018-06-22T05:38:58.590Z Reads: 153

```
When you power them the lights turn on blue?
```

---
## \#5 Posted by: dareno Posted at: 2018-06-22T05:52:18.012Z Reads: 141

```
no nothing
```

---
## \#6 Posted by: Eboosted Posted at: 2018-06-22T06:07:53.580Z Reads: 139

```
Is there voltage on the xt60s before the ESC?
```

---
## \#7 Posted by: dareno Posted at: 2018-06-22T06:13:41.538Z Reads: 129

```
yeah voltage and the receiver powers up but no output or anything from the units
```

---
## \#8 Posted by: Eboosted Posted at: 2018-06-22T06:59:53.538Z Reads: 128

```
Did you try to make motor detection?
```

---
## \#9 Posted by: dareno Posted at: 2018-06-22T07:43:51.899Z Reads: 117

```
Theres no connection at all.  stripped both down and they are perfect.  nothing fried.
```

---
## \#10 Posted by: mikenyc Posted at: 2018-06-22T08:56:19.801Z Reads: 104

```
This just happened to me a couple of days ago
```

---
## \#11 Posted by: Kug3lis Posted at: 2018-06-22T09:05:36.406Z Reads: 104

```
If you powered single unit while another one was off and it's connected via CANBus I can guarantee that CANBus chip is fried and now it is shortening 3.3V/5V line don't remember which one. Happened to me before
```

---
## \#12 Posted by: lrdesigns Posted at: 2018-06-22T09:15:55.404Z Reads: 99

```
This :arrow_up: I hope you didn't do this. Its not obvious, so many have done it. Almost needs a warning label on the product.
```

---
## \#13 Posted by: Kug3lis Posted at: 2018-06-22T09:17:22.774Z Reads: 98

```
Yeah... By removing CAN chip it starts to work, but replacing CAN chip with new one CAN didn't worked anymore  anyway later on the whole FocBox fried so I didn't looked why CAN wasn't working :)
```

---
## \#14 Posted by: Silverline Posted at: 2018-06-22T09:39:14.410Z Reads: 94

```
So glad i'm not using CAN bus
```

---
## \#15 Posted by: dareno Posted at: 2018-06-22T19:51:16.551Z Reads: 74

```
Ive got them apart and there is no sign of fried chips.  Would a bad can chip be obvious?
```

---
## \#16 Posted by: dareno Posted at: 2018-06-22T19:59:12.862Z Reads: 73

```
I only did this as part of the test process after they stopped.  I did then connect each up individually to check my connectors and didn't think to disconnect the can bus but the problem was there already and I'm hoping I haven't made it worse
```

---
## \#17 Posted by: Jansen Posted at: 2019-04-19T04:36:46.679Z Reads: 59

```
Did you ever figure this out @dareno cause I just had the same thing just happen to me today.... just finished a build, did motor detection and all of that and was on my first test ride and in the middle of it all of a sudden after a mile or so I just lost half of my power so just cruised back home (which wasn't far at all) and one motor wasn't working anymore... opened it up and only one focbox is on blinking and the other with the motor not working isn't... I'm not using canbus and running split ppm so can't be that issue. Took apart focbox and don't see any obvious burn marks or blown anything on either side. Tried switching connectors to make sure it wasn't that or something dumb and everything still works with other stuff, it's just one focbox won't power on so I can't even pull it up to connect on the VESC tool to check. What is wrong with it or is there anything I can do?
```

---
## \#18 Posted by: dareno Posted at: 2019-04-19T04:42:06.210Z Reads: 60

```
Hey mate, mine was the dreaded can bus death but it killed both.  Yours sounds like a different issue with the same result.  I've since had drv errors faults on other vesc and you get blinking red lights.  I'm sure the focbox would give some indication if it was the drv chip.  Total blackout is what happens when the can bus fries.  Is it in warranty?
```

---
## \#19 Posted by: Jansen Posted at: 2019-04-19T04:45:50.677Z Reads: 62

```
fuck me. No warranty is done. No lights and not seeing anything. Dammit. Whyyyyyyy. Can you see a DRV issue to the naked eye cause I didn't see any black or anything that looked fried but I am not electronics engineer or expert either? Can you fix that and any way I could check or test for this without power or anything to look for that I can try?
```

---
## \#20 Posted by: Jansen Posted at: 2019-04-19T04:46:00.967Z Reads: 62

```
Thanks BTW @dareno
```

---
## \#21 Posted by: dareno Posted at: 2019-04-19T04:55:08.142Z Reads: 58

```
Its displaying the characteristics of can bus failure.  No power or anything.  I fixed both my can bus focboxes by removing the chips.  They are right here
![image|640x480](upload://gPJGPFdjVtY9sjrWvb9hQwQWUls.jpg) 

As the thing is bricked already and you use split ppm you could try snipping it off as it won't affect it even if it turns out to be something else.
Heres the full thread
https://www.electric-skateboard.builders/t/have-i-focked-my-focboxs/30428/20

@Jansen  just run through the obvious power checks first like connecting it to the cabling you know works.  I presumed you did that already but please do that first if you haven't.
```

---
## \#22 Posted by: Jansen Posted at: 2019-04-19T15:15:38.245Z Reads: 48

```
Dang, No luck bro... I tried all of the power and connector checks and Im still getting power to the focbox and out the phase wires but still can't figure it out. Went ahead and tried cutting off the canbus chip but that didn't help at all either. I noticed only one thing and that is that one little diode I believe. Let me get a pic and Ill send it over to see if you think that could be my issue maybe....
```

---
## \#23 Posted by: Jansen Posted at: 2019-04-19T15:42:02.403Z Reads: 47

```
C12 on the bottom left corner of the last pic is the only i noticed and can’t tell the difference from my other FOCBOX still working and this one that will not show that any signs of getting power to it even though I’ve tested to find out that power is going through it still.... wtf! Been trying to figure this shit out all dam night and. Is the sun is coming up..... fml. Just want a board for my vacation I leave for today in a few hours and all 3 of my builds are out of commission, 2 with only one FOCBOX working and 1 I’m waiting for a unity to finally ship. Ahhhhhhhh. So lame. Everything else is fine and ready on all 3 builds too. Dammit! What shitty luck to blow to focboxes on 2 different builds in the same week after 6-12 months of use on each build and no changes to warrant this happening. Lmk if you have any thoughts or input after looking at the pics and if you think that missing diode could be causing my issue. Thanks again brotha. 

![image|375x500](upload://23mYwt3Go7ZtiVQ3Gz8w1PAZnxo.jpeg) ![image|375x500](upload://bjPgwjr0sVMcS1BwmTxJaX6uoZO.jpeg) ![image|375x500](upload://86Lydoj15Y0Ew1zJjSdycWZT4We.jpeg) ![image|375x500](upload://go5lsc352UybCEYQkJnrRb6RMnQ.jpeg)
```

---
## \#24 Posted by: dareno Posted at: 2019-04-19T19:41:31.666Z Reads: 34

```
That sucks mate really.  Above my paygrade from here on in I'm afraid.  Sorry I couldn't be more help.
Where are you based because they can be repaired
```

---
## \#25 Posted by: Jansen Posted at: 2019-04-20T03:56:42.713Z Reads: 26

```
Darn thanks for the help thus far though bro. I've already learned some things with your guidance so appreciate it. And yeah I was going to hit up @JohnnyMeduse  who is one person I always see people talk about fixing them right? Im in the OC (SoCal USA). Do you know where I could look to try and find someone local in Cali to repair it by chance? Thanks again
```

---
## \#26 Posted by: Sn4pz Posted at: 2019-04-20T04:33:07.519Z Reads: 26

```
@ThermalM16 (I hope this is right) is your guy for USA vesc repairs, if the Canadian post takes too long
```

---
## \#27 Posted by: ThermalChild Posted at: 2019-04-20T04:38:42.328Z Reads: 26

```
A for effort, My buddy @ThermalM16 is the droid you're looking for.
```

---
## \#28 Posted by: Sn4pz Posted at: 2019-04-20T04:49:21.494Z Reads: 23

```
Greatest heck. So close.
```

---
