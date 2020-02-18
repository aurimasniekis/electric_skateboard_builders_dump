# Adding Qi Charging to my GT2B Mod

### Replies: 25 Views: 2776

## \#1 Posted by: mason Posted at: 2016-06-14T06:03:10.567Z Reads: 261

```
So I have this Qi Reciever for my phone that I don't use very often, and I just realized that I can possibly use this to charge my kickass gt2b mod. Pics:
<img src="/uploads/db1493/original/2X/c/c11c413ca04efdd0a5fdce91ecee188d521f35b3.jpg" width="281" height="500">
Here is a close up of the connection terminals:
<img src="/uploads/db1493/original/2X/6/64e862bcf300602f680ace8125c935b10ef656d7.jpg" width="281" height="500">
Theoretically, if I just soldered the ground and +5v connections to the small lipo in the controller (in parallel) it should be able to charge, correct? I don't wanna screw up. (also I'm doing this because I uber screwed up the usb charging port and have no way of charging atm) :slight_smile:
```

---
## \#2 Posted by: mason Posted at: 2016-06-14T06:16:28.666Z Reads: 252

```
Oh yeah I should mention the enclosure is the madmunkey v1 from @FLATLINEcustoms
```

---
## \#3 Posted by: Maxid Posted at: 2016-06-14T06:26:10.409Z Reads: 248

```
awesome idea and I think it can work.
I want that munkey so bad!
```

---
## \#4 Posted by: seanpain4 Posted at: 2016-06-14T06:29:28.674Z Reads: 246

```
Don't solder it straight to the lipo inside. It needs to go into a charging circuit then to the battery. So you need to solder the positive and negative to the positive and negative of the USB input in parallel.
```

---
## \#5 Posted by: mason Posted at: 2016-06-14T14:38:31.302Z Reads: 215

```
there is a tiny BMS attached to the battery, would I be finde soldering to it?
```

---
## \#6 Posted by: Maxid Posted at: 2016-06-14T14:44:54.256Z Reads: 210

```
just do it like @seanpain4 suggested. Parallel to the incoming USB wires and you are all set.
```

---
## \#7 Posted by: FLATLINEcustoms Posted at: 2016-06-14T14:55:17.364Z Reads: 202

```
@link5505 this is so awesome! Hope it works for you! 

@Maxid did you see the MadMunkey thread yet?
```

---
## \#8 Posted by: Maxid Posted at: 2016-06-14T14:55:52.681Z Reads: 197

```
[quote="FLATLINEcustoms, post:7, topic:4665, full:true"]
@Maxid did you see the MadMunkey thread yet?
[/quote]

Already downloaded and sent to print :slight_smile:
```

---
## \#9 Posted by: mason Posted at: 2016-06-15T01:31:17.192Z Reads: 177

```
Aw sweet! It works! <img src="/uploads/db1493/original/2X/7/77d13add77ab286ae18e0f57ab123ce30ffa3599.jpg" width="281" height="500">
```

---
## \#10 Posted by: FLATLINEcustoms Posted at: 2016-06-15T13:39:32.221Z Reads: 166

```
Nice work Mason!
```

---
## \#11 Posted by: clpjan Posted at: 2016-06-15T16:50:08.746Z Reads: 158

```
now add qi charging to your board!
```

---
## \#12 Posted by: mason Posted at: 2016-06-15T18:07:07.896Z Reads: 152

```
too inefficient to work :/
```

---
## \#13 Posted by: sl33py Posted at: 2016-06-15T18:25:34.269Z Reads: 152

```
great idea!  This coupled with the battery LED monitor would be great to check battery status at a glance and easily charge it.  I'm a huge fan of QI chargers (on several of my phones and tablets).

Nice work!!
```

---
## \#14 Posted by: mason Posted at: 2016-06-15T19:14:23.863Z Reads: 150

```
I got [this](http://m.ebay.com/itm/282030494790?_mwBanner=1) coming in the mail, I have a small cutout for the LEDS in the front side so it should be nice and easy :slight_smile:
```

---
## \#15 Posted by: sl33py Posted at: 2016-06-15T20:35:19.751Z Reads: 146

```
exactly.  only sucky part is $5 shipping for a 2.50 item.
```

---
## \#16 Posted by: mason Posted at: 2016-06-15T21:42:56.996Z Reads: 148

```
yeah but oh well :/
```

---
## \#17 Posted by: mason Posted at: 2016-07-27T05:34:58.229Z Reads: 125

```
ok so none of this really works after all. The 4 LED battery indicator didn't work from the get go, and I've had this controller on the charging pad for a week now and it still isn't fully charged. In fact, I think it just died! Whenever I put the controller on the pad I get LEDs on to indicate that I am charging, but whenever I take it off, it won't turn on. I have the controller super glued together, so taking this apart will not be fun.

Any suggestions? I have microusb connectors lying around somewhere, but I'm not 100% sure where the positive and negative pins are.
```

---
## \#18 Posted by: Pantologist Posted at: 2016-07-27T05:56:02.120Z Reads: 127

```
If you have one connected, can't you use a multimeter to find the +/- pins? Maybe desolder it first.
```

---
## \#19 Posted by: Maxid Posted at: 2016-07-27T06:40:58.551Z Reads: 125

```
quick google search:
http://pinouts.ru/visual/micro_usb.jpg

You are sure that selling high-energy custom batteries is a good idea? :wink:
```

---
## \#20 Posted by: quanze Posted at: 2016-07-27T07:38:23.607Z Reads: 119

```
This guy is a savage :joy:
```

---
## \#21 Posted by: mason Posted at: 2016-07-27T14:36:50.683Z Reads: 101

```
Thanks, every time I looked or asked friends I got conflicting results.
```

---
## \#22 Posted by: Cptanpanic Posted at: 2016-09-07T15:45:13.541Z Reads: 80

```
Ever get this working?
```

---
## \#23 Posted by: mason Posted at: 2016-09-07T18:01:37.628Z Reads: 73

```
I've abandoned it all together.
```

---
## \#24 Posted by: Pantologist Posted at: 2016-09-07T18:45:11.107Z Reads: 70

```
Looking at the Winning remote, it looks pretty simple.

 <img src="/uploads/db1493/original/3X/1/f/1fb0e1f30143684c343b0ac9876edc8348437a34.png" width="351" height="500">

A positive and negative trace. That's it.
```

---
## \#25 Posted by: mason Posted at: 2016-09-07T19:13:18.028Z Reads: 65

```
Go for it!
```

---
