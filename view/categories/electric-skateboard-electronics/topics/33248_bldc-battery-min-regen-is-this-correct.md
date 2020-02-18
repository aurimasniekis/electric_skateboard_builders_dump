# BLDC Battery Min (Regen) - is this correct?

### Replies: 28 Views: 1432

## \#1 Posted by: rolexbene Posted at: 2017-09-16T07:09:57.636Z Reads: 209

```
I am trying to work out my correct battery min.

I have 2x 4s1p 20c 5000mah in series, to make an 8s battery.

Spec:
Configuration: 4S1P / 14.8v / 4Cell
Constant Discharge: 20C 
Peak Discharge (20sec): 30C
Max Charge Rate: 5c

So I have 8S1P correct, does this mean I can charge at 5c or 10c?

So lets say I can charge at 5C, should I set my Bat min regen to -5A, or is that 5C x 5A = -25C?
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2017-09-16T10:39:15.222Z Reads: 201

```
You are running your batteries in series so the 5000mah remains as the capacity with all the same limits. I would try around 2c first, so -10 to -12. If you are running dual then you need to use -5 to -6 for each vesc and go up from there if needed. This affects the brakes at higher speeds so test it and be cautious at first. Try it on flat ground. The recharge part will be fine, to me it's more about brakes.

Be safe and report back.
```

---
## \#3 Posted by: rich Posted at: 2017-09-16T10:49:31.020Z Reads: 188

```
Your max charge rate is still 5C (25A in your case), I would say you can set bat min regen up to to -20A. I have battery with max charge rate of 50A and my batt min regen is set to -40A (-20A on both vescs). Regenerative braking is not continious and probably you even won't reach the set limit in reality.
```

---
## \#4 Posted by: rolexbene Posted at: 2017-09-16T11:06:25.310Z Reads: 168

```
Thanks guys for you input, think I understand a bit more now. Just been out for a ride and set it to BLDC watt mode with settings:

Motor max: 60A
Motor min: -50A
Max battery: 50A
Min battery: -30A

Braking seems nice and responsive, although my belt was slipping quite a bit so might of been a bit harsh. Do you think these settings are safe for my battery setup. Running a 8s 270kv 60mm motor with focbox.
```

---
## \#5 Posted by: rich Posted at: 2017-09-16T11:27:09.477Z Reads: 151

```
Looks fine but I would not exceed -25A bat min. Belt skipping is annoying, I know :wink:, you could set the motor min to -30A or -40A. Which belt width do you use?
```

---
## \#6 Posted by: MontPierre Posted at: 2017-09-16T14:05:39.283Z Reads: 144

```
Try adjusting tension of the belt, looser or tighter. It's a matter of trying few possibilities until belt doesn't skip. You will eventually find correct tension. Also new vesc tool has breaking curve adjustment. I have used it to have breaks lighter an the begging and then stronger towards end of the throttle ( when pushed towards the end of reach). Now breaks work better, slight press of the throttle doesn't lock the wheel any more. It does lock the wheel when applied at full force but that's how it will work.
```

---
## \#7 Posted by: rolexbene Posted at: 2017-09-16T14:14:56.930Z Reads: 136

```
Yeah very annoying, mostly worried about wearing out the belt too quickly, just made some adjustments and seems to be good again. I think its just because I need some decent bolts to lock the motor down rather than little screws that are hard to get tight enough.
```

---
## \#8 Posted by: rolexbene Posted at: 2017-09-16T17:12:53.662Z Reads: 127

```
@rich belt is 15mm
```

---
## \#9 Posted by: rich Posted at: 2017-09-17T06:02:05.239Z Reads: 118

```
15mm is good. The best solution is an idler pulley (on the slack line) if you have enough space on your motor mount. The problem is, when you have too much belt tension, you could harm the bearings (wheel+motor). On my longboard I had 9mm belt and awful skipping so I tried it with a lot of tension but had to change the bearings of the driving wheel every week. Now I have a dual motor build with 15mm belts (not tight) and on hard brake there is still sometimes skipping.

Also check your pulleys, in my case it was a bad quality motor pulley, too. Look at this, compared to a proper one :joy:

<img src="/uploads/db1493/original/3X/8/2/82c8b2acb3b79880f6fefe4eef1245064a3b289d.jpg" width="690" height="388">
```

---
## \#10 Posted by: scepterr Posted at: 2017-09-17T06:22:52.150Z Reads: 105

```
The right combination will lock down every screw and pulley forever unless you use a torch 😉
<img src="/uploads/db1493/original/3X/4/4/44d5e12dc2883fc156f9a017237e2b0fee8a9cf7.jpg" width="375" height="499">
```

---
## \#11 Posted by: Menjos Posted at: 2017-09-17T08:58:28.441Z Reads: 99

```
I have some fully eroded windings on my torqueboards hub motors. Do I have a chance of getting the bolts to hold again with any of these?
```

---
## \#12 Posted by: scepterr Posted at: 2017-09-17T09:00:42.896Z Reads: 99

```
If you clean down to bare metal, use primer, yes
Loctite product catalog, a solution to any problem 😁 http://hybris.cms.henkel.com/medias/sys_master/catalogsync/catalogsync/9030422331422.pdf
```

---
## \#13 Posted by: Menjos Posted at: 2017-09-17T09:52:04.620Z Reads: 99

```
Cool thanks, I guess I can go for high strength? What is the primer for, to build the new winding surface? So I clean to bare metal first, insert primer, then the bolt to create the new winding, then loctite to keep it all in place? Sorry if this doesn't make sense.
```

---
## \#14 Posted by: scepterr Posted at: 2017-09-17T09:53:30.976Z Reads: 100

```
That catalog has step by step guides, it depends on what you're using when/how it's applied. 
<img src="/uploads/db1493/original/3X/a/c/acd88af51d13b6939a5828e17c557e6043dbd5ab.jpg" width="281" height="500">
```

---
## \#15 Posted by: pat.speed Posted at: 2017-09-17T11:42:57.161Z Reads: 91

```
Do you mean the thread on the bolt is worn out?
```

---
## \#16 Posted by: Menjos Posted at: 2017-09-17T12:19:36.703Z Reads: 89

```
No the bolts are fine, it's windings that are worn out. Two out of eight on the motor casing. So the bolts don't hold anymore.
<img src="/uploads/db1493/original/3X/f/7/f7485608d830787a995bcae7100a5cd6c31ffc25.jpg" width="374" height="500">
<img src="/uploads/db1493/original/3X/b/6/b6d26ca3d89b8e9fc58960afb0ecb86524b9d4ac.jpg" width="374" height="500">
```

---
## \#17 Posted by: scepterr Posted at: 2017-09-17T12:33:45.019Z Reads: 77

```
Getting that clean is gonna be a p.i.t.a
The threads are likely gunked up likely crazy
The thread that holds the screw is at the top or bottom of the screw? Or the whole length?
```

---
## \#18 Posted by: scepterr Posted at: 2017-09-17T12:37:12.282Z Reads: 82

```
Is this the whole thread that holds those screws?
<img src="/uploads/db1493/original/3X/1/8/1897ca9ce718b976e6c23a98aa03efc202e3d6a4.jpg" width="374" height="500">
```

---
## \#19 Posted by: Menjos Posted at: 2017-09-17T12:59:41.385Z Reads: 75

```
Yes correct!
```

---
## \#20 Posted by: scepterr Posted at: 2017-09-17T13:02:14.709Z Reads: 76

```
Oh ok, cleaning shouldnt be that bad then.
```

---
## \#21 Posted by: Menjos Posted at: 2017-09-17T13:54:11.155Z Reads: 68

```
Yes those threads only hold the bottom of the screw
```

---
## \#22 Posted by: pat.speed Posted at: 2017-09-17T21:11:09.674Z Reads: 65

```
Yes that is what I was meaning sorry about not being clear. Locktite will hold that in if you use some strong stuff just make sure you don't have to try and get it back out once you use it
```

---
## \#23 Posted by: Menjos Posted at: 2017-09-18T17:11:01.341Z Reads: 63

```
OK cool yeah once they hold I don't intend to open them again. I wish I had known before that this is another week point of these to torqueboards motors. However, I'm not quite sure how I am supposed to tighten the bolts in the threads. Do I fill in the loctite, wait for it to harden, and then tighten the bolt?
```

---
## \#24 Posted by: rolexbene Posted at: 2017-09-18T20:06:34.965Z Reads: 61

```
[quote="Menjos, post:23, topic:33248"]
supposed
[/quote]

So my setup is running almost sweet. My problem is that I keep getting ABS_OVER_CURRENT Fault.

Can anyone tell me what could be causing this?

<img src="/uploads/db1493/original/3X/a/9/a9bcd9e667faf3ab2b846f792934d7347874ccbf.jpeg" width="281" height="500">
```

---
## \#25 Posted by: pat.speed Posted at: 2017-09-18T21:07:56.724Z Reads: 56

```
What normally happens is you would put locktite on the bolt and the hole that it's going into the tighten it in and let it sit for a day or two to harden then it should be good. Look on hobby kind for thread locker it's really cheap
```

---
## \#26 Posted by: Menjos Posted at: 2017-09-20T08:42:31.600Z Reads: 57

```
OK but my problem is this: the thread inside the hole is fully eroded - gone! So I cannot tighten the bolt, there is zero grip. The method you're describing is what I should have done in the first place to prevent this from happening. I will experiment with adding material inside the hole, like little strings of copper wire.
```

---
## \#27 Posted by: Menjos Posted at: 2017-09-20T08:59:21.422Z Reads: 59

```
Sorry man for highjacking your post! I would set battery currents as low as possible, and work yourself up to what you really need, to avoid stressing your components more than necessary. I'm running my battery min at 2x 4A and motor min at  2x 30A (dual VESC, 10s2p 25r), I used to run 2x 3A and 2x 25A and even that was giving me quite reasonable braking power (hubs). My bat max is at 2x11A to tame the beast slightly, still gets me plenty of torque and 40kmh max speed. I try to make it a habit of only braking or accelerating hard when necessary. That way the motors and batteries will stay cooler and live longer.
```

---
## \#28 Posted by: pat.speed Posted at: 2017-09-20T12:57:37.255Z Reads: 53

```
Ahhh what you might have to do is re tap the thread with a larger bolt size and use a larger bolt if you can
```

---
