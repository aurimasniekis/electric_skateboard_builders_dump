# Where to get old version of BLDC_Tool

### Replies: 14 Views: 1501

## \#1 Posted by: NerijusM Posted at: 2017-07-11T10:43:55.198Z Reads: 94

```
Hi,

my VESC are running on 4.16, but i need to upgrade to latest version. I dont have xml for my settings.
Can i update and keep settings, or i need to make xml?
Where can i download bldc_tool for that? MAC OS or windows...

Thank you.
```

---
## \#2 Posted by: rpn314 Posted at: 2017-07-11T10:52:20.322Z Reads: 93

```
You can use any version of BLDC-Tool to flash a firmware. Just make sure that firmware is compatible with the hardware version you have.

When you update, your setting will be lost so you will need to make a manual back (write them down, which I'd recommend over an xml anyways) and/or export the setting to an xml.
```

---
## \#3 Posted by: NerijusM Posted at: 2017-07-11T11:06:10.538Z Reads: 88

```
Can you give me download link or just share your tool over dropbox etc...?
Simply i cant find working download...
```

---
## \#4 Posted by: rpn314 Posted at: 2017-07-11T11:08:00.998Z Reads: 84

```
Oh, you don't have BLDC-Tool at all?
```

---
## \#5 Posted by: NerijusM Posted at: 2017-07-11T11:09:44.675Z Reads: 82

```
Yes, and i cant find any working download link... All VESC supporting websites are down or what...
```

---
## \#6 Posted by: rpn314 Posted at: 2017-07-11T11:11:17.222Z Reads: 81

```
Oh yeah. The ones that were hosted by a member of the forum did die. I only have the Mac version, but Enertion has a download on their site: 
http://www.enertionboards.com/new-focbox-speed-controller/focbox-bldc-tool-win/
```

---
## \#7 Posted by: NerijusM Posted at: 2017-07-11T11:12:21.759Z Reads: 78

```
Can you share MAC version? Thanks.
```

---
## \#8 Posted by: rpn314 Posted at: 2017-07-11T11:13:33.571Z Reads: 75

```
http://www.enertionboards.com/new-focbox-speed-controller/focbox-bldc-tool-mac/

edit:
Or http://www.esk8.de/tutorials-d-e-f/ has all versions as well (just click Download Links on the left hand side)
```

---
## \#9 Posted by: NerijusM Posted at: 2017-07-11T11:29:50.082Z Reads: 67

```
Yes, thank you.
But i got error - my VESC firmware is too old... So i looking for older bldc_tool....
Oh well :slight_smile:
Thank you!
```

---
## \#10 Posted by: rpn314 Posted at: 2017-07-11T11:40:58.718Z Reads: 68

```
Are you just trying to update or are you also trying to export your settings?
```

---
## \#11 Posted by: NerijusM Posted at: 2017-07-11T11:47:11.200Z Reads: 67

```
I want to update, but also to get all my settings back... I need 2 diferent versions of bldc_tool for that... Now i have latest, but also i need older one, for 4.16 FW.
```

---
## \#12 Posted by: rpn314 Posted at: 2017-07-11T11:58:54.185Z Reads: 66

```
Yeah, you're gonna have a hard time finding an old bldc-tool download floating around. Best bet is probably to make a Ubuntu virtual machine, clone vedder's BLDC-Tool github, revert back to that version of BLDC-Tool, and build it yourself.
```

---
## \#13 Posted by: NerijusM Posted at: 2017-07-12T06:29:15.558Z Reads: 60

```
Solved!
If someone else needs - https://www.dropbox.com/sh/y45400qo6shgqah/AACuUgBrGlQL3DPKQ_FYepPsa?dl=0
```

---
## \#14 Posted by: cnd Posted at: 2019-04-27T12:09:09.325Z Reads: 23

```
FYI - You CANNOT update old firmware using "any version of bldc tool or vesc tool" - because the old versions simply say "blah too old blah. update with a programmer" and REFUSE to connect, and the firmware update steps do not run without a connect. (Folk with new VESC's probably don't know that old VESC's do that, because they've never seen old firmware before).
```

---
