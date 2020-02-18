# Why is my vesc not working with my r spec

### Replies: 16 Views: 1840

## \#1 Posted by: gmcgaffey Posted at: 2016-06-28T19:37:02.748Z Reads: 123

```
I just connected my vesc to my board and hooked up my remote. the vesc flashes red and blue then solid blue. when I try to use the remote the vesc flashes green? do I need to do a motor detection.
```

---
## \#2 Posted by: Skitzor Posted at: 2016-06-28T20:03:05.400Z Reads: 123

```
I will post you some screens from my settings. which motor is it btw? I've got the dual 6355's

<img src="/uploads/db1493/original/2X/7/7513270d468afac1068e0066741173b53537f395.PNG" width="690" height="393">

<img src="/uploads/db1493/original/2X/b/b3bffac36a28cccc9cfbe995e502afbf2f2c5a46.PNG" width="690" height="393">

<img src="/uploads/db1493/original/2X/c/c21e38b7664a0e4e17c6896ed377e88e884cf5a7.PNG" width="690" height="393">

<img src="/uploads/db1493/original/2X/5/5ae34a577aefe8817ed31d82450389423148affb.PNG" width="690" height="393">

<img src="/uploads/db1493/original/2X/a/af6f05f9f7ae3fe7353ee5319b9c3fd9f7c8ebda.PNG" width="690" height="393">

<img src="/uploads/db1493/original/2X/c/c6060618d2c09fac65b888b0ae12bc73eb33aa03.PNG" width="690" height="393">

<img src="/uploads/db1493/original/2X/6/6aad608031f63a5f2ea45d0ded5617a7a28aeb5a.PNG" width="690" height="393">

<img src="/uploads/db1493/original/2X/a/adca450b46c48a7a0727f179acbaf0065b73ae1a.PNG" width="690" height="393">

<img src="/uploads/db1493/original/2X/4/4731360726be8191a0ada15c04a2070fa6684a0b.PNG" width="690" height="393">

<img src="/uploads/db1493/original/2X/5/55b0f847064465480643a1d4a8dfa6c2c7c729a2.PNG" width="690" height="393">

<img src="/uploads/db1493/original/2X/7/71b5b07820762b2b38645348e72c1163b5f5fcdf.PNG" width="690" height="393">

And a link for the proper receiver wiring:
http://www.electric-skateboard.builders/t/enertion-receiver-wiring/5170/5 

Hope this helps
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2016-06-28T20:50:51.979Z Reads: 98

```
Maybe This will help you. You need to Configure the remote and the Motor, on brand new VESC, or each time you change a component. 
http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980
```

---
## \#4 Posted by: sl33py Posted at: 2016-06-28T21:09:00.823Z Reads: 93

```
@gmcgaffey - you need to do a motor detection!  These are not fully "plug-n-play" speed controllers.

follow the directions or youtube video vedder posted up and it should only take a few minutes.  Until you do this, you are likely going to have it not work at all, or possibly damage the VESC.  So make sure you get it configured for your motor!

GL!
```

---
## \#5 Posted by: gmcgaffey Posted at: 2016-06-28T21:13:10.008Z Reads: 93

```
motor detection failed?
```

---
## \#6 Posted by: sl33py Posted at: 2016-06-28T21:45:56.822Z Reads: 89

```
check your connectors - swap to a different or shorter USB cable next - retry.

must. detect. motor!  Otherwise you have a $100+ paper weight.
```

---
## \#7 Posted by: gmcgaffey Posted at: 2016-06-28T21:53:21.801Z Reads: 87

```
OK I feel like enertion sent me a bad vesc
```

---
## \#8 Posted by: gmcgaffey Posted at: 2016-06-28T22:22:01.982Z Reads: 84

```
it says under voltage in the terminal
```

---
## \#9 Posted by: Jinra Posted at: 2016-06-28T22:54:49.167Z Reads: 76

```
What's the voltage of the pack you're hooking up to it? I'd verify with a voltmeter/multimeter
```

---
## \#10 Posted by: gmcgaffey Posted at: 2016-06-28T23:11:49.673Z Reads: 75

```
it's two lipos wired in series. there 5s 5000mah my voltage meter says 18.4v each
```

---
## \#11 Posted by: sl33py Posted at: 2016-06-29T00:16:08.711Z Reads: 67

```
that sounds reasonable.  ;)

How about you give details on why you think this?  I read "how do i do motor detection", followed by "it's a bad VESC"...  Hmm...

giving you a hard time (deservedly), but we can help if you provide some detailed steps and error codes.

under voltage - what are your voltage settings in BLDC tool?  I configure mine on 12v (lab power supply w/ minimal amperage) - to avoid any possible issue.  So configuring should not need 12s 100A voltages...

Where are you located?  perhaps someone local can lend a hand?

GL!
```

---
## \#12 Posted by: gmcgaffey Posted at: 2016-06-29T00:39:21.830Z Reads: 62

```
I am in Vancouver wa. the absolute max is 130 a
```

---
## \#13 Posted by: gmcgaffey Posted at: 2016-06-29T01:15:37.210Z Reads: 58

```

the voltage limits are (max=42v,min=8v)
```

---
## \#14 Posted by: sl33py Posted at: 2016-06-29T20:26:15.686Z Reads: 47

```
voltage limits look good.  8-42v should not be giving you any under voltage errors.

using a small single battery (i like the small 1k-1500mAh 3s, or 12v lab power), does it connect up in BLDC tool?  are you using the correct ported one in Windows, or did you compile in linux?  What firmware and hardware is your VESC?  Single or dual VESCs?

I can let you know my motor detection settings for my R-Spec - but that's definitely not ideal.  They do vary and mine are the original Red versions.

Last - i'm in Seattle, are you ever up this way?
```

---
## \#15 Posted by: gmcgaffey Posted at: 2016-06-29T20:35:28.275Z Reads: 47

```
I connects to bldc tool on Windows and says firm ware 2.18
```

---
## \#16 Posted by: sl33py Posted at: 2016-06-29T20:46:23.407Z Reads: 46

```
there were easily 3 or 4 other questions...

let's try again.

OK - FW 2.18.  what version of the Windows ported BLDC are you using?  And where did you d/l it from?

Only a single VESC then?

Did you try a few other USB cables - especially shorter ones if you had a 10ft USB charging cable for a phone...

Let' shoot for more than a single line response huh?  I'd like to help, but seriously we shouldn't need to hold your hand and do it for you.  If this is beyond your ability to follow (more specifically the step-by-step videos on youtube from Vedder), then perhaps you should cut your losses and get a simpler ESC (DIYes is a good one - i'd avoid Flyer/APS), or XERUN/FVT if you can keep 6s or less.

If you did not do the motor detection and still tried to use it, it's also possible you damaged your VESC.  That would suck.  Have you reached out to @onloop or enertion support?

I also think there was someone who was willing to do remote support for VESC at some reasonable cost.  Likely a remote teamviewer session to help - this might be a good idea.  I'd of course see what enertion can do to help first.

best of luck.
```

---
