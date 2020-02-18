# Another First Build needing help &#124; Evo Falcon &#124; DIY 10S3P Li-Ion &#124; Single 6374

### Replies: 23 Views: 627

## \#1 Posted by: RHill051 Posted at: 2018-08-30T01:20:35.334Z Reads: 159

```
First off huge thanks to everyone here, the information is never ending. I've been meaning to start a post for awhile but I now need advice so here we go.

Here is my full build list:
![image|176x499](upload://7A2UQz3dHZVnj8NYb5APhK8NYuJ.png)

I have been hesitant to start as I might have been overly ambitious and decided for my first project I'd build my own battery as well. That meant buying or building a spot welder. I opted to build the spot welder. Of all the ways I saw to make one I landed on the built by [Darkkevind1978](https://www.youtube.com/user/darkkevind1978) with a slight modification. 
![image|375x500](upload://uFBSE3nzwa3lhHLq4rFynMyyuVC.jpg)![image|375x500](upload://w5OQuXEDhDyvAdEEVARbHDuqhEW.jpg)
It worked incredibly well and I got the entire battery welded up very quickly. I could apply even pressure to each point as they were independent of each other. Here is the battery so far. 
![image|666x500](upload://4IwVkrPalxrVCQsQQEliMXTvVc.jpg)
![image|666x500](upload://phvYkZTorkkRCowGtaUjFA0vhFn.jpg)
![image|666x500](upload://kSnzK3eT0C6IGp3AeSaoBzcDNtZ.jpg)
![image|666x500](upload://npfd8IZxcfpfZQV2esOMRvRILVb.jpg)
I was working on connecting my e-switch and I thought I was doing everything correctly. I have a DC-DC step down converter to reduce the voltage to 12V for my switch. I spent quite awhile looking for exactly how the switch connects to the BMS and came to the conclusion it was the 2 white wires on the BMS that complete the loop for the switch. Here is the diagram for the switch I was trying to use. ![image|565x303](upload://iJh8PGUBnPvs5nWbFA4zdArjmy1.jpg)
After connecting everything I pressed the button and the light came on as I expected it to but I also heard a fizzing sound followed by some smoke between the BMS boards.... I don't know what I did wrong, I'm hoping I didn't ruin the board :( If anyone can point out my mistake I'd be incredibly grateful. 

I'm waiting for my 10AWG wire to come in the mail so I can solder on the positive and negative leads for the battery. Hopefully I'll have the switch and BMS sorted out by then. Here are a couple more pictures of the battery that show the welds a little better.
![image|666x500](upload://AwV6LPy5cxEFZRT71Sdd0OKYXh.jpg)
![image|666x500](upload://50F83cCw8dWOKp6nAr0NwjqFldv.jpg)
![image|374x500](upload://btQQ7y5EU1IZZAwBtyTNsxhhz4C.jpg)
```

---
## \#2 Posted by: RHill051 Posted at: 2018-08-30T01:49:57.815Z Reads: 127

```
It just dawned on me that maybe the two white wires are not interchangeable and one needs to be positive and the other needs to be negative.. that's all I can think of..
```

---
## \#3 Posted by: mmaner Posted at: 2018-08-30T02:36:08.483Z Reads: 128

```
The 2 white wire simply complete a circuit when bridged by the switch. I doubt that's the issue as even a bad switch would just not trip the circuit and turn in the BMS. 

Only if you connected the wires incorrectly ncouke that be an issue when including the power for the LED. Do you have a pic if how the bottom of the switch isnwired?
```

---
## \#4 Posted by: mmaner Posted at: 2018-08-30T02:37:51.145Z Reads: 134

```
It should look like this...

![latching%20switch%20-%20how%20to%20wire%20v3%20022718|690x433](upload://zzcMWwwzNcfaQ1PC4ZLLhDp4wMH.jpg)

Instead of using the PPM header use your buck convertor.
```

---
## \#5 Posted by: RHill051 Posted at: 2018-08-30T02:44:33.104Z Reads: 127

```
Here is what I had.. It does look like I had it different from that.
![image|374x500](upload://s5Nm3h1pN2ZCTAZ9qstXgbS3m4s.jpg)
![image|374x500](upload://5WdkZYo3TwUilKaRzgq2s87M6F.jpg)
sorry for all the solder...
```

---
## \#6 Posted by: RHill051 Posted at: 2018-08-30T03:44:27.438Z Reads: 118

```
Well I'm pretty sure the BMS is toast... I put a load on the battery and the BMS dropped to 2.4V and didn't change regardless of the switch being open or closed :( ... anyone have a 10S Bestech Li-Ion BMS you want to sell? lol
```

---
## \#7 Posted by: RHill051 Posted at: 2018-08-30T03:56:57.634Z Reads: 116

```
Just ordered another BMS... are there any chances I could repair the damaged BMS? is there a fuse that can be replaced? I think I've read about a fuse being somewhere
```

---
## \#8 Posted by: mmaner Posted at: 2018-08-30T11:58:38.851Z Reads: 108

```
I doubt it's repairable, I've never seen a Bestech BMS that had a fuse.

I know it sucks, but we have all done it at some point.
```

---
## \#9 Posted by: Andy87 Posted at: 2018-08-30T14:01:19.676Z Reads: 95

```
Maybe that’s the reason why the moq for bestech bms on Alibaba.com is two devices 😅🙈
```

---
## \#10 Posted by: RHill051 Posted at: 2018-08-30T14:20:04.945Z Reads: 91

```
haha it all makes sense now!! I didn't realize the wires couldn't accept any power.. I had read somewhere that it could handle up to 12v switch but I don't know.. live and learn. Now I just want to figure out how to get the switch to light up only when the board is on.
```

---
## \#11 Posted by: mmaner Posted at: 2018-08-30T16:28:14.474Z Reads: 85

```
install the buck convertor after the BMS, connect the POS & NEG to the switch and the on/off circuit to the BMS.  Then when you hit the switch it will power the buck convertor and then the switch.
```

---
## \#12 Posted by: RHill051 Posted at: 2018-08-30T18:47:07.309Z Reads: 72

```
aww man.. why didn't I think of that.... So the positive of the buck converter would still be connected to the positive of the battery its just the negative that would go to the "P-" right?
```

---
## \#13 Posted by: mmaner Posted at: 2018-08-30T19:06:42.811Z Reads: 73

```
I would do it after the XT90 on the battery myself, that way its not completely tied in and is still removable.  

What I mean is battery > xt90 female > xt90 male > buck > xt90 female > xt90 male > VESC(s).  that way you can pull the buck convertor and reconnect without any reworking of the connectors.  I prefer to make things modular so that repairs are faster and easier.

Give me a few mins and Ill diagram it...
```

---
## \#14 Posted by: mmaner Posted at: 2018-08-30T19:22:07.331Z Reads: 71

```
Something like this (not to scale)...

![image|690x278](upload://tIkqvnP1wDqbXP07wyt88q0ZrDv.png)
```

---
## \#15 Posted by: RHill051 Posted at: 2018-08-30T20:07:09.597Z Reads: 66

```
Dude you are the bomb!! (what did you use to make the diagram?) 
Also, would xt60's be sufficient? I have both 90's and 60's but the Focbox has a 60 on it
```

---
## \#16 Posted by: mmaner Posted at: 2018-08-30T20:09:18.070Z Reads: 66

```
I used [Microsoft Visio](https://products.office.com/en-us/Visio/microsoft-visio-online-plan-compare-visio-options?&OCID=AID717927_SEM_X2BNwfPt&lnkd=Google_O365SMB_App).  XT60's are likely OK, but I prefer XT90's at the battery as they support higher amps.  An XT90 on the battery and VESC side should be fine, then XT60's after the buck convertor.
```

---
## \#17 Posted by: RHill051 Posted at: 2018-08-30T20:17:45.557Z Reads: 61

```
So what are your thoughts on this configuration? And how about wire gauge?
![image|690x278](upload://lV4ZNE1MpDr1XZzTrgCGtziJBsg.png)
```

---
## \#18 Posted by: mmaner Posted at: 2018-08-30T20:21:32.789Z Reads: 59

```
I would use 10g wire everywhere other than after the buck., your XT connector placement is fine.
```

---
## \#19 Posted by: RHill051 Posted at: 2018-09-04T19:11:42.311Z Reads: 52

```
Regarding the Battery I'm building, Do people think the nickle stick is sufficient? This is what I used: https://www.amazon.com/gp/product/B075FL7JNY/ref=oh_aui_search_detailpage?ie=UTF8&psc=1 I added two series connections using 16AWG wire to helpl reduce the draw on the nickel.
```

---
## \#20 Posted by: RHill051 Posted at: 2018-09-06T16:57:35.206Z Reads: 51

```
Ok, here is what I'm working on. How does it look to you guys?
![E-Scate%20Diagram%20(1)|690x296](upload://enJYp57YhJFOehskqug4WwsE4NI.jpg)
though they aren't pictured the balance wires are already done and won't be forgotten
```

---
## \#22 Posted by: Andy87 Posted at: 2018-09-06T17:36:23.124Z Reads: 43

```
You can switch on off your battery meter?
If no place it better on the xt90 which is behind the switch, close to the focbox.
In this postion where it’s now it’s always switched on
```

---
## \#23 Posted by: RHill051 Posted at: 2018-09-06T17:46:47.784Z Reads: 43

```
I didn't think to move the negative to match the buck converter. The documentation on the meter says it auto powers off after 10 seconds or some other predetermined time. I think I can change the auto time out so that its always on and then just use the power switch to turn it off or on. Thanks for the suggestion
```

---
## \#24 Posted by: RHill051 Posted at: 2018-09-09T01:57:28.964Z Reads: 33

```
I truly hope that I'm not the only person to ever make 2 stupid mistakes in a row... after verifying that I had all the wires connecting the random components correct I proceed to reconnect the new BMS to the battery... as I pressed the power button I heard a sizzle and there was smoke again.... This time however I made the hasty mistake of reconnecting the #10 ballance lead to the wrong cell on the pack after fixing some of the poor solder joints I had... basically instead of connecting it to the final positive lead of the battery I connected it to the first negative lead... I quickly realized what I did wrong and fixed it.  reconnected everything and it seems to work fine.. the power switch looks like it turns on and off the battery but I'm wondering if now the balancing portion of the pack is gone. Thoughts?
```

---
