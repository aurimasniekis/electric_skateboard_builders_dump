# BMS Voltage Output Question?

### Replies: 17 Views: 1475

## \#1 Posted by: darkkevind Posted at: 2018-01-08T16:32:16.515Z Reads: 102

```
I've got a little issue that has be stumped :frowning: I think I have a DOA BMS but need to sense check with everyone to make sure that's the case please?

It's a 10s3p pack and I have a 10s BMS attached to it. I've checked the balance wire configuration 4 times now and I just think it's a dud! :frowning:

At the battery terminals I'm getting 34.8v but out of the BMS I'm getting exactly half that! 17.4v!!!??

Any ideas anyone? :confused:
```

---
## \#2 Posted by: pjotr47 Posted at: 2018-01-08T18:24:23.957Z Reads: 90

```
Does it have a e-switch? Try to put the charge in the bms and measure the voltage.
```

---
## \#3 Posted by: Ishayc Posted at: 2018-01-09T13:56:34.393Z Reads: 77

```
What BMS is that?
Do you have a drawing of how you wired it?
```

---
## \#4 Posted by: darkkevind Posted at: 2018-01-09T14:12:16.269Z Reads: 75

```
This is the BMS.

<img src="/uploads/db1493/original/3X/8/e/8e94f565784a156e61cf82e06a94dfef36e5e0ef.jpg" width="690" height="388">
```

---
## \#5 Posted by: darkkevind Posted at: 2018-01-09T14:13:22.296Z Reads: 71

```
No e-switch

I'll try and get some charge to it but I don't have a DC jack at the moment so I'll have to improvise :confused:
```

---
## \#6 Posted by: Ishayc Posted at: 2018-01-09T14:39:35.869Z Reads: 68

```
Does not say much.
try showing how you wired it.
Have checked if between every two sequential balance wires you have ~3.48v and between the first wire and the third you have 2X3.48v and between the first and the 4th you have 3X3.48 and so?
```

---
## \#7 Posted by: darkkevind Posted at: 2018-01-09T14:53:46.414Z Reads: 66

```
It's wired exactly like this... ie. The number balance wire etc.

<img src="/uploads/db1493/original/3X/b/c/bc8c885dc6749f735805fc98347c6179f442f7d6.jpg" width="690" height="175">

I've checked each cell and they're all the same voltage, and they all go up in the right increments as I go down the line.

I'm getting the full voltage when slapping the meter on the main pack's + & - ends, but when the neg goes through the BMS it halves the voltage :confused:
```

---
## \#8 Posted by: Ishayc Posted at: 2018-01-09T15:16:29.258Z Reads: 62

```
Seems right.
I'm almost sure iv'e seen this issue before.
as I recall it was solved with a new BMS.
```

---
## \#9 Posted by: darkkevind Posted at: 2018-01-09T15:20:29.227Z Reads: 61

```
That's my thinking.. I think the BMS is kaput :frowning:
```

---
## \#10 Posted by: gogomrrobot Posted at: 2018-01-09T18:22:48.113Z Reads: 58

```
Isn't B1 balance lead supposed to be the output from positive side of pack #1? Your first wire on your diagram looks like the first balance wire is B0 or B-
```

---
## \#11 Posted by: darkkevind Posted at: 2018-01-09T18:44:13.486Z Reads: 62

```
The markings on the BMS are B- (black, the only black, B1 in the diagram) all the way down the line to B+, which in this diagram is B11.
```

---
## \#12 Posted by: gogomrrobot Posted at: 2018-01-09T18:55:06.868Z Reads: 61

```
Yeah so your BMS requires 11 wires to fill in the balance leads for your 10S battery pack?

That's usually not how bestech or supower BMS work. I don't know about yours.

See a bestech BMS wiring below...

The first balance wire B1 is attached to the positive/negative between packs #1 & #2
![10S4P diagram|690x388](upload://eagjTTFtQa5cXqQagyWajUU4yGK.)
```

---
## \#13 Posted by: darkkevind Posted at: 2018-01-09T21:39:14.827Z Reads: 58

```
This one seems different to that diagram...

This is the one I have. I actually forgot I was bypassing the BMS for discharge with this pack but I was still worried about the charging, until I found this diagram on the listing...

I was using P- whereas I should have been using C- !!!!

![image|500x500](upload://mLbZOlsKQQTD8tYBItlk6460fM6.jpg)
```

---
## \#14 Posted by: gogomrrobot Posted at: 2018-01-09T21:53:21.540Z Reads: 55

```
Ok you got a screwy wired BMS  -- I don't like BMS's that have that extra balance wire.

Now did you try and it maybe hard now but measure each progressive balance lead to see the voltage is increasing?  See above what @Ishayc that technique.
```

---
## \#15 Posted by: Ishayc Posted at: 2018-01-10T08:04:45.123Z Reads: 49

```
then everything is good now?
```

---
## \#16 Posted by: darkkevind Posted at: 2018-01-10T09:54:36.872Z Reads: 46

```
Yes, when I use C- instead of P- for the neg discharge, all is good :slight_smile:

Thanks for your help guys, I didn't realise it was a weird BMS :confused:
```

---
## \#17 Posted by: Ishayc Posted at: 2018-01-10T11:12:51.189Z Reads: 44

```
Have fun and ride safe
```

---
