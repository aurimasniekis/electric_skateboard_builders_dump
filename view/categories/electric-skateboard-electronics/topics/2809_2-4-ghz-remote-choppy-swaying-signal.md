# 2.4 Ghz remote choppy/swaying signal

### Replies: 10 Views: 1260

## \#1 Posted by: massy Posted at: 2016-05-02T12:58:45.352Z Reads: 93

```
So I have gotten a 2.4 GHz controller (the mini one a lot of people uses). However as soon as I turn the remote on the signal automatically sways a lot. For example the signal in the BLDC-tool varies from like 48-55% without me doing anything on the remote. This makes for an extremely choppy ride. 

Would you suspect that I have done something wrong or is the controller the culprit?
```

---
## \#2 Posted by: treenutter Posted at: 2016-05-02T13:02:53.365Z Reads: 93

```
@massy if you increase the deadband setting on the PPM tab of BLDC Tool it will smooth out the fluttering signal response.
```

---
## \#3 Posted by: trbt555 Posted at: 2016-05-02T13:06:01.952Z Reads: 94

```
Have you set the pulsewidth endpoints in the VESC to the actual ones being transmitted ?

What do you mean by choppy ride ? Does the signal vary a lot when you keep your trigger steady ?

You can increase the deadband in the ppm app tab to account for signal variation around neutral.
```

---
## \#4 Posted by: massy Posted at: 2016-05-02T13:19:05.051Z Reads: 86

```
@treenutter @trbt555

Yes, the signal varies 5-10% when keeping it steady. Should changing the deadband show in the displayed bar(in BLDC-tool), because it keeps fluttering around 5-10% no matter what I set the deadband to. 

I have tried setting the pulse width to the actual values. Problem is say that the highest and lowest value is fluctuating between  (for example) 1.90 and 1.98 (or whatever 5-10% is). Keeping a steady throttle results in 5-10% fluctuation in motor power.

Max pulsewitdth with particular trim setting fluctuates between ~1.820 and ~1.880 very quickly.

_"You can increase the deadband in the ppm app tab to account for signal variation around neutral."_
Problem is it fluctuates at 60%, at 22%, at 88%, not just around neutral. Increasing the deadband did help with finding a stable neutral state but the throttle is not smooth.
```

---
## \#5 Posted by: trbt555 Posted at: 2016-05-02T13:29:37.819Z Reads: 77

```
Setting the deadband won't make the display in BLDC more stable, your VESC will just ignore larger fluctuations around the neutral position. That prevents your board from jittering.
If you have this problem when actually riding it sounds to me like a wonky transmitter.
Check the "use median filter" option on the ppm app tab, which should smooth out the signal. I have no experience using this though. I'm not even sure it's still in the BLDC version you're running.
```

---
## \#6 Posted by: massy Posted at: 2016-05-02T13:44:55.941Z Reads: 72

```
Yeah, got hopeful when the deadband was mentioned as I might have missed to config that but I'm really starting to think it's the remote now too. Deadband won't help the throttle fluctuations in any way.

Edit: Why am I always so fricking lucky. Gaaah.
```

---
## \#7 Posted by: trbt555 Posted at: 2016-05-02T13:52:14.092Z Reads: 68

```
What about the median filter ?
```

---
## \#8 Posted by: massy Posted at: 2016-05-02T13:52:43.653Z Reads: 67

```
Tried it both on and off, goes crazy either way.
```

---
## \#9 Posted by: trbt555 Posted at: 2016-05-02T14:07:27.569Z Reads: 63

```
Is it a brand new controller ? Can you return it ?
If not and if it were mine I'd open it up and spray some contact cleaner on the trigger potmeter.
```

---
## \#10 Posted by: massy Posted at: 2016-05-02T14:35:18.732Z Reads: 59

```
It's completely new so I've opened a dispute about it. Let's hope the seller is easy to deal with. Ordered it from China though so let's see where it leads.
```

---
