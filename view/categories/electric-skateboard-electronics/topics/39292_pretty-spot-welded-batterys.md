# Pretty spot welded battery&rsquo;s?

### Replies: 10 Views: 526

## \#1 Posted by: Sapphirinia Posted at: 2017-11-26T02:35:09.946Z Reads: 105

```
https://m.aliexpress.com/s/item/32814189809.html?spm=a2g0n.search-cache.0.0.2e3aa29b6tGUot#autostay

I'm not too good with this stuff but I thought it 2as kind of cool.
```

---
## \#2 Posted by: scepterr Posted at: 2017-11-26T03:14:46.511Z Reads: 96

```
They are individually tabbed...no use for us
```

---
## \#3 Posted by: Sapphirinia Posted at: 2017-11-26T03:29:39.651Z Reads: 82

```
Oh, I thought that meant you could just solder the tabs together.
```

---
## \#4 Posted by: scepterr Posted at: 2017-11-26T03:33:47.198Z Reads: 79

```
You could but I doubt they're pure nickel and you still need to connect in series,those tabs won't handle series connections.

Also I would never trust welds that look like this 
Horribly skinny too
<img src="/uploads/db1493/original/3X/f/9/f99ee1de4d565f36e07657a1120f8b1eaea19305.jpg" width="690" height="458">
Mine look like this
<img src="/uploads/db1493/original/3X/1/c/1c6e4d01d846c29dc8815b3c6c8f48a8dece4288.jpg" width="690" height="209">

@Sapphirinia if you bring me cells I'll spotweld them in whatever configuration you want while you wait (30-45min)
```

---
## \#5 Posted by: deucesdown Posted at: 2017-11-26T06:57:43.395Z Reads: 53

```
Hm I was gonna keep quiet but others might be curious.

Is that 10mm 0.2mm pure nickel, 2 layers? Is it enough to handle the current?
```

---
## \#6 Posted by: scepterr Posted at: 2017-11-26T07:11:39.368Z Reads: 50

```
On a 3P I find single layer more than enough, on 4+ I double up
Also I feel it makes a difference having the series nickel covering the length of both P, vs just nickel between the last and first cell

I'll be doing a write-up of the all the 30q packs I'm making after I'm done with them
```

---
## \#7 Posted by: deucesdown Posted at: 2017-11-26T07:22:05.354Z Reads: 44

```
This is so confusing, I'm trying to figure out how much conductor I want in my packs.

from https://endless-sphere.com/forums/viewtopic.php?t=68005

<img src="/uploads/db1493/original/3X/2/a/2ae87f47af6bb55cdae161a1a2724d9c135bb9e2.png" width="549" height="500">

Resistance is a function of volume, so cross section times length. .2mm * 10mm = 2mm^2. On the chart (being lazy), .3mm * 7mm is closest to 2mm^2, which is:
<10A optimal
~15A acceptable
>20A poor/hot

Your photo shows 1 series connection between parallel groups, so that connection carries the full amperage of the pack. I know I pull 60A out of my pack quite often, though only a few seconds at a time.

The table above also looks very conservative to me.

I feel like I need to build a proper DC load and test this for myself...
```

---
## \#8 Posted by: scepterr Posted at: 2017-11-26T07:24:38.573Z Reads: 37

```
That chart always looked very conservative to me lol
Simplest real-world way I've found to see if your series connection isnt enough is if you're getting more sag then expected under load, though not "scientific" you can spot it

Another thing that's always bugged me about that chart..what about length? Does that assume 1mm? As well as weld spots, 6 will carry better than 2
```

---
## \#9 Posted by: deucesdown Posted at: 2017-11-26T08:01:58.482Z Reads: 29

```
I have a FLIR so I can get approximate temps, but I don't have a way to generate the load in a controlled fashion...
```

---
## \#10 Posted by: scepterr Posted at: 2017-11-26T08:06:24.576Z Reads: 28

```
A 2000watt 36V to AC inverter would do the trick
```

---
