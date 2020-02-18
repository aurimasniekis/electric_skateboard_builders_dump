# Erpm only 7000 and motor wont detect

### Replies: 24 Views: 743

## \#1 Posted by: yelnats8j Posted at: 2017-10-01T15:41:37.336Z Reads: 64

```
I just started testing my esk8 and found a problem. The erpm is only 7000 and the vesc wont detect the motor.
```

---
## \#2 Posted by: Nix Posted at: 2017-10-01T16:08:16.188Z Reads: 59

```
I think it would help if people knew your set up and maybe some pictures
```

---
## \#3 Posted by: GrecoMan Posted at: 2017-10-01T16:14:06.583Z Reads: 58

```
+1 to what @Nix said
```

---
## \#4 Posted by: yelnats8j Posted at: 2017-10-01T18:34:33.903Z Reads: 45

```
<img src="/uploads/db1493/original/3X/f/3/f3b976f42d1e9d8bc9efc03447449f9188f58fe7.png" width="690" height="431"><img src="/uploads/db1493/original/3X/8/9/8983e0a534dce0efb3acfaae175b487e8e97696c.png" width="690" height="431"><img src="/uploads/db1493/original/3X/1/0/10313773224942055cb61d884e362c4b0d1abdcd.png" width="690" height="431">
```

---
## \#5 Posted by: GrecoMan Posted at: 2017-10-01T19:18:01.862Z Reads: 34

```
click on terminal and type in "FAULTS"
```

---
## \#6 Posted by: GrecoMan Posted at: 2017-10-01T19:20:07.289Z Reads: 34

```
wait a second... it says your only running 6.4v...
Is that true?

If that's what your meaning to do:
You might get 5mph on flats
Lower the minimum input voltage to below 6.4v volts if you want it to "work"
```

---
## \#7 Posted by: yelnats8j Posted at: 2017-10-01T21:21:33.299Z Reads: 33

```
i have two 3s batterys what should it be
```

---
## \#8 Posted by: GrecoMan Posted at: 2017-10-01T21:29:43.004Z Reads: 32

```
It should be at 24v
```

---
## \#9 Posted by: MysticalDork Posted at: 2017-10-01T21:35:26.976Z Reads: 34

```
looks like you may have a weak connection somewhere. Do you have an antispark loopkey installed?
```

---
## \#10 Posted by: yelnats8j Posted at: 2017-10-01T21:43:41.903Z Reads: 33

```
no but i have a 4mm hxt bullet to xt 60 then xt 60 to xt 90
```

---
## \#11 Posted by: yelnats8j Posted at: 2017-10-01T21:44:36.183Z Reads: 31

```
i also had to fix a bulet connector on the motor they sent me it had solder in the wrong end.
```

---
## \#12 Posted by: MysticalDork Posted at: 2017-10-01T21:55:38.266Z Reads: 28

```
Unplug, wiggle and replug all your connections. If you have a 24v pack and a bad connection, it may be sagging under load.
```

---
## \#13 Posted by: yelnats8j Posted at: 2017-10-01T21:58:49.772Z Reads: 28

```
allright
ill try that
```

---
## \#14 Posted by: yelnats8j Posted at: 2017-10-01T22:01:13.216Z Reads: 25

```
i just notice the battery connectors get 3/4 of the way in the parallel connector then stop
```

---
## \#15 Posted by: GrecoMan Posted at: 2017-10-01T22:04:48.398Z Reads: 25

```
Wait wait... parallel connector?
```

---
## \#16 Posted by: yelnats8j Posted at: 2017-10-01T22:09:32.179Z Reads: 26

```
i think its a parallel connector
```

---
## \#17 Posted by: MysticalDork Posted at: 2017-10-01T22:11:34.953Z Reads: 27

```
post up a picture please.
```

---
## \#18 Posted by: yelnats8j Posted at: 2017-10-01T22:13:26.512Z Reads: 25

```
its a parallel i must of order the wrong thing
```

---
## \#19 Posted by: yelnats8j Posted at: 2017-10-01T22:14:09.309Z Reads: 25

```
this is probly what i should of ordered
https://www.amazon.com/Serial-Bullet-Battery-Adapter-Turning/dp/B01LYLI4KA/ref=sr_1_1?ie=UTF8&qid=1506895881&sr=8-1&keywords=4mm+hxt+bullet+connectors+series
```

---
## \#20 Posted by: GrecoMan Posted at: 2017-10-01T22:15:49.406Z Reads: 25

```
parallel should still be giving you 11 volts...

but series is what you need
```

---
## \#21 Posted by: yelnats8j Posted at: 2017-10-01T22:16:58.369Z Reads: 25

```
all right but that will that fix the vesc cant detect problem
```

---
## \#22 Posted by: MysticalDork Posted at: 2017-10-01T22:18:43.603Z Reads: 23

```
It will probably help, but it may not fix it entirely. even with just parallel, you should  be getting at least 11 volts, not 6.
```

---
## \#23 Posted by: yelnats8j Posted at: 2017-10-01T22:19:26.084Z Reads: 24

```
allright Thanks
```

---
## \#24 Posted by: Nix Posted at: 2017-10-02T01:47:57.532Z Reads: 19

```
The battery max is also only 25 amps...
```

---
