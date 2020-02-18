# \[SOLVED\] Low peak motor current draw

### Replies: 12 Views: 756

## \#1 Posted by: Bataleon Posted at: 2017-04-21T19:08:16.906Z Reads: 107

```
Hey all,

I'm running a single 200kv 5065 motor (from @chaka) which has a rated peak power output of ~46A. My VESC battery and motor current are capped at 35A.

However, at full throttle my board only pulls a max of about 15A. Any ideas why?

The 10S LiFePO4 pack I'm using is capable of up to 100A discharge and is barely warm after riding.

Thanks
```

---
## \#2 Posted by: rpn314 Posted at: 2017-04-21T19:34:53.447Z Reads: 103

```
Do you have a BMS? Have you looked at your max ERPM and your peak duty cycle while riding?
```

---
## \#3 Posted by: Bataleon Posted at: 2017-04-21T19:53:32.893Z Reads: 96

```
Nope, I don't have a BMS installed (using a regular hobby charger at the moment). I'll take a look at max ERPM and peak duty cycle next time I ride. Thanks for the suggestions.
```

---
## \#4 Posted by: rpn314 Posted at: 2017-04-21T19:59:03.852Z Reads: 87

```
Also look at your voltage sag and cutoff. With a good LiFePO4 pack I'd be surprised if that were it, but worth checking
```

---
## \#5 Posted by: Okami Posted at: 2017-04-21T21:12:44.122Z Reads: 67

```
@Bataleon What wheels are u using?

It might as well be that it is all you need lol.. at least that''s what I think.. Do you reach the max speed with full throttle or do you feel that the motor could go more and more?

Try to go uphill to see if there really is this limitation..

With 36v nominal and 15A =  540W..

Your second bet would be to try to accelerate very hard to see what the peak is..

--

So yeh, if you do find you cannot push past 15A up a hill or when accelerating hard, then the problem is probably in software or in electronics, not in the environment or in power you require..
```

---
## \#6 Posted by: laurnts Posted at: 2017-04-21T21:32:13.656Z Reads: 59

```
This is normal. My motor have so low kv that I only draw 1.5 amps at full speed. The load only takes as much energy as it needs.
```

---
## \#7 Posted by: Hummie Posted at: 2017-04-21T21:51:24.813Z Reads: 61

```
The vesc "motor current" setting is limiting u. It gets confusing with the duty cycle and blah blah but the only way youre going to hit a true 35 amps is if u increase it or you put the motor under a large load at high speed (high duty cycle). Move ur motor amps up..or if u want to be more knowledgeable about what to set it to search for devins posts on buildanelectricboard.com since everything he wrote here got deleted or do akamaniacs software
```

---
## \#8 Posted by: makevoid Posted at: 2017-04-21T23:38:09.204Z Reads: 55

```
I agree with @Hummie, try to increase your motor max or try Ackmaniac's firmware which has the watt control mode (and it lets you draw an acceleration curve), my guess is that you're limited by the current control mode + the motor max setting.
```

---
## \#9 Posted by: Bataleon Posted at: 2017-04-22T17:20:21.227Z Reads: 46

```
Thanks for all of the replies.

I increased my motor and battery max current to 60A and 50A respectively. Acceleration is noticeably quicker, however, motor peak power is still < 500w.

I tried climbing a small hill: duty cycle was hitting 0.8, I could hear the motor bogging down hard, but it refused to pull more than 380w. The pack voltage never dropped below 32v (battery low voltage cutoff start).

 Here’s my motor configuration from the BLDC tool.

<img src="/uploads/db1493/original/3X/5/c/5cde9f2f50825f7fcc14d872c68de477fa4ee4ae.jpg" width="690" height="381">
```

---
## \#10 Posted by: Hummie Posted at: 2017-04-22T21:39:46.149Z Reads: 33

```
Motoramps.com
```

---
## \#11 Posted by: Bataleon Posted at: 2017-04-22T21:54:49.036Z Reads: 35

```
Excellent! Thanks for the link.
```

---
## \#12 Posted by: Bataleon Posted at: 2017-04-23T11:30:50.147Z Reads: 33

```
Turns out I was wrong: my "battery cutoff start" was being hit, hence the reduced power output. Lowering this value solved my issue.
```

---
