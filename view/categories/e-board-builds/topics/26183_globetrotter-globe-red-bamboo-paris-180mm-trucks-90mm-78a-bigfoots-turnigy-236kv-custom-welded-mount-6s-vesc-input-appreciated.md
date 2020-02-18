# GLOBETROTTER &#124; Globe Red Bamboo &#124; Paris 180mm Trucks &#124; 90mm 78a Bigfoots &#124; Turnigy 236kv &#124; Custom Welded Mount &#124; 6S &#124; VESC &#124; Input appreciated!

### Replies: 12 Views: 1097

## \#1 Posted by: brok249 Posted at: 2017-06-26T04:01:40.519Z Reads: 182

```
Hello everyone,

I've got parts for a first build on the way (2*3s 4000mAh in series, VESC, 236kv Turnigy SK3, self-built mount) but wanted some input on my wiring setup. I've got a rough diagram below that I'd be happy to refine on demand, but the goal is to be able to charge both 3S packs without removing them from the board.

**Novice Electrician Questions. Have been resolved**

With the loop key removed, I should be able to plug in the XT60 connector as shown in the diagram (Labeled with a 2) from the charger, along with the balance lead using this harness:

https://hobbyking.com/en_us/6s-battery-pack-balance-charge-adapter-lead.html<img src="/uploads/db1493/original/3X/b/b/bbd3685e034bfea2d3f57fd84a1f01c621c95912.jpg" width="690" height="388">

The 3S lead with the black wire on that harness goes into the bottom battery (that provides the ground wire to the VESC), while the top one uses the other 3 wires as they all converge into the 6s port which ends up in the IMAX B6.

So in the end, on the outside of my cover, I'll have...

1 XT60 Connector (Loop Key)
1 XT60 Connector (Charging Port)
1 6S Balance Lead

And in order to charge I will **always always always** remember to remove the loop key first.

**END OF IMPORTANT STUFF**

I know just 4000mAh 6s in series isn't likely to get me very far very fast, but I'm planning on making this 9S or 6s2P sooner or later as budget and riding skill improves. Thanks in advance and looking forward to getting involved with this community.

EDIT: Quick format error

EDIT 2 Electric Boogaloo: Put some thought into it and decided having both the charging and Loop Key ports being the same size would be a bad move. I'll probably order some XT90s and use that for the loop Key and an XT60 for charging.

**End of Novice Electrician Questions**

The build went great, had the mount welded by Anthony over at Qualitig, a local welder who did an amazing job. The batteries go together in a single case, I do need to take it apart to charge because of the balance connector, but it's not a huge deal. Eventually planning on dremeling out a slit and putting a balance lead on the outside I can put an extension on to.

The VESC was a joy to program, currently have a max of 50A to the motor while I get used to the speed. Controller seems solid, no problems so far. 

Riding experience is great, I can recommend the Globe deck for a budget drop-through that can be top-mounted if needed, and while I went the now-unconventional route of a welded mount on Paris trucks I can say they feel great too.

**Pictures - Sorry, phone camera is showing it's age**

<img src="/uploads/db1493/original/3X/1/b/1b4d6b028567082a72e7ce0a1a2a4c0c764a079a.jpg" width="281" height="500">

<img src="/uploads/db1493/original/3X/0/8/08701ad74a397e17ebafe8627e8211fe896b26fe.jpg" width="281" height="500">

<img src="/uploads/db1493/original/3X/8/6/860892fb66d977e29b3665513dada4ef6c066085.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/2/8/2823a41237a590f4eaa573c1502f4a6cd4f669fb.jpg" width="690" height="388">
```

---
## \#2 Posted by: pat.speed Posted at: 2017-06-26T22:13:57.084Z Reads: 126

```
That should all work well just be careful about how hot the vesc gets because you are using it on 6s. 9s would be better
```

---
## \#3 Posted by: brok249 Posted at: 2017-06-26T22:31:30.563Z Reads: 118

```
Thanks. I'm planning on going 10sXp eventually but didn't have the budget for it at the moment. Just to be super extra sure, my balance lead layout is correct (balance ground goes to battery that the negative terminal goes to VESC), and my current 2-plug charging layout won't cause any damage to the VESC if the loop key is removed.
```

---
## \#4 Posted by: pat.speed Posted at: 2017-06-26T23:00:36.512Z Reads: 114

```
If I am reading your layout correctly ten there will be a short between te balance connectors. Will you be using a connector so that it becomes 1 6s plug?
```

---
## \#5 Posted by: brok249 Posted at: 2017-06-26T23:06:56.121Z Reads: 110

```
Yes. That's the plan, I linked the balance connector plug I'll be using above the picture.
```

---
## \#6 Posted by: pat.speed Posted at: 2017-06-26T23:13:05.281Z Reads: 100

```
Ah yes that will work. I thought you might have been using one of eBay like I have used and shorted my lipos with it because I plugged it in the wrong way. But that connect doesn't have the same wiring as mine so that should work fine. Good luck
```

---
## \#7 Posted by: brok249 Posted at: 2017-07-19T03:03:29.338Z Reads: 69

```
bump because I'd like some feedback.
```

---
## \#8 Posted by: Smorto Posted at: 2017-07-19T11:57:24.825Z Reads: 61

```
Feedback on what exactly?
```

---
## \#9 Posted by: brok249 Posted at: 2017-07-19T16:41:18.041Z Reads: 60

```
Just kind of thoughts in my build what I could have done better or possible future upgrades.
```

---
## \#10 Posted by: brok249 Posted at: 2017-07-20T00:21:45.450Z Reads: 51

```
It's my first build so I was wondering if there were any finishing-off tips "Getting started on esk8" advice.
```

---
## \#11 Posted by: Smorto Posted at: 2017-07-20T00:31:30.401Z Reads: 48

```
I would say just aesthetics wise, make it one enclosure and make it so the motor wires are a little more discreet. Either route them in your deck which is the more difficult option but looks the best, or simply find another way to make them look  little better and without that yellow stuff on them. You could also remove the SK3 stuff on your motor and replace it with a carbon fiber vinyl of sorts? Maybe you could wrap the entire underside of your deck with the carbon vinyl.
```

---
## \#12 Posted by: brok249 Posted at: 2017-07-20T03:37:59.879Z Reads: 43

```
Thanks with the suggestion, I'll black heatshrink over the yellow shrink on the wires, or pare the yellow back to black. I've already stapled and ziptied them to the board to get them a little bit cleaner. I'll probably get a single enclosure when I up the battery quality/count. Thanks for your help.
```

---
