# Turnigy B6 Compact charger not charging up 2x series LiPo 3s 5800mAh batteries

### Replies: 18 Views: 824

## \#1 Posted by: Armitage Posted at: 2017-11-12T15:17:57.955Z Reads: 62

```
Hey, I have a problem with my build. I am charging two Zippy 3s 5800mAh batteries in series. I charge them with Turnigy B6 Compact automatic charger. The problem is that it never reaches the charged state. I have kept it on and it never finishes. I'm also concerned about the fact that the batteries could overcharge, so I need your help :slight_smile: 
Thanks a lot

Here are links: [Batteries](https://hobbyking.com/en_us/zippy-flightmax-5800mah-3s1p-30c.html),[Charger](https://hobbyking.com/en_us/turnigy-b6-compact-50w-5a-automatic-balance-charger-2-6s-lipoly.html)
```

---
## \#2 Posted by: florensvb Posted at: 2017-11-12T15:48:33.024Z Reads: 60

```
Maybe the cells got too far out of balance so the charger doesnt even attempt to charge anymore? do you have a voltage meter to check?
```

---
## \#3 Posted by: FredrikHems Posted at: 2017-11-12T15:49:40.397Z Reads: 56

```
You can't charge batteries in series if i remember right. Try to charge them separately from each other.
```

---
## \#4 Posted by: Armitage Posted at: 2017-11-12T16:00:44.521Z Reads: 52

```
@FredrikHems  No you can :slight_smile:
```

---
## \#5 Posted by: Armitage Posted at: 2017-11-12T16:01:58.947Z Reads: 49

```
@florensvb I do have one but not in reach right now, the bldc tool says 24.2 volts, but I'm not sure how accurate it is.
```

---
## \#6 Posted by: akhlut Posted at: 2017-11-12T16:14:44.546Z Reads: 47

```
You want one of [these](https://hobbyking.com/en_us/hobbyking-parallel-charging-board-for-6-packs-2-6s-xt-60.html) if you want to charge two packs at the same time.  If you don't know WTF you're doing just charge them one at a time or you'll burn your house down.

[READ THIS AND UNDERSTAND IT BEFORE ATTEMPTING](https://www.rchelicopterfun.com/parallel-lipo-charging.html)
```

---
## \#7 Posted by: Armitage Posted at: 2017-11-12T16:18:26.105Z Reads: 45

```
@akhlut I am charging them in series and like on this diagram, except red BALANCE LEAD that is together with black one is disconnected.<img src="/uploads/db1493/original/3X/f/1/f174b6f5bd455c632e5458a49d2c0ca859698feb.png" width="690" height="489">
```

---
## \#8 Posted by: Armitage Posted at: 2017-11-12T17:03:36.464Z Reads: 39

```
Still needing help!!!
```

---
## \#9 Posted by: Armitage Posted at: 2017-11-12T17:51:03.829Z Reads: 34

```
I figured out, that the battetries should be fully charged at 25.2v, considering 4.2v/cell is normal? So i still have some volts to go.
```

---
## \#10 Posted by: florensvb Posted at: 2017-11-12T18:22:49.096Z Reads: 32

```
let me know when you checked the cell voltages
```

---
## \#11 Posted by: Armitage Posted at: 2017-11-12T19:48:18.553Z Reads: 31

```
@florensvb I meant that I have a regular voltage meter, I can't check each cell with it, can I?
```

---
## \#12 Posted by: PXSS Posted at: 2017-11-12T19:52:54.570Z Reads: 29

```
I'll help you out in about 30 minutes. People here so far have no clue as to what they are talking about. 

You can use a multimeter to check individual cell voltage by measuring between pins in the balance port. 

You could have a cell that is dead. Zippy batteries are not that reliable. I've had it happen to most zippy packs I own.

Also is your B6 charger a real SkyRC charger or a knockoff? If it's a knockoff then that might be the issue as they do not have accurate voltage sensors in them and can overcharge your cells constantly until they go bad. The screen would still show the correct voltage even if they are overcharged.
**Never mind this ^^^** I thought you had an iMax B6 not a turnigy B6. You may still want to double check that it is charging to the correct voltage with a multimeter 

The way you have your batteries connected is correct. Don't let others tell you otherwise
```

---
## \#13 Posted by: pat.speed Posted at: 2017-11-12T20:02:59.956Z Reads: 25

```
Hey mate, same thing happens to me my cells charge up to about 4v then stop. I actually just think it's a good thing now because my cells will last longer
```

---
## \#14 Posted by: Armitage Posted at: 2017-11-12T20:15:36.089Z Reads: 26

```
@PXSS Thank you so much for the advice, I'm gonna check that tommorrow, I'll let you now :slight_smile:
```

---
## \#15 Posted by: Armitage Posted at: 2017-11-12T20:16:40.685Z Reads: 27

```
@pat.speed Yeah, I also think that they charge to somewhere about 4 volts and the charger cuts off but doesn't show that it's fully charged.
```

---
## \#16 Posted by: Armitage Posted at: 2017-11-18T15:20:50.183Z Reads: 21

```
@PXSS Sorry I couldn't reply, cause I was sick. I'll hopefully check them today. Still up for helping?
```

---
## \#17 Posted by: PXSS Posted at: 2017-11-18T15:43:38.222Z Reads: 21

```
Yep
123456
```

---
## \#18 Posted by: Armitage Posted at: 2017-11-27T17:38:17.328Z Reads: 14

```
Sorry for not replying, but I actually found out, that some of the balance leads were broken from the inside, so I replaced them and now it should be charging normally.
```

---
