# Focbox Unity and Motor Tension

### Replies: 7 Views: 138

## \#1 Posted by: achatham Posted at: 2019-08-26T17:19:58.308Z Reads: 57

```
Just recently got the focbox unity and got everyting configured but running into an issue with the motor tension it seem like. Using the Focbox UI app (windows USB connection) when I go to test the board the wheels/motor doesnt spin freely. When I release the throttle, the wheels just lockup. I've seen a little bit about it on the forum, but my question is: Is there anything in the focbox ui settings (maybe advanced throttle settings?) that will allow the wheels to spin?
```

---
## \#2 Posted by: achatham Posted at: 2019-08-27T00:24:44.711Z Reads: 44

```
Doing additional testing this afternoon it seems if you set the Motor Braking Max to -30 it places so much tension on the wheels that you cant even manual pushing the board. If you set it to -12 it rolls, but does brake. What the heck?!

It this a known issue with the focbox ui app?
```

---
## \#3 Posted by: accrobrandon Posted at: 2019-08-27T00:46:21.062Z Reads: 43

```
Releasing throttle and braking at so called zero sounds like a remote calibration issue....and/or fail safe. Reducing the braking value only reduces the amount of brake youd actually feel. That would be where I start.
```

---
## \#4 Posted by: achatham Posted at: 2019-08-27T01:15:24.054Z Reads: 39

```
Think I fixed the issue. I used the Focbox Tool instead of the Focbox UI tool. It has a few more options and one I noticed is the Motor Resistance 1 (R) was set to something like 642 m instead of 15m. I'm not sure if 15 is the best number but its the default and works. I thinking it has to do with the motor testing with sensors and then doing the flux  linkage test with handing spinning. Thanks for the note.
```

---
## \#5 Posted by: pundahh Posted at: 2019-08-27T01:17:17.615Z Reads: 35

```
Motor resistance should be what it calibrates to be. Typically is in the 13-18 range though.
```

---
## \#6 Posted by: achatham Posted at: 2019-08-27T01:45:08.430Z Reads: 35

```
It calibrated my motor at 61568.51! lol
![2019-08-26_21-43-44|689x389](upload://wJkeNYqkNCQewn1JTrHpPMoCojh.png)
```

---
## \#7 Posted by: pundahh Posted at: 2019-08-27T02:35:39.510Z Reads: 33

```
yikes?! try the ackmaniac software then, that's what I use :stuck_out_tongue:
```

---
