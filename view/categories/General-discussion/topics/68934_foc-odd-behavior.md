# FOC odd behavior

### Replies: 17 Views: 286

## \#1 Posted by: Jmding Posted at: 2018-09-23T07:06:17.188Z Reads: 124

```
I'm getting really weird behavior in FOC mode where throttle causes the board to brake instead of accelerate.

Everything works perfectly in BLDC mode. 

After writing an FOC config, while bench testing under no load, throttle causes the wheels to spin up as normal. While riding though, when I engage the throttle it actually causes the board to brake. When I engage the brakes, it also brakes (so it's not an inverted controller config). Any idea what's going on? 

Flipsky 6.6, stock firmware 
Current no reverse with breaks 
FOC
```

---
## \#2 Posted by: dareno Posted at: 2018-09-23T08:51:31.555Z Reads: 112

```
This might be a stupid question but are both wheels spinning in the same direction?
```

---
## \#3 Posted by: Andy87 Posted at: 2018-09-23T09:12:00.565Z Reads: 106

```
Strange that it works in bldc and foc no.
You run your esc via CAN or split ppm?
Did you already go through the FOC motor detection on both again? Maybe it helps just to refresh it.
Check that your remote is fully charged, right adjusted and the fail safe is set right too.
```

---
## \#4 Posted by: Silverline Posted at: 2018-09-23T09:50:49.193Z Reads: 98

```
What motors ?
```

---
## \#5 Posted by: Jmding Posted at: 2018-09-23T13:12:28.424Z Reads: 87

```
One motor only, 6374 sk3 200kv
Ppm yeah, went through motor detection a couple times. Remote is charged, working fine on BLDC
```

---
## \#6 Posted by: Andy87 Posted at: 2018-09-23T16:05:34.324Z Reads: 76

```
Still don’t understand why it’s in bldc functioning.
For me it sounds more like a connection issue with the remote. Did you try a other remote or position of the receiver?
```

---
## \#7 Posted by: Jmding Posted at: 2018-09-23T16:37:48.411Z Reads: 72

```
To be clear, I'm saying that when I have it configured to BLDC mode, it works fine and is totally rideable.  That's why I'm pretty confident it's not a receiver issue.  When I reconfigure to FOC, that's when it starts braking instead of throttling.
```

---
## \#8 Posted by: Trdolan03 Posted at: 2018-09-23T17:14:16.308Z Reads: 66

```
What remote?
```

---
## \#9 Posted by: Jmding Posted at: 2018-09-24T02:26:46.824Z Reads: 54

```
this one

![image|225x224](upload://nmIFd3Gj8hc0JToxgX5wi9FDN1G.jpeg)
```

---
## \#10 Posted by: rey8801 Posted at: 2018-10-23T07:41:46.735Z Reads: 43

```
Hi man! Did you perhaps solve it? Yesterday I configured the new Flipsky 6.6. Motors right direction in BLDC sensorless but a lot of rattle at the beginning (I already used these motors at 10s no problem, now 12s and vesc 6.6), so moved to FOC and they spin in the other direction...@Ackmaniac firmware. I will try to swap the motors wires because I tired just by reverse the motor directionninbthebvesc tool. It does the trick but then after acceleration if I brake gently the motors don't brake but keep spinning really slow, engaging the brake more stops the motors from spin. So weird!
```

---
## \#11 Posted by: Dudek Posted at: 2018-10-23T13:19:15.583Z Reads: 29

```
yeah
it happend to me to
my board went from full throttle to full break in a split second and send me flying
I run maytech remote, two maytech 100A VESC and two 6374 motors in FOC, 12s lipo
firs I thought it was my gloves, some how they got stuck on remote
but it happened few times on the same trip
there seems to be direct correlation between applied throttle and brake
i.e. it will reverse the same amount of throttle to brake
I run my board since september and It never happened before

this is serious problem if you like riding at speed
as its give you no time to bail !!!

any thoughts ??????????????????????????
```

---
## \#12 Posted by: rey8801 Posted at: 2018-10-23T13:28:05.984Z Reads: 28

```
That's scary!
I think what you have is a different behaviour than what I meant. In my case if after acceleration I use the brake gently they motors don't stop but keep cruising at really low speed. In your case seems that there is no too much range between acceleration and brakes. Maybe try to redo the remote mapping. Once I had similar behaviour and then realised that I did the mapping with the remote in slow mode. I am not saying that this is your case but maybe it will help. You can also adjust the braking curve if you use @Ackmaniac's Firmware
```

---
## \#13 Posted by: Jmding Posted at: 2018-10-23T15:11:50.966Z Reads: 24

```
For me, I recalibrated the FSESC with the motor by itself and that fixed it.
```

---
## \#14 Posted by: rey8801 Posted at: 2018-10-23T15:12:24.629Z Reads: 23

```
What do you mean with by itself?
```

---
## \#15 Posted by: Jmding Posted at: 2018-10-23T15:12:56.052Z Reads: 21

```
Make sure the belt isn't connected
```

---
## \#16 Posted by: rey8801 Posted at: 2018-10-23T15:13:33.909Z Reads: 22

```
Ah ok, no I am using hub motors. Same motors I used in the past. I will redo the process this evening and see it.
```

---
## \#17 Posted by: Dudek Posted at: 2018-10-23T19:55:16.975Z Reads: 13

```
I got over 200 miles on this board probably 100 miles with maytech remote and never had any problems
I've instaled bluetooth recently, but this will not cose problems like this ??????

I did reset controller settings and added traction between esc
I can set up motors from beginning
but this expierience put me off fast riding until I will fully test it
I wan't giet to bottom of this so it will never happend again
this board goes really fast and I fell really hard...
```

---
