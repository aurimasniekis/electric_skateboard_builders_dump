# How I failed at my controller

### Replies: 34 Views: 1149

## \#1 Posted by: Clonkex Posted at: 2017-09-18T00:32:05.412Z Reads: 98

```
I did a silly thing. When I made my 3D-printed custom remote for my board I connected the 1S lipo cell directly to the electronics and a SPDT switch. The switch selected between powering the electronics and connecting the battery to the charging port. The electronics don't currently include any over-discharge protection because the controller only draws a tiny tiny bit and I was happy to just check the voltage manually.

Yesterday I got my board reassembled with the new trucks and an idler pulley and was all ready to test it out, so I grabbed my controller and switched it to the charging port so I could stick a multimeter on it to check the voltage. _No voltage. Wut. Oh right, somehow I failed to get the switch to the charging position..._

1.7v. On a lipo cell. 0_o Oh dear.

And then I realised why I'd failed to get the switch to the charging position the first time: it was in the "on" position when I picked it up.

So yeah. I failed by not having over-discharge protection and also by having the switch mounted sideways so when I inevitably sit the controller on something it's very easy for the switch to be turned on by accident. I'm not actually annoyed that I killed the lipo (they're cheap and easy to get), more that I have to desolder it and prepare a new cell, and that I couldn't take the board out for another test. Also the fact that I _think_ I accidentally threw out the other 2 cells of the 3S lipo that cell came from with the packaging. Will have to dig through our bins and see if I can find them because I don't want our bins to catch fire.

Next step is buying an over-discharge protection chip (or making one, should be pretty easy! Thinking just a voltage divider and a mosfet controlled by the arduino).
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-09-18T01:33:11.463Z Reads: 89

```
Post some pics of the remote 😉
```

---
## \#3 Posted by: Clonkex Posted at: 2017-09-18T01:33:50.855Z Reads: 84

```
True, I should do that. Actually I just need to make a build thread and then I can post them in there. At work currently and the board is at home so no pics for now :'(
```

---
## \#4 Posted by: GrecoMan Posted at: 2017-09-18T01:34:20.654Z Reads: 81

```
Awwwww I love seeing DIY remote pics 😭
```

---
## \#5 Posted by: Clonkex Posted at: 2017-09-18T01:40:12.028Z Reads: 72

```
Me too, that's how I designed my remote, by looking at heaps of photos of other people's remotes :P Going to make the design and software open source once it's reliable and a bit more tested. The goal is for it to be as easy to make as possible using the most available parts possible. Currently the brake has too much travel and it's awkward to apply 100% brakes (not that I think I'd ever want to do that, basically stops the board on a dime when I do that :P ).
```

---
## \#6 Posted by: GrecoMan Posted at: 2017-09-18T01:40:53.721Z Reads: 61

```
Maybe try to embark on a zero modification GT2B mod, that would get a lot of interest
```

---
## \#7 Posted by: Clonkex Posted at: 2017-09-18T01:43:03.438Z Reads: 59

```
Never looked at the GT2B remote. Is it a digital or analogue controller? Also what do you mean by zero modification mod?
```

---
## \#8 Posted by: GrecoMan Posted at: 2017-09-18T01:44:06.071Z Reads: 60

```
Zero modification as in no soldering, no battery modification, just moving electronics. All the current mods for it require some very careful soldering and patience
```

---
## \#9 Posted by: Clonkex Posted at: 2017-09-18T01:44:16.817Z Reads: 56

```
Mods to achieve what?
```

---
## \#10 Posted by: GrecoMan Posted at: 2017-09-18T01:44:32.050Z Reads: 54

```
Make it smaller
```

---
## \#11 Posted by: GrecoMan Posted at: 2017-09-18T01:45:08.048Z Reads: 52

```
It’s huge controller but it’s reliable.  It can be made much smaller (benchwheel remote size) with just a different case
```

---
## \#12 Posted by: Clonkex Posted at: 2017-09-18T01:46:34.636Z Reads: 50

```
OOOooohh, right. I can't afford to buy one but I reckon if I had one I could invent a way to make it small and neat (and clean, can't stand messy-looking remotes).
```

---
## \#13 Posted by: GrecoMan Posted at: 2017-09-18T01:47:16.628Z Reads: 50

```
I know the feeling of not being able to afford a $25 remote 😂
```

---
## \#14 Posted by: Clonkex Posted at: 2017-09-18T01:54:15.801Z Reads: 49

```
Haha. I've got myself on a pretty strict budget at the moment because I have a number of moderately-sized debts that need to be paid off ASAP. Accounting for internet, food, board and fuel costs that leaves me just over $100/week, and this week (because I screwed up a calculation in my spreadsheet) I need that money for my internet.
```

---
## \#15 Posted by: GrecoMan Posted at: 2017-09-18T01:55:29.385Z Reads: 48

```
Man, $100 a week is a little over double I make per week, then again I don’t have to pay takes, internet... 🤔
```

---
## \#16 Posted by: scepterr Posted at: 2017-09-18T01:59:31.453Z Reads: 50

```
TP4056 1S lipo charger with over charge/discharge protection https://www.amazon.com/dp/B074CQF5MC/ref=asc_df_B074CQF5MC5174606/
```

---
## \#17 Posted by: Clonkex Posted at: 2017-09-18T02:00:09.632Z Reads: 55

```
Well that's AUD of course and I think you're in the US so that's only about 80USD. But yeah, I work full time in IT as a programmer/website engineer dude. In all honesty I would much rather only work 3-4 days a week and have less money but more time. It sucks only having 2 days per week to myself.
```

---
## \#18 Posted by: Clonkex Posted at: 2017-09-18T02:02:59.529Z Reads: 53

```
Already bought a pack of 5 of those from eBay after you suggested it in general chat, but I didn't know they did discharge protection as well. Is that what the datasheet means by _under voltage lockout_? I assumed it meant it wouldn't try to charge it if it was below a certain voltage.
```

---
## \#19 Posted by: scepterr Posted at: 2017-09-18T02:04:51.578Z Reads: 51

```
There are 2 diff versions, with and without over/under protection. The ones with protection have extra solder pads next to batt pads for output to device being powered by lipo. It charges at 100ma if it detects low voltage cell and then ramps up when it hits threshold mentioned in datasheet. You can also adjust charge rate by changing a resistor
```

---
## \#20 Posted by: Clonkex Posted at: 2017-09-18T03:16:22.734Z Reads: 46

```
Ah interesting. So based on that, the [ones I bought](http://www.ebay.com.au/itm/182632018873) should have the undervoltage protection? Ah, with some googling I can see that board has two different lipo protection ICs aside from the TP4056 so I guess it does. I'm not sure why there would be two different ICs that seem to do the same thing though :thinking:
```

---
## \#21 Posted by: scepterr Posted at: 2017-09-18T03:26:44.002Z Reads: 38

```
Old lower cost version and new updated version
```

---
## \#22 Posted by: Clonkex Posted at: 2017-09-18T03:29:30.332Z Reads: 39

```
? The boards I bought appear to have 3 ICs on them. The TP4056, a DW01A and an 8205A, the latter 2 being lithium protection ICs (both with charge and discharge protection). I'm not sure what you mean.
```

---
## \#23 Posted by: scepterr Posted at: 2017-09-18T03:32:40.662Z Reads: 37

```
You got the right one, there's an older cheaper version without those 2 ic
```

---
## \#24 Posted by: Clonkex Posted at: 2017-09-18T03:33:49.041Z Reads: 40

```
Oh cool, that's what I thought. Still confused why there's 2 ICs on there that seem to do the same thing, but hey, as long as they do their thing I don't really care :P
```

---
## \#25 Posted by: scepterr Posted at: 2017-09-18T03:36:01.267Z Reads: 40

```
Bad <img src="/uploads/db1493/original/3X/1/e/1e27e545622516598c640ad182f20ba634b57781.jpg" width="500" height="500">
Good
<img src="/uploads/db1493/original/3X/7/9/798257de9a792323b187792e182b55e58ca61a72.jpg" width="675" height="278">
```

---
## \#26 Posted by: Clonkex Posted at: 2017-09-18T03:41:55.694Z Reads: 38

```
Yep I understand that bit, I think you are misunderstanding me. Perhaps this will make it more clear:

<img src="/uploads/db1493/original/3X/b/c/bc5c8e8045edb1e1e090d37455ab3ac5c3b488e1.png" width="690" height="283">

But really I was just commenting on the fact that there's 2 ICs that seem to do the same thing. I wasn't really asking anyone to explain it for me :)
```

---
## \#27 Posted by: scepterr Posted at: 2017-09-18T03:46:35.070Z Reads: 34

```
Oh lol. I believe 1 is used for over and 1 for under protection
```

---
## \#28 Posted by: Clonkex Posted at: 2017-09-18T03:47:15.650Z Reads: 33

```
Oh righto, yeah probably. I did vaguely wonder that but the thoughts never continued down that path :P

This is a pretty cool little board. More useful than I thought.
```

---
## \#29 Posted by: scepterr Posted at: 2017-09-18T03:52:42.897Z Reads: 35

```
Always in my bag
Edit: fixed ;)
<img src="/uploads/db1493/original/3X/a/a/aabf8d924d5ef28028c6d8682b6e64f6211027e6.jpg" width="375" height="500">
```

---
## \#31 Posted by: Clonkex Posted at: 2017-09-18T03:58:37.844Z Reads: 29

```
What is that for? I mean obviously for charging, but what kind of battery would fit in that holder that could be charged by a 1S lipo charger?
```

---
## \#32 Posted by: scepterr Posted at: 2017-09-18T03:59:27.850Z Reads: 32

```
18650 bro lol
```

---
## \#33 Posted by: Clonkex Posted at: 2017-09-18T04:01:35.449Z Reads: 30

```
Oh wow that must be smaller than it looks. I think I mistook the size of it :O So does your controller run on 18650s? Or do you plan to charge each of your board's cells individually in an emergency? :P
```

---
## \#34 Posted by: scepterr Posted at: 2017-09-18T04:06:06.803Z Reads: 32

```
When you have more 18650s than you can count, you use them for everything lol <img src="/uploads/db1493/original/3X/2/6/2644326bb4a4e6c27bb162f24bc8b03e113b8525.jpg" width="690" height="398">
http://www.diypowerwalls.com/t-CyberWall
```

---
## \#35 Posted by: Clonkex Posted at: 2017-09-18T04:10:49.752Z Reads: 32

```
oh lol, I guess I would as well
```

---
