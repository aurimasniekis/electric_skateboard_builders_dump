# Damaged BMS/E-Switch?

### Replies: 15 Views: 761

## \#1 Posted by: Gynpe Posted at: 2018-01-13T01:38:38.269Z Reads: 94

```
Hello builders,

Before the year ended I wet my system, and one of the BMS's seemed to stop working.

Over the holidays I took it to my parents home, and wired it just because I was bored. I did a few runs, and everything seemed on check.

I've gotten back home, and tried the build again to notice that it doesn't work anymore. It is strange because I get voltage from the battery, but when I turn on the E-Switch sometimes (most of the time) it doesn't turn on. 

I know this because I get 40.5V when its off and get like 41.2 or something like that when it turns on.

I think the E-Switch might be the problem. Is there anyway to find out exactly what it is, and how to fix it?

BTW, its a HCX-D223V1 10s BMS from Bestech Power

Thanks!
```

---
## \#2 Posted by: scepterr Posted at: 2018-01-13T01:40:28.236Z Reads: 90

```
It will show a voltage when off with no load, replace the eswitch
```

---
## \#3 Posted by: Namasaki Posted at: 2018-01-13T01:40:59.330Z Reads: 88

```
it is normal to see voltage when the bms is off if you dont have a load connected to the output
```

---
## \#4 Posted by: Gynpe Posted at: 2018-01-13T01:46:54.838Z Reads: 78

```
Yes, I know!

The thing is if I connect the focbox, sometimes it turns on and most times it does not, and when it turns on if I apply throttle the focbox goes off again.
```

---
## \#5 Posted by: scepterr Posted at: 2018-01-13T02:02:46.246Z Reads: 72

```
Yeah so replace the eswitch to try to fix that particular issue, replace the wires too they've been known to be faulty, the first thing is not an issue
```

---
## \#6 Posted by: Gynpe Posted at: 2018-01-13T02:07:34.253Z Reads: 66

```
Right... But there is no particular switch on right now, I just join the cables together to make contact. Sorry I didn't make this clear earlier.

I am refering to the BMS's actual switch...
```

---
## \#7 Posted by: scepterr Posted at: 2018-01-13T02:15:14.772Z Reads: 62

```
Lol yeah that's something you should specify 
Try replacing the wires either way
```

---
## \#8 Posted by: Gynpe Posted at: 2018-01-13T02:58:08.288Z Reads: 61

```
Sometimes I don't even understand what I'm trying to say :laughing:

Anyway, on board switch seems to be fine, I used a voltimeter between the fuse and the switch and that field is working properly.

I also unscrewed the board to check for burn marks or anything out of place, but I can't find anything.

If you guys don't have other suggestions, I might just hang this on my workshop as "First cooked BMS" maybe show it to my kids and grankids one day... Who knows...

Thanks for the help and patience!
```

---
## \#9 Posted by: scepterr Posted at: 2018-01-13T03:03:41.606Z Reads: 53

```
Yes replace the physical wires you are using as a switch
```

---
## \#10 Posted by: Gynpe Posted at: 2018-01-17T20:58:42.842Z Reads: 46

```
Hello again guys,

Hmm... I'm loosing my mind over this. I just spend quite a while soldering cables back together to fit in my new enclosure, and also the new 10s BMS, everything was going great when I decided I was going to solder in the charge port and charge it and continue tomorrow... When all of the sudden, out of no where the damn FOCBOX turns on... By itself. 

Thinking I had turned on the switch myself, I look for it, but no its off.

So I unplug the focbox from the power source (battery with bms) . Next I unsolder EVERYTHING again, and leave the battery leads going into the BMS, the negative wire from my battery pack to the -P (port whatever its called) and -B as output for the focbox.

So now without the switch even connected, I connect the power source to the focbox and still turns on by itself.

So I don't know what the fuck is going on, and its quite annoying.

One bms does not turn on, and the other is on at all times. 

The only weird thing I've done is attatch a velcro piece to the back of the BMS so it will stick to my board.. I don't know if stickers mess with the circuit which I doubt, and also there is a sticker there already. But I just don't know what else to think.

Been talking to Lucy, and I'm going to write to her again.

Some help would be highly appreciated guys.
```

---
## \#11 Posted by: Martinsp Posted at: 2018-01-17T21:20:02.258Z Reads: 39

```
I have not used the BMS but doesnt -B indicate negative battery side?
```

---
## \#12 Posted by: scepterr Posted at: 2018-01-17T21:23:28.442Z Reads: 38

```
Yeah b- is main battery negative, p- is discharge negative
```

---
## \#13 Posted by: Acido Posted at: 2018-01-17T21:28:29.627Z Reads: 36

```
You fried the switch probably i did the a simmilar thing few days ago connected charger minus to 10th balance lead and now its stuck on on state
Donna said its probably some pulse regulator thing
```

---
## \#14 Posted by: Gynpe Posted at: 2018-01-17T22:26:20.177Z Reads: 31

```
![20180117_231643|690x388](upload://5M6wX1GstkS0dgwdu7XRkTQrAKK.jpg)

OK, that's what I have. And yes negative battery main is on B-. I have trouble explainin these things.

The battery leads are currently unplugged, and so is the charge port, those are the two circles I made.

I'be hooked up the bms several times before, I always use Namasakis blueprint he made, always on my desk when soldering. 

I'm pretty sure I haven't done anything wrong.
```

---
## \#15 Posted by: Gynpe Posted at: 2018-01-20T03:53:55.930Z Reads: 27

```
Just for info, I unsoldered everything... Resoldered everything... And... It works?

So... yeah... I don't know what the hell happened. The battery is being charged as I speak.
```

---
