# DRV Error&hellip;but only one VESC!

### Replies: 27 Views: 2168

## \#1 Posted by: flywithgriff Posted at: 2017-07-09T21:24:36.807Z Reads: 159

```
Finally got my board finished and took it out for a ride. FAILURE 😭

10s Lipo
Dual VESC
Dual 6374 190kv
15/36
97mm Clones

I made about a 10 minute ride and noticed my board felt sluggish all of a sudden. Knowing I was nowhere near the voltage or temperature shutdown I stopped and removed my enclosure. One vesc was still operating perfectly, the other would flash 3 red lights when I applied throttle. I took the board home and plugged it into the BLDC tool. The still running vesc, no errors. The other vesc, DRV 3802 Error. How can one vesc die and the other keep going. They are literally set up identical. They are joined with a Y Cable with one of the 5v wires clipped. The board was running perfectly!
```

---
## \#2 Posted by: flywithgriff Posted at: 2017-07-09T21:47:05.750Z Reads: 146

```
If it makes a difference for anything. The vesc with the DRV error was setup on a brand new 6374.
```

---
## \#3 Posted by: rpn314 Posted at: 2017-07-09T21:58:22.693Z Reads: 135

```
I had that happen to me once. Could be a plethora of things. Can you see what the current ramp step is currently?
```

---
## \#4 Posted by: flywithgriff Posted at: 2017-07-09T22:29:26.209Z Reads: 132

```
<img src="/uploads/db1493/original/3X/1/e/1e668da2c329f61eb41926561df70af96e93f419.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/a/8/a868dc021f2439ad8836d490207348caa14a916b.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/7/1/71967edec57845d321c4cb20b6f00171d58d9ccc.JPG" width="666" height="500">
```

---
## \#5 Posted by: rpn314 Posted at: 2017-07-10T00:14:41.729Z Reads: 108

```
Those all look okay. Could have been an ERPM issue (you've got it set to 100,000, I usually say 60,000), but I'd be surprised. can you get a screenshot of the motor advanced tab?
```

---
## \#6 Posted by: flywithgriff Posted at: 2017-07-10T00:50:06.803Z Reads: 105

```
Here you go. I have never changed anything in this page.<img src="/uploads/db1493/original/3X/e/c/ecd18e247bedee2a92a5e122da2d10262c97386c.JPG" width="666" height="500">
```

---
## \#7 Posted by: Namasaki Posted at: 2017-07-10T01:06:47.687Z Reads: 103

```
There's your problem. the max current ramp step is 40 and it's suppose to be .04
this is certainly what blew your DRV chip
Yours
 <img src="/uploads/db1493/original/3X/8/2/822943df0e62791af9e65270390334a730392322.png" width="474" height="157">

What it should be
<img src="/uploads/db1493/original/3X/1/f/1f33b183aa5ab6bf2e29a4c21819f15fbf12d521.png" width="586" height="168">

This is caused by a ramp step bug that was present in an old version of vesc firmware.

Aside from that issue, your motor max is really low at 55a. most motors can go 80a easy.
And your Battery min setting is really high at -35a and is might be more than your battery can handle for regen charging.
```

---
## \#8 Posted by: flywithgriff Posted at: 2017-07-10T01:21:06.002Z Reads: 102

```
Dude thanks for the info!! I had no clue this was an issue. This sucks!!
```

---
## \#9 Posted by: Namasaki Posted at: 2017-07-10T01:35:52.025Z Reads: 99

```
Creds to @rpn314 for thinking of it first.
This is a fairly old issue that was corrected some time ago with revised firmware.
```

---
## \#10 Posted by: flywithgriff Posted at: 2017-07-10T01:43:19.125Z Reads: 111

```
Unfortunately I have never had a vesc with this issue and when I purchased this one I wasn't aware of such an issue. I purchased this vesc from a member here who is a great guy and very credible. This is a tough lesson to learn.
```

---
## \#11 Posted by: Namasaki Posted at: 2017-07-10T01:48:11.951Z Reads: 107

```
Time to call the DRV Wizard
http://www.electric-skateboard.builders/t/johnny-vesc-repair-services-now-with-soldering-tips/11267/18?u=namasaki
```

---
## \#12 Posted by: flywithgriff Posted at: 2017-07-10T01:53:41.396Z Reads: 103

```
Any clue what it will cost? Pretty sure this was a repaired cheapo vesc to start with. It may be worth buying used or cheap. I plan to do the @Titoxd10001group buy for 2 FOCBOX.
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2017-07-10T01:55:12.672Z Reads: 98

```
where are you located ?
```

---
## \#14 Posted by: flywithgriff Posted at: 2017-07-10T01:55:43.556Z Reads: 94

```
New York City
```

---
## \#15 Posted by: JohnnyMeduse Posted at: 2017-07-10T02:00:57.993Z Reads: 93

```
Price for repair is 45USD per Units (return shipping include)... 

Or if I also have some FOCBOX for sale right now :wink:

https://www.electric-skateboard.builders/t/tada-focbox-aka-vesc-x-for-sales-in-stock-canada-and-us-free-shipping-tada/25259?u=johnnymeduse
```

---
## \#16 Posted by: flywithgriff Posted at: 2017-07-10T02:03:30.275Z Reads: 87

```
Pm sent sir
```

---
## \#17 Posted by: rpn314 Posted at: 2017-07-10T02:23:02.214Z Reads: 86

```
Sorry for the loss, but glad I could help you find the issue! If you haven't already, I'd check the second one as well, just to be safe :slight_smile:
```

---
## \#18 Posted by: flywithgriff Posted at: 2017-07-10T02:26:07.134Z Reads: 83

```
Thank you for the help man!! I just checked the other and i doesn't seem to have the same issue.
```

---
## \#19 Posted by: rpn314 Posted at: 2017-07-10T02:28:56.723Z Reads: 82

```
My pleasure! Good. Just in case, you check it by writing and read a few times. The values shouldn't change. The bug was when you wrote data, it would increase by 10x. It was a bug with the initial release of 2.18 and plagued many of us (me included). It was fixed, but the firmware version was not incremented so both the buggy version and the clean version are v2.18 and the only way to tell is the repeated read/write above.
```

---
## \#20 Posted by: JLabs Posted at: 2017-07-10T02:40:15.259Z Reads: 80

```
Quick question and a complete thread hijack.. 

What's with the solution thing? Can only mods pick which comment is the solution? I looked and could not see antlything in the threads I have created.
```

---
## \#21 Posted by: flywithgriff Posted at: 2017-07-10T02:59:25.885Z Reads: 72

```
Umm idk, I was able to choose my solution. It's a little gray check mark beside the like and link buttons on each reply.
```

---
## \#22 Posted by: rpn314 Posted at: 2017-07-10T11:01:33.413Z Reads: 71

```
@JLabs The solution option was enabled (forum wide) by onloop a few weeks ago. It was just disabled when the forum was created way back. I believe the topic creator and maybe the mods can select the solution.
```

---
## \#23 Posted by: flywithgriff Posted at: 2017-07-10T13:28:56.158Z Reads: 70

```
I just checked my other vesc and noticed it too has the wrong value. I have never checked this so I guess I'm lucky it didn't blow as well!
<img src="/uploads/db1493/original/3X/f/e/fe564ded8fad3d0c1ab1d108542b8297a16c0d44.jpg" width="666" height="500">
```

---
## \#24 Posted by: rpn314 Posted at: 2017-07-10T17:59:27.771Z Reads: 65

```
0.04 looks like the right value...or is that picture after you changed it?
```

---
## \#25 Posted by: Jinra Posted at: 2017-07-10T18:03:12.990Z Reads: 62

```
The moral here is to always reflash f/w when you buy a VESC.
```

---
## \#26 Posted by: flywithgriff Posted at: 2017-07-10T18:21:36.443Z Reads: 62

```
Oops that pic was after I changed it. It was .40 when I read it. What do you guys think about flashing to @Ackmaniac firmware?
```

---
## \#27 Posted by: Jinra Posted at: 2017-07-10T18:30:18.610Z Reads: 62

```
Why not :), you can also flash the stock f/w again, which should be a fixed version depending when you downloaded BLDC tool. Also, according to @ackmaniac on the buggy f/w you should write to .04 and make it read .40 as it's an issue with the tool reading from f/w. This means that while you're reading a .4 value, the actual value is .04.
```

---
