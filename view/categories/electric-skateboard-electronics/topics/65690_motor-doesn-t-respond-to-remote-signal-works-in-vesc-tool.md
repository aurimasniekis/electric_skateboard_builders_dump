# Motor doesn’t respond to remote signal, works in vesc tool

### Replies: 11 Views: 152

## \#1 Posted by: 12meterkuk Posted at: 2018-08-22T09:13:23.595Z Reads: 46

```
I reset every setting in the vesc tool after the motor stopped working suddenly and any input will short the phases, now it won’t respond to my signal, works with keyboard and motor detection in vesc tool. Any idea how to fix this?
```

---
## \#2 Posted by: 12meterkuk Posted at: 2018-08-22T09:18:28.576Z Reads: 45

```
Ok it suddenly works again for some reason, will update it it stops again
```

---
## \#3 Posted by: bigben Posted at: 2018-08-22T09:18:50.829Z Reads: 43

```
Have you gone through the input setup wizard and selected the control method?
```

---
## \#4 Posted by: 12meterkuk Posted at: 2018-08-22T09:19:08.120Z Reads: 42

```
Yeah, saved all the configs
```

---
## \#5 Posted by: bigben Posted at: 2018-08-22T09:19:37.510Z Reads: 43

```
And what is your control type set as?
```

---
## \#6 Posted by: 12meterkuk Posted at: 2018-08-22T09:20:10.489Z Reads: 42

```
mini remote, ppm I think.
```

---
## \#7 Posted by: 12meterkuk Posted at: 2018-08-22T09:20:47.845Z Reads: 42

```
I don’t think this had anything to do with app settings, I reset motor settings to default and it started spinning with input
```

---
## \#8 Posted by: bigben Posted at: 2018-08-22T09:22:15.546Z Reads: 44

```
![image|666x500](upload://skImY1Qvnuamn7EmDWc13RkitrC.jpg)
Not like this then with it set to off?
![image|666x500](upload://25eZ5saZ2gpAj1GUsvPntiF7yqu.jpg)
Should look like this. 
Worth checking the ppm tab then control type.
```

---
## \#9 Posted by: 12meterkuk Posted at: 2018-08-22T09:25:34.685Z Reads: 41

```
Oh, I’m using current no reverse with brake
```

---
## \#10 Posted by: 12meterkuk Posted at: 2018-08-22T09:27:50.846Z Reads: 41

```
I think I know what happened, after the motor stopped working I couldn’t get the hall sensors to detect, so I think it broke and I forgot to reset the settings to sensorless
```

---
## \#11 Posted by: bigben Posted at: 2018-08-22T09:28:06.942Z Reads: 38

```
That sounds right then. 
Worth running through the input setup wizard again and enable current no reverse with brake on both tabs.
```

---
