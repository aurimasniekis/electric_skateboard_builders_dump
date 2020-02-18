# Losing power on Board with CarvOn Single Hub

### Replies: 9 Views: 1685

## \#1 Posted by: joeykache Posted at: 2016-06-06T05:05:44.986Z Reads: 104

```
Hey everyone, I have a board I made using the Enertion space cell, a VESC from chaka and CarvOn Single Hub motors. I go around a few blocks probably averaging around 18-24 mph and I lose power after a single run. I then push the throttle all the way and I'm literally going at 4mph. Is there a reason for this? I also have a yuneec e-go and this is never the case with the e-go. Am I doing something wrong? The VESC settings are default. I haven't done any additional tweaks. I then have to turn off my receiver and the board for around 10 minutes and I'm back to normal for a short period  time before it starts to lose power again. Should I change VESC settings to push a little harder?   Thanks again in advance. <img src="/uploads/db1493/original/2X/a/ab17f59ab1b39cbb04f53d3afae788f8043e48ab.jpg" width="666" height="500"
```

---
## \#2 Posted by: barajabali Posted at: 2016-06-06T05:07:24.425Z Reads: 102

```
and you charge your battery pretty often? that sounds like a battery problem or maybe a low voltage detection
```

---
## \#3 Posted by: Blasto Posted at: 2016-06-06T05:23:11.113Z Reads: 97

```
[quote="joeykache, post:1, topic:4330"]
The VESC settings are default.
[/quote]

I think you're lucky your vesc is still alive. You need to configure it to your setup.
```

---
## \#4 Posted by: joeykache Posted at: 2016-06-06T05:24:15.298Z Reads: 97

```
I don't charge it over excessively. I'm really good with charging. I don't think it's the battery, it actually lasts me quite a few miles. Sorry, I'm still somewhat of a newb for eskate. How do I go about upping my voltage detection?
```

---
## \#5 Posted by: joeykache Posted at: 2016-06-06T05:25:22.801Z Reads: 94

```
Really? Ah crap. I had no idea. I thought the VESC would just auto populate to the power and all. Ughhhh..
```

---
## \#6 Posted by: Blasto Posted at: 2016-06-06T05:26:14.201Z Reads: 91

```
http://www.electric-skateboard.builders/t/easy-vesc-configuration-in-windows-mac-for-noob/2963?u=blasto

Some good compiled info here.
```

---
## \#7 Posted by: DeathCookies Posted at: 2016-06-06T06:08:39.917Z Reads: 85

```
[quote="joeykache, post:1, topic:4330"]
I then push the throttle all the way and I'm literally going at 4mph.
[/quote]

For me it sounds like the LVC (Low Voltage Cut-Off). If your battery hits a presetted voltage it will reduce the output power until you reached the LVC. Then it will shut off completely. Do not forget that you will have a bit less voltage when you hit the throttle.
I.e. Battery: 36V LVC: 35 --> In this case your battery would sag some voltage under load and can easily go under the LVC.
```

---
## \#8 Posted by: treenutter Posted at: 2016-06-06T13:05:49.866Z Reads: 63

```
I agree with @barajabali @Blasto and @DeathCookies. It sounds you're hitting LVC and it's very concerning that you've never configured VESC... Did you do a motor detection at the beginning? Definitely read the link  below, and ping us here if you have questions. Good luck!

http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980
```

---
## \#9 Posted by: Blasto Posted at: 2016-06-06T14:10:29.396Z Reads: 55

```
Your build looks pretty clean, don't worry you're about 5 mins away on being up and rolling properly.
```

---
