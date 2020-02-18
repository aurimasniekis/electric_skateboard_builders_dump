# Electrical layout help

### Replies: 12 Views: 1934

## \#1 Posted by: Bender Posted at: 2016-04-23T20:10:34.650Z Reads: 133

```
I'm working on my 1st esk8 build (I'll post it when I start)
I've ordered most of the parts and I'm pretty comfortable with all the other aspects of the build, but the electronics make me a little nervous, so any help or advice would be much appreciated 
Please critique my layout
Thanks in advance 

I'm using 4x 3s 4000mAh lipos two pairs in parallel to get 2x 6s 4000mAh, and then that in serial to get to 6s 8000mAh (does that make sense?)

Already have question, can I put a on/off switch behind the XT90S anti-spark instead of using it as a loop key?

<img src="/uploads/db1493/original/2X/c/c64d1243d62f1df87f517387a2ca9f6c6ed9d278.jpg" width="221" height="500">

EDIT:
thanks to Krudte for noticing that my series circuit was not correct and making a new diagram, so it should actually look like this:
<img src="/uploads/db1493/original/2X/9/93895a36a3d0f7f1e56b7fbc54f471516602e229.jpg" width="221" height="500">
```

---
## \#2 Posted by: trbt555 Posted at: 2016-04-23T20:34:18.437Z Reads: 111

```
You want to replace the loop key with an on/off switch ?
```

---
## \#3 Posted by: Bender Posted at: 2016-04-23T20:46:14.262Z Reads: 109

```
I was wondering if I can keep the XT90s  but yes place an on/off switch where the loop would be essentially 

I don't fully understand the spark thing
My basic understanding is that when the system is first turned on or connected in the case of the loop key that there is an initial surge that creates a spark and that the resistor in the XT90s would prevent that

Or would it be easier to just put a resistor in-line and add a switch and remove the XT90s?
```

---
## \#4 Posted by: Pantologist Posted at: 2016-04-23T21:48:31.618Z Reads: 100

```
Isn't the anti-spark switch/loop key supposed to go on the positive side?
```

---
## \#5 Posted by: Maxid Posted at: 2016-04-23T21:55:26.728Z Reads: 98

```
The problem of putting an on/off switch in the battery cable lines is the amperage it needs to be able to handle. The current is travelling directly through the switch so you can not just use any switch - you'd need a switch specifically able to handle the current.
Your XT90 is capable of doing that as it is not really a switch but just a connecting cable thick enough for the current to go through without a problem.
An anti spark switch has its actual switch not in direct contact with the high current cables.
```

---
## \#6 Posted by: Bender Posted at: 2016-04-23T22:39:41.337Z Reads: 88

```
The Switch being a weak link makes a lot of sense, so I think I'll just keep the loop key for now.

I read this this morning so that's why I thought it should go on the negative side

DeathCookies:
Which one is preferred? And why? positive or negative?

laurnts:
I prefer negative side, because thats were the electrons (the current) is flowing from. Also BMS'es seems to alternate the negative side for either charging or power switching, so I believe negative side is better.

[link to disscution here](http://www.electric-skateboard.builders/t/xt90-s-loop-key-short-circuit/2383/12?u=bender)
```

---
## \#7 Posted by: Bender Posted at: 2016-04-23T22:42:14.636Z Reads: 83

```
So how does the rest of the layout look, going from Parallel to serial, everything look ok?
I don't want anything bursting into flames :open_mouth:
```

---
## \#8 Posted by: lox897 Posted at: 2016-04-23T22:42:21.049Z Reads: 83

```
Looks good to me. Hope everything works out.
```

---
## \#9 Posted by: Krudte Posted at: 2016-04-24T01:23:02.937Z Reads: 87

```
Most look good but the way I read your schematic, it looks like you are actually shorting out your batteries, when you are connecting your batteries in series. See the example below (Just disregard the values). Now I'm no expert in electronics (yet) so let others confirm :) otherwise good luck with the build! make sure to make a build thread! :D
<img src="/uploads/db1493/original/2X/1/130590ba297016989009d96ea9829eaa08d2fdb3.png" width="690" height="363">

Or like this:

<img src="/uploads/db1493/original/2X/b/b672839dbffa59ee40eea101c640adfe9b78602f.jpg" width="221" height="500">
```

---
## \#10 Posted by: Bender Posted at: 2016-04-24T01:53:24.161Z Reads: 81

```
@ Krudte

Yep, I believe your right
Nice catch!
Thank you very much!

Plus your edit of my diagram looks great and extremely helpful, cheers!
```

---
## \#11 Posted by: trbt555 Posted at: 2016-04-24T06:39:30.417Z Reads: 75

```
It does't matter where you put the loop key.
```

---
## \#12 Posted by: DeathCookies Posted at: 2016-04-25T06:38:14.640Z Reads: 67

```
[quote="trbt555, post:11, topic:2541, full:true"]
It does't matter where you put the loop key.
[/quote]

Just keep in mind that it is not "polarity safe". You need to plug it in correctly otherwise you will short the key like i did!
[Shorten XT90-S loop key](http://www.electric-skateboard.builders/t/xt90-s-loop-key-short-circuit/2383/28)
```

---
