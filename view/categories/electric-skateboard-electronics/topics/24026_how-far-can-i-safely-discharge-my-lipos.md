# How far can I safely discharge my Lipos?

### Replies: 3 Views: 549

## \#1 Posted by: marcus Posted at: 2017-05-27T23:04:11.147Z Reads: 87

```
Hey guys,

I am currently in the process of completing my 10s board. As I set my VESC settings, what would you recommend my low voltage cutoff be? In other words, how far do you guys generally discharge your lipo batteries? Is there a sweet spot between max range and longevity?
```

---
## \#2 Posted by: paul775 Posted at: 2017-05-27T23:34:51.254Z Reads: 86

```
For 10S the cutoff start should be 35.0V and the cutoff end should be 33.0V (or 3.3V per cell). I have my voltage alarm set to 3.7V so at that point I never reach that cutoff.

For charging/longevity most people recommend to not charge all the way to 4.20V. Charge to 4.17 or 4.18 and that will increase you LiPo life.

<img src="/uploads/db1493/original/3X/8/4/8470f5aa0b4fa7df68dd5cd6b94864617a7b01e7.PNG" width="573" height="195">
```

---
## \#3 Posted by: Namasaki Posted at: 2017-05-28T03:34:19.768Z Reads: 74

```
The best option is to build a battery with more capacity(range) than you need.
Because the less you drain your battery the better.  If your not using alarms or a bms to monitor individual cells, it can be  risky going too low because cells can drift and some cells can discharge faster than others. You could wind up killing a whole pack by trashing one cell. 
So if your depending only on monitoring whole pack voltage then you might not want to go below 36v under load.
You could set your vesc low voltage start at 36 and stop riding when your board slows down rather than when it shuts down.
There is a popular theory that undercharging lithium batteries increases there cycle life.
I will not say that you should or shouldn't do this.
I have been fully charging my Lipos for 8 months now and they are still doing great.
But I have ruined brand new Lipos by over discharging them, and it only takes one time.
```

---
