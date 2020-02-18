# More WH than should be possible

### Replies: 11 Views: 348

## \#1 Posted by: hoeksame1 Posted at: 2018-09-28T07:01:25.015Z Reads: 164

```
I dont understand.. 
It was windy.. 
I only tot 24km range. But i dont understand one thing.. my battery is 10sp4 made from Samsung 30q. The ah is 12 ah 36v.  Total wh is 432. 
Please take a look at the ride.. 
![Screenshot_20180927-160915_metr|281x500](upload://ua44MkcemTSF1df2nJxYEPyh6CV.jpeg) 
Is something wrong or?? More WH than my battery can deliver.. 
More weird is.  I started at 90% and ended at 21%.. 
So i could have ride even more but. How !?

I would love to understand it.

Gr sam
```

---
## \#2 Posted by: Colson003 Posted at: 2018-09-28T07:33:43.796Z Reads: 143

```
Regenerative breaking
```

---
## \#3 Posted by: hoeksame1 Posted at: 2018-09-28T07:35:04.484Z Reads: 144

```
But 100wh regen? Is that possible ?!
```

---
## \#5 Posted by: Sebike Posted at: 2018-09-28T09:24:05.363Z Reads: 128

```
But the Wh (432) is based on the capacity from full charge to ~2,5v/cell, so any higher cutoff means lower Wh.
```

---
## \#6 Posted by: Andy87 Posted at: 2018-09-28T09:30:51.385Z Reads: 126

```
:thinking:
that´s right...
than he has an flux generator inside i guess...
```

---
## \#7 Posted by: Benjamin899 Posted at: 2018-09-28T09:44:13.963Z Reads: 117

```
432 is based on nominal WH.
```

---
## \#8 Posted by: Blix Posted at: 2018-09-28T22:09:04.516Z Reads: 85

```
Which Vesc/Esc do you have and how much do you weigh?
Some more info about the setup would help but I am not sure...
@rpasichnyk could help maybe...
```

---
## \#9 Posted by: hoeksame1 Posted at: 2018-09-28T22:17:09.820Z Reads: 81

```
I run dual focbox 
Dual sk3 192kv 6374 motors. 
My weight is 78kg..
```

---
## \#10 Posted by: strattos Posted at: 2018-09-28T22:46:59.212Z Reads: 82

```
I've had this same glitch before it's only happened once where I got absolutely crazy readings. I swear I've seen other ppl talking about this glitch before with metr.
```

---
## \#11 Posted by: Adam0311 Posted at: 2018-09-28T23:39:29.467Z Reads: 76

```
I’ve had this happen as well. I have a 10s3p battery.
![image|281x499](upload://1kmWduvfHZ5hPnLDaj4F2RvXU4L.jpeg)
```

---
## \#12 Posted by: rpasichnyk Posted at: 2018-09-29T07:30:21.863Z Reads: 54

```
@hoeksame1 @Adam0311 there was a bug in Metr Pro firmware, which resulted in wrong Wh calculation sometimes. Please update Metr Pro firmware via Metr app. Click on blue gear in Settings.
```

---
