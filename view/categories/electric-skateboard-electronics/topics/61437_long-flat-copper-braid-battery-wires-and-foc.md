# Long flat copper braid battery wires and FOC

### Replies: 11 Views: 492

## \#1 Posted by: bobbobman Posted at: 2018-07-10T08:46:45.248Z Reads: 199

```
I'm building a bit of Boosted clone type board on which I'm planning to use a split enclosure design connected by 15mm flat copper wires ran over the top of the board. I got myself a pair of FOCBOXES to run the setup. 

Thing is, I've been reading some posts saying thay FOC doesn't like long wires and that in order to use wires longer than 20cm, I have to add capacitors to deal with the inductance. However, I've also read other posts saying that flat wires have lower inductance than round ones so it's not going to be a problem. And, on top of a that, I've scoured all the builds on this forum that are similar to mine and I can't seem to find any reference of anything adding capacitors to their VESC. So what's the conclusion here? Do I need to add capacitors? And if I do, how do I even go about doing that? Where would I even solder them to?
```

---
## \#2 Posted by: xilw3r Posted at: 2018-07-10T08:59:21.329Z Reads: 190

```
Just add the caps.

The "flat wire has lower inductance" argument does not make much sense. The only way it can have lower inductance is because of the shorter possible center to center distance between the positive and negative wire. Y'know, because the positive and negative wires have magnetic fields that cancel each other out.

Anyway, just add the caps. Most people do not need to do this because most vescs i see these days come with caps preinstalled.

Get some low ESR capacitors, 63V is usually recommended, unless you are running above 12s... like 3 units of 1000 microfarads should be cool.

Hell, I have 3x 1200 microfarads and my vesc is literally on the side of the battery. Well, can't hurt, so why not.
```

---
## \#3 Posted by: BooYA Posted at: 2018-07-10T10:20:49.772Z Reads: 163

```
Honestly since you will use a pair à focboxes, it's already a lot of capa ( 4 caps total) so it should be fine but yeah better be sure and add 2 x1000.
Also keep these cables close to each other!
```

---
## \#4 Posted by: xilw3r Posted at: 2018-07-10T11:02:55.392Z Reads: 154

```
I honestly just skipped the part where he says he has focboxes :D If they have good capacity, perhaps he does not need extra caps after all? I mean he will have only 15 cm of wire between the battery and vesc, not too critical.

edit: no never mind, im illiterate. 15mm wire, not 15cm of length...
@bobbobman how long will your wires be between battery and vesc?
```

---
## \#5 Posted by: E1Allen Posted at: 2018-07-10T13:33:21.306Z Reads: 122

```
Four feet of wire between battery and focbox didn't matter.  I doubt you will go past that.  Only the length between motor and ESC shouldn't be long.
```

---
## \#6 Posted by: Battosaii Posted at: 2018-07-10T13:41:52.232Z Reads: 111

```
Good to know thanks
```

---
## \#7 Posted by: bobbobman Posted at: 2018-07-10T16:30:05.727Z Reads: 93

```
I haven't gotten it completely laid out yet but it's looking like about 15 inches, give or take one or two. Where would I add the caps? Would I have to open the FOCBOX case and basically just solder some extra capacitors on top of the existing ones?
```

---
## \#8 Posted by: bobbobman Posted at: 2018-07-10T16:34:22.405Z Reads: 95

```
Dang 4 feet? How long have you been running that setup?
```

---
## \#9 Posted by: deucesdown Posted at: 2018-07-10T16:51:42.815Z Reads: 91

```
I've consistently read the opposite... (phase wire length is not critical but battery wire length is)
```

---
## \#10 Posted by: xilw3r Posted at: 2018-07-10T16:54:24.477Z Reads: 90

```
Everyone says the opposite... That phase wires between esc and motor can be long. And it kind of agrees with physics.

Care to elaborate why you say they shouldnt?
```

---
## \#11 Posted by: mmaner Posted at: 2018-07-10T16:55:48.354Z Reads: 92

```
If you phase wires are too long you can suffer from de-synch.  If the battery wires are too long they can get hot and resistance is increase.  The trick is figuring how how long 'too long is'.  If you dont go over 10in you should be fine on either.
```

---
