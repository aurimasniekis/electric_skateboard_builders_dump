# How to update the vesc firmware

### Replies: 33 Views: 2780

## \#1 Posted by: dg798 Posted at: 2017-08-23T21:12:30.511Z Reads: 234

```
<img src="/uploads/db1493/original/3X/1/5/15623cb8435f27e67ec7b7f9304b6e4f012d6be7.JPG" width="374" height="500">

Which one do I pick to update to 4.12
```

---
## \#2 Posted by: onepunchboard Posted at: 2017-08-23T21:16:19.231Z Reads: 228

```
default default default
```

---
## \#3 Posted by: dg798 Posted at: 2017-08-23T21:17:29.953Z Reads: 225

```
ok thank you but i keep getting "buffer erase timeout"
```

---
## \#4 Posted by: onepunchboard Posted at: 2017-08-23T21:32:34.466Z Reads: 222

```
it might not have bootloader
```

---
## \#5 Posted by: dg798 Posted at: 2017-08-23T21:33:17.953Z Reads: 219

```
does my vesc need to be connected to update the firmware
```

---
## \#6 Posted by: onepunchboard Posted at: 2017-08-23T21:46:41.174Z Reads: 213

```
if vesc don't have bootloader u need ST LINK.  or if u have beta bldc tool u can use that. which I don't know where to get
```

---
## \#7 Posted by: onepunchboard Posted at: 2017-08-23T21:47:32.464Z Reads: 198

```
and u need to connect vesc first of course
```

---
## \#8 Posted by: dg798 Posted at: 2017-08-24T00:42:23.904Z Reads: 193

```
i tried connecting the vesc and i upload the firmware and it gets to 100% and then it just disconnects fom the vesc and it doesnt end up updating.
```

---
## \#9 Posted by: onepunchboard Posted at: 2017-08-24T13:02:57.978Z Reads: 186

```
yeap looks like urs don't have bootloader. is it chinesium vesc?
```

---
## \#10 Posted by: L3chef Posted at: 2017-08-24T13:48:46.212Z Reads: 186

```
So after it disconnects, and you reconnect to bldc tool. What FW does it say it has?
```

---
## \#11 Posted by: rich Posted at: 2017-08-24T13:58:56.010Z Reads: 189

```
[quote="L3chef, post:10, topic:31340, full:true"]
So after it disconnects, and you reconnect to bldc tool. What FW does it say it has?
[/quote]

Yes, that's the main question.
If the FW stays the same as before I welcome you to the angry maytech family :joy:
VESC Tool should be released very soon and uploading the bootloader is just one click, I did it with my smescs 4.12 (shitty maytech esc) without problems.
```

---
## \#12 Posted by: dg798 Posted at: 2017-08-24T23:31:16.390Z Reads: 174

```
It still says 2.18 after I reconnect it. So should I download boot loader and if so how do I do that??
```

---
## \#13 Posted by: dg798 Posted at: 2017-08-24T23:31:44.163Z Reads: 174

```
And my vesc is from enertion.
```

---
## \#14 Posted by: onepunchboard Posted at: 2017-08-25T05:42:25.322Z Reads: 164

```
u sure updating to higher ver? beside if it's focbox why r u updating? it works fine out of the box
```

---
## \#15 Posted by: rich Posted at: 2017-08-25T07:32:50.042Z Reads: 164

```
[quote="dg798, post:13, topic:31340"]
my vesc is from enertion
[/quote]

AFAIK only the maytech have missing bootloader, so this shouldn't be a problem in your case. 
I guess you wanted to update to FW 2.54, right?
```

---
## \#16 Posted by: Hardwiring Posted at: 2017-08-25T08:11:15.832Z Reads: 149

```
Anyone know where to get the beta tool from?I have amongst my vesc collection a couple of Maytechs for a project I'm still getting around to
```

---
## \#17 Posted by: rich Posted at: 2017-08-25T08:41:04.864Z Reads: 144

```
VESC Tool should be released soon :wink: (only available for VESC 6 beta users so far)
```

---
## \#18 Posted by: dg798 Posted at: 2017-08-25T14:04:37.108Z Reads: 135

```
i wanted to update to 4.12.
i have the firmware but as i said it completes the update but then it automatically disconnects and when i reconnect it, its still at 2.18.
```

---
## \#19 Posted by: L3chef Posted at: 2017-08-25T14:08:42.353Z Reads: 138

```
4.12 is the HW version.(hardware) 2.18 is FW version. And 2.18  should be the latest version afaik
```

---
## \#20 Posted by: dg798 Posted at: 2017-08-25T14:10:28.294Z Reads: 144

```
so how do i update to 4.12.
thats what my vesc is supposed to be and how would i check what hardware version it is??
```

---
## \#21 Posted by: Blasto Posted at: 2017-08-25T14:19:14.535Z Reads: 136

```
[quote="dg798, post:20, topic:31340"]
so how do i update to 4.12.
[/quote]

[quote="L3chef, post:19, topic:31340"]
4.12 is the HW version.(hardware)
[/quote]
[quote="L3chef, post:19, topic:31340"]
And 2.18  should be the latest version
[/quote]



The lattest FIRMWARE is 2.18
```

---
## \#22 Posted by: rich Posted at: 2017-08-25T14:20:13.425Z Reads: 131

```
You can't update the hardware but the firmware. When did you buy the vesc? And firmware 2.18 ist the latest
```

---
## \#23 Posted by: L3chef Posted at: 2017-08-25T14:21:34.530Z Reads: 129

```
Okay. One more time. Your Vesc is hardware version 4.12.  
And the firmware that is loaded on your Vesc is version 2.18
Don't mix up hardware version and firmware.

So to make it absolutely crystal clear... Your vesc is Up To Date.
```

---
## \#24 Posted by: dg798 Posted at: 2017-08-25T14:28:21.677Z Reads: 124

```
ok thanks guys
```

---
## \#25 Posted by: onepunchboard Posted at: 2017-08-25T16:19:25.579Z Reads: 120

```
😂 hahahaha
```

---
## \#26 Posted by: Hardwiring Posted at: 2017-08-25T19:29:37.936Z Reads: 116

```
Before we have to much fun.... I was sure someone said there was a beta version they had used to update the FW !??! I mean I can wait though😂🤣😂🤣😂 I mean FW not HW to btw
```

---
## \#27 Posted by: rich Posted at: 2017-08-25T19:56:08.022Z Reads: 115

```
True, but it's called VESC Tool which is the new software instead of BLDC Tool, released soon :grin:
Beside VESC 6 it can upload new FW 3.26 on HW 4.7 - 4.12 (and bootloader if needed)
```

---
## \#28 Posted by: TehAtheist Posted at: 2017-08-26T07:58:37.047Z Reads: 116

```
That's awesome. I'm planning on buying an ST link to update, but I may just wait for the release of this tool then?
```

---
## \#29 Posted by: rich Posted at: 2017-08-26T09:24:19.012Z Reads: 122

```
I ordered a STLinkV2 plus cables from china and received it after 4 weeks. I did research for days and came to the conclusion that I don't do it :joy: It looks soo complicated to me and I didn't want to harm my HW because I'm neither a computer nor a electriconics expert but I'm sure for some people it's easy to do that. But since I know how simple it is with VESC Tool by clicking just a button I would wait for it except you know what you are doing.

But I want to mention that from my experience FW 2.18 ist still the best for maytech V4.12 (which you have). The problem is that most (or all?) of them have the buggy FW (current ramp step bug). With bootloader it's possible to upload bug free FW.

With my dual maytech V4.12 i tested FW 2.18, FW 2.54 and FW 3.26 with equal settings for 20km each. Then I connected it to Vesc/bldc tool and checked for faults in terminal.

FW 2.18 (bug free): 0 FAULTS
FW 2.54: 37 ABS over current and 1 drv FAULTS
FW 3.26: 0 FAULTS but one motor got very hot while the other is just warm (the new FW has a different way to control dual motos which my maytech didn't like)

Tried FOC but there are cut offs and drv faults every single time when hitting the break.

So I ordered new quality ones from esk8.de and are super happy with them. I'm running FW 3.26 in sensored FOC mode without problems so far. There are a lot of improvements regarding FOC in the new FW, that's why I gave it a try.
```

---
## \#30 Posted by: cliofreak Posted at: 2018-01-24T13:02:47.824Z Reads: 83

```
So I really want to take full advntage of all the features on @rpasichnyk Metr app but Im getting this message. The VESC details from seller are also seen in screen grab. How do I get newer FW on this with no Bootloader and Im using a Mac?!
 This is my VESC: https://eskating.eu/product/electric-skateboard-speed-controller-maytech-based-upon-the-vesc/



[10|690x159](upload://m758xeFMI8ea1T216BZKi2965AF.png)![48|419x500](upload://vj8MfJZxrXXEIfWoefG7FmpnLqU.png)
```

---
## \#31 Posted by: Lumaci Posted at: 2018-01-24T13:22:28.443Z Reads: 77

```
With no bootloader you would need to install one, buy a cheap ST Link V2 of ebay they are 1 Dollar shipped and install it and download vesc project after to install the new firmware.
```

---
## \#32 Posted by: cliofreak Posted at: 2018-01-24T13:25:54.215Z Reads: 75

```
Thanks, Ive just ordered an STLV2. Ive also just discovered  that @rpasichnyk has released a VESC TOOL for Mac! Awesome... its opened. So, do I still need the STLINK if I have the VescTool?
```

---
## \#33 Posted by: Lumaci Posted at: 2018-01-24T13:28:07.591Z Reads: 71

```
Yes, unless they recently changed that.

You can try and go into Vesc Project and Bootloader and find the right one and see what it says, i had to use a ST Link when i did it a few months ago.
```

---
