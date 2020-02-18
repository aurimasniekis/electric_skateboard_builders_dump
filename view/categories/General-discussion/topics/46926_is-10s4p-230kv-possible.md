# Is 10s4p 230kv possible?

### Replies: 28 Views: 1049

## \#1 Posted by: GJHS Posted at: 2018-02-20T06:54:25.212Z Reads: 95

```
Hey guys,  

I have a twin 230kv motor setup with a 10s4p battery.  I was originally told the motors were 190kv before buying, though they are marked 230kv.  I get different opinions on whether i will blow up my FOCboxes with this setup.

Thanks
```

---
## \#2 Posted by: b264 Posted at: 2018-02-20T06:56:06.074Z Reads: 95

```
Set a maximum erpm in the ESC settings
```

---
## \#3 Posted by: Jebe Posted at: 2018-02-20T06:57:18.336Z Reads: 92

```
Set erpm max to 60 000. Will be fine.
```

---
## \#4 Posted by: GJHS Posted at: 2018-02-20T06:58:31.503Z Reads: 89

```
Uncheck limit ERPM with Negative torque? Is anyone running a similar setup?  Does gearing matter?
```

---
## \#5 Posted by: Jebe Posted at: 2018-02-20T06:59:36.588Z Reads: 86

```
Best do some more research bud. Can blow vescs up if you arent careful. Some great tutorials on youtube.
```

---
## \#6 Posted by: b264 Posted at: 2018-02-20T06:59:48.667Z Reads: 87

```
http://calc.esk8.today/advanced/

drop efficiency to 85%

try 15T / 36T pulleys
```

---
## \#7 Posted by: b264 Posted at: 2018-02-20T07:01:44.191Z Reads: 83

```
keep max erpm below 60,000
```

---
## \#8 Posted by: scepterr Posted at: 2018-02-20T07:01:54.286Z Reads: 83

```
I would adjust gearing and wheel size to keep it below 60k erpm vs software limiting
```

---
## \#9 Posted by: GJHS Posted at: 2018-02-20T07:02:03.582Z Reads: 76

```
My setup shows max erpm 57960.00
```

---
## \#10 Posted by: scepterr Posted at: 2018-02-20T07:03:09.244Z Reads: 74

```
You could exceed that downhill and really not the place you want throttle limiting to kick in
```

---
## \#11 Posted by: CarlCollins Posted at: 2018-02-20T07:03:57.599Z Reads: 73

```
Why don't you replace your motors with 190 KV ones?
```

---
## \#12 Posted by: GJHS Posted at: 2018-02-20T07:04:53.928Z Reads: 73

```
is there a way to test kv?
```

---
## \#13 Posted by: CarlCollins Posted at: 2018-02-20T07:08:53.793Z Reads: 72

```
@GJHS I am not sure but you can try following these steps mentioned here: http://fishpepper.de/2017/10/17/tutorial-how-to-measure-the-kv-of-a-brushless-motor/
```

---
## \#14 Posted by: pat.speed Posted at: 2018-02-20T07:09:41.920Z Reads: 69

```
There is a thread on this forum, it can be measured with the vesc
```

---
## \#15 Posted by: CarlCollins Posted at: 2018-02-20T07:10:10.483Z Reads: 69

```
@pat.speed

Can you please link that post?
```

---
## \#16 Posted by: GJHS Posted at: 2018-02-20T07:11:28.303Z Reads: 68

```
BTW Thanks for your help before @CarlCollins
```

---
## \#17 Posted by: pat.speed Posted at: 2018-02-20T07:13:44.883Z Reads: 64

```
https://www.electric-skateboard.builders/t/realistic-kvs-and-you/23346
```

---
## \#18 Posted by: CarlCollins Posted at: 2018-02-20T07:15:24.507Z Reads: 63

```
It's my pleasure :slight_smile:
```

---
## \#19 Posted by: CarlCollins Posted at: 2018-02-20T07:15:34.382Z Reads: 60

```
Thanks man
```

---
## \#20 Posted by: pat.speed Posted at: 2018-02-20T07:16:21.719Z Reads: 58

```
What branded motors do you have?
```

---
## \#21 Posted by: GJHS Posted at: 2018-02-20T07:19:30.438Z Reads: 54

```
They are KALY motors.  I was just chatting with @scepterr and he believes they are closer to 190kv.  I would like to confirm
```

---
## \#22 Posted by: CarlCollins Posted at: 2018-02-20T07:20:49.893Z Reads: 52

```
If possible, can you please click an image and share it with us?
```

---
## \#23 Posted by: CarlCollins Posted at: 2018-02-20T07:21:51.203Z Reads: 53

```
It looks like one of these?
http://www.electric-skateboard.builders/uploads/db1493/original/3X/6/b/6b9349c70a2dd651b550f79de9014b9c995a273c.JPG
```

---
## \#24 Posted by: GJHS Posted at: 2018-02-20T07:23:41.362Z Reads: 56

```
Yes Exactly
```

---
## \#25 Posted by: scepterr Posted at: 2018-02-20T07:23:43.121Z Reads: 55

```
Sorry 200-210
[quote="Jinra, post:1, topic:23346"]
Kaly’s 230kv motor = 200-210kv calculated (20 samples)
[/quote]

https://www.electric-skateboard.builders/t/realistic-kvs-and-you/23346/5?u=scepterr
```

---
## \#26 Posted by: CarlCollins Posted at: 2018-02-20T07:24:31.277Z Reads: 51

```
Thank you for the results. @GJHS I think you need 190 KV motors.
```

---
## \#27 Posted by: GJHS Posted at: 2018-02-20T07:26:01.205Z Reads: 50

```
According to @scepterr post, I am good, right?
```

---
## \#28 Posted by: b264 Posted at: 2018-02-20T08:24:21.727Z Reads: 45

```
You might be good, just keep your gear ratios so your max erpm never goes above 60k.
```

---
