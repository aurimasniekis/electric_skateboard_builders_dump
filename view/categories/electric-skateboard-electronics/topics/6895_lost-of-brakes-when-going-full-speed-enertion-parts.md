# **Lost of brakes when going full speed - Enertion Parts

### Replies: 21 Views: 2851

## \#1 Posted by: joeadams101 Posted at: 2016-07-31T06:45:35.056Z Reads: 231

```
Ok so went for an hour of riding to test out everything. Everything seemed fine until I was going at max speed I guess 23+ plus and I suddenly hit the brakes because i saw someone crossing the street and the board braked for 0.1 seconds and i felt it stopped braking. I tried to brake again and it didn't do anything, after like 3 seconds i tried it again and it braked but this time i wen easy on the throttle while braking. It was a very scary experience. Curious to know what causes that. Any help will be appreciated as I need to fix that....let me know what do you guys think. My specs/screenshot of current set up are on the first post. Using exertion space cell 3, exertion standard VESC and 6372 motor spec r.

My specs: <img src="/uploads/db1493/original/2X/3/348c6cf51fe4a441a40196805faab3a9fc9176f1.png" width="690" height="431">
```

---
## \#2 Posted by: elkick Posted at: 2016-07-31T06:52:49.094Z Reads: 227

```
Replace the max. Input voltage of 42V with 57V and test it again. 

Are those values preset? If so, that's not so good.
```

---
## \#3 Posted by: onloop Posted at: 2016-07-31T06:58:01.707Z Reads: 225

```

your max input voltage is probably too low, a voltage spike may cause the vesc to shut down... 

**Maximum Input Voltage 60V**

is this mono or dual?

if its mono, i would change current limits:

**Motor Max 60A**
**Motor Min REGEN -20** (this really depends on your weight & preferences, maybe go down from -40 in increments of 5 & test it)
**Batt MAX 40A** (slightly higher is ok, but eventually you'll blow a fuse, go up in 1A increments & test it)
**Batt Min REGEN -12** (this is probably correct, it's always best to try to keep Motor Min Regen & Batt Min REGEN as close as possible)
```

---
## \#4 Posted by: joeadams101 Posted at: 2016-07-31T07:17:45.253Z Reads: 219

```
Hey I replaced those earlier with this:

<img src="/uploads/db1493/original/2X/7/7d55a67e1a196dff28e9aabc51115b1034e2ef4c.png" width="690" height="232">


Was still giving me problems with it.  It is a Mono.
```

---
## \#5 Posted by: Jinra Posted at: 2016-07-31T07:28:07.415Z Reads: 207

```
Can you take a screenshot of your BLDC tab? If it doesn't respond for 3 seconds it sounds like the VESC is rebooting for some reason.
```

---
## \#6 Posted by: joeadams101 Posted at: 2016-07-31T07:46:51.550Z Reads: 206

```
Current  configuration:

<img src="/uploads/db1493/original/2X/6/6650891c99a6bf15f2b57ae823ef7f82adbb1f83.png" width="690" height="368">
<img src="/uploads/db1493/original/2X/7/7fd00a32517aa199eecc50efcf4321b6610f0891.png" width="690" height="369">
```

---
## \#7 Posted by: Jinra Posted at: 2016-07-31T07:55:33.457Z Reads: 188

```
Can you check the advanced tab as well? There's a setting (Max Current Ramp Step) in there that multiplies itself by 10 every time you write config on the motor config tab (software glitch). It should be .04 at default. Not sure if this affects your braking, but I'm sure it's not great to leave at 10x/100x/1000x/etc the normal value. See here:

http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262
```

---
## \#8 Posted by: laurnts Posted at: 2016-07-31T12:33:21.528Z Reads: 173

```
It could be that the battery regen braking setting you have is incompatible with the amount of current the battery could handle. Try reducing the regen current.
```

---
## \#9 Posted by: joeadams101 Posted at: 2016-07-31T16:49:41.504Z Reads: 158

```
Here you go

<img src="/uploads/db1493/original/2X/c/c77ba9a24eb3b3835cfe1a1f3aae8581868092e4.png" width="690" height="366">
```

---
## \#10 Posted by: Jinra Posted at: 2016-07-31T17:01:34.189Z Reads: 148

```
yea looks like it multiplied by ten. set it to .004 and write config, this will change it back to the default of .04
```

---
## \#11 Posted by: joeadams101 Posted at: 2016-07-31T17:05:47.924Z Reads: 144

```
[quote="Jinra, post:10, topic:6895"]
.004
[/quote]


So I input all the settings including the ones from @onloop and I am bench testing it. The board is at 100% and when i give full throttle and instantly try to brake it doesn't do anything. Going slower and braking works just fine...any ideas?
```

---
## \#12 Posted by: Jinra Posted at: 2016-07-31T17:11:10.853Z Reads: 138

```
what app config are you running?
```

---
## \#13 Posted by: joeadams101 Posted at: 2016-07-31T17:13:50.042Z Reads: 140

```
<img src="/uploads/db1493/original/2X/8/81daee661785cc48238ba07e28899546509da7b6.png" width="690" height="412">

@Jinra
```

---
## \#14 Posted by: Jinra Posted at: 2016-07-31T17:14:56.188Z Reads: 128

```
any reason you're on ppm/uart? most people run ppm, could you screenshot your ppm tab as well.
```

---
## \#15 Posted by: joeadams101 Posted at: 2016-07-31T17:16:50.286Z Reads: 136

```
it came default like that. Haven't changed it.

<img src="/uploads/db1493/original/2X/a/a035676dbc1b406d1408d8056abdb0efe7d2f5d0.png" width="690" height="409">
```

---
## \#16 Posted by: Jinra Posted at: 2016-07-31T17:18:31.970Z Reads: 132

```
I guess you can try with ppm and see if that helps. Running out of ideas myself :p

Also check what your remotes min and max pulsewidth is.
```

---
## \#17 Posted by: joeadams101 Posted at: 2016-07-31T17:36:15.966Z Reads: 131

```
How do I check the remote?
```

---
## \#18 Posted by: Jinra Posted at: 2016-07-31T17:38:30.336Z Reads: 132

```
connect VESC and check the display box in the above picture. Full throttle and you'll get the max pulsewidth, min throttle and you'll get the min pulsewidth. Put the values in the respective boxes and apply. Make sure to switch to ppm only!
```

---
## \#19 Posted by: elkick Posted at: 2016-07-31T17:45:34.325Z Reads: 133

```
You are running "multiple ESC over CAN" and "traction control" with a mono setup? That's not a good idea.
```

---
## \#20 Posted by: ra.rend Posted at: 2016-08-01T19:58:05.382Z Reads: 121

```
it probably shut down due to high temps. Happened to me once, but I knew how to foot brake so I didn't die :)
```

---
## \#21 Posted by: lrdesigns Posted at: 2017-01-23T07:43:03.369Z Reads: 60

```
Did you find a solution? I have had a similar issue braking down hill at full speed, but the brake came back when I re applied it. So I just pulsed it until I was slow enough to run.
```

---
