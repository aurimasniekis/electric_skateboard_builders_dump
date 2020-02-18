# 10s3p Electronics Wiring Help

### Replies: 11 Views: 1115

## \#1 Posted by: Preston Posted at: 2017-11-20T20:48:24.129Z Reads: 119

```
I've never used a BMS on any of my electric skateboard builds, so I have no idea how to set it up with a battery meter, charging port, and switch. 

My BMS ( http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html ):
<img src="/uploads/db1493/original/3X/0/c/0c95f23943d28909bbbc07ba5b113aecb3393bf8.jpg" width="300" height="239">

 How do I wire this to my batteries? And add a voltage meter, charging port, switch.

Thanks,
     Preston
```

---
## \#2 Posted by: themegak Posted at: 2017-11-20T21:15:22.235Z Reads: 110

```
Check this forum post.  Tons of diagrams.

http://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179/6?u=themegak
```

---
## \#3 Posted by: Preston Posted at: 2017-11-21T00:18:21.437Z Reads: 96

```
Thank you so much!
```

---
## \#4 Posted by: Namasaki Posted at: 2017-11-21T00:50:07.836Z Reads: 96

```
Your gonna need to buy an external E-switch.
Or make an anti-spark loop key.
That bms does not have any type of switch capability.
```

---
## \#5 Posted by: Preston Posted at: 2017-11-22T06:49:57.233Z Reads: 83

```
Yeah, I was thinking about using something like this: https://miamielectricboards.com/shop-1/120amp-12s-power-switch 

I know Miami and DIY sell these eswitches but is there anywhere I could find a better deal @Namasaki ?
```

---
## \#6 Posted by: Namasaki Posted at: 2017-11-22T12:27:57.400Z Reads: 68

```
I haven't heard of an E-switch yet that's is dependable except for the one that is built in on the Bestech bms.
```

---
## \#7 Posted by: Preston Posted at: 2017-11-22T20:23:33.743Z Reads: 62

```
@michaelcpg  Why is there a fuse leading from the positive terminal of the battery pack to the XT60 connector?
```

---
## \#8 Posted by: themegak Posted at: 2017-11-22T20:26:54.796Z Reads: 58

```
This is how the space cell was designed, and you should use a fuse in your battery design.

Also i linked michalecpg design as just an example.  Make sure to use some kind of fuse switch or fuse design in your battery set up.
```

---
## \#9 Posted by: BoostedBuilder Posted at: 2017-11-22T20:41:33.179Z Reads: 56

```
[quote="Preston, post:5, topic:38850"]
is there anywhere I could find a better deal
[/quote]
http://www.antisparkheaven.com/product/directfet-antispark-3-way-6s-12s-plug-n-play 
it's not cheaper but worth it! hopefully it will be back in stock soon!
```

---
## \#10 Posted by: michaelcpg Posted at: 2017-11-22T21:00:37.769Z Reads: 50

```
I would have to disagree. 

Not having at least a main fuse in your circuit is just lazy design. With batteries the size we use, safety should be a top priority and although a fuse in this position won't protect the battery from all situations, it still helps.

Ideally, if you're building your own battery, you should be fusing each cell separately. 
There's already been several instances of people's boards going up in flames on these forums from various types of short circuits etc, even when using the standard design that the space cell uses. Something that I don't use anymore
```

---
## \#11 Posted by: themegak Posted at: 2017-11-22T21:06:07.697Z Reads: 45

```
Yes you are correct, it is wise to use one.  I am mistaken.  Some antispark switches have fuses integrated or have options to do so as well.  We should be using fuses.
```

---
