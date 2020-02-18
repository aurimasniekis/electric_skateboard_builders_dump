# One final check before take off Need the OK

### Replies: 18 Views: 944

## \#1 Posted by: joeadams101 Posted at: 2017-10-01T08:36:36.959Z Reads: 164

```
Hey guys! Moving into FOC now(sensorless). I've followed vedders tutorial on how to setup FOC ( https://www.youtube.com/watch?v=bYYNbxPXNEU ) and I am just looking for a final OK from the community to take this on a test drive. After the detections and settings being applied the motor seems to be spinning fine and all.

Setup: 

dual 6355 190kvs 
dual focbox's
36/16 
10s3p

These are the VESC settings


<img src="/uploads/db1493/original/3X/e/8/e84ec8299b62be66667e1b1947b2c67c8850caed.png" width="690" height="349"><img src="/uploads/db1493/original/3X/6/2/6222889c8c784ce0a07308db7cc33e7f5a7a2b97.png" width="690" height="369">
```

---
## \#2 Posted by: scepterr Posted at: 2017-10-01T18:03:47.852Z Reads: 118

```
Why is your max erpm 100000?
```

---
## \#3 Posted by: florensvb Posted at: 2017-10-01T18:05:48.694Z Reads: 117

```
I think 100k is the default .. Correct me if I am wrong, but isn't his max erpm under 60k in any case with a 10s 190kv setup? :) 

Can't say anything about your foc values bro hahah!
```

---
## \#4 Posted by: joeadams101 Posted at: 2017-10-01T18:27:05.727Z Reads: 111

```
That is the default. Ive been running it like that since day one on BLDC
```

---
## \#5 Posted by: joeadams101 Posted at: 2017-10-01T18:27:32.656Z Reads: 106

```
I have no idea, which is why I am asking for last minute inputs to test it out
```

---
## \#6 Posted by: scepterr Posted at: 2017-10-01T18:27:46.037Z Reads: 104

```
Thats weird. That should be 60000, what vesc do you have?
```

---
## \#7 Posted by: florensvb Posted at: 2017-10-01T18:27:59.375Z Reads: 101

```
I think a best practice is to limit the erpm to 60k, as it can fry your vesc if you ever go beyond that
```

---
## \#8 Posted by: florensvb Posted at: 2017-10-01T18:28:31.364Z Reads: 96

```
My focbox is also set to 100k on default
```

---
## \#9 Posted by: scepterr Posted at: 2017-10-01T18:29:08.614Z Reads: 97

```
Yes he technically couldn't , unless going down a steep downhill, also if he ever decided to upgrade to 12s that would instantly be an issue
```

---
## \#10 Posted by: florensvb Posted at: 2017-10-01T18:30:33.084Z Reads: 95

```
Side question: If i limit to 60k and i am going down a steep hill, will my vesc actually brake to keep it below 60k??
```

---
## \#11 Posted by: joeadams101 Posted at: 2017-10-01T18:37:26.392Z Reads: 94

```
@scepterr I have 2 focbox's
```

---
## \#12 Posted by: scepterr Posted at: 2017-10-01T18:42:18.085Z Reads: 92

```
Yep that's what the limit should do
Just like low voltage cut
```

---
## \#13 Posted by: Blasto Posted at: 2017-10-01T18:43:42.209Z Reads: 93

```
Foc does not take into account the max erpm anyways
```

---
## \#14 Posted by: BigBoyToys Posted at: 2017-10-04T06:04:29.903Z Reads: 62

```
Glad to see you're taking the plunge with FOC. The only problem with your settings I see is the 20A batt max limit. That should be 30A 😜.

We are ready to hear your FOC results/reaction now btw :slight_smile:.
```

---
## \#15 Posted by: joeadams101 Posted at: 2017-10-04T06:06:42.992Z Reads: 63

```
I am in LOVE with it. So fucking silent!  Only problem is I think I need to replace my battery pack!!sagging like a b!! My 10s3p has that 40 fuse. Idk if this space cell can handle that 30...What do you think?
```

---
## \#16 Posted by: florensvb Posted at: 2017-10-05T16:31:47.521Z Reads: 50

```
i also feel like my battery has been sagging more since switching to foc ...
```

---
## \#17 Posted by: florensvb Posted at: 2017-10-05T16:34:30.290Z Reads: 49

```
You are saying that you have a 10s battery, but your _baterry cutoff end_ is at 27.0V

That would mean you drain the cells to 27.0V / 10 = 2.7V ?
```

---
## \#18 Posted by: BigBoyToys Posted at: 2017-10-05T17:08:34.485Z Reads: 45

```
If you are already sagging then not the best idea, but I think the fuse will handle it just fine. I run my 3P packs with 40A fuse higher and have never popped a fuse. You get the BMS cutoff before the fise pops. Sounds like its time for you to build a 12S5P 😉
```

---
