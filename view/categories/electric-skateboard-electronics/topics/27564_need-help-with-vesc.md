# Need help with vesc

### Replies: 4 Views: 350

## \#1 Posted by: Decdog Posted at: 2017-07-13T23:19:13.003Z Reads: 47

```
Hello- 
I finished my board today with these specs:
sk3 6364 245kv
6s lipo 25c
vest
90mm wheels
36/16 gearing
mini remote

I took I out and when I went, I only got to 5mph. The vest doesnt say any errors. The motor doesnt seem to spin very fast at all or have any torque.

Here are my settings:
<img src="/uploads/db1493/original/3X/f/e/fee225930a0f7aed31d589e5174a85881524a413.png" width="690" height="388"><img src="/uploads/db1493/original/3X/2/9/295a204b821436914f00e31f9d0ce9ccb1d7fc75.png" width="690" height="388"><img src="/uploads/db1493/original/3X/b/5/b501e81825f25363497fec13c79fa9fd5d0057c3.png" width="690" height="388"><img src="/uploads/db1493/original/3X/1/b/1b45f9176f14c9fca1cc097d137b3f68a4f8f970.png" width="690" height="388"><img src="/uploads/db1493/original/3X/8/c/8c5c2e1a9c63032eb80663975be372a4f4806cd1.png" width="690" height="388">
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-13T23:33:04.679Z Reads: 34

```
Your cutoff is triggering, you need to lower battery cutoff start/end. I would use 23 start 21 end.
```

---
## \#3 Posted by: Jinra Posted at: 2017-07-13T23:34:23.435Z Reads: 36

```
It also doesn't look you did detection and apply it, make sure you do that as well.
```

---
## \#4 Posted by: Decdog Posted at: 2017-07-13T23:54:17.912Z Reads: 35

```
@Jinra is a legend!!
```

---
