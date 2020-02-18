# Recommended VESC settings?

### Replies: 9 Views: 1563

## \#1 Posted by: joeadams101 Posted at: 2016-08-21T22:20:57.202Z Reads: 245

```
Hello I was just curious about the recommended vest settings for 

10s Space cell 3 
Enertion VESC
83 m wheels
16t/36t pulleys
Ollin 5065- 170kv motor

Sometimes when I am full throttle, after 30 seconds or less it will boost up with more speed? Kinda doesn't make sense. Its like it is not pushing out all the power it has when I full throttle, delayed?

This is what I have it set as:

<img src="/uploads/db1493/original/2X/3/30361b4a1f2f93c74d5de03ab19393d86f07e518.png" width="690" height="484">
```

---
## \#2 Posted by: michaelcpg Posted at: 2016-08-21T22:40:42.907Z Reads: 226

```
Should be able to push your motor max up to 60A or so and your battery max up to 40A. I believe the space cells still come with 40A fuses
```

---
## \#3 Posted by: joeadams101 Posted at: 2016-08-21T23:09:07.081Z Reads: 220

```
I have a lot of uphills on my area. I think going up to those will cause it to overheat?
```

---
## \#4 Posted by: michaelcpg Posted at: 2016-08-21T23:18:53.349Z Reads: 220

```
Same here. I'm using an Enertion 6374 which should draw more current than your Ollin motor. As a reference I regularly ride up a hill that's about 1.8km long with an average gradient of 11.7% and my VESC usually starts to cut back on power as it begins to reach the temperature thresholds just as I'm reaching the top with my motor max set to 60A so I expect your setup would better in that sort of situation. 

If you give it a go I'd be interested to see how things go. How have you found your motor to handle hills? I'm looking at upgrading to a pair of ollin motors at some point so I'm interested to hear from people how well they handle large hills.
```

---
## \#5 Posted by: joeadams101 Posted at: 2016-08-21T23:23:33.241Z Reads: 210

```
I have that motor. And I was having issues:

http://www.electric-skateboard.builders/t/update-not-enough-power-or-lost-of-it-enertion-build/7104/81

http://www.electric-skateboard.builders/t/overheating-issue-fixed-enertion-motor-6372-replaced/7640/37
```

---
## \#6 Posted by: joeadams101 Posted at: 2016-08-21T23:23:53.266Z Reads: 195

```
Ill try going maybe 40on motor and 40 on batt
```

---
## \#7 Posted by: michaelcpg Posted at: 2016-08-21T23:34:37.439Z Reads: 191

```
Oh right haha. So you swapped out the Enertion motor for an Ollin motor then? How do they compare?
```

---
## \#8 Posted by: Skitzor Posted at: 2016-08-22T01:07:06.930Z Reads: 179

```
The one and honest answer to get good performance, go dual and 15/36 ratio ...
```

---
## \#9 Posted by: cesargrimmelprez Posted at: 2016-08-22T09:05:23.994Z Reads: 158

```
There gotta be a setup where a 6372 rspec motor runs correctly with an enertion vesc?
```

---
