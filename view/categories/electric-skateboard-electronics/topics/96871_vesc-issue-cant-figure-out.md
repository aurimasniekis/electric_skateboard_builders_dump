# Vesc issue &hellip;can&rsquo;t figure out

### Replies: 21 Views: 416

## \#1 Posted by: Jcammarata4 Posted at: 2019-06-18T17:11:37.517Z Reads: 130

```

One of my maytec super escs began acting up and won't work properly. I checked all connections ..I swapped motors and they're both good. It is the vesc but I dont know what's the cause or if fixable here's some pics and a vid. It Powers up fine. It shows up in vesc tool and is up to date w firmware. Do they just go bad after some time? Is it fixable? ! Here's a video of the issue in action and a pic or two.....
https://youtu.be/eJyBYbELCF0

[20190618_121751|281x500](upload://8cf5TjhTHViB0lNhBIH4bGoCGpV.jpeg) ![20190618_121834|281x500](upload://jBKuc7mrNihnRKIyOktOmjhkokS.jpeg)
```

---
## \#2 Posted by: Jcammarata4 Posted at: 2019-06-18T17:16:13.144Z Reads: 117

```
I also checked it out for any faults and none show up.
```

---
## \#3 Posted by: linsus Posted at: 2019-06-18T18:41:03.938Z Reads: 101

```
Its literraly flashing red, that can't be right. Try again
```

---
## \#4 Posted by: dareno Posted at: 2019-06-18T19:01:35.600Z Reads: 97

```
I can't tell but is that chirping coming from the motor?  Are the input lights coming on as normal when you hit the throttle?
Usually a red flashing light does mean fried drv but thats all you get and fault log should show something.  So long as you have verified that its not a motor issue then try re detecting the motor on that vesc.
```

---
## \#5 Posted by: Jcammarata4 Posted at: 2019-06-18T19:25:47.683Z Reads: 89

```
Yes chirps comming from motor trying to spin....which it will work fine when put on the other vesc.
```

---
## \#6 Posted by: Jcammarata4 Posted at: 2019-06-18T19:26:11.376Z Reads: 87

```
And yes it's flashing red
```

---
## \#7 Posted by: Jcammarata4 Posted at: 2019-06-18T19:30:48.217Z Reads: 84

```
I did re detect the motors...it will show up as the slave but it's clearly got some issues....again motors are not even 2months old and both are running properly when tested on a good vesc....but the vesc in question seems trashed somehow....nothing got hot...wet...or anything I can think of......beyond maybe riding on a rough surface or two........but I dont see anything that could've shorted or arced out
```

---
## \#8 Posted by: AgressivStreetLamp Posted at: 2019-06-18T19:44:39.326Z Reads: 75

```
Smell test for burnt parts?
```

---
## \#10 Posted by: Jcammarata4 Posted at: 2019-06-18T20:34:52.302Z Reads: 67

```
Ya nothing..no smell no heat no damage......I guess it's just worn out? Doesn't sound like a good answer but idk......anyone think that a dual vesc would be a better option than keeping the single vescs per motor? Thinking about flipsky dual
```

---
## \#11 Posted by: AgressivStreetLamp Posted at: 2019-06-18T20:47:54.951Z Reads: 63

```
Electronics don't "wear out" 
I suppose you can heat cycle them to death but in this situation, you'd die before it did. 


If your considering an upgrade might just do that.
Sounds mostly like a firmware thing. did you flash it directly and try that? not through CAN that is
```

---
## \#12 Posted by: Jcammarata4 Posted at: 2019-06-18T23:42:05.464Z Reads: 60

```
Yes then it won't register ...it will via can
```

---
## \#13 Posted by: AgressivStreetLamp Posted at: 2019-06-19T00:51:07.058Z Reads: 55

```
Hm shows up as slave but not a via usb. sus. No clue man, best guess is DRV or ARM is cooked
```

---
## \#14 Posted by: dareno Posted at: 2019-06-19T04:49:07.722Z Reads: 55

```
Red flashing and drv usually.  Sorry dude looks like you got yourself a bricked esc.  Have you tried detecting it on bldc?
```

---
## \#15 Posted by: Jcammarata4 Posted at: 2019-06-19T19:08:24.171Z Reads: 39

```
Does bricked imply firmware because it was not due to any use of programming. It happened during a ride
```

---
## \#16 Posted by: Jcammarata4 Posted at: 2019-06-19T19:09:34.967Z Reads: 40

```
So is something burnt out somehow.....never had any issue like this b4
```

---
## \#17 Posted by: Jcammarata4 Posted at: 2019-06-19T19:10:55.269Z Reads: 39

```
And any ideas on good replacement ideas such as dual vs single vescs and any good rugged brand names
```

---
## \#18 Posted by: dareno Posted at: 2019-06-20T08:11:15.634Z Reads: 33

```
Esc's fail.  They do it to piss you off.  Seriously unless you run full telemetry then its pretty hard to know why most of the time if the fault log shows nothing.  Doesn't make that particular vesc a bad choice because it happens to most at some point.  
Flipsky are pretty good by all accounts.  I use focboxes and they are discontinued so I am in the exact same place as you right now with choices.
```

---
## \#19 Posted by: ARetardedPillow Posted at: 2019-06-20T08:16:08.417Z Reads: 33

```
Take off the heat shrink and take photos of the vesc
```

---
## \#20 Posted by: linsus Posted at: 2019-06-20T09:16:29.922Z Reads: 29

```
if you can still talk to the vesc and its flashing red. It means that its producing faults. You should be able to see them.
```

---
## \#21 Posted by: Jcammarata4 Posted at: 2019-06-21T00:37:17.030Z Reads: 23

```
Well reinstalled firmware but still acts like a spoiled little b****. I'm going to extract the rotten parts and teach them a lesson ....it'll make all the other parts listen and behave.
```

---
## \#22 Posted by: Jcammarata4 Posted at: 2019-07-02T16:17:33.183Z Reads: 10

```
https://s.amsu.ng/8o3hlOpV2f0N
```

---
