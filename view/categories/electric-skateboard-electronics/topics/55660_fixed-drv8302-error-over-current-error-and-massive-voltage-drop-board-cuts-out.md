# (FIXED) DRV8302 error, Over Current error, and massive voltage drop (board cuts out)

### Replies: 9 Views: 536

## \#1 Posted by: Tijmen Posted at: 2018-05-16T14:28:05.486Z Reads: 104

```
My board is experiencing some major issues. First a backstory.

I had been running a focbox for a while in FOC with no issues. And suddenly I started getting DRV errors when I'd accelerate hard.
Since then, I've swapped to dual focboxes. Both brand new
Dual Torqueboards 6355 190kv
Dual focbox in FOC
VTC6 10S4P with Bestech 80A BMS

Started with:
Battery max: 50A
Motor max: 80A

Since, to try fix it, I've decreased battery max to 30, and motor to 60. Doesn't fix it.

When I throttle hard, and the board cuts out, my metr module tells me I get a DRV error, and an overcurrent error. At the same time, the voltage drops to 26V or 15V (nominal is 36V with 10s pack).
This recovers fairly fast, but did land me on the floor hard the first time I experinced this error.
The very first test ride I did with this setup went flawlessly. Pushed the board hard and nothing went wrong

Here's a metr record of 13 total errors:
https://metr.at/r/83r3m

Some help would be amazing!
```

---
## \#2 Posted by: DavidBanner Posted at: 2018-05-16T15:47:22.488Z Reads: 78

```
- removed due to not reading original post properly and making a stupid reply as a result :) -
```

---
## \#3 Posted by: Blasto Posted at: 2018-05-16T15:59:49.388Z Reads: 76

```
This sounds more like a broken P pack on the battery with that massive sag
```

---
## \#4 Posted by: DavidBanner Posted at: 2018-05-16T16:04:36.635Z Reads: 76

```
[quote="Blasto, post:3, topic:55660, full:true"]
This sounds more like a broken P pack on the battery with that massive sag
[/quote]

that would also cause DRV errors to be thrown ? what is the reason for that (just trying to learn more not disputing your prognosis)?
```

---
## \#5 Posted by: Tijmen Posted at: 2018-05-16T16:30:51.572Z Reads: 70

```
[quote="Blasto, post:3, topic:55660, full:true"]
This sounds more like a broken P pack on the battery with that massive sag
[/quote]

I also have a feeling there's a pack issue somewhere. I forgot to mention this issue only started once I switched to the pack I'm currently running.
My guess is that it could have to do with a badly connected balance wire. This could cause the BMS to think there's an issue, shutting it down briefly, causing the errors.
Really don't want to cut the shrink wrap off my pack again because I'm running low on wrap, but tomorrow I'm going to have to do it and double check everything
I must add that the pack is charging fine to 100%, indicating that there's not a major disconnect or error in the pack itself

[quote="DavidBanner, post:4, topic:55660"]
that would also cause DRV errors to be thrown ? what is the reason for that (just trying to learn more not disputing your prognosis)?
[/quote]

Yes I've read that confusion in power delivery can actually cause DRV errors. This can lead people to think their chip is fried, when in reality it's just a problem with the pack
```

---
## \#6 Posted by: DavidBanner Posted at: 2018-05-16T18:48:06.526Z Reads: 60

```
[quote="Tijmen, post:5, topic:55660"]
Yes I’ve read that confusion in power delivery can actually cause DRV errors. This can lead people to think their chip is fried, when in reality it’s just a problem with the pack
[/quote]
That makes sense, thinking it through if the DRV chip isn't getting enough voltage its going to do weird things which would trigger an error state.
```

---
## \#7 Posted by: banjaxxed Posted at: 2018-05-18T10:50:38.382Z Reads: 47

```
Interesting problem, there is very good components in this build.

AFAIK thereis no way sag can account for these voltage drops and subsequant recovery

![image|690x224](upload://giHW8WIZ6TpctyOLfVsHwnVkx9c.png)

So loose connection in the packs or BMS is going awry if wired for discharge
```

---
## \#8 Posted by: Tijmen Posted at: 2018-05-18T16:13:18.934Z Reads: 40

```
**BIG UPDATE AND FIX!!**

Ladies and gentlemen! My board lives, and it lives stronger than ever!

The issue was the BMS.
I bypassed it and there's no sign of issues. Nowhere even close. 
I did spark the bms a tiny bit at the start, which I guess caused this issue, but I'm not sure.

I did test all group voltages of my pack before bypassing my BMS to make sure it wasn't a legitimate pack issue, and my pack was perfectly balanced after discharge.

Hope this can help out some others in the future! Thanks for the suggestions guys!
```

---
## \#9 Posted by: DavidBanner Posted at: 2018-05-18T16:20:46.366Z Reads: 39

```
awesome! glad you got it working :)
```

---
