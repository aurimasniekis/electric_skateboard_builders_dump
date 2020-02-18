# Programming SK8 VESC on MacBook via USB C

### Replies: 11 Views: 340

## \#1 Posted by: Kuchi Posted at: 2018-06-14T03:20:02.298Z Reads: 111

```
Ok so I have pretty good knowledge with reg esc and electronic programming on my MacBook such as betaflight. But I have not been able to find the download to program my Vesc on my MacBook. Also what software do you recommend I use for them, I am running Hobbyking SK8 VESC with the SK8 6374 149kv motors on 12s with an AT setup. I appreciate any help I can get just can’t find much on this. FYI I want to have good torque and top speed.
```

---
## \#2 Posted by: telnoi Posted at: 2018-06-14T03:27:43.178Z Reads: 110

```
There are osx builds Available in the vesc tool thread here, though not official and maybe not the latest.

The windows version also works with parallels or bootcamp where the former is actually the easiest solution. Not going to explain how to use it, plenty of info online. In my opinion it's self explanatory.

Last step, USB-c to USB adapter.
```

---
## \#3 Posted by: Kuchi Posted at: 2018-06-14T04:38:14.124Z Reads: 100

```
So is there no legit OS X tools for vesc so would it be better to just do it on windows, if so what protocol works the best with the hobby king vesc
```

---
## \#4 Posted by: telnoi Posted at: 2018-06-14T04:46:35.431Z Reads: 95

```
Ackmaniac's version of the vesc tool or the official firmware at vesc-project.com. Personal preference. Ackmaniac's firmware offers better failsafe and has watt control, but imo it's a bit more complex to setup.

I personally haven't had issues with 
https://github.com/rpasichnyk/vesc_tool/releases

Which is the unofficial osx build of the vesc tool. Been updated 3 days ago so it's most likely the most recent version of the vesc tool.
```

---
## \#5 Posted by: Kuchi Posted at: 2018-06-16T03:48:25.720Z Reads: 59

```
Is that the link for Ackmaniac's version
```

---
## \#6 Posted by: telnoi Posted at: 2018-06-16T09:12:54.794Z Reads: 50

```
No, vesc tool.
```

---
## \#7 Posted by: Kuchi Posted at: 2018-06-16T16:49:44.254Z Reads: 46

```
Ok do you have a link for ackmaniacs version then
```

---
## \#8 Posted by: telnoi Posted at: 2018-06-17T20:47:58.511Z Reads: 39

```
Dunno if there is one. Search his thread for the typical terms...osx/mac
```

---
## \#9 Posted by: Jack_Roy Posted at: 2019-02-10T21:13:41.746Z Reads: 26

```
I can't seem to get the software (or perhaps hardware) to connect, all is switched on, and it runs through all the possible connections, then acts as if there is nothing there. I suspect the USB C adapter, of which I have tried two. Anyone having trouble like this?
```

---
## \#10 Posted by: Pimousse Posted at: 2019-02-10T21:46:52.498Z Reads: 21

```
Same issue here. It worked for a time, than nothing.
VESCs are still recognised with a PC under Win10.
```

---
## \#11 Posted by: telnoi Posted at: 2019-02-11T05:27:05.890Z Reads: 18

```
Haven't connected it yet using a touchbar MBP or USB-C type connection, so can't tell if the adapter might be to blame or not. 
You can at least check if the vesc is unrecognized. 

https://community.smarttech.com/articles/HOW_TO/How-to-identify-Unknown-USB-device?r=2&RecordGvp.getRecord=1&ArticleTopicList.getTopics=1&ArticleView.getArticleHeaderDetail=1&QuestionPost.getInitData=1&Headline.getInitData=1&Quarterback.validateRoute=1

Typical failure is also a cable that is too fat and doesn't go all the way in vesc side. Get a knife and cut off as much plastic of the connector as you can.
```

---
