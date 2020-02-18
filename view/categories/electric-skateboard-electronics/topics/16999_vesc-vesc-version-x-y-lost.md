# Vesc (vesc version x,y)? lost

### Replies: 20 Views: 820

## \#1 Posted by: shwill Posted at: 2017-02-01T03:19:18.673Z Reads: 88

```
firmware which was originally 2.16 now says version x,y and firmware to old tried all firmwares available none seem to work or connect please help!
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2017-02-01T03:22:06.394Z Reads: 88

```
What vesc did you have? Latest version should be 2.18..

Edit: your bldc tool is too recent for the firmware on your vesc, so you need to update your vesc to the firmware 2.18
```

---
## \#3 Posted by: shwill Posted at: 2017-02-01T03:26:33.510Z Reads: 83

```
ive tried to upload and I get buffering erase timout
```

---
## \#4 Posted by: shwill Posted at: 2017-02-01T03:27:44.502Z Reads: 81

```
vesc hw 4.12 firmware was 2.16 old windows style
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2017-02-01T03:44:47.917Z Reads: 75

```
where did you get your bldc tool... also have you try to close everything and reopen them (just in case you've got communication problem with the bldc tool)
```

---
## \#6 Posted by: shwill Posted at: 2017-02-01T03:48:19.736Z Reads: 71

```
I have tried these options bldc tool came from vesc.au its a nightmere
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2017-02-01T03:52:16.114Z Reads: 68

```
Are you talking about this web site http://vesc.net.au/download-now/ ... If not maybe give it a try it should work.
```

---
## \#8 Posted by: shwill Posted at: 2017-02-01T04:04:03.479Z Reads: 63

```
did that but when trying to upload firmware it says erasing buffer timeout
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2017-02-01T04:11:20.951Z Reads: 63

```
where did you bought your vesc.... and have you've ever try to upgrade it before
```

---
## \#10 Posted by: shwill Posted at: 2017-02-01T04:18:14.931Z Reads: 60

```
Dave (pychotiller) I believe they came from ollin.ive never upgraded just programed with2.16 which I was helped with it was running in FOC awesome for about three months.
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2017-02-01T04:22:57.855Z Reads: 62

```
Maybe you can try using a old bldc version http://vesc.net.au/BLDC-TOOL/Windows/OLD%20Versions/ ... the 2.16 is still available
```

---
## \#12 Posted by: shwill Posted at: 2017-02-01T04:27:30.451Z Reads: 57

```
that's what I used originally and have tried again today but it just says firmware to old andvesc x,y
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2017-02-01T04:36:05.862Z Reads: 58

```
I think you might have a corrupt bootloader
```

---
## \#14 Posted by: shwill Posted at: 2017-02-01T05:10:37.875Z Reads: 56

```
that's what I was thinking but how do I fix that
```

---
## \#15 Posted by: shwill Posted at: 2017-02-01T05:11:43.904Z Reads: 56

```
thank you for your time and effort much appreciated my man
```

---
## \#16 Posted by: JohnnyMeduse Posted at: 2017-02-01T05:18:46.913Z Reads: 54

```
you need a StLink programmer 

there a procedure for it on vedder web site you can take a look at it, but it is for linux http://vedder.se
```

---
## \#17 Posted by: shwill Posted at: 2017-02-01T05:21:07.527Z Reads: 53

```
shitty I suck with Linux but thanks again
```

---
## \#18 Posted by: JohnnyMeduse Posted at: 2017-02-01T05:24:11.719Z Reads: 51

```
but does it still work on your board ?
```

---
## \#19 Posted by: shwill Posted at: 2017-02-01T08:40:26.426Z Reads: 44

```
correction both motors now work w/ different remote other one wasn't binding I guess but still don't know why I cant get bldc to read configuration
```

---
## \#20 Posted by: shwill Posted at: 2017-03-28T07:47:24.799Z Reads: 22

```
Just to put it out there the x,y thing was caused by the pc I was using not having proper drivers and updates things working as should be I happen to have now. thanks for your help Also Dave told me you were gonna be doing some drv fixing on vescs I happen to have two Id love to send you. Let me know where to send and what you need and ill make it happen thanks brotherman.
```

---
