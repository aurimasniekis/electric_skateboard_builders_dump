# Help: Robot battery

### Replies: 10 Views: 222

## \#1 Posted by: ZachTetra Posted at: 2019-04-06T19:19:45.228Z Reads: 92

```
I'm working with @DarkVortex to make a robot with a 4s1p battery, would we still need a BMS for something that small or can we skip it and just use a charger?

If we need it what are thoughts on these items
https://www.ebay.com/itm/4S-100A-14-8V-Li-ion-Lithium-18650-Battery-BMS-PCM-Protection-Board-with-Balance/264049094781?epid=2208124429&hash=item3d7a8d707d:g:BKQAAOSwKO5b8oVR&thm=10
https://www.ebay.com/itm/US-plug-power-4-2V-8-4V-12-6V-13-8V-16-8V-21V-1A-2A-Li-ion-Battery-LiPo-Charger/192609438527?hash=item2cd86acb3f:m:mNx083cke1yCQ3In3LxaOSQ
```

---
## \#2 Posted by: SeanHacker Posted at: 2019-04-06T19:25:45.269Z Reads: 86

```
@DerelictRobot
```

---
## \#3 Posted by: mmaner Posted at: 2019-04-06T19:39:08.062Z Reads: 76

```
If your using batteries you need a BMS. If you can charge to 95% and discharge to no more than 30% everytime you are ok for a few charge cycles, then you need to balance charge manually. A BMS makes life a lot easier.
```

---
## \#4 Posted by: evoheyax Posted at: 2019-04-07T02:47:14.548Z Reads: 43

```
When in doubt, bring in the robot experts haha!
```

---
## \#5 Posted by: DEEIF Posted at: 2019-04-07T03:45:03.193Z Reads: 32

```
I’m not sure if @DerelictRobot Has the same number of calls as @mmaner but here goes

@DerelictRobot @DerelictRobot @DerelictRobot
```

---
## \#6 Posted by: mmaner Posted at: 2019-04-07T03:50:13.304Z Reads: 29

```
I'm just offering advice based on experience. @DerelictRobot is an expert and professional in the. I don't he will dane to visit you plebes 😆
```

---
## \#7 Posted by: DEEIF Posted at: 2019-04-07T03:56:15.944Z Reads: 24

```
Haha I meant it as a joke because whenever I see KaramQ TSG you to call a thread he tags you 3 times in one line... 🤣(ps mmaner advice is always correct even if it doesn’t sound so)
```

---
## \#8 Posted by: DerelictRobot Posted at: 2019-04-07T04:34:15.903Z Reads: 24

```
[quote="ZachTetra, post:1, topic:89615"]
would we still need a BMS for something that small or can we skip it and just use a charger?
[/quote]

This is entirely up to you as a design choice. Personally I find it easier to build in a BMS just so you don't have to bother carrying around and hooking up a balance charger, but I've done both. 

I recently built out a 4S8P pack for a friend who is building a hexapod- using a similar BMS to what you picked out there. Charging just requires a CC/CV charger intended for li-ion/lipo.
```

---
## \#9 Posted by: KaramQ Posted at: 2019-04-07T04:38:09.115Z Reads: 22

```
I only did that once buddy
```

---
## \#10 Posted by: DEEIF Posted at: 2019-04-07T04:44:40.343Z Reads: 19

```
Only time I ever saw you close a thread 😉
```

---
