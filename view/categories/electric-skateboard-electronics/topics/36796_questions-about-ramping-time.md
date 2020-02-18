# Questions about ramping time

### Replies: 6 Views: 1002

## \#1 Posted by: RiGo Posted at: 2017-10-29T11:10:10.596Z Reads: 165

```
I'm finding this a bit confusing. The explanation for Positive Ramping Time in the new VESC-Tool reads as follows:

_"Positive ramping time constant. This filters the input with ramping. This constant represents the amount of seconds it takes to ramp from zero to full output."_

What does "full output" mean in this instance? 100% throttle? So what happens if I rapidly flick the throttle from 0 to say 50% and the ramping time is 1s. Will it take 0.5s to get to half throttle or will it take 1s?

Also, is this a linear progression up to full throttle or does it wait 1s and the it gets up to full throttle instantly?
```

---
## \#2 Posted by: RiGo Posted at: 2017-10-30T23:25:06.793Z Reads: 128

```
A little help please?
```

---
## \#3 Posted by: Jinra Posted at: 2017-10-30T23:38:07.678Z Reads: 125

```
From my understanding, it's from any given point of throttle to another given point. For example, with a pos ramping time of 1s, going from 50% to 100% will take one second; similarly going from 50% to 51% would also take 1 second.
```

---
## \#4 Posted by: RiGo Posted at: 2017-10-31T02:27:09.784Z Reads: 111

```
Thanks. This seems a bit counterintuitive though. It would make responsiveness VERY mushy and inconsistent.

Can anyone else confirm pls?
```

---
## \#5 Posted by: MrHappy Posted at: 2017-10-31T02:52:54.927Z Reads: 103

```
Honestly, it makes it more comfortable to ride. I used to use a shitty car esc, and the input was way to sensitive. Once you ride for a while, you wont even notice it.
```

---
## \#6 Posted by: Jinra Posted at: 2017-10-31T03:05:04.521Z Reads: 99

```
that's why you set it lower
```

---
