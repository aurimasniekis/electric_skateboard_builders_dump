# VESC 4.12 layout

### Replies: 9 Views: 2539

## \#1 Posted by: mt37 Posted at: 2017-03-04T22:54:26.978Z Reads: 216

```
My VESC came wrapped and couldn't figure the wiring, and there were only old layouts online.

Here is the back screen of the VESC 4.12 exported from kicad.

You have to be careful since the plug is on the other side of that normally.

<img src="/uploads/db1493/original/3X/3/3/33424e027a8668be5df162a292a219df793bb016.png" width="363" height="499">
```

---
## \#2 Posted by: rpn314 Posted at: 2017-03-05T19:25:58.499Z Reads: 165

```
....sorry if I misunderstood something, but what are you asking exactly?
```

---
## \#3 Posted by: mt37 Posted at: 2017-03-05T19:27:34.120Z Reads: 162

```
Not asking anything, it was "hard work" to find the latest layout as a picture. So I thought I'd post as material for others (and also google indexing).

Edit: only one I could find is this seriously outdated one [1], and there is png export of the layout on vedder's github.

[1] http://vedder.se/2015/01/vesc-open-source-esc/
```

---
## \#4 Posted by: SeanHacker Posted at: 2017-03-05T19:51:56.463Z Reads: 144

```
I found these within a few seconds of a google search. They were in PDF form but they might help someone. Not sure if they are the same as yours though. 

<img src="/uploads/db1493/original/3X/a/0/a03adb0f87c098087af55787a90a16dd78b74d82.png" width="351" height="500">

<img src="/uploads/db1493/original/3X/b/9/b92e767bbfcced88f707c053b513f02a61732a45.png" width="351" height="499">
```

---
## \#5 Posted by: mt37 Posted at: 2017-03-05T19:53:35.272Z Reads: 121

```
looks similiar, mine is an export from the github kicad files so it's definitely what's on the 4.12 board. (I couldn't see because of the shrink wrap).

may I ask what you searched for ? Could only find old layouts.
```

---
## \#6 Posted by: SeanHacker Posted at: 2017-03-05T20:51:45.812Z Reads: 114

```
No problem. 

I google searched "VESC 4.12 kicad"

which brought me to this...

http://vedder.se/forums/viewtopic.php?t=572

which i obtained this...

https://cloud.itsi.li/s/qYKVNHHwwHyvEnT

All took a matter of seconds. Hope this helped.
```

---
## \#7 Posted by: JTAG Posted at: 2017-03-05T21:05:35.454Z Reads: 109

```
Or you could have looked here:
https://github.com/vedderb/bldc-hardware

https://github.com/vedderb/bldc-hardware/tree/master/design/PNGs

edit: my apologies, you are right. old pictures removed.

:stuck_out_tongue:
```

---
## \#8 Posted by: mt37 Posted at: 2017-03-05T21:07:14.925Z Reads: 101

```
@JTAG this layout is clearly not up to date. Latest UART connector has 7 pins not 6

Edit: I spent a fair amount of time trying to find the right one out of the exported svg / pngs in github. Will open a ticket for Vedder to hopefully have it kept up to date.
Edit2: Ah! Can't open Issues on Vedder's github.
```

---
## \#9 Posted by: mt37 Posted at: 2017-03-06T00:38:16.066Z Reads: 77

```
Actually my VESC 4.12 from Miami boards seems to differ a little from vedder's design.
```

---
