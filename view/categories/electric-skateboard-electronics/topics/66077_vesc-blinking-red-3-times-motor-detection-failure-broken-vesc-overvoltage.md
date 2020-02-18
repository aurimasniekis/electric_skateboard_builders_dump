# Vesc blinking red 3 times motor detection failure, broken Vesc? Overvoltage?

### Replies: 3 Views: 470

## \#1 Posted by: Ryguy Posted at: 2018-08-26T00:07:16.368Z Reads: 78

```
I am having trouble with motor detection, I connect to the vesc tool and choose FOC, input motor and battery maxes and max brake and regen. Put in a soft battery cutoff and choose hall sensors. Now when it asks me to mesure RL it takes a while then makes the normal noise but only measures L and says, "R is 0, Please measure it first". And it makes the L measurement green. I'm really not sure why the detection for R isn't working?

![IMG_3743|375x500](upload://8uYc05i2XtTHI675u74bjkcrxgC.JPG)
![IMG_3741|375x500](upload://9Qu28nc7nbn4IGYNNl4Pv8A4G9D.JPG)
![IMG_3745|666x500](upload://dmNI0n3aDGK2bLHuBSBucQFW5Z0.JPG)
![IMG_3744|666x500](upload://gbjcwoUTu5CKGh2XKy3ysYfYO8w.JPG)
```

---
## \#2 Posted by: Ryguy Posted at: 2018-08-26T18:03:39.647Z Reads: 48

```
If I choose BLDC motor type then hall sensors and run the test which is supposed to spin the motor. The Vesc blinks red three times, then it blinks red three times again then says detection failed. Is there a problem with the vesc? In FOC when I run RL it blinks red three times right after the command then 30ish seconds later the motor makes the usual noise I think, and says: "Calculate Error: R is 0. Please measure it first. I'm really lost and I have no clue what else to try
```

---
## \#3 Posted by: Ryguy Posted at: 2018-08-28T01:49:53.840Z Reads: 34

```
Ok so I did lots of reading and when you send a signal with your remote and the vesc blinks red three times that basically means you have a faulty DRV issue. So basically you have to replace that. Luckily I got the warranty, hope I helped someone in the future lol.
```

---
