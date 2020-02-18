# Will this diagram work?

### Replies: 5 Views: 216

## \#1 Posted by: stalejarmynd Posted at: 2019-04-24T16:30:45.830Z Reads: 69

```
![11|690x378](upload://96Qrq3m89R21nVuV3bi4rFkN8M5.jpeg) 

Hi, I'm new to building eboards and electronics. I'm wondering if this setup will work? Or does the VESC need to be connected from the P- connection instead of the B- connection? Is it the same with the voltagemeter?

In advance, thanks for help!
```

---
## \#2 Posted by: olestra Posted at: 2019-04-24T17:43:35.808Z Reads: 57

```
I'd put the voltmeter negative right off the battery(like you have diagrammed), and the positive after the anti-spark. I would like everything shutoff, when I shut it off -- if it sits, I wouldn't want a slow drain going on. 

As far as the vesc, it depends on whether you want the BMS to be charge only ( use your diagram) or run through the BMS -- if you run it through the BMS, your amp draw is limited by what the BMS can handle, but supposedly it would help keep the cells balanced during discharge
```

---
## \#3 Posted by: stalejarmynd Posted at: 2019-04-24T19:44:04.699Z Reads: 43

```
Thanks for helpful answer! The BMS is 60A rated, will it be enough or would you rather keep it the same? Battery I'm using is 10S3P 30Q samsung batteries
```

---
## \#4 Posted by: olestra Posted at: 2019-04-24T22:07:49.747Z Reads: 32

```
I'm far from an expert -- 'enough' is relative. there are many threads talking about these topics.
```

---
## \#5 Posted by: b264 Posted at: 2019-04-24T22:15:29.938Z Reads: 27

```
No, you want something like this

https://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179/129?u=b264

except with [a fuse](https://www.mouser.com/ProductDetail/576-099707.5WXN) on the charge port negative line

And also at this time (April 2019), I would recommend a loop key instead of an antispark switch.
```

---
