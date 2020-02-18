# Is this 10s4p wiring ok?

### Replies: 6 Views: 337

## \#1 Posted by: chickengun Posted at: 2018-10-08T00:05:35.852Z Reads: 125

```
I was planning to 3d print a enclosure for the Jet Spud 29" deck and noticed I don't have a lot of room for the batteries... The Bestech HCX-D223V1 BMS and the two vesc's (EScape) I want to use take quite some space:

![Untitled|359x499](upload://gcHvxLOQmKG16ZLmjw5md5r9ykP.jpeg) 

I was planning to spot welder all 4p batteries using nickel plate strips (0.15 mm thickness and 10 mm width) and connecting all 4p batteries with each other in series using 10 awg wires. The problem is, I have to put 10 batteries in one row which means two batteries remain in the end that I will need to connect in a square formation as you can see here:

![Untitled2|690x488](upload://1ugQjwiTZ8TVpDY6UWLpT9Ap0W8.jpeg) 

In green you can see the nickel plate strip connection (4p) and in black/red the connections in series I was thinking of. I would rather have something symmetrical but this is the only way I can realize this configuration for the jet spud. The enclosure will probably have a depth of around 50 mm because of the batteries. 

Looking at the green square, is it ok to solder the 10 awg wire at any position on the nickel strip? For the 4 linear 4p connections I would solder the wire right in the middle but on the green squares it won't be symmetrical. Do you think this can be a problem?
```

---
## \#2 Posted by: baxtred Posted at: 2018-10-08T09:27:45.060Z Reads: 87

```
Do something like this. Sorry for the terrible picture. Basically make them all into 4 cluster parallel packs. The use nickel strips to create the series connections (shown in red). I will draw a better picture tomorrow if you don't understand. 

![Screenshot_20181008-032611_Autodesk%20SketchBook|243x500](upload://8w3EhMQ7VfI1CmP05wthn0YF16x.jpeg)
```

---
## \#3 Posted by: chickengun Posted at: 2018-10-08T18:15:15.068Z Reads: 67

```
I understand what you mean. If I do it this way where exactly should I solder the series wire? It will look a little bit unsymmetrical, is that ok for the discharge?

![Untitled|503x500](upload://gdBJzlzZRV4yXSfXbsjw3QlsXfD.jpeg) 


I was just wondering if it is better to have something symmetrical (solder spot in the middle, I ned to spot welder two more nickel strips for that):


![Untitled|365x500](upload://j3Qb1TvEqlmeDEtvopBDjc1ZnNZ.jpeg) 

What do you think?

![Untitled|574x500](upload://icPy32OxPrk6XK5rq4STdq1StAE.jpeg)

EDIT: It sucks a bit to solder the wires in series that are between both packs because it makes it fragile and I lose space. Maybe something like this:

![Untitled|488x218](upload://1CfORkNfUe4F9JGsbC7fCFo8qX2.jpeg) 

I could just weld 4 nickel strip layers to handle the current and then fold the pack (marked in orange)
```

---
## \#4 Posted by: baxtred Posted at: 2018-10-08T20:03:55.157Z Reads: 44

```
![jpg_350x350|350x350](upload://sVlDFcQQbzfG5lZOCYFz6AbSAWJ.jpeg)

Here a picture of how you could do the series connections. They still can be nickel strips. Soldering to nickel isn't always that easy. Using Flux helps but the wires get very stiff when solder wicks into them, so your 10 awg wires between packs can get very hard to manage.
```

---
## \#5 Posted by: chickengun Posted at: 2018-10-08T20:06:25.629Z Reads: 43

```
Thanks. I edited my last post. So basically do some nickel layers and then fold it.
```

---
## \#6 Posted by: baxtred Posted at: 2018-10-08T20:12:18.004Z Reads: 43

```
Folding doesn't work too well, too high of a risk in breaking a weld while doing it. I meant that you build the top pack using all nickel, then attach the top and bottom packs with wire. Putting wire between each parallel group in a dense pack will give you headaches. Here's mine but I have alot more room. 

![20180915_155650|375x500](upload://el4cDegKVqMyAv0RwqwXmdvpPP8.jpeg)

![20180927_022431|210x499](upload://fmmQUkXKhLAXMvnaH8Ovb2cubUV.jpeg)

![ad04bf0c-bf5a-4d07-8a12-0e15704ef130|243x500](upload://rN5Ewm4cCVgkmk2LEjvClQzSH9A.jpg)
```

---
