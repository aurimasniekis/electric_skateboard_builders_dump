# Finished build - APS 6374 3.2kw &amp; VESC \[need advices\]

### Replies: 16 Views: 1092

## \#1 Posted by: mclightning Posted at: 2016-09-14T08:25:44.387Z Reads: 149

```
Hi everyone!

I just finished and did some test rides on my skateboard.

Here is a video of it on street : https://www.instagram.com/p/BKTNTW6hKJP/
Setup under the board : https://www.instagram.com/p/BKTI5wjBwH4
3D printed failed designs vs final : https://www.instagram.com/p/BKULkyAB31I/

Advices needed on :

1 - Should I connect my lipos in parallel or serial if I am satisfied with speed?
I have 2 3s 5000mah Zippy Compact batteries that I have been using with my drone. Now I ran the board with 1 3S battery. Speed is not impressive but it feels safer. I care more about range. I want to get 15km range.
 
2 - Is there a remote control app for Android?
I want to control with my phone. I don't want to carry an extra remote. I have quite a few BT UART modules that I have been using with my other DIY hobbies.

3 - Any settings which are MUST BE configured before running any tests?
Max Amp draw? Max Voltage? etc. Any setting that can ruin my electronics if I keep running it.  

Best Regards,
Ahmet
```

---
## \#2 Posted by: DeathCookies Posted at: 2016-09-14T09:00:50.494Z Reads: 132

```
[quote="mclightning, post:1, topic:9578"]
1 - Should I connect my lipos in parallel or serial if I am satisfied with speed?I have 2 3s 5000mah Zippy Compact batteries that I have been using with my drone. Now I ran the board with 1 3S battery. Speed is not impressive but it feels safer. I care more about range. I want to get 15km range
[/quote]

If you change the from parallel to series you will get more speed but in both configuration you will get the same distance. (W = U * I)
[quote="mclightning, post:1, topic:9578"]
2 - Is there a remote control app for Android?I want to control with my phone. I don't want to carry an extra remote. I have quite a few BT UART modules that I have been using with my other DIY hobbies.
[/quote]



http://www.instructables.com/id/Electric-Skateboard-v20/?ALLSTEPS
At the bottom is an instruction for making one.[quote="mclightning, post:1, topic:9578"]
3 - Any settings which are MUST BE configured before running any tests?Max Amp draw? Max Voltage? etc. Any setting that can ruin my electronics if I keep running it.
[/quote]

Do you use a VESC or a normal ESC. If you use a normal ESC you dont need to set up anything except lipo count ;)
```

---
## \#3 Posted by: mclightning Posted at: 2016-09-14T09:07:16.547Z Reads: 119

```
Thank you so much for all detailed answers!

I am using VESC. Are there any must setups?
I plan to do advanced setups like regen later.
```

---
## \#4 Posted by: DeathCookies Posted at: 2016-09-14T09:23:11.367Z Reads: 114

```
[quote="mclightning, post:3, topic:9578"]
Are there any must setups?
[/quote]

* Motor Max
* Motor Min
* Battery Max
* Battery Min
* Battery Cutoff start
* Battery Cutoff end
* PPM bandwith
```

---
## \#5 Posted by: mclightning Posted at: 2016-09-14T09:38:54.582Z Reads: 112

```
Do I need to connect balance plug onto VESC as well?

My motor is this:
http://alienpowersystem.com/shop/brushless-motors/alien-6374-outrunner-brushless-motor-240kv-3200w/

It doesn't show any minimum ampere value on spec. How can I determine that value?
```

---
## \#6 Posted by: kampfhahn Posted at: 2016-09-14T09:44:56.360Z Reads: 106

```
[quote="DeathCookies, post:2, topic:9578"]
If you change the from parallel to series you will get more speed but in both configuration you will get the same distance. (W = U * I)
[/quote]

Just to mention the obvious: The range will only be the same when you ride with the same average speed in both setups (parallel / series).
```

---
## \#7 Posted by: DeathCookies Posted at: 2016-09-14T11:12:12.255Z Reads: 95

```
Not really. When you drive faster you will get there quicker but the range is more or less the same!
```

---
## \#8 Posted by: DeathCookies Posted at: 2016-09-14T11:13:22.112Z Reads: 98

```
[quote="mclightning, post:5, topic:9578"]
It doesn't show any minimum ampere value on spec. How can I determine that value?
[/quote]

Minimum amp is for braking. You can either set it like the max amp value or if you want less braking just lower the value.

But generally you can set it to the max amp value ;)
```

---
## \#9 Posted by: kampfhahn Posted at: 2016-09-14T11:50:48.622Z Reads: 87

```
Mainly due to higher air resistance doubling the speed will at least quadruple the amount of energy you need to ride a distance of x miles, even at these low 3-6s speeds. That´s why the 108 Wh max. get drained more than twice the fast riding with double the speed. It´s the same with cars btw.
```

---
## \#10 Posted by: mason Posted at: 2016-09-14T11:55:45.100Z Reads: 85

```
you should replace the 3d printed motor pulley with a steel or aluminum one. I think it will break down easily
```

---
## \#11 Posted by: DeathCookies Posted at: 2016-09-14T12:29:04.870Z Reads: 82

```
Thanks for the clarification! Yeah thats right. But if he want to get the most range he could go either way and ride the same speed. That way there will be no additional resistance :D
```

---
## \#12 Posted by: kampfhahn Posted at: 2016-09-14T12:33:57.345Z Reads: 81

```
[quote="DeathCookies, post:11, topic:9578"]
But if he want to get the most range he could go either way and ride the same speed. That way there will be no additional resistance
[/quote]

That´s right and exactly what i´ve written before. Like you i would @mclightning totally recommend putting the two batterys in series just to have that reserve of speed.
```

---
## \#13 Posted by: mclightning Posted at: 2016-09-14T12:55:46.358Z Reads: 79

```
Do you guys know if it is possible just attach an UART bluetooth module onto UART port on VESC?

I don't want to waste an Arduino board as done in linked instructables project. I believe it must be possible to give commands directly through UART.
```

---
## \#14 Posted by: DeathCookies Posted at: 2016-09-14T13:06:45.762Z Reads: 79

```
It is definitively possible but there is no app at the moment... You would have to program it yourself.
```

---
## \#15 Posted by: mclightning Posted at: 2016-09-14T13:09:00.050Z Reads: 78

```
I will give it a try, something very simple. Just to control throttle with a slider.

If I succeed, I will share here.
```

---
## \#16 Posted by: mclightning Posted at: 2016-09-14T13:18:55.407Z Reads: 76

```
yes it broke down around 9 times. I made a lot of optimizations, now the printed piece seems to hold pretty good.

%100 infill, 1.2 mm shell thickness, printed ABS at 245 degrees
```

---
