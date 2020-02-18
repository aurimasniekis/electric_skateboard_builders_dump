# Help with first time setup vesc: no led blinks on startup, no firmware read response

### Replies: 15 Views: 919

## \#1 Posted by: Khix Posted at: 2017-09-21T09:26:23.795Z Reads: 118

```
After putting together my first eboard build, when I tried connecting my vesc to the BLDC tool it says connected for about two seconds then it reads "no firmware read response". I've searched around the forum for people with similar problems and tried their solutions but nothing has worked for me so far. If it helps, when I turn it on (with anti-spark key) the vesc doesn't blink at all, but my voltmeter turns on and reads 0.0. 

Any help would be appreciated.


Don't have access to pics atm,

10s battery
battery support 10s 60a bms
Vesc is diy and was sold to me by @ekitesurfer  and was repaired by @JohnnyMeduse
```

---
## \#2 Posted by: krloz Posted at: 2017-09-21T09:46:21.118Z Reads: 113

```
Post your setup
```

---
## \#3 Posted by: krloz Posted at: 2017-09-21T10:32:46.225Z Reads: 107

```
Do you have a link to your voltmeter? If it is a 3 wire meter I think you have it wrongly wired.  If 2 wire I think its not working properly.  Anyway I think this has nothing to do with the vesc issue. Unless some kind of power mistake damaged both
```

---
## \#4 Posted by: krloz Posted at: 2017-09-21T10:34:45.414Z Reads: 99

```
[quote="Khix, post:1, topic:33637"]
when I tried connecting my vesc to the BLDC tool it says connected for about two seconds then it reads "no firmware read response".
[/quote]

This happens every time you connect the vesc to computer or just the first time
```

---
## \#5 Posted by: Khix Posted at: 2017-09-21T10:46:11.609Z Reads: 94

```
Everytime I press connect
```

---
## \#6 Posted by: krloz Posted at: 2017-09-21T11:31:46.680Z Reads: 91

```
Maybe incompatible firmware? What bldc tool are you using.  And does your vesc have a boot loader?
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2017-09-21T12:52:27.616Z Reads: 88

```
[quote="Khix, post:1, topic:33637"]
the vesc doesn't blink at all, but my voltmeter turns on and reads 0.0.
[/quote]

If your volt meter read 0.0 it does mean that you don't have power going to your VESC, can you post some picture ?
```

---
## \#8 Posted by: Khix Posted at: 2017-09-21T16:53:49.001Z Reads: 76

```
https://cdn.discordapp.com/attachments/224414138145701899/343605814063529984/unknown.png

<img src="/uploads/db1493/original/3X/2/b/2bcb97b21d9e7dbbcd2fdf4eab9c88fd23571f71.jpg" width="666" height="500">
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2017-09-21T17:14:19.196Z Reads: 72

```
Do you have a Multimeter ?
```

---
## \#10 Posted by: Khix Posted at: 2017-09-21T17:22:38.730Z Reads: 67

```
yes (granted its old but it'll work)
```

---
## \#11 Posted by: jmasta Posted at: 2017-09-21T17:30:59.476Z Reads: 65

```
Is that a 3-wire voltmeter? Hard to tell from the picture
```

---
## \#12 Posted by: Khix Posted at: 2017-09-21T17:33:49.745Z Reads: 65

```
Yes, should the white be connected to something?
```

---
## \#13 Posted by: jmasta Posted at: 2017-09-21T17:40:20.476Z Reads: 64

```
Yes... It's not there for show :joy:

Many high voltage meters like yours require an auxiliary power source, usually 12-24V, to power the meter itself.  One wire is meter power input (12V), one is the voltage reading (~42V), and one is ground

The easiest solution is to buy a 2-wire voltmeter. There are plenty available that can accept 10S voltage
```

---
## \#14 Posted by: Khix Posted at: 2017-09-21T17:50:10.617Z Reads: 64

```
Thanks for the info. I definitely didn't put as much thought into it as I should have. Woops.
```

---
## \#15 Posted by: jmasta Posted at: 2017-09-21T17:55:04.576Z Reads: 63

```
It's all good. We've all been there. Just look for one with only two wires, like this:

https://www.amazon.com/Waterproof-4-5-150V-Automative-Electric-Voltmeter/dp/B00P7FX0BY
```

---
