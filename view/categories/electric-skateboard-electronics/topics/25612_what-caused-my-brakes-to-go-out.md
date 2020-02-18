# What caused my brakes to go out?

### Replies: 20 Views: 1088

## \#1 Posted by: oct0f1sh Posted at: 2017-06-18T05:39:17.197Z Reads: 121

```
So I just completed my dual motor build and I took it out for a test ride around my neighborhood. As I was going down one of the hills the brakes started and after about two seconds they went out completely. Thankfully I was able to jump off before I fell but the board hit a curb and flipped over a couple times, but it was pretty dang scary. I'd **really** like to figure out why this happened and fix it before I move to San Francisco where I'd prefer not to die going down the hills. These are the settings I was able to grab from the BLDC tool:
<img src="/uploads/db1493/original/3X/5/4/5421635864ba5687fff2f6974af3c6adebb6b14d.png" width="690" height="385"><img src="/uploads/db1493/original/3X/a/0/a0c6517c903caafcf9941633da7feb10f27268a2.png" width="690" height="385"><img src="/uploads/db1493/original/3X/7/c/7ceea6179141cc22a718836a5f07ec3c79763b8c.png" width="690" height="385">

While I was putting the board together I noticed that both of the motors didn't brake at the same speed, I would go full throttle and then full brake but one of the motors came to a complete stop much before the other. I've checked multiple times to make sure that both VESCs are configured with the same settings and everything seems to match up, I just assumed that it was because one of the motors was reused from a previous build and one of them was brand new, both 6355 torqueboards motors. I'm using a 10S4P battery.
```

---
## \#2 Posted by: Namasaki Posted at: 2017-06-18T06:03:30.838Z Reads: 112

```
first of all put the max input voltage back to the default setting of 57v
```

---
## \#3 Posted by: oct0f1sh Posted at: 2017-06-18T06:07:24.663Z Reads: 111

```
Even for a 10S4P battery? I'm not really sure how a lot of this stuff works...
```

---
## \#4 Posted by: Namasaki Posted at: 2017-06-18T06:07:55.975Z Reads: 110

```
Yes, even for a 6s battery
```

---
## \#5 Posted by: oct0f1sh Posted at: 2017-06-18T06:08:33.535Z Reads: 107

```
Ok I'll do that. Would that affect the braking at all?
```

---
## \#6 Posted by: Namasaki Posted at: 2017-06-18T06:09:02.098Z Reads: 106

```
Vesc Rule Number 1
Don't change any default settings that you don't understand
```

---
## \#7 Posted by: oct0f1sh Posted at: 2017-06-18T06:09:34.377Z Reads: 108

```
That's a rule I think I can live by.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-06-18T06:09:53.270Z Reads: 108

```
I think I've heard of others having the same problem when they lower the max input voltage
```

---
## \#9 Posted by: Namasaki Posted at: 2017-06-18T06:10:54.798Z Reads: 109

```
And are you running FOC or BLDC?
Because you have BLDC selected on the first motor page

Here is a link to Vedder's webpage with lots of info on vesc settings
http://vedder.se/2015/01/vesc-open-source-esc/
```

---
## \#10 Posted by: oct0f1sh Posted at: 2017-06-18T06:36:11.572Z Reads: 104

```
I'm running BLDC. I tried to run on FOC hybrid but every time I connect my sensor wires to either of my VESCs it disconnects from the BLDC tool and I can't get it to reconnect without unplugging the sensor wires.
```

---
## \#11 Posted by: Jinra Posted at: 2017-06-18T06:41:16.559Z Reads: 99

```
Sounds like your sensor wires are hooked up wrong. You didn't apply your motor detection values, after detection you have to hit "apply" AND "write config". If you want a reliable system stick with just BLDC.
```

---
## \#12 Posted by: oct0f1sh Posted at: 2017-06-18T06:47:29.903Z Reads: 98

```
Thanks! I think I probably will just avoid FOC then.
```

---
## \#13 Posted by: Hummie Posted at: 2017-06-18T07:10:01.865Z Reads: 95

```
bet it was when you were braking and you had your max voltage at 42 the regen spiked it up and brought it beyond that.
```

---
## \#14 Posted by: oct0f1sh Posted at: 2017-06-18T07:21:39.177Z Reads: 93

```
Oh ok, that makes sense. I've changed the max voltage to 57 so hopefully that'll fix it.
```

---
## \#15 Posted by: Namasaki Posted at: 2017-06-18T19:33:53.847Z Reads: 76

```
That was my thought as well and that raises a question. Why isn't there some sort of voltage regulation on the regen braking?
```

---
## \#16 Posted by: Hummie Posted at: 2017-06-18T23:04:29.680Z Reads: 66

```
maybe it's decided by how high you set the regen then the voltage maybe follows.  so if you set a low regen maybe the spike wouldn't be as high.  a total guess.  other guess being it's determined by your rpm when you brake.
```

---
## \#17 Posted by: Ackmaniac Posted at: 2017-06-18T23:33:54.117Z Reads: 61

```
Thought already about a automatic regulation of the voltage when it goes too high at braking. 
But finally it doesn't make sense to have that.

Because normally your system should not reach this high voltages. It only touches them when something is wrong. For example when the BMS cuts off because the charge voltage us too high during braking. But in this case there is nothing the vesc can do about it. 
The value should not be editable. Only makes sense to change it when you vesc components can't handle 60V.
```

---
## \#18 Posted by: JdogAwesome Posted at: 2017-06-18T23:52:37.129Z Reads: 57

```
Hey @oct0f1sh thought I'd chime in cause I'm having the same problem. I personally have a Carvon Single Hub running 6S and am using a GT2B remote in a BadWolf housing. Pretty much with my GT2B I had to adjust my  minimum and maximum pulsewidth to make it so my center throttle would actually be center. But what that means is that when I push my trigger all the way up to fully brake, it goes under 1ms pulsewidth down to 0.8 which the VESC takes as having no input and just stops braking as if the controller lost signal. I'm not sure how I'm gonna fix this yet but maybe your having the same issue.
```

---
## \#19 Posted by: Ackmaniac Posted at: 2017-06-18T23:58:30.161Z Reads: 56

```
Just use my firmware mod where you can set a center pulsewidth position and by that you can set the brake pulse width to the real value.
```

---
## \#20 Posted by: lrdesigns Posted at: 2017-06-19T05:29:31.585Z Reads: 36

```
I had same issue with my GT2B in a babybuffalo case. Ackmaniac's firmware was the only proper way to fix it. Or you can add a physical bump stop to prevent the trigger being pushed all the way in. I think the adjustable end points is one of the greatest things about his firmware. Really should be a standard feature. If your in this situation  going down a hill you can move the brake back to the mid area and the breaking will come back.
```

---
