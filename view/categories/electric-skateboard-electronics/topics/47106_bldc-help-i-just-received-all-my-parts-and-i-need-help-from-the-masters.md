# \[BLDC HELP\] I just received all my parts and I need help from the MASTERS!

### Replies: 10 Views: 535

## \#1 Posted by: Provoke Posted at: 2018-02-22T02:38:45.440Z Reads: 81

```
Hey ladies and gents!

I finally have all my parts and had some questions regarding the BLDC settings & numbers. 

What should I have my Motor max, motor min, batt max, batt min, and absolute max set to? I'll be using this board to commute to work 5 days a week. So reliability is KING!

Thanks in advance for any advice & tips!

* 1x [12s4p battery from DIYeletricskateboards](products/electric-skateboard-battery-epower-pack-12s4p)
* 2x [Torque Boards 6370 (190v)](products/electric-skateboard-motor-6374-190kv)
* 2x [Enertion FocBox](http://www.enertionboards.com/electric-skateboard-parts/FOCBOX-programmable-brushless-motor-controller/)

![BLDC setup|690x407](upload://vzyH0AvcMV5r10qhUMKGW3jLvPx.png)
```

---
## \#2 Posted by: ShutterShock Posted at: 2018-02-22T02:45:11.592Z Reads: 70

```
Well there are quite a few posts on the forum detailing settings for a 12S build, but here's what I use.

The motor amps can control how powerful the board feels, feel free to turn them down if it knocks you off your feet every time.


Motor Max: 80A
Motor Min: -80A
Batt Max: 30A/2 = 15A  (your battery is rated for this, it is low because of the two VESCS)
Batt Min: -12A (depends on battery, this is what I use)

For the absolute max and stuff, load the default settings first, and use those.

Someone else that knows the DIY battery feel free to comment - Also @Provoke try searching too, I got a lot of help from that when I was looking at this stuff, especially with settings.
```

---
## \#3 Posted by: GrecoMan Posted at: 2018-02-22T02:50:24.523Z Reads: 64

```
holy f#*% -20a batt min?
```

---
## \#4 Posted by: ShutterShock Posted at: 2018-02-22T02:53:45.458Z Reads: 60

```
Lol ya what do you use?  Actually now that I think about it, it is probably -12A.

It never actually hits that though
```

---
## \#5 Posted by: GrecoMan Posted at: 2018-02-22T02:55:53.383Z Reads: 60

```
yea the highest i’ll ever recommend is -12a... unless special circumstances. i use -12a personally
```

---
## \#6 Posted by: Apolo Posted at: 2018-02-22T02:57:16.971Z Reads: 60

```
You can probably push bat max to 40A (20A for each vesc & motor).

I use 35A for my single drive on my TB 12s2p
```

---
## \#7 Posted by: ShutterShock Posted at: 2018-02-22T02:57:53.988Z Reads: 58

```
Yeah that is what I use for mine, but it says on the website that the DIY battery only does 30A cont?
```

---
## \#8 Posted by: ShutterShock Posted at: 2018-02-22T02:58:21.006Z Reads: 58

```
Oh interesting, they must have underrated it
```

---
## \#9 Posted by: Apolo Posted at: 2018-02-22T02:59:58.208Z Reads: 56

```
Well it doesn't cut off the current at 30A, They only say 30A because that's the absolute safest (if we're talking about bms). 35A shouldn't do any harm since you only really make the battery work hard on hills.
```

---
## \#10 Posted by: Travo Posted at: 2018-07-12T21:22:24.277Z Reads: 26

```
Hey everyone I'm having trouble uploading the 2.17 firmware to my vesc so by that I can use the BLDC Tool. My current VESC is the one supplied from DIY electric skateboards. Hardware V4.12 V3.38
```

---
