# Poll: What ⚡️ voltage do you primarily run?

### Replies: 18 Views: 1288

## \#1 Posted by: Michaelinvegas Posted at: 2016-08-30T23:23:17.808Z Reads: 121

```
What Voltage is your primary Esk8 ride running?

[poll]
 
 - 6s
 - 8s
 - 10s
 - 12s
 - Other

[/poll]
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-30T23:26:17.567Z Reads: 117

```
10s master race! Though I've been considering going 8s5p for higher discharge rate with the same amount of cells as 10s4p
```

---
## \#3 Posted by: Hillso Posted at: 2016-08-31T00:04:17.292Z Reads: 108

```
why would you like to do that? I mean you will get same wattage from battery, unless the esc have low amp limit, than you will get lower wattage.
```

---
## \#4 Posted by: Jinra Posted at: 2016-08-31T00:05:52.151Z Reads: 96

```
It's for higher discharge rate which will wear the cells down at a slower rate. The further you are away from max continuous discharge, the better.
```

---
## \#5 Posted by: Hillso Posted at: 2016-08-31T00:08:54.069Z Reads: 95

```
I don't think the amps alone matters, the watt gives you power. so it will be the same watt per amp per cell
```

---
## \#6 Posted by: Jinra Posted at: 2016-08-31T00:09:53.285Z Reads: 89

```
I'm not talking about the wattage. I'm talking about discharge rate.. It has nothing to do with supplied power (wattage)
```

---
## \#7 Posted by: Hillso Posted at: 2016-08-31T00:30:39.589Z Reads: 85

```
What i'm saying is I think you will discharge your cells at the same rate as if with less parallel cells, because you will need more amps to get to the same power.
```

---
## \#8 Posted by: Jinra Posted at: 2016-08-31T00:34:41.197Z Reads: 79

```
I'm sure I'll use more current in some scenarios, but I'll generally be far away from max continuous draw most of the time. In this case, it'd be more beneficial to have the additional head room of +20A discharge.
```

---
## \#9 Posted by: JuniorPotato93 Posted at: 2016-08-31T00:38:57.388Z Reads: 76

```
I went straight to 8S6P mainly because I have no idea what I was thinking but also because the motors I could get my hands on were 260 kv sk3s. And I wanted long range.
```

---
## \#10 Posted by: Jinra Posted at: 2016-08-31T00:42:30.941Z Reads: 72

```
I would love to run the SK3 260 6354 in 8s! Too bad HK is always out of stock.
```

---
## \#11 Posted by: JuniorPotato93 Posted at: 2016-08-31T00:44:47.189Z Reads: 72

```
I had the option to back order and wait. Is that not a thing? Ended up waiting a month and a bit  before I got a notification that they were being shipped.
```

---
## \#12 Posted by: Jinra Posted at: 2016-08-31T00:45:22.384Z Reads: 67

```
My backorder button is unclickable. It's okay though, I'd rather run sensored anyway.
```

---
## \#13 Posted by: Namasaki Posted at: 2016-08-31T00:45:59.086Z Reads: 66

```
But with higher voltage, you need less amps for same power.
```

---
## \#14 Posted by: JuniorPotato93 Posted at: 2016-08-31T00:52:04.350Z Reads: 62

```
On my next build I'm thinking I'll go sensored.  Have you ride both? Any noticeable differences in performance or feel in your opinion?
```

---
## \#15 Posted by: Jinra Posted at: 2016-08-31T00:54:39.269Z Reads: 64

```
I've tried both and I like sensored (hybrid) more if you're running a VESC. Starting from dead stop smoothly everytime is pretty nice. I never cog with it compared to sensorless. It does leave more room for error though. For instance, My sensor wire became a little loose and made my motor completely unresponsive until it hit the sensorless eRPM threshold in which it just run sensorless fine.

As long as you check your connections, you'll have a blast in sensored! I wouldn't run it on a hobby ESC as it's not as efficient at high speeds and made my motors pretty toasty when I ran it pure sensored.

@Namasaki See my post above

"I'm sure I'll use more current in some scenarios, but I'll generally be far away from max continuous draw most of the time. In this case, it'd be more beneficial to have the additional head room of +20A discharge."
```

---
## \#16 Posted by: JuniorPotato93 Posted at: 2016-08-31T01:06:42.265Z Reads: 60

```
I will be running 2 SK3s on chakas VESCs once I get those bad boys in. It's the last thing I need, as well as an e-switch which I'm getting from him as well.  Then I was planning to post my build thread and then probably immediately after post my first trouble shoot thread too 😂
```

---
## \#17 Posted by: lox897 Posted at: 2016-08-31T06:04:37.233Z Reads: 46

```
Running 6S on my one and only board right now. Collecting parts for my second build which will be 10/12S
```

---
## \#18 Posted by: Okami Posted at: 2016-08-31T06:12:35.331Z Reads: 46

```
I think @Jinra brought up an interesting topic.. whenever to go for 8s or 10s, if the count of elemenets (cells) does not change. Perhaps, @chaka could answer this question better but viewing it from theoretical side for me it looks like this: 


 ---
With 8s and 5p config, you gonna have ~100A discharge capability, while with 10s 4p you got 80a discharge capabilty, which would translate to roughly 28.8v (nominal) x 100 = 2880W, where's 10s would get also 2880w. So the same wattage, since the number of elements does not really change..

So in this case.. the only area where it might change something is the capacity, I think. But for estimating the impact on capacity you would still need to know the real discharge rate.. It turned out that with 10s system you would consome only 0.78 of what you would consome with 8s system. That would be 15.73 A (~4/5) instead of 20 amps (5/5) for achieving the same amount of watts (576W in my case, or 20A for 8s at 28.8v nom)

So it is questionable at what amp rates is it better to go with 8s or 10s.. Some real world tests would probably tell this :) 

If we divide the theoretical 15.73 / 4 = 3.93 A per cell, where 20 / 5  = 4 A per cell.
And this is only with taking into account the nominal voltage, perhaps if we measure the voltage X amps = Watts, at each step.. we get a totally different picture.. I think this topic would deserve a special thread on its own for discussing the disharge rates etc :)
```

---
