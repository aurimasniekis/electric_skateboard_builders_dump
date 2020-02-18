# Just a (simple?) question about regenerative braking

### Replies: 7 Views: 425

## \#1 Posted by: Alex.Scheff Posted at: 2018-03-31T08:07:03.089Z Reads: 117

```
Nearly everybody uses a charge only bms, me too. But If we bypass the bms while regerative braking would we damage the liion cells?
Maybe a dumb question but I really dont know.
Thanks

Alex
```

---
## \#2 Posted by: Martinsp Posted at: 2018-03-31T08:17:06.790Z Reads: 117

```
You are not charging the battery during braking for long enough to do any harm IMO
```

---
## \#3 Posted by: Sebike Posted at: 2018-03-31T08:20:32.735Z Reads: 113

```
You limit the current going back to the battery in the VESC, so if you want to be conservative with your regen charging currents (even though cells will typically be charged only for very limited periods of time) that's where you adjust settings.
```

---
## \#4 Posted by: Alex.Scheff Posted at: 2018-03-31T08:23:19.496Z Reads: 106

```
Okay thanks, which vesc do you have and what settings?
```

---
## \#5 Posted by: Sebike Posted at: 2018-03-31T08:31:34.166Z Reads: 98

```
I'm using FocBoxes, but this setting is the same for all VESCs (not all ESCs though, but maybe you knew that)

Batt Min - which is set to a negative value, -8 to -12 are conservative settings for a single motor system. Some people set this down to -16 or -20.

If you want to go strict within recommended charging limits you have to look at the specs for the cell you are using and adjust settings according to that, but as mentioned before, cells will probably not take significant harm if charging a bit above recommended current.
```

---
## \#6 Posted by: Alex.Scheff Posted at: 2018-03-31T15:34:45.326Z Reads: 68

```
Okay thank you!
```

---
## \#7 Posted by: Namasaki Posted at: 2018-03-31T20:11:53.740Z Reads: 41

```
[quote="Martinsp, post:2, topic:50759, full:true"]
You are not charging the battery during braking for long enough to do any harm IMO
[/quote]

Unless you are riding the brakes down a long steep hill with a full battery. 
In such a situation you could easily be over charging your cells.
```

---
