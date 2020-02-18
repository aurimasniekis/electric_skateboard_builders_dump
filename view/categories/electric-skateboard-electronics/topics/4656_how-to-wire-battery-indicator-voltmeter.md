# How to wire battery indicator/voltmeter

### Replies: 10 Views: 2497

## \#1 Posted by: jwu97 Posted at: 2016-06-14T01:12:39.056Z Reads: 327

```
I just want to make sure before i blow something up :joy:
Do I wire the voltmeter in parallel with the ESC like so?
<img src="/uploads/db1493/original/2X/a/aaf0302a457350fa9cc69967dd706e900935c428.JPG" width="375" height="500">
Will post more pic later as a build :)
```

---
## \#2 Posted by: barajabali Posted at: 2016-06-14T01:13:56.646Z Reads: 311

```
Yes! 

As long as your volt meter can handle the voltage some do some don't without extra parts
```

---
## \#3 Posted by: Russell23 Posted at: 2016-12-26T16:00:32.562Z Reads: 225

```
Sorry for opening up an old thread but when i tried to do this, it just sparks.(i soldered the battery indicator and the esc together to a 4mm banana jack)
```

---
## \#4 Posted by: mmaner Posted at: 2016-12-26T16:03:49.370Z Reads: 226

```
Its better to put the volt meter just after the battery pack, before everything else.  If you are using the typical [DROK DC8](https://www.amazon.com/dp/B00VUUKIMY?psc=1) volt meter, its really simple, just POS to POS, NEG to NEG.
```

---
## \#5 Posted by: DilatedPupils Posted at: 2016-12-27T14:44:48.639Z Reads: 208

```
You might need an anti spark switch. Or use xt90-S in place of the banana Jack
```

---
## \#6 Posted by: fraannk Posted at: 2016-12-27T15:15:52.008Z Reads: 200

```
I've always wondered how you set the voltmeters config. How does it know when 100% is 100%? Is there a button to set it for the specific voltage?
```

---
## \#7 Posted by: mmaner Posted at: 2016-12-27T15:27:50.572Z Reads: 186

```
On the Droks there is a button, or 2 buttons, on the back. You hold the bottom button down as you power it up and set the type and number of cells.  When you power it up normally it measures available voltage against peak capacity to define a percentage.  I, personally, like the meter that are settable to voltage instead of percentage.
```

---
## \#8 Posted by: Morxy49 Posted at: 2018-07-17T06:14:24.006Z Reads: 71

```
Sorry to bring up an old thread, but I'm really confused by this. If I connect the voltmeter directly to the battery with + to + and - to -, won't just *all* the current from the battery run straight into the voltmeter and blow it up? I highly doubt that this tiny little thing with 26 AWG wires can handle 54v 100A or whatever the battery puts out.

Please correct me since I'm probably wrong here, but I just don't get how this would work.
```

---
## \#9 Posted by: thisguyhere Posted at: 2018-07-17T06:19:00.369Z Reads: 71

```
it won't, the voltmeter has its own resistance and will only draw what it needs.
```

---
## \#10 Posted by: Morxy49 Posted at: 2018-07-17T06:22:43.517Z Reads: 67

```
Oh of course. You're absolutely right. :man_facepalming: Thanks.
```

---
