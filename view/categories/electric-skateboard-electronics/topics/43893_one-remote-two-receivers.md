# One remote, Two receivers

### Replies: 8 Views: 659

## \#1 Posted by: Sebike Posted at: 2018-01-16T19:57:47.013Z Reads: 138

```
There's been some discussion on whether CAN or Y-split ppm should be used for 2x/4x vesc-systems and I believe I've seen some ppl mention they were using dual receivers for even less interaction and risk of having one vesc killing the other. 

I couldn't find much on this though. Maybe not many use this method, but from those that do, what are your thoughts and experience so far (mainly interested in info regarding the GT2B)? @Namasaki maybe? 


https://img.tttcdn.com/product/original/p/gu1/R/RM318/RM318-2-70ef.jpg



https://d3ham790trbkqy.cloudfront.net/wp-content/uploads/sites/5/2015/05/14161036/pressreleasethomas-wilson-1431705053.png
```

---
## \#2 Posted by: bigben Posted at: 2018-01-16T20:01:11.643Z Reads: 129

```
I've had it running faultlessly with the mini remote. Just did the bind separately on each receiver.
A few extra sheckles for the other receiver but it's one extra failsafe.
```

---
## \#3 Posted by: Achmed20 Posted at: 2018-01-16T20:22:21.727Z Reads: 119

```
intresting. i went the Y way and so far no problems.
```

---
## \#4 Posted by: Sebike Posted at: 2018-01-16T20:33:01.049Z Reads: 113

```
Yes, this seems to be the safer way between those two, but some have run into issues with Y-split as well, and @trampa is usually quick to let everyone know that the Y-route is daaangerous. Anyway. Can't see any major downsides in using 2xreceivers apart from the few extra bucks, but maybe there are cons I'm not aware of.
```

---
## \#5 Posted by: Achmed20 Posted at: 2018-01-16T20:35:58.079Z Reads: 104

```
if it works, why not. i would just make sure that they are both the same model.
```

---
## \#6 Posted by: longhairedboy Posted at: 2018-01-16T20:43:55.573Z Reads: 95

```
i split my ppm to twin receivers, each feeding a twin ESC group on CAN bus. without doing the resistor hack, or using two remotes, its the only way to reliably tie four VESC based ESCs together at the moment. the other way is to split the ppm four ways and that has a tendency to introduce issues in my experience.
```

---
## \#7 Posted by: Sebike Posted at: 2018-01-16T20:46:37.783Z Reads: 91

```
And you have zero issues from the twin receiver setup? What remotes do you use for that?
```

---
## \#8 Posted by: Namasaki Posted at: 2018-01-17T00:19:38.009Z Reads: 67

```
running multiple receivers with a single remote works with the mini RC remote.
I can't say if it works with any others because I have only tried it with the mini RC.
```

---
