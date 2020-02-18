# Board won&rsquo;t turn on \[Prebuilt\]

### Replies: 9 Views: 3393

## \#1 Posted by: PotatoHo Posted at: 2017-08-31T03:37:55.331Z Reads: 104

```
Hi, I am in real trouble here and I don't know what to do. I bought a board from china (GT-M6, aka the Halo Board) and rode like a dream for the past week. 

Today I went for a cruise and had to go on the sidewalk since there were no bike lanes and cars going fast on the street. Of course the expansion joints in the sidewalks make the board go *kadunk* *kadunk* *kadunk* and all of a sudden my board just stops. It doesn't turn on anymore no matter how long I wait or press the power button. No light or anything. Battery was freshly charged as well.

Was something detached from the constant bangs and vibrations of the sidewalk?

How can I pinpoint what is broken or needs to be fixed?
```

---
## \#2 Posted by: faithfulpuppy Posted at: 2017-08-31T03:41:14.415Z Reads: 101

```
im not an expert or anything but from your description it sounds like either the esc failed or the battery disconnected.  I guess open up the enclosure on it and see if the battery wires aren't plugged in/are broken.
```

---
## \#3 Posted by: PotatoHo Posted at: 2017-08-31T03:48:40.515Z Reads: 97

```
Hmm, is there a way to test it? The battery seems okay since I plug it in and shows that it charges, and whenever I disconnect/reconnect the battery to the motherboard i hear a tiny little crack (means power jolts though? idk)

I did find this little white cable but I think I remember them saying it was the signal cable to connect to the remote.

http://imgur.com/a/xiiJf
```

---
## \#4 Posted by: onepunchboard Posted at: 2017-08-31T05:07:52.018Z Reads: 79

```
sound like something shorted or cold solder joints. 
it could be bec unit is burned. happened to me before. I would upgrade to esc or vesc
```

---
## \#5 Posted by: PotatoHo Posted at: 2017-09-01T03:32:17.214Z Reads: 51

```
Hmm, I see. Is there a way to test parts individually to find out what the particular problem is?
```

---
## \#6 Posted by: onepunchboard Posted at: 2017-09-01T03:41:51.604Z Reads: 49

```
multimeter? if u know how to use it.
or thoroughly look for solder joints or short or burn mark
```

---
## \#7 Posted by: wafflejock Posted at: 2017-09-01T03:51:46.677Z Reads: 49

```
Appears to be a burn mark on the board where the red positive wire is coming in between there and the capacitor.  Hard to say what all is fried exactly without schematics or a multimeter and lots of time to look up data sheets and see what's what and what fried.  You can replace the ESC, what you're calling the motherboard is basically responsible for delivering power at a controlled rate from the battery to the motor based on the receiver input.  It appears they may have slapped together the receiver and the ESC and possibly BMS into a sandwich here, basically you can gut those parts and use the board/battery/motor assuming you can't find a way to fix them.

Given the price of the board I would say seal it up like you didn't touch anything and call support and ask them what to do, they should be able to guide you or replace the broken parts.  If you were just riding the board it's not your fault if something broke so would see if it's covered under warranty.  If you start ripping things apart it will certainly void your warranty.
```

---
## \#8 Posted by: boramiNYC Posted at: 2017-09-01T04:22:33.623Z Reads: 42

```
Just FYI, the ESC looks like the same one as this:
http://www.ebay.com/itm/Dual-motors-longboard-skateboard-control-modula-ESC-Substitute-with-remote/322688412411?_trkparms=aid%3D222007%26algo%3DSIM.MBE%26ao%3D1%26asc%3D46089%26meid%3Da83652835ed141ffa3a2f9756578944b%26pid%3D100011%26rk%3D2%26rkt%3D12%26sd%3D302332736118&_trksid=p2047675.c100011.m1850
```

---
## \#9 Posted by: PotatoHo Posted at: 2017-09-01T04:54:18.002Z Reads: 38

```
Oh cool, so essentially I can just pop out the current one and put that one in and it will work (if it was indeed a broken esc)? What if it's not exactly the same model or specs etc? It's also a different remote if that means anything.
```

---
