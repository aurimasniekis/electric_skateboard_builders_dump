# PSA: Remember to reset your max current ramp step when programming your VESC

### Replies: 13 Views: 5356

## \#1 Posted by: Jinra Posted at: 2016-07-18T06:57:54.029Z Reads: 570

```
I've downloaded BLDC tool for Mac fairly recently and the "Max Current Ramp Step" bug still seems to be present. For those unaware, when you read and write config on the motor configuration tab, the Max current ramp step field under "advanced" will multiply by 10. This can possibly be fatal to your VESC so remember to reset it whenever you write to motor configuration.

The default value is **0.04**, however, if you set it to that and write it will change to **0.4** since it multiplies by 10, so set it to **0.004** and write config.

I've heard the issue was fixed, but i'm unsure as to where or what versions it's fixed for. This information is accurate as of 5/30 (when I downloaded BLDC tool) off Jacob's site (vesc.net.au) for OSX firmware v2.18. I can't confirm if this is happening on Linux/Windows.

EDIT: This issue is fixed on latest f/w revisions by @jacobbloy and @elkick. Not sure who else has updated f/w's uploaded, but these two have confirmed bug-free versions. The version will still be 2.18 so you won't know if you have a bug free version until you test it out. Information accurate as of 8/28/16
```

---
## \#2 Posted by: NNGG Posted at: 2016-07-21T07:00:24.129Z Reads: 490

```
Is this only for mac?
```

---
## \#3 Posted by: Jinra Posted at: 2016-07-21T14:07:53.172Z Reads: 444

```
windows confirm as well
```

---
## \#4 Posted by: NNGG Posted at: 2016-07-21T15:54:30.287Z Reads: 431

```
thanks for the info
```

---
## \#5 Posted by: elkick Posted at: 2016-07-27T19:37:18.119Z Reads: 402

```
I compiled FW 2.18 for VESCs 4.10 - 4.12 as a standalone version, it's tested but no guarantees though: [esk8.de](http://www.esk8.de/app/download/5802635032/VESC_default.)
```

---
## \#6 Posted by: elkick Posted at: 2016-07-31T15:20:19.207Z Reads: 379

```
Ok, some more people tested it, the error is fixed and it works without any issues.
```

---
## \#7 Posted by: Skitzor Posted at: 2016-08-01T18:30:04.001Z Reads: 360

```
I was just checking this because of my battery cutoffs at startup. It could have been related.

Both my VESC's had this setting at 50,000. (new one from you @elkick FW2.18) and my other enertion one which was at FW2.16. I've updated the enertion VESC to 2.18. Reading and writing the config on the enertion one at 2.18 still has this bug. The other vesc doesn't have this.
```

---
## \#8 Posted by: elkick Posted at: 2016-08-01T19:34:18.876Z Reads: 335

```
It should not be there anymore if you use the above posted version. But i don't understand, which of the updated VESCs is still showing the max. current step fault? 

I started uploading the new version directly with STlink under Ubuntu a while ago, but I could have also missed a few. :slight_smile:
```

---
## \#9 Posted by: Skitzor Posted at: 2016-08-01T19:39:48.103Z Reads: 316

```
The one from enertion that wasn't fried. So either the firmware 2.18 from jacob bloy still has the bug. Or firmware upload (no st-link yet) doesn't work, but changes the firmware number to 2.18
```

---
## \#10 Posted by: elkick Posted at: 2016-08-01T19:49:19.364Z Reads: 309

```
Jacobs FW and BLDC tool folder is not yet updated and still has this bug. 

You have to upload the exact firmware I linked above with any BLDC tool.  The BLDC tool you are using for this doesn't matter, the error is in the FW.
```

---
## \#11 Posted by: Skitzor Posted at: 2016-08-01T20:13:59.501Z Reads: 306

```
Allright, thanks for clearing that out. I will flash your firmware tomorrow !
```

---
## \#12 Posted by: krloz Posted at: 2017-03-29T14:29:40.654Z Reads: 170

```
I have a couple of new scramboards vescs with the Max current issue.
Does anyone have a working link for the bug free firmware??? The one posted above By @elkick IS not working.
Thank you very much
```

---
## \#13 Posted by: rpn314 Posted at: 2017-03-31T02:58:24.055Z Reads: 153

```
[quote="krloz, post:12, topic:6262, full:true"]
Does anyone have a working link for the bug free firmware??? The one posted above By @elkick IS not working.
Thank you very much
[/quote]

Honestly, just get @Ackmaniac's firmware. I know it's free from that bug, and does does everything that the original firmware does, plus much more.
```

---
