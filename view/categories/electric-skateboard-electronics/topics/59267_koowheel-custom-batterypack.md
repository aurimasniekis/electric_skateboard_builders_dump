# Koowheel custom batterypack

### Replies: 17 Views: 1280

## \#1 Posted by: willumpie82 Posted at: 2018-06-18T11:52:56.962Z Reads: 173

```
Hi,

i'm working on a custom larger battery pack that will fit the koowheel gen2

10s3P (preferable with 30Q's) for a total op 9000mah (standard pack 10s2p = 5500mah)
Simple chinese BMS (40A), smart BMS does not fit the width
D-sub 2w2 30A connector (as per original pack)
It is about 46cm long, to mount it you'll have to remove the front trucks
The design is modular, the mid sections are identical everything held together with four M4 threads
printing time on UM2 clone, ~4h/part, with 8 parts > 32h

1st Renders:
![f75ca1776cb53ffa7e8dc624e3097fbed4e60fc6|690x352](upload://zigowLG5WOJVoIDtOyugaJzY3eC.JPG)

Cell configuration
![efdf1ea4fb705c038f87f434c214440563995d51|690x352](upload://ye097PZETlOxEd8FpnLpenvEi53.JPG)

3d prints (partially with random cells) :
![IMG_20180617_181115|375x500](upload://74KwitdxJKHhzFW6gEEQMkZ6kLg.jpg)
![IMG_20180617_181014|375x500](upload://wMe33pMbW6YQ05z2R3WoFuXf05g.jpg)
```

---
## \#2 Posted by: sunnyD Posted at: 2018-06-19T04:26:15.187Z Reads: 134

```
genius 

10char
```

---
## \#3 Posted by: willumpie82 Posted at: 2018-06-25T07:41:13.154Z Reads: 124

```
**update**: All parts printed, old set of batteries (for testing/fitting purpose) battery arrangement is a pain, the 3P packs are okay, spot welded the cells together and than solder the strips in series, the split 3P's are a pain, there is not a lot of room for the wire to the split cell, also wiring them in series is a real brain pain ;-)

But it is all in, the lids close (mostly) but my CAD design need some tweaks since i used an exacto knife to make stuff (wires and plates) fit, later i'll post a pic of the finished pack, waiting for the BMS now...

One of the pictures is my kitchen, that's the only place where it won't shut-off my house when spot welding, fuse trips ever so often

![IMG_20180622_202654|375x500](upload://fhjlvxpj9jihOMFM0VsOKsJ2mii.jpg)![IMG_20180622_170151|666x500](upload://tg0efc8NoOWkmB0u4NOpf5rNbhv.jpg)![IMG_20180623_152857|666x500](upload://mh5WMUDDlupsa9wTJDG4qOOUg6i.jpg)![IMG_20180623_152902|666x500](upload://yggyQNaidJATgThwWIwnCR48EDe.jpg)
```

---
## \#4 Posted by: sunnyD Posted at: 2018-06-25T17:29:19.369Z Reads: 115

```
OOO! colorful :slight_smile:
```

---
## \#5 Posted by: careyer Posted at: 2018-08-28T08:32:47.412Z Reads: 103

```
This is so awesome! Can't wait to see the finished product. Hopefully you will share the finished design (and maybe the CAD files) on thingiverse? What CAD program have you used to design it?

I wonder if it is also possible to build a smaller Battery - maybe 10SP1 (using cells with a  higher C-Rating, what would be the appropriate Cell here?), so that the battery gets air-travel safe (<100Wh)? Since your design is modular this might work?

It would also be great if you could share links to the BMS and the power connector! Thanks!!!
Keep up the excellent work!

P:S: Nice kitchen! =D
```

---
## \#6 Posted by: willumpie82 Posted at: 2018-08-28T08:51:04.527Z Reads: 99

```
thanks :grin:

The design is made in Solidworks, i'll share the STL and a zip with design files soon

The design is modular, but didn't account for smaller packs, but the cad design is such that it can be easily modified :smiley:
```

---
## \#7 Posted by: careyer Posted at: 2018-08-28T09:08:44.839Z Reads: 94

```
Awesome! I use Solidworks myself. So it will easily be possible to adapt it for my use case. Thank you very much!!!!
```

---
## \#8 Posted by: ADi_HD Posted at: 2018-09-23T08:50:32.573Z Reads: 85

```
Are you using the original bms, they have a flaw in that one of the 3 screws retaining the bms come loose and shorted my batt, , any idea where to get one ?
```

---
## \#9 Posted by: willumpie82 Posted at: 2018-09-24T06:18:07.781Z Reads: 81

```
Nope, the original BMS does nothing special, I plan to use a cheap chinese BMS (unfortunately the smart bluetooth BMS wont fit the width). Imo you could put any BMS in there (except for the ones with power button) it's just a matter of taste and what you require w.r.t. safety temperature sensors, balance current, etc
```

---
## \#10 Posted by: careyer Posted at: 2018-10-08T12:24:00.316Z Reads: 73

```
Any news on your build to share? #ImpatientlyWaiting :wink:
```

---
## \#11 Posted by: willumpie82 Posted at: 2018-10-09T07:11:02.902Z Reads: 69

```
consider it done

https://www.thingiverse.com/thing:3145023
```

---
## \#12 Posted by: careyer Posted at: 2018-10-09T08:36:58.106Z Reads: 64

```
Awesome! Thank you very much for sharing! =) Looks sweet... can't wait to give it a try next summer!
```

---
## \#13 Posted by: careyer Posted at: 2018-10-10T08:55:15.669Z Reads: 59

```
Had a look through the files! Man this is awesome! Thank you very much for including the solidworks files as well. I want to try building three 10s1P modules which stack together. This way it will be airtravel safe since each module is <100Wh. This way you can take a huge battery with you which you can easily assemble at your travel destination.
Or you can also decide to ride with a single, dual or tripple module. 

P.S: The "koowheel-bms-cover.STL" has 0KB is corrupt. You may want to change this in the archive for people not having Solidworks at hand and can't convert the file easily. 

Thanks for sharing.
```

---
## \#14 Posted by: willumpie82 Posted at: 2018-10-10T09:24:30.143Z Reads: 58

```
hey careyer, 

thanks!

Youre idea of 1p10 made me thinking,... currently the wiring is a pain, with the cell groups, but what if we would wire them as 3 spererate 1p10s packs, that makes life way easier just wire them as 6 packs of 5s, only the balance wires has to get crazy, but since they do not pass the high current they can be something like awg24 or even smaller (ballancing hapens mostly at 200mA@4.2v thats like 840mW)


I checked the archive and it unpacks correctly on my machine
![image|415x238](upload://oiQNXH5cjDZkFdzls7xf4vK27Yg.png) 

![image|377x353](upload://z2dgjlLto9ae3UJ90Jk2flsAYDL.png)
```

---
## \#15 Posted by: careyer Posted at: 2018-10-10T12:36:10.164Z Reads: 51

```
Haha...  Sorry for putting an idea in your head! =)
That was exactly what I was thinking... 

3packs 1p10s each which can be easily taken apart and plugged together. (makes them airtravel compatible). And yes... this should make cabling much much easier.
I thought of 3 packs each with a D-sub 2w2 30A connector (so that they can also be used seperatly with the Koowheel) incl. pass-through balance connectors on each pack.
This way the can be driven as 1p10S, 2p10S, 3p10S ... and they can be balance charged with a single BMS (which is housed in Pack1) when they are all plugged together.

This will also solve the "need to remove the front axle to install" problem.

![KooWheelBatPack3|690x167](upload://55la0tYntP6fGubt1qXJCjEuYry.jpeg) 

Unfortunately I am not such a wizard than you designing in Solidworks. Do you mind working together on this project maybe?

Oh.. as for your ZIP:
I have redownloaded it twice... regardless with what Program I open it: 7Zip, WinRar, WinZip... it gives me this:
![Zip|621x500](upload://13oHKONiARcMl0dG0aoWDIQ1YsE.jpeg)
Maybe consider re-upping it to Thingyverse - just in case.
```

---
## \#16 Posted by: willumpie82 Posted at: 2018-10-10T13:26:58.880Z Reads: 43

```
note, for the balancing of 3 1p10s packs you must be careful, it is tricky to wire all the balance leads in parallel, when one or more cells are out of balance, the other parallel cell(s) will start to charge that cell(s) (with the max current the battery supports) I can imagine this happening when you mix and match used 1p-packs, this will evaporate the thin balance wires and you'll end up with ~30 small lithium rockets under your board or in your backpack

A solution would be to charge the packs 1 by 1 with an external bms, don't connect the balance wires in parallel. the board itself does not need a BMS afterall, only during charging

when you build/weld a full pack you always have to make sure the cells are balanced correctly. fresh cells mostly come balanced (storage voltage) but still check, check, check.


but if you are brave, you could use a 13w3 connector for the balancing & power from [aliexpress](https://www.aliexpress.com/item/D-Sub-Connector-30-AMP-Current-13-Power-Position-10-3-Combo-Plug-Male-Pins-Machine/32829763495.html)

thingiverse generates that zip-file if you download the full package in once, i re-upped the cover.stl and it downloads correctly now, its just weird.

I would love to support you on this quest, but i see quite some risks with this approach
```

---
## \#17 Posted by: careyer Posted at: 2018-10-10T14:10:30.286Z Reads: 40

```
I think your idea of leaving the BMS out of the equation is good... I have plenty of RC-Lipo chargers hanging around anyway.... so yes... let's build it without BMS and lets charge the packs separately outside of the board. No problem with that. Makes the cabling even more simple. Would be awesome to quest this together.

BTW: for balancing with an external balance charger these work out pretty well and they integrate nicely into enclosures: http://www.cnc-modellbau.net/bilder/Pfosten-ST-10pol.JPG
```

---
