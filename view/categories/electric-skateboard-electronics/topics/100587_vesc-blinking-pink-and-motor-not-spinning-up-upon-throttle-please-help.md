# VESC blinking pink and motor not spinning up upon throttle Please help!

### Replies: 9 Views: 149

## \#1 Posted by: chatherton99 Posted at: 2019-08-20T02:43:59.472Z Reads: 37

```
So my build consists of a flipsky 4.12 VESC with a flipsky 6374 motor running on a 12s4p battery from DIY electric. I had everything working nicey nice and had the board riding perfectly today. But upon returning home, when i turn it on and throttle, the vesc has a pink light that comes on and the motor just does a twitching motion and does not spin at all or just stays still. I'm unsure what the issue is here if the board was literally working an hour prior to the second turn on. Any help would be greatly appreciated!!!
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-08-20T03:07:08.712Z Reads: 36

```
Plug the vesc into your computer without powering it off first (any error codes are stored in volatile memory - if it loses power, they disappear) and type `faults` in the vesc tool terminal.
```

---
## \#3 Posted by: chatherton99 Posted at: 2019-08-20T03:20:37.920Z Reads: 34

```
Alright i will try that. does the VESC tool from vescprojects have that fault feature
```

---
## \#4 Posted by: MysticalDork Posted at: 2019-08-20T03:43:53.344Z Reads: 32

```
ayup. They all do, or should.
```

---
## \#5 Posted by: chatherton99 Posted at: 2019-08-20T04:03:32.079Z Reads: 31

```
Now is there anyway it could be the voltage bounds are wrong on the vesc and arent matching up with what the battery is pushing through?
```

---
## \#6 Posted by: MysticalDork Posted at: 2019-08-20T04:16:32.738Z Reads: 30

```
Possible I guess, but I suspect it's something else. Did the faults command bring up anything? Maybe post a screenshot of your settings?
```

---
## \#7 Posted by: chatherton99 Posted at: 2019-08-20T04:27:54.282Z Reads: 30

```
unfortunately the board isnt currently with me. Tomorrow i will post screenshots of what the VESC tool says. Thank you for your help so far.
```

---
## \#8 Posted by: chatherton99 Posted at: 2019-08-20T16:10:52.629Z Reads: 22

```
https://www.electric-skateboard.builders/t/vesc-sparking-and-motor-not-spinning-up-please-help/100617![unnamed%20(1)|375x500](upload://mD1xEf51MPoj8zzfR88EP9gn1B7.jpeg) ![unnamed|374x500](upload://5T4E8IgEX2qVvkccbUvXNaGgj1r.jpeg)
```

---
## \#9 Posted by: seaborder Posted at: 2019-08-20T18:38:10.452Z Reads: 19

```
looks a bit like burn marks over your DRV Chip. What does the fault command say?
```

---
