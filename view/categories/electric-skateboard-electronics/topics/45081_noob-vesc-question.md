# Noob VESC question

### Replies: 17 Views: 641

## \#1 Posted by: Freddiecook Posted at: 2018-01-30T21:01:46.322Z Reads: 124

```
Hey guys, still relatively new here so please bare with me :wink: basically last year I decided I was going to build a board and bought most of the electronics but ditched the project for a while as I had no time, fast forward to now and I've started to pick the project up again and am finishing the rest of the build. My question is that I want to run my system in FOC preferably and last year I bought a dual VESC 4 from enertion, just wondering if I should upgrade to the FOCBOXs or if I should use what I have. I ask because I have read a lot of threads about FOC being a bit sketchy on the older models.
Many thanks, Freddie
```

---
## \#2 Posted by: Der6FingerJo Posted at: 2018-01-30T21:03:31.347Z Reads: 122

```
That depends, among other factors, on the rest of the system you are running. What about your Battery and Motor? Generally lower kv is better for FOC afaik.
```

---
## \#3 Posted by: GrecoMan Posted at: 2018-01-30T21:03:37.797Z Reads: 119

```
don’t use foc on those vescs. use bldc and pick up some focboxes off someone
```

---
## \#4 Posted by: Freddiecook Posted at: 2018-01-30T21:04:43.424Z Reads: 114

```
Getting a 10s4p pack from samsung 25r cells
running dual 170kv motors
```

---
## \#5 Posted by: Freddiecook Posted at: 2018-01-30T21:05:10.790Z Reads: 104

```
Yeah that's what I thought the general consensus would be :smile:
```

---
## \#6 Posted by: Steve-81 Posted at: 2018-01-30T21:06:34.562Z Reads: 101

```
I red a lot on here, most people using FOC on 4,10 - 4,12 have problems in a 12s configuration. In case of 10s and lower nearly no problems by most users.

I'm going do solder my own 4.12, and I think it will be fine with FOC on a 10s battery :slight_smile:
```

---
## \#7 Posted by: Der6FingerJo Posted at: 2018-01-30T21:07:03.749Z Reads: 97

```
Wouldn't risk it either with this setup. 170 is a bit high.
```

---
## \#8 Posted by: GrecoMan Posted at: 2018-01-30T21:09:14.458Z Reads: 95

```
170kV with 10s? that’s extremely low
```

---
## \#9 Posted by: Freddiecook Posted at: 2018-01-30T21:11:24.894Z Reads: 95

```
You thinking I won't get enough torque? :thinking:
```

---
## \#10 Posted by: Der6FingerJo Posted at: 2018-01-30T21:14:00.065Z Reads: 94

```
I meant for FOC, I only know of @Rich who successfully ran 10S FOC on standard 4.12 with 130kv. I myself popped a drv at 10S 168kv during regular low speed cruising. 

@Freddiecook 170kv on 10s should be fine for torque in most circumstances and if you aren't very heavy and/or in a hilly area
```

---
## \#11 Posted by: Freddiecook Posted at: 2018-01-30T21:16:46.508Z Reads: 90

```
ahh okay, I see enertion is still waiting for more FOCBOXes :smile: , anyone know of any other cheap/reputable suppliers? Forgot to add I'm in the UK
```

---
## \#12 Posted by: Surfer Posted at: 2018-01-30T21:45:28.423Z Reads: 78

```
Check it out this:
https://www.electric-skateboard.builders/t/eu-2x-esk8-de-controller-1-1-vesc/45070
@telnoi
```

---
## \#13 Posted by: Freddiecook Posted at: 2018-01-30T21:48:38.748Z Reads: 74

```
Thanks man, interested :wink:
```

---
## \#14 Posted by: b264 Posted at: 2018-01-30T22:17:45.217Z Reads: 73

```
[quote="GrecoMan, post:8, topic:45081, full:true"]
170kV with 10s? that’s extremely low
[/quote]

It's *on the low end* but I definitely wouldn't say "extremely low"

I have a dual running 140kv on 10S

I'd say 120kv is "extremely low" for 10S

Some people gotta have da power and don't go over 25mph anyway
```

---
## \#15 Posted by: telnoi Posted at: 2018-01-31T06:19:23.687Z Reads: 60

```
Let me know. Esk8.de tested their controllers rigurously with FOC/10s on mountainboards. They are most certainly capable. 

Only reason I used bldc is because the vesc tool at the time had sketchy braking in FOC mode (with all vesc).
```

---
## \#16 Posted by: sash Posted at: 2018-01-31T07:17:31.379Z Reads: 54

```
I think you'll get plenty of torque.

Lower kv = Less top speed = More torque

I am running 190kv motors with 10S battery, and I can climb any hill I can find.   Even with a single motor, I can go up many hills.
```

---
## \#17 Posted by: rich Posted at: 2018-01-31T17:53:18.394Z Reads: 33

```
I don't know enertion but I can confirm that HW4.12 from esk8.de is reliable for FOC with new FW. It should be safe with 170kv, it's a fair offer from @telnoi for the 1.1 controller.

It depends on your gearing and wheel size how much torque the 170kv motors can deliver.
```

---
