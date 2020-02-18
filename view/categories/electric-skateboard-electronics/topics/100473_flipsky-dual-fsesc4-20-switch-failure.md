# FlipSky Dual FSESC4.20 switch failure

### Replies: 11 Views: 233

## \#1 Posted by: Treezie Posted at: 2019-08-17T23:53:29.801Z Reads: 79

```
Hi all,

I have a FlipSky Dual FSESC4.20. It has been working well for the past few weeks; however, now the switch does nothing and the ESC powers up automatically when connecting the xt60. Previously it would require the switch to activate the ESC due to anti-spark function. Any Ideas how I can resolve the issue? I have tried another switch and it still does nothing. 

Thanks 

Luke
```

---
## \#2 Posted by: captclearleft Posted at: 2019-08-18T03:40:58.321Z Reads: 69

```
I am sure you have tried this.  With everything unplugged.  Can you unplug the switch cable.   Then plug the battery in?
```

---
## \#3 Posted by: Treezie Posted at: 2019-08-18T08:01:12.721Z Reads: 64

```
I did try that but unfortunately it didn't do anything. The ESC turns on automatically when I connect the xt60 and I still cant use the switch to turn it on or off.
```

---
## \#4 Posted by: gee Posted at: 2019-08-18T08:38:30.948Z Reads: 62

```
have this problem also. Would like to know why. Did the vesc failed or the switch failed.
```

---
## \#5 Posted by: Gamer43 Posted at: 2019-08-18T22:38:38.714Z Reads: 46

```
One if the MOSFETs failed short circuit.
This is expected. 
Flipsky is working on a better design to replace them with.
```

---
## \#6 Posted by: Treezie Posted at: 2019-09-06T02:34:23.952Z Reads: 29

```
Is there any solution to solving it without having to purchase a new ESC? @Gamer43 

cheers, 

Luke
```

---
## \#7 Posted by: jun1208 Posted at: 2019-09-06T03:25:03.399Z Reads: 28

```
Have you tried using a loop key on the negative end of the power to the VESC?

If the VESC is still working but just can't be turn off, I think loop key might be a possible solution :+1:
```

---
## \#8 Posted by: Gamer43 Posted at: 2019-09-06T05:32:51.058Z Reads: 25

```
Yes you can, but you will need a heat gun or hot air station and confidence in your soldering abilities.
```

---
## \#9 Posted by: Treezie Posted at: 2019-09-06T22:13:10.288Z Reads: 16

```
Something like this but on the negative side? @jun1208

![A205E40F-21DC-411E-9024-2C4D73FADB5C|690x381](upload://rF5RA2bCSI6EulXp7LKTFP2F5HE.jpeg) 

Credit:  hyperlon1
```

---
## \#10 Posted by: jun1208 Posted at: 2019-09-07T04:16:50.170Z Reads: 13

```
Yeap that's right :+1:

That's of course if the VESC is working when you plug the battery to it, because if it works when you plug the battery to the VESC that means it has just bypassed the anti spark switch so a AS loop key should work as a switch in the absence of the built in AS switch :slight_smile:
```

---
## \#11 Posted by: Treezie Posted at: 2019-09-07T06:16:30.612Z Reads: 12

```
Perfect. The VESC definitely works so I will put one together this week and see how I go. Thanks for the help mate, much appreciated.
```

---
