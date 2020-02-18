# (SOLVED) Please Help! Motor is having trouble moving the weight of the board (without me standing on it)

### Replies: 22 Views: 1166

## \#1 Posted by: nikolas Posted at: 2017-07-21T06:54:15.672Z Reads: 132

```
@Blasto

Hi! I just built  my first esk8. I was unhappy to see that my board was not working. After many hours of troubleshooting, I still could not find out why it is not working. It seems to be related to low torque, which is weird because I have a 190kv motor. Warning in advance: ALL MY VIDEOS ARE LINKS due to a problem wih downloading.

**When board is on the ground:**

VIDEO: https://drive.google.com/file/d/0B5BaErN4DS8JU1VMbkcyRXpRb2c/view?usp=sharing

* The board jitters and does not move.

* If I give the board a kick, it moves very slowly



**When the board is not on the ground:**

VIDEO: https://drive.google.com/file/d/0B5BaErN4DS8JLWotSDdEcklZdGs/view?usp=sharing

* Wheels spin much faster

* No jittering




Here are my parts:

* 6355 190kv motor from diyelectricskateboard   (diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/)

*  TORQUE ESC VESC ® BLDC Electronic Speed Controller [diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/](diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/)

* I use 2 5000mah 3s1p 20c lipo batteries connected in series.

* TorqueBoards 2.4ghz Nano Remote Controlle      r[diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-nano-remote-controller/](diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-nano-remote-controller/)


While I am riding the board, this is the fastest it goes:

https://drive.google.com/file/d/0B5BaErN4DS8JRXROcVE0WkFLNFU/view?usp=sharing

I can supply you wiith the BLDC Tool screenshots if needed!

Thank you in advance!
```

---
## \#2 Posted by: aigenic Posted at: 2017-07-21T06:58:40.442Z Reads: 123

```
Send the BLDC screenshots ;)
```

---
## \#3 Posted by: Blasto Posted at: 2017-07-21T20:56:19.923Z Reads: 106

```
Sounds like your being throttled by your settings, did you perform a motor detection?
```

---
## \#4 Posted by: nikolas Posted at: 2017-07-21T22:04:11.519Z Reads: 92

```
Yes. Here are the settings.


<img src="/uploads/db1493/original/3X/3/8/3849a03358cf8e7ad0fb28bcab76401a9bba7cbe.PNG" width="690" height="356"><img src="/uploads/db1493/original/3X/5/b/5bbf8b282647e9720299ccff5cf9fdde4cc96bc4.PNG" width="690" height="358"><img src="/uploads/db1493/original/3X/9/2/925a512bd45f8331553169a8e278466644407631.PNG" width="690" height="351"><img src="/uploads/db1493/original/3X/3/f/3f274d96f6a82ca127215ed82744c433544c6225.PNG" width="690" height="359">
```

---
## \#5 Posted by: darkkevind Posted at: 2017-07-21T22:12:45.584Z Reads: 82

```
Looks like you haven't had a successful motor detection. Up the amps 1 or 2 and try it again. Don't forget to 'Apply' the results and write config. Then, reboot and try it...

EDIT: Also, it's in battery cut-off mode. Your voltages are too high for your battery configuration. 2 x 3s is only 25.2v fully charged and you're telling the VESC it should have more than 33!

Change cut-off start to 20.5v and end to 19.5v
```

---
## \#6 Posted by: Blasto Posted at: 2017-07-21T22:15:42.695Z Reads: 80

```
Your voltage cutoffs are set for a 10S system, you have a 6S system
```

---
## \#7 Posted by: darkkevind Posted at: 2017-07-21T22:16:18.570Z Reads: 81

```
lol, beat you to it :slight_smile:
```

---
## \#9 Posted by: nikolas Posted at: 2017-07-21T22:49:49.631Z Reads: 71

```
What does that mean. How do I fix it?
```

---
## \#10 Posted by: nikolas Posted at: 2017-07-21T22:51:00.831Z Reads: 70

```
Ok I will try and post my results. Thanks for your time!
```

---
## \#11 Posted by: Blasto Posted at: 2017-07-21T22:51:01.415Z Reads: 67

```
Change your cut off start and end

[quote="darkkevind, post:5, topic:28183"]
Change cut-off start to 20.5v and end to 19.5v
[/quote]
```

---
## \#14 Posted by: nikolas Posted at: 2017-07-21T23:10:39.132Z Reads: 59

```
Wooooow... Thank you sooooo much  @Blasto @darkkevind... Just one more question, when we are riding, no matter the position on the controller(only forward positions actually) , the board will go full speed.
```

---
## \#15 Posted by: darkkevind Posted at: 2017-07-22T00:00:56.287Z Reads: 55

```
You need to calibrate the controller in the application section of the BLDC software. PWM.
```

---
## \#16 Posted by: nikolas Posted at: 2017-07-22T00:15:02.955Z Reads: 56

```
What is PWM and do I need to plug in the controller? BTW thank you for your help!
```

---
## \#17 Posted by: darkkevind Posted at: 2017-07-22T00:17:06.034Z Reads: 58

```
Pulse width modulation. It's too do with how the controller talks to the ESC.

Please look up on YouTube: VESC setup
```

---
## \#18 Posted by: nikolas Posted at: 2017-07-22T01:07:31.292Z Reads: 55

```
Ok Thanks... Would this also include how to make my board go backwards as well?
```

---
## \#19 Posted by: Luke Posted at: 2017-07-22T02:42:07.271Z Reads: 49

```
you can just tick "current" in your App configuration/PPM settings
```

---
## \#20 Posted by: nikolas Posted at: 2017-07-23T20:14:05.963Z Reads: 39

```
Thanks!  It worked out great!
```

---
## \#21 Posted by: nikolas Posted at: 2017-08-15T19:32:52.934Z Reads: 33

```
Hi again! What would I change in my BLDC tool to go from a 6s set up to a 10s setup?
```

---
## \#22 Posted by: darkkevind Posted at: 2017-08-15T19:35:07.788Z Reads: 34

```
You should really do a motor detection again and then change your voltage cut-off levels for 10 cells.

Work out the values that we gave you last time, then change them for 10 cells instead of 6 :slight_smile:
```

---
## \#23 Posted by: nikolas Posted at: 2017-08-15T19:36:40.818Z Reads: 35

```
What should i change it to?
```

---
## \#24 Posted by: darkkevind Posted at: 2017-08-15T19:38:59.663Z Reads: 30

```
Like I said, work out what we told you last time for your levels with 6 cells, then adjust it for 10 cells.

The values we told you in the previous post...

[quote="darkkevind, post:5, topic:28183"]
Change cut-off start to 20.5v and end to 19.5v
[/quote]

Divide those by 6, then times that by 10....
```

---
## \#25 Posted by: nikolas Posted at: 2017-08-15T20:00:10.338Z Reads: 29

```
Ohhhh, ok i didnt know that it varied porportionally.
```

---
