# Is the xt60 on this VESC the wrong way around?

### Replies: 20 Views: 1283

## \#1 Posted by: michaelcpg Posted at: 2016-04-19T06:13:20.022Z Reads: 130

```
Can someone please confirm this for me but I'm fairly sure the XT60 on my VESC is the wrong way around?

<img src="/uploads/db1493/original/2X/2/254e7cb1e5cf67b5625457e9f505472f5cd05ffd.jpg" width="282" height="500">

<img src="/uploads/db1493/original/2X/1/116f17a1eb2ee0ec649a8b3237f56674760b20f8.jpg" width="689" height="390">

I bought this VESC and I've been having trouble getting it to power my motor, when connected to the BLDC tool I don't get any LED's lighting up and attempting to connect to the BLDC tool would just tell me that there was a "firmware read response error". Initially I thought it was an issue with the firmware so bought an st-link programmer and reuploaded the firmware following Vedder's instructions which seemed to all go as planned, LED's lit up etc. But afterwards, I plugged it back into my motor/battery/usb cable and tried to connect it to the bldc tool again and I got the same result. No lights, nothing.

Could this be why?...
```

---
## \#2 Posted by: claudiofiore88 Posted at: 2016-04-19T06:31:02.781Z Reads: 127

```
Yep, it's backwards. Where did you get this from?
```

---
## \#3 Posted by: michaelcpg Posted at: 2016-04-19T06:34:17.512Z Reads: 127

```
Not sure if I should say at this stage? The guy has been very helpful with everything so far so I don't want to give him bad rep for what was likely a silly mistake. 

Last time I plugged it into my space cell it also made a decent sized spark very briefly, what're the chances of the VESc being ruined? I haven't tested the VESC since but the battery seems to be ok, the fuse didn't blow and it still reads the same voltage as before.
```

---
## \#4 Posted by: claudiofiore88 Posted at: 2016-04-19T06:41:01.182Z Reads: 127

```
If the vesc doesn't have reverse polarity protection, then it's possible that it may have been damaged. The seller definitely should fix or replace it.
```

---
## \#5 Posted by: michaelcpg Posted at: 2016-04-19T06:42:01.273Z Reads: 125

```
Is it worth plugging it back in once I've swapped the polarity to test it?
```

---
## \#6 Posted by: claudiofiore88 Posted at: 2016-04-19T06:45:09.536Z Reads: 123

```
I don't see why not. If it's already damaged, then I don't see you making things worse, but I'm no expert.
```

---
## \#7 Posted by: chaka Posted at: 2016-04-19T13:09:00.699Z Reads: 109

```
Anyone need a job? It pays $10 an hour and I have a position opening today! 

 Really sorry for the inconvenience Let me know the prognosis on that VESC and I can send a replacement if needed.
```

---
## \#8 Posted by: karma Posted at: 2016-04-19T14:20:11.686Z Reads: 105

```
What's the job  @chaka ? :)
```

---
## \#9 Posted by: lowGuido Posted at: 2016-04-19T15:13:59.647Z Reads: 104

```
soldering connectors on the right way apparently.
```

---
## \#10 Posted by: chaka Posted at: 2016-04-19T15:17:37.994Z Reads: 102

```
I was only joking a little, I try to run a tight ship but I would never send someone walking over a little mistake. 

I do have plans on expanding and possibly moving into a larger building. I'm not sure how many people would want to move to a little town in the middle of the desert but I will be looking for people who just want to ride and build sweet decks.
```

---
## \#11 Posted by: karma Posted at: 2016-04-19T15:39:28.929Z Reads: 98

```
Lol, you got me... Why do some people perfer XT60 connectors over HXT?
```

---
## \#12 Posted by: lowGuido Posted at: 2016-04-19T15:42:14.044Z Reads: 98

```
[quote="karma, post:11, topic:2447"]
Why do some people perfer XT60 connectors over HXT?
[/quote]

size?

----------------
```

---
## \#13 Posted by: longhairedboy Posted at: 2016-04-19T17:55:08.463Z Reads: 90

```
yeah totally just take an xacto and an iron to that and flip it around. 

I have a drawer full of XT60s that i've taken off of things because i don't use them. I'm starting to see that i'm pretty much the only person alive not using them.  I just got another set of 6S Favs from DIY and even they have them now, but thank god they upped the phase leads to 5.5mm bullets from 4mm bullets.
```

---
## \#14 Posted by: Bender Posted at: 2016-04-20T12:43:50.283Z Reads: 80

```
Did the spell checker change ESCs to Favs? Or is that some part I've never heard of yet
```

---
## \#15 Posted by: longhairedboy Posted at: 2016-04-20T12:52:11.241Z Reads: 80

```
Favourite is a company that makes ESCs. I have been using their 6S 120amp models from DIY for over a year now and i like them for the most part when i'm not frying them. They have a catchy beep code and they perform really well.
```

---
## \#16 Posted by: chaka Posted at: 2016-04-20T12:57:25.058Z Reads: 71

```
I have some sweet 6s BMS modules stashed away somewhere ;)
```

---
## \#17 Posted by: longhairedboy Posted at: 2016-04-20T13:55:45.728Z Reads: 65

```
That would make a lovely addition to my rat board. I'd have to refactor the box but that's how i stay in practice! PM me what you want for it and the specs. 

I'm about to order a couple of 12S BMSs as well. Got any of those laying around?
```

---
## \#18 Posted by: chaka Posted at: 2016-04-20T14:51:19.805Z Reads: 63

```
The only trouble is you might trigger the over-current protection unless you used a 44 tooth wheel pulley on the 6s module. It would work well on something geared to go 20-25mph. If you paired it with a vesc you could gear it to go faster. 

All my 12s modules are spoken for but I plan on stocking them in my shop very soon.

I'll check my inventory on the 6s BMS, I need to make sure I leave one for myself, have a little pocket cruiser in the works for my 3 year old.

<img src="/uploads/db1493/original/2X/7/78d9831d6f6d7d366297a184534085853c8cf441.jpg" width="689" height="499">
```

---
## \#19 Posted by: treenutter Posted at: 2016-04-20T22:16:47.189Z Reads: 51

```
You're not the only one @longhairedboy! I don't use xt60s. I use Dean's connectors! I'm so retro!
```

---
## \#20 Posted by: NNGG Posted at: 2016-04-20T22:30:13.414Z Reads: 51

```
Someone who uses deans for once! I thougfht I was the only one.
```

---
