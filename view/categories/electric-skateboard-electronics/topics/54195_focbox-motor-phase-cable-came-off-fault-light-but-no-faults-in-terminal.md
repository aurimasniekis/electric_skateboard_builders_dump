# FOCBOX motor phase cable came off - fault light but no faults in terminal

### Replies: 28 Views: 897

## \#1 Posted by: moadymoad Posted at: 2018-05-03T03:17:49.316Z Reads: 124

```
Has anyone had this issue on FOCBOX? Brand new FOCBOX and I believe it has shorted as it smells like burnt electronics smell.

It looks like DRV has blown but there are no faults reporting when I hook it up to the BLDC tool. THe green fault light is on the focbox though.

I've logged a support ticket and am waiting to hear what to do next.

I am having a terrible run on my first build. Two dud TB vescs and now this.... I haven't been more than 5km
```

---
## \#2 Posted by: E1Allen Posted at: 2018-05-03T03:29:22.624Z Reads: 119

```
Pictures of the FocBox. Closeup
```

---
## \#3 Posted by: moadymoad Posted at: 2018-05-03T03:30:12.892Z Reads: 119

```
as in with the cover removed? what specifically the DRV chip?
```

---
## \#4 Posted by: E1Allen Posted at: 2018-05-03T03:44:43.168Z Reads: 116

```
Yes. Both sides
```

---
## \#5 Posted by: Scoo_B_SK8 Posted at: 2018-05-03T03:44:51.650Z Reads: 112

```
open focbox up and get as good of pic as you can of both sides of pcb.  DRV is a microchip

upper left
https://www.electric-skateboard.builders/uploads/db1493/original/3X/9/6/9655f26ee66bf20293077b963a9996352c476d54.jpeg

could also be fets (6 on left lower)
```

---
## \#6 Posted by: moadymoad Posted at: 2018-05-03T04:20:31.618Z Reads: 111

```
Looks like its both, the fet in the middle which is the one that came off had some discolouration. The drv chip also looks like its busted.

this sucks, another long wait!!

![IMG_4556|375x500](upload://xrv8raJdJdMwbwxAjHka23TLBTm.jpg)![IMG_4553|375x500](upload://wivqJjjb1d1tyIOT2bEsi7FFOAy.jpg)![IMG_4554|375x500](upload://8pb3LiWfKbtdbtdfgfmKO0J16k.jpg)![IMG_4552|375x500](upload://d5GsMcj1Lquq2bPi27gs8thkNwL.jpg)
```

---
## \#7 Posted by: E1Allen Posted at: 2018-05-03T04:24:25.560Z Reads: 104

```
@JohnnyMeduse looks like you have another customer.
```

---
## \#8 Posted by: moadymoad Posted at: 2018-05-03T04:26:56.035Z Reads: 106

```
its brand new... It's a faulty product the manufacturer will have to replace under Australian consumer law.

The consumer law here is very favourable for the consumer, I paid for platinum warranty for this even though I didn't really need to so I will be covered either way!
```

---
## \#9 Posted by: E1Allen Posted at: 2018-05-03T04:29:20.248Z Reads: 106

```
Good to hear
```

---
## \#10 Posted by: moadymoad Posted at: 2018-05-03T04:30:36.207Z Reads: 104

```
still frustrating, thats 3/4 vescs i have had issues with.

its been a 5 month build because of this crap haha, sounds like thats not uncommon.

Anyway thanks for verifying, hopefully enertion just send me one out while I send this back
```

---
## \#11 Posted by: Scoo_B_SK8 Posted at: 2018-05-03T04:33:40.762Z Reads: 94

```
you should still take screen shots of your settings and post em here... 3 out of 4 would be absolute terrible luck, gotta be something in your settings.

good pull on the platinum warranty
```

---
## \#12 Posted by: moadymoad Posted at: 2018-05-03T04:37:26.923Z Reads: 89

```
I triple checked. the cable literally came off the board on the focbox this time so it wasn't config.

The other 2 were tb vescs, one overheated and the other was running fine until I increased battery max then it blew drv. I've just got to send them back for a refund.

I've had the settings confirmed already on the TB vescs, I will post my settings before applying once I get this one replaced and everything wired up again.
```

---
## \#13 Posted by: Scoo_B_SK8 Posted at: 2018-05-03T04:38:50.268Z Reads: 87

```
i'm guessing the reason the wire came off in the first place was do to overheating.  and we should find out what that reason is...

but ya when ever you get the chance to post them (without changing em as they are now)
```

---
## \#14 Posted by: moadymoad Posted at: 2018-05-03T04:44:00.435Z Reads: 84

```
I have the read out from hm-10 module let me check temp
```

---
## \#15 Posted by: moadymoad Posted at: 2018-05-03T04:47:16.788Z Reads: 82

```
Max temp 62 celcius
```

---
## \#16 Posted by: E1Allen Posted at: 2018-05-03T04:49:48.548Z Reads: 81

```
That's not very hot
```

---
## \#17 Posted by: moadymoad Posted at: 2018-05-03T04:50:15.460Z Reads: 84

```
settings:

190kv
10s3p (30q)
dual 6374

BLDC (ran detection unloaded)
motor max 70
motor min -40
bat max 25
bat min -8

temp and voltage cutoff default
PPM and UART 
slave was set to send status over can and both were set to multiple esc over canbus
-60k/60k erpm

I've read and reread the settings after the TB vescs blew just to make sure it wasn't my fault. The bat max and min are slightly more than what the cells are rated continous but from what i've read about the 30q cells the settings are acceptable
```

---
## \#18 Posted by: JohnnyMeduse Posted at: 2018-05-03T05:14:53.540Z Reads: 80

```
[quote="Scoo_B_SK8, post:13, topic:54195"]
i’m guessing the reason the wire came off in the first place was do to overheating.  and we should find out what that reason is…
[/quote]

That kind of true... but not in a way that everyone think... Have you ever wonder why you can’t really give warranties when people are changing their connector? Because if you heat up too much the the connector you are trying to solder, the heat will transer of the existing solder on the other end of the cable, and if your not careful enough it migh creates a cold solder joint... So the question here is : Did you change your bullet connector?
```

---
## \#19 Posted by: moadymoad Posted at: 2018-05-03T05:22:07.702Z Reads: 80

```
Nope... I made adapters because I didn't want to void the warranty!
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2018-05-03T05:23:10.629Z Reads: 81

```
Then contact Enertion support... (on their website)
```

---
## \#21 Posted by: moadymoad Posted at: 2018-05-03T05:33:55.551Z Reads: 80

```
yeah have done am waiting now, main point was to confirm drv issue and vent I guess. If my biggest problem in the world is that my electric skateboard isn't working I guess life is pretty good

Appreciate the responses
```

---
## \#22 Posted by: moadymoad Posted at: 2018-05-03T08:24:50.611Z Reads: 66

```
Apologies to the guys that posted here to try and help me today. I feel like a bit of a dick. Was just disappointed...

Good things come to those who wait huh!
```

---
## \#23 Posted by: briman05 Posted at: 2018-05-03T09:22:31.200Z Reads: 59

```
I would after reading this it you will get a new one especially since you got the platinum warranty. Could you take a picture of the other side where the cables are soldered to the board. How long ago did you order these focboxes? There has been a number of people who received there new focboxes with a clear film still on the thermal pad from when it was first applied.
```

---
## \#24 Posted by: moadymoad Posted at: 2018-05-03T09:34:29.391Z Reads: 55

```
Ordered 3-4 weeks ago, there was no clear film on the joints.

There was a white pad over the fets. Just waiting on support I’m sure it will be fine.

Edit: sorry I see what you mean. I left it at work will take a look tomorrow.
```

---
## \#25 Posted by: moadymoad Posted at: 2018-05-05T08:22:55.719Z Reads: 42

```
FYI enertion have shipped me out a replacement already.

Happy I got the platinum warranty just to get back on the road as quick as possible.
```

---
## \#26 Posted by: RedEagle Posted at: 2018-05-05T14:19:58.717Z Reads: 37

```
What value did you increase it to? What was your battery max before?
```

---
## \#27 Posted by: moadymoad Posted at: 2018-05-05T14:45:43.002Z Reads: 32

```
On the Tb vesc?

From 15a/vesc to 25a/vesc
```

---
## \#28 Posted by: RedEagle Posted at: 2018-05-05T23:56:27.631Z Reads: 27

```
That's.... disappointing.
I run 30a on my maytech.
```

---
