# Why does my slave VESC keep blowing?

### Replies: 25 Views: 2482

## \#1 Posted by: meercat Posted at: 2016-12-19T21:49:02.785Z Reads: 216

```
I'm on my second blown (DRV error) slave VESC and have no idea what is going on. Bought two motors and VESCs from DIY. Ran BLDC detection on each, etc. Followed [this set of instructions](http://www.electric-skateboard.builders/t/vesc-faq-connect-two-vesc-via-canbus-for-dual-motors/142/50) on configuring CAN bus. Everything seemed fine. The board ran great, for a half mile until I started going uphill it started stuttering and I noticed that only one wheel was getting power.

Turns out the slave VESC had a DRV error. I couldn't find any obvious visible issues with the VESC and I wasn't exactly sure why it blew, but I thought I probably hadn't insulated the leads well enough. Ordered another one (this time with the warranty) which took a few weeks to receive. In the meantime, I removed the second motor and put at least 100 miles on the board with a single motor/VESC. Zero problems. Up/down hills, all over the place.

Received the new VESC. Carefully ran through motor detection and everything. Over-insulated every lead and used CAN bus to connect the VESCs. This time, I got about 2 miles on it before I ran into the same problem, again which I noticed again while going uphill. Sure enough, same DRV error.

I'm not even sure where to start looking or what could be causing this. Any ideas?
```

---
## \#2 Posted by: flatsp0t Posted at: 2016-12-19T21:58:25.340Z Reads: 205

```
Can you please post screenshots of your BLDC-Tool config of both VESCs, so we can have a look if there is some gremlin in the settings?
```

---
## \#3 Posted by: susplus Posted at: 2016-12-19T22:03:21.857Z Reads: 198

```
maybe a simple Y cable should be better than CAN
```

---
## \#4 Posted by: Lukas Posted at: 2016-12-19T22:15:59.551Z Reads: 193

```
Maybe your second motor is broken.
So that it produces a short
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2016-12-19T22:21:52.546Z Reads: 188

```
Drop the max erpm on each vesc to 60k
```

---
## \#6 Posted by: meercat Posted at: 2016-12-19T22:42:06.854Z Reads: 190

```
Here are the screenshots of the BLDC-tool for both VESCs.

https://s3.amazonaws.com/meercat/master_motorcfg_a.png
https://s3.amazonaws.com/meercat/master_bldc_a.png
https://s3.amazonaws.com/meercat/master_app_gen_a.png
https://s3.amazonaws.com/meercat/master_app_ppm_a.png
https://s3.amazonaws.com/meercat/slave_motorcfg_a.png
https://s3.amazonaws.com/meercat/slave_bldc_a.png
https://s3.amazonaws.com/meercat/slave_app_gen_a.png
https://s3.amazonaws.com/meercat/slave_app_ppm_a.png
```

---
## \#7 Posted by: rpn314 Posted at: 2016-12-19T23:50:08.299Z Reads: 176

```
[quote="JohnnyMeduse, post:5, topic:14943, full:true"]
Drop the max erpm on each vesc to 60k
[/quote]

Yep, exactly what @JohnnyMeduse said. @meercat you're currently set at 100k (first and fourth screenshots). Drop to 60k. (that the min ERPM to -60000 and the max to ERPM to 60000)
```

---
## \#8 Posted by: guyguy Posted at: 2016-12-20T00:52:04.047Z Reads: 175

```
https://www.youtube.com/watch?v=5HLZaMcYRuY&t=1753s

Batt max needs to be halved for dual vescs

Outside of your settings it sounds like a short in your 2nd motor.
```

---
## \#9 Posted by: meercat Posted at: 2016-12-20T02:00:09.526Z Reads: 172

```
Thanks to you and @JohnnyMeduse. Would that make sense that it would blow the DRV? Or should I still suspect that 2nd motor?
```

---
## \#10 Posted by: rpn314 Posted at: 2016-12-20T02:31:55.958Z Reads: 168

```
That could definitely do it. Also, one more big one to check. It's called Max Current Ramp Step in the motor configuration advanced tab. Double check it on both the master and slave. There's a bug in some iterations of the firmware that multiply it by 10 each time you write the configuration. That's what killed the DRV on both my VESCs
```

---
## \#11 Posted by: Eboosted Posted at: 2016-12-20T05:54:14.829Z Reads: 154

```
You should try the @Akmaniac BLDC tool, seems to be more stable and less prone to this kind of errors
```

---
## \#12 Posted by: meercat Posted at: 2016-12-20T06:03:40.177Z Reads: 154

```
Son of a....I can't believe these VESCs are so touchy...and I work with this kind of stuff for a living..

Thanks for all the help and advice. I'll let you know how things pan out.
```

---
## \#13 Posted by: rpn314 Posted at: 2016-12-20T06:09:37.057Z Reads: 152

```
If I'm not mistaken, the ramp step current bug was in the VESC firmware itself, not in the bldc tool. It's long been resolved (8 months maybe?), but I'm sure there's a bad copy of the firmware floating around somewhere and if you download the wrong one then you've got it.

@meercat oh yeah, they're touchy until you've got them set up just right, and then they're a dream :grinning:
```

---
## \#14 Posted by: Eboosted Posted at: 2016-12-20T06:13:34.813Z Reads: 149

```
So, what would you suggest to avoid this issue?, would you suggest this procedure? 

Write Max Current Ramp Step with a 12V power supply, reboot VESC, read motor configuration advanced tab, see if the value was correctly written?
```

---
## \#15 Posted by: rpn314 Posted at: 2016-12-20T06:20:59.644Z Reads: 149

```
You don't even have to reboot it. Just read and write a few times. Start it at .04. If the parameter changes, get a different copy of the firmware (and if you've ridden with a high value, then you'll probably need a new DRV chip). If it doesn't change then you're good.

[quote="Jinra, post:1, topic:6262"]
I've downloaded BLDC tool for Mac fairly recently and the "Max Current Ramp Step" bug still seems to be present. For those unaware, when you read and write config on the motor configuration tab, the Max current ramp step field under "advanced" will multiply by 10. This can possibly be fatal to your VESC so remember to reset it whenever you write to motor configuration.

The default value is 0.04, however, if you set it to that and write it will change to 0.4 since it multiplies by 10, so set it to 0.004 and write config.

I've heard the issue was fixed, but i'm unsure as to where or what versions it's fixed for. This information is accurate as of 5/30 (when I downloaded BLDC tool) off Jacob's site (vesc.net.au) for OSX firmware v2.18. I can't confirm if this is happening on Linux/Windows.

EDIT: This issue is fixed on latest f/w revisions by @jacobbloy and @elkick. Not sure who else has updated f/w's uploaded, but these two have confirmed bug-free versions. The version will still be 2.18 so you won't know if you have a bug free version until you test it out. Information accurate as of 8/28/16
[/quote]
```

---
## \#16 Posted by: Jebe Posted at: 2016-12-20T07:41:35.882Z Reads: 132

```
The which one now? There's an alternative??
```

---
## \#17 Posted by: rpn314 Posted at: 2016-12-20T07:53:06.071Z Reads: 137

```
Yes. It's an alternative to the BLDC Tool that most people use.

Though I will re-iterate my point in my previous post: the max current ramp step bug is the only bug I've ever seen related to writing the VESC config, and it was NOT an issue with vedder's BLDC Tool, it was an issue with the firmware on the VESC itself, so it wouldn't have mattered what tool you were using if you have the bad firmware (though a new, modified firmware is required to use @Ackmaniac's version, since it adds some great features). I have never seen any issues with BLDC Tool before (so I'm not sure about the claim of better stability). Granted I'm usually on Mac, which is much closer to Linux (which BLDC Tool was written on and so may be more stable than on Windows)
```

---
## \#18 Posted by: chaka Posted at: 2016-12-20T14:49:48.706Z Reads: 127

```
They are not touchy. I have never had a single failure due to the current ramp step bug we had in the past. If manufactured with care the vesc is very robust and reliable. Guess what happens when you outsource manufacturing to the cheapest bidder. :dizzy_face:
```

---
## \#19 Posted by: flatsp0t Posted at: 2016-12-20T15:32:54.236Z Reads: 124

```
Yes, but they still are prone to user error.
```

---
## \#20 Posted by: chaka Posted at: 2016-12-20T16:14:16.170Z Reads: 121

```
Agreed, but everything is susceptible to that. If you choose your vendor wisely you can still have it repaired for little to no cost regardless of the cause.
```

---
## \#21 Posted by: rpn314 Posted at: 2016-12-20T18:39:45.847Z Reads: 108

```
Oh definitely. I would argue that if not watched for, the Max Current Ramp Step can blow the DRV, even with a quality piece (I soldered my VESC myself with parts straight from Mouser, so I think that's pretty good quality....where do you source your parts from?). I didn't know I had it, and ended up with a value of 40 or 50. After running with it like that (going up some pretty solid hills) I got a DRV error. It is possible that there was another cause, but I couldn't find one.
```

---
## \#22 Posted by: chaka Posted at: 2016-12-20T19:19:52.533Z Reads: 108

```
I tried my best to blow a chip with bad current ramp step and could not do it. Even so, I think vendors need to handle replacement is someone did actually blow a chip due to the bug. Not the customers fault. 

There are a lot of variables to manufacturing the VESC and all of them contribute to the overall quality. This huge difference in quality from manufacture to manufacture is probably why Vedder is hesitant to release v6 to the public before he can set a precedence in reliability and quality of the design. 

I really do not like to step in and clear the air but the VESC does not deserve the reputation of being touchy or failure prone.
```

---
## \#23 Posted by: rpn314 Posted at: 2016-12-20T20:46:23.243Z Reads: 100

```
I'm sure it was my fault at some point (since I was my own vendor...) I'm happy to stand corrected :)
```

---
## \#24 Posted by: chaka Posted at: 2016-12-20T20:48:08.272Z Reads: 101

```
Haha yeah, I was not referring to you.
```

---
## \#25 Posted by: Psmrman90 Posted at: 2018-12-02T20:46:04.022Z Reads: 25

```
Is there a thread that explains the whole slave/master vesc thing?
```

---
