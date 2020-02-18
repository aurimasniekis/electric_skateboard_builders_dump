# Severe battery sag/degradation?

### Replies: 14 Views: 435

## \#1 Posted by: murdomeek Posted at: 2019-01-11T07:00:26.647Z Reads: 133

```
I built a diyeboard 10s5p kit back in August: http://www.diyeboard.com/10s5p-360wh-batteryescpower-truck-kit-dual-9052mm-hub-motors-p-598.html

Been riding super great.  getting around 25-35km full charge all summer and fall.  (I am super light weight).

I'd say it went through ~40-50 full charge/discharge cycles since then.
Recently, I've been taking it out on dry days, and only getting 8-12km before the battery cutoff. (All distance was measured with the same app)

The temperature difference isn't too cold these days (5-8 degrees Celsius vs 15-20 in summer/fall).  But the board is always kept indoors in room temperature.  

Is this expected behavior from a cheap pack?
Maybe its time to upgrade to a 30Q pack? :)

Thanks
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-01-11T07:19:31.663Z Reads: 125

```
Before you tear stuff all apart and start throwing new parts at the problem, I'd check a couple things first: Chck your individual cell voltages. See if there are any that don't match the rest. This will give some indication of (A) whether the cells are matched, and if the BMS has been doing it's job. I'd recommend doing this twice, once when full, once when empty. Next, I'd charge it up and monitor the voltage under load. See if it holds steady, or dips down significantly when you apply throttle. This will give you some indication of the internal resistance of the cells.
```

---
## \#3 Posted by: Trdolan03 Posted at: 2019-01-11T07:24:12.030Z Reads: 112

```
What will the internal resistance tell you? Not to hijab the thread but I have a similar issue getting just 12 miles on a 12s 8p with pneumatics. Should be closer to 20-24 from what I can tell but no such luck.
```

---
## \#4 Posted by: MysticalDork Posted at: 2019-01-11T07:37:34.575Z Reads: 103

```
high resistance will tell you the cells are worn out. Either that, or the interconnects are crappy and you're wasting lots of power heating your battery.
```

---
## \#5 Posted by: sk8l8r Posted at: 2019-01-11T10:38:14.981Z Reads: 94

```
could it be the ESC overheating? I had to cut away the drilled holes near the enc for it to get proper cooling otherwise it 'felt' like battery died way to early

OR 

I noticed an old well used diye 5p battery seemed to get better after leaving it plugged in after full charge for about at day - started to think it balanced things a little
```

---
## \#6 Posted by: bartroosen12 Posted at: 2019-01-11T10:51:19.029Z Reads: 89

```
Charge the battery (measure the voltage of every cell) and ride again until the battery says it's empty.
Then measure the voltage of every cell.
That will tell a lot about the battery status
```

---
## \#7 Posted by: murdomeek Posted at: 2019-01-11T16:37:24.466Z Reads: 75

```
I assume I would have to rip the battery apart to measure the cell voltages?

(the blue wrap thing)
```

---
## \#8 Posted by: murdomeek Posted at: 2019-01-11T17:39:03.686Z Reads: 70

```
no, its not that.
I've experienced it before also, and know its not that
```

---
## \#9 Posted by: tardyparty7 Posted at: 2019-01-11T17:54:58.041Z Reads: 70

```
u mean heat shrink?
```

---
## \#10 Posted by: MysticalDork Posted at: 2019-01-12T03:20:52.944Z Reads: 60

```
Yeah, you'll almost certainly have to slit open the heatshrink to get to the cells. It's not a hug deal, if you're careful you can tape it shut again after you're done. If needed, it's cheap to replace, and if you don't want to go that route, some stout packing tape will do a fine job in its place.
```

---
## \#11 Posted by: murdomeek Posted at: 2019-01-12T06:05:46.418Z Reads: 49

```
If i find cells that are damaged, I'd hafta buy some new cells and get a spot welder, nickel strips, etc to fix it right?

Think I might just get a new pack at this point.  due to the lack of tools and experience, I'm probably gonna eff up the new cells XD
```

---
## \#12 Posted by: dareno Posted at: 2019-01-12T06:34:50.488Z Reads: 46

```
[quote="murdomeek, post:11, topic:80559"]
Think I might just get a new pack at this point.
[/quote]
This is the best thing for you to do be honest.
I've got a few of those packs and when you open it up its a lottery as to how it was built.  I had a 10s5p that looked like crap under the skin.  Really badly assembled and once I looked at it I binned it the other one was nicely built. I have a 10s 2p and a 10s3p.  and both of these are pretty well assembled and working fine.  You'd be much better off getting a battery builder to build you a decent 30q pack and save yourself a headache.  Its the heart of the board and the last thing you should do on the cheap.
```

---
## \#13 Posted by: ShutterShock Posted at: 2019-01-12T10:02:40.497Z Reads: 40

```
I mean yeah you never know.  It is possible that there are just 2 or 3 cells a bit low that are causing that issue.  Hard to tell unless you open it to see.

I've taken apart several lipo packs, including the complex pouch kind.  What do you think you'll do with the old pack if you buy a new one?
```

---
## \#14 Posted by: murdomeek Posted at: 2019-01-12T18:02:30.046Z Reads: 28

```
either build a cheapo board.
Or most likely sell it on craigslist or this forum
```

---
