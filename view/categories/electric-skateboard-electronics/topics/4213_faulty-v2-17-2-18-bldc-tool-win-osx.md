# Faulty v2.17-2.18 bldc-tool win/osx!

### Replies: 55 Views: 5564

## \#1 Posted by: chaka Posted at: 2016-06-04T01:21:36.753Z Reads: 240

```
Anyone updating to the win/osx version 2.17-2.18 bldc-tool should know that it is causing VESC's to fail. @jacobbloy please take this faulty version down. 

We will be asking those that have already toasted their VESC to  carry the material expense and shipping for this repair. Don't worry, it wont be much, probably just a drv chip. Hopefully it  isn't frying the pcb's. We will have a better idea of the cost once the first round of repairs comes in.

The linux version 2.18 operates fine. win/osx users should stay on 2.16 until further notice.
```

---
## \#2 Posted by: NNGG Posted at: 2016-06-04T01:31:09.000Z Reads: 225

```
thanks m8 4200
```

---
## \#3 Posted by: jakobnator Posted at: 2016-06-04T01:34:19.120Z Reads: 218

```
Wow just got a used 4.7 VESC and tried to update it to 2.18 using that version and it kept saying that it was 2.15 even after updating firmware. Downgraded tool to 2.15 (version that was installed) and it worked fine, glad I didn't keep trying to get it to work......
```

---
## \#4 Posted by: jacobbloy Posted at: 2016-06-04T02:09:00.093Z Reads: 214

```
@chaka I updated it a week ago mate!

The only problem was with FIC giving the wrong kp and Ki results.
```

---
## \#5 Posted by: c4Lvin Posted at: 2016-06-04T03:29:05.954Z Reads: 202

```
Guys I have no idea what version is my boards VESC is. I just started riding today as I bought a used board which was already setup for me. Do I just plug it up to the PC with the program? I have no complaints so far so why should I upgrade the FW and risk damaging it? Thanks guys.
```

---
## \#6 Posted by: chaka Posted at: 2016-06-04T03:58:23.925Z Reads: 193

```
We'll see what is going on. We had something like this happen awhile back with an update and all that was needed was a reflash of the firmware.  Until then I suggest staying at 2.16 on win/osx and 2.18 linux.
```

---
## \#7 Posted by: jacobbloy Posted at: 2016-06-04T05:46:51.649Z Reads: 189

```
Also the few ppl that have contacted today about this have all said they tried to update there firmware and then started to have problems,
I asked all of them what version vesc they are using and all of them said they didn't know.

Sadly this is a problem we don't know if they have used a 4.7 firmware on a 4.12 vesc.

I have know tested Windows and OS X and have done over 20 firmware updates on both going from 2.16 and 2.17 to 2.18 and then done a ride up and down the hall way and no problems, 
I have a bad detection on 1 vesc in FOC but this vesc flashed red 4 times like it does when you don't have an updated c18.

I will keep testing tho.
```

---
## \#8 Posted by: treenutter Posted at: 2016-06-04T15:33:09.045Z Reads: 172

```
[quote="jacobbloy, post:7, topic:4213"]
I asked all of them what version vesc they are using and all of them said they didn't know.
[/quote]


If they don't know which HW version they have, how can they select the right firmware to install? Is it possible that the problem is not with the Windows port but that folks are attempting to update VESC without fully understanding the process first?

I empathize with those who end up with a dead VESC!
```

---
## \#9 Posted by: treenutter Posted at: 2016-06-04T15:35:07.217Z Reads: 174

```
@c4Lvin this thread is a great way to get started with your VESC. There's some learning to do before you start upgrading the firmware. Short answer to your question is that you don't have to upgrade if you are already happy with performance. 

http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980
```

---
## \#10 Posted by: jacobbloy Posted at: 2016-06-04T15:50:12.406Z Reads: 162

```
I empathise with them 2 and after @chaka gets them back and checks what the problem is, if it's my doing I'll try and chuck some money the part replacement fund. But I use the ported software at least for an hour a day and I'm not having these problems.
```

---
## \#11 Posted by: chaka Posted at: 2016-06-04T19:20:30.657Z Reads: 146

```
Awesome that you would offer something like that! We will probably not charge anyone for this, I think the worst of it is over so we can take the hit. Worst case I can send these guys some rebuilds I have set aside for myself. 

The good news is on every case they have not been able to revert back to version 2.16 so I think something is going on during the initial update to 2.18 on wind/osx I am betting it will be resolved with a reflash on an st-link.
```

---
## \#12 Posted by: michaelcpg Posted at: 2016-07-21T00:50:49.118Z Reads: 117

```
Is this still an issue or has the BLDC tool been fixed?
```

---
## \#13 Posted by: chaka Posted at: 2016-07-21T01:20:38.520Z Reads: 116

```
Only an issue for those that downloaded during that short period of time.
```

---
## \#14 Posted by: Jinra Posted at: 2016-07-21T01:28:41.565Z Reads: 117

```
This still seems to be an issue, however.

http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262
```

---
## \#15 Posted by: michaelcpg Posted at: 2016-07-21T05:06:12.758Z Reads: 113

```
Thanks @jinra. I can confirm that this is still an issue with the latest Windows version of the BLDC tool downloaded from @jacobbloy's site
```

---
## \#16 Posted by: jacobbloy Posted at: 2016-07-21T05:32:12.353Z Reads: 109

```
I would say this is an issue with all code, as I have build this direct from Benjamin's branch. And building it in a new OS does not change little code sections like this.
```

---
## \#17 Posted by: jrpwit Posted at: 2016-07-21T05:54:56.805Z Reads: 111

```
Where can you even find 2.16??? It isn't under the "older versions" on Jacob's website which is an obvious problem. Is their anywhere else to download the the tool?
```

---
## \#18 Posted by: Jinra Posted at: 2016-07-21T05:55:48.413Z Reads: 107

```
2.18 has worked fine for me, the only thing weird is the bug I mentioned above.
```

---
## \#19 Posted by: jrpwit Posted at: 2016-07-21T06:02:13.417Z Reads: 102

```
Good to know that 2.18 is still safe except for the minor bug.
```

---
## \#20 Posted by: jacobbloy Posted at: 2016-07-22T07:11:02.194Z Reads: 103

```
@michaelcpg @chaka  From looking into it and talking to Vedder today this problem originates in the firmware not BLDC tool, it has been fixed on GitHub but not with the previous firmware files that are made when building BLDC tool, so those using Linux will not have the problems.

I will try and find time to rebuild the firmware and reupload them.
```

---
## \#21 Posted by: Bender Posted at: 2016-07-22T11:53:13.907Z Reads: 96

```
Thanks Jacob!

Please post here when you do.:beers:
```

---
## \#22 Posted by: jacobbloy Posted at: 2016-08-15T01:58:30.765Z Reads: 81

```
hey guys i have fixed the issue so that you shouldn't have the ramp step issue any more. as of the 15th of august. this was an issue with the firmware to BLDC TOOL
```

---
## \#23 Posted by: Namasaki Posted at: 2016-08-15T02:29:52.938Z Reads: 81

```
So, the issue is in the firmware on the Vesc?
Then we need to update our Vesc's firmware?
```

---
## \#24 Posted by: Jinra Posted at: 2016-08-15T02:31:37.861Z Reads: 83

```
Yep it's a firmware issue not BLDC.
```

---
## \#25 Posted by: Namasaki Posted at: 2016-08-15T04:52:23.200Z Reads: 80

```
So where do we download the new fixed firmware
```

---
## \#26 Posted by: Jinra Posted at: 2016-08-15T05:02:01.231Z Reads: 82

```
vesc.net.au If you download the windows version it'll place the firmwares in C:\program files (x86)\bldc tool\drivers\firmwares
```

---
## \#27 Posted by: Namasaki Posted at: 2016-08-15T05:02:48.656Z Reads: 78

```
same for mac?
```

---
## \#28 Posted by: Jinra Posted at: 2016-08-15T05:03:19.919Z Reads: 80

```
Different location but it should be there. Just check the firmware tab in BLDC tool and hit "choose"
```

---
## \#29 Posted by: Namasaki Posted at: 2016-08-15T05:31:28.575Z Reads: 76

```
So, I need to re-download the bldc tool and re-install it and it will have the new firmware?
```

---
## \#30 Posted by: Jinra Posted at: 2016-08-15T05:33:49.591Z Reads: 74

```
If you're on Mac I think it comes with a folder with all the firmware, but Windows yea I think you gotta reinstall to extract the files.
```

---
## \#31 Posted by: Namasaki Posted at: 2016-08-15T05:39:55.533Z Reads: 74

```
Mac is super simple. you don't have to "uninstall" a program to remove it. 
You just grab the icon in the applications folder and drop it in the trash then empty the trash and it's automatically uninstalled.
That's what I'll do then re-install the new ver.
```

---
## \#32 Posted by: Jinra Posted at: 2016-08-15T05:41:11.846Z Reads: 71

```
Yea I know, I use both :) You technically don't even have to 'install' it. Just run the program
```

---
## \#33 Posted by: lox897 Posted at: 2016-08-15T05:43:13.239Z Reads: 69

```
Aren't there still files in say Application support, or config and log files?
```

---
## \#34 Posted by: Namasaki Posted at: 2016-08-15T05:44:19.075Z Reads: 72

```
Just drop the icon into the applications folder and done.
I used windows for years then switched to mac about 6 years ago.
Mac is so much better imo
```

---
## \#35 Posted by: Namasaki Posted at: 2016-08-15T05:44:50.703Z Reads: 71

```
you mean on windows?
```

---
## \#36 Posted by: lox897 Posted at: 2016-08-15T05:45:15.963Z Reads: 74

```
No, I mean Mac.
```

---
## \#37 Posted by: Jinra Posted at: 2016-08-15T05:45:29.002Z Reads: 74

```
Nope, it's stand alone.

@namasaki I like both, and I have to use Mac for work. Some things it does better, but some things I like on Windows more.
```

---
## \#38 Posted by: Namasaki Posted at: 2016-08-15T05:46:01.894Z Reads: 73

```
you on windows
```

---
## \#39 Posted by: lox897 Posted at: 2016-08-15T05:46:03.497Z Reads: 70

```
I really do learn something new on this forum every day. Thanks guys.
```

---
## \#40 Posted by: Namasaki Posted at: 2016-08-15T05:48:32.826Z Reads: 75

```
I used to discount mac because there hardware specs where always less than pc for the same or more $$
But hardware specs are misleading. The Mac OS is so much better than windows that it performs better with less hardware power.
Really what your paying for with Mac is perfectly matched hardware with no conflict issues and the OS.
Also when ever they come out with a new OS, the upgrade is always free. Unlike Windows.
Oh forgot, your also paying for style and dependability.
My mac mini is 6 years old and still going strong and I have never had to wipe my drive and reinstall the OS to improve performance or clean off some virus.
```

---
## \#41 Posted by: Namasaki Posted at: 2016-08-15T05:54:30.889Z Reads: 70

```
So, got the new bldc and firmware on my sys.
My Vesc's are coming tomorrow. 
So, on the firmware update, should I connect each vesc and update the firmware first? and where is that function in the bldc tool?
Never mind, I found it.
Wow what a dumb question that was.
```

---
## \#42 Posted by: Jinra Posted at: 2016-08-15T05:55:36.990Z Reads: 70

```
Yea you should probably update the firmware first so you dont have to worry about the max current ramp bug.

And lol
```

---
## \#43 Posted by: Namasaki Posted at: 2016-08-15T05:58:43.536Z Reads: 69

```
This bldc tool supports firmware ver 2.17 and 2.18
The firmware files in the firmware folder are not identified this way
Not sure which is the correct one or what subfolder to choose in the path window
```

---
## \#44 Posted by: Jinra Posted at: 2016-08-15T05:59:42.597Z Reads: 72

```
[quote="Namasaki, post:40, topic:4213, full:true"]
I used to discount m̶a̶c̶ complete boards because there hardware specs where always less than p̶c̶ DIY for the same or more $$But hardware specs are misleading. The M̶a̶c̶ ̶O̶S̶ Boosted ESC firmware is so much better than w̶i̶n̶d̶o̶w̶s̶ ̶ DIY that it performs better with less hardware power. Really what your paying for with M̶a̶c̶ ̶ Boosted is perfectly matched hardware with no conflict issues and the O̶S̶ ESC.Also when ever they come out with a new O̶S̶ ESC firmware, the upgrade is always free. Unlike W̶i̶n̶d̶o̶w̶s̶ VESC revisions.Oh forgot, your also paying for style and dependability.My m̶a̶c̶ ̶m̶i̶n̶i̶ Boosted Board is 6 years old and still going strong and I have never had to w̶i̶p̶e̶ ̶m̶y̶ ̶d̶r̶i̶v̶e̶ ̶a̶n̶d̶ ̶r̶e̶i̶n̶s̶t̶a̶l̶l̶ ̶t̶h̶e̶ ̶O̶S̶ reflash and configure my ESC to improve performance or clean off some v̶i̶r̶u̶s̶ errors.
[/quote]

:grin: Just playing around though
```

---
## \#45 Posted by: Jinra Posted at: 2016-08-15T06:00:32.372Z Reads: 72

```
You use the firmware with the corresponding hardware version. If you just bought a VESC it should be 4.11 or 4.12.
```

---
## \#46 Posted by: Namasaki Posted at: 2016-08-15T06:04:03.772Z Reads: 73

```
So the folder marked 410,411,412?
Do you just put the folder in the path or do you have to designate a specific file?
```

---
## \#47 Posted by: Jinra Posted at: 2016-08-15T06:05:22.996Z Reads: 72

```
I think you can just use the VESC_default.bin file.
```

---
## \#48 Posted by: Namasaki Posted at: 2016-08-15T06:06:36.075Z Reads: 73

```
Need to be sure. Uploading wrong firmware could break the Vesc
```

---
## \#49 Posted by: Jinra Posted at: 2016-08-15T06:08:08.373Z Reads: 75

```
Looks like it.

https://youtu.be/JZSM_DmKx_Y?t=131
```

---
## \#50 Posted by: Namasaki Posted at: 2016-08-15T06:12:22.115Z Reads: 70

```
Thanks, I bookmarked the vid.
So, do really think the boosted firmware is better than the vesc firmware?
```

---
## \#51 Posted by: Jinra Posted at: 2016-08-15T06:15:35.343Z Reads: 71

```
Nah I was just joking around. VESC is customizable, but I'm sure Boosted's ESC is very stable.
```

---
## \#52 Posted by: Namasaki Posted at: 2016-08-15T06:20:24.717Z Reads: 73

```
What kept me from buying a boosted is their lack of deck choices and their lack of range
```

---
## \#53 Posted by: Jinra Posted at: 2016-08-15T06:20:53.638Z Reads: 72

```
You build your own boards, much cooler anyway!
```

---
## \#54 Posted by: Namasaki Posted at: 2016-08-15T17:46:28.305Z Reads: 65

```
So, do you set and save all the Vesc parameters and then do motor detection ?
```

---
## \#55 Posted by: Jinra Posted at: 2016-08-15T17:48:46.867Z Reads: 65

```
Either one. It shouldn't rely on your VESC parameters to do motor detection. Though low voltage cut off might affect if it's able to run.
```

---
