# How often do you service your esk8?

### Replies: 36 Views: 1215

## \#1 Posted by: Eboosted Posted at: 2017-12-27T06:16:50.370Z Reads: 218

```
Well this should be on the electronics subforum as well but anyways.

I do not consider myself am expert but, damn! this things really break down pretty often, there are too many variables that need attention, it's not possible, at least for me, to have a daily commuter board that you can charge and ride for 6 months with no service at all.

Being said that I service my esk8 at least once every two weeks, sometimes every week. 

These are the most common issues I've ran into:
1. Broken nut inserts (at least 2 broken every week). Since then I've upgraded from M4 to M5, they seem to be holding much better now

https://www.amazon.com/gp/aw/d/B01N4BAW6R?psc=1&ref=yo_pop_mb_pd

2. The motor mount bolts kept backing out, no matter how hard I tighted them, i used red loctite but they keep backing out, you need to use the correct amount otherwise it would be impossible to unscrew them in the future or they will back out.

3. The enclosure bolts keep on backing out, use Loctite to prevent this and tight them every week or every ride under bad roads. Use bigger screws until they keep being tight

4. Every time you have a disconnection or signal loss you need to remove the enclosure for inspection, no matter what, just do it, buy it really gets annoying after a lot of inspections.

5. The antispark switch button dies, this happened to almost all switches I've used, I suggest you buy a bigger 19mm button from eBay.

6. Board couldn't be turned off, mosfets on antispark switches were shorted, it happened to me 5 times with different brand of switches. Buy a stock of 10 mosfets from mouser.Com. There seems to be no solution on the market of a switch that does not fail. If you want to avoid all this just replace the switch with a loop key. Personally I don't like them, is not an elegant solution.

7. Battery does not charge up to 100%, this usually means cell drifting, you need to open the enclosure and measure each pack check for broken nickel strips or bad soldering jobs. I fixed the drifting and broken nickel strips by using silicone wires between packs, they won't ever disconnect or break. I'd the packs drift them manually balance them using the BMS balance plug and a lab power supply or a car bulb light to discharge the packs with higher SOC. 

8. Battery capacity tester dies too many times, after I have up on them i tried the last hope and used potty silicone behind the display to keep the vibrations outside if the electronics, it has worked so far and I stopped changing meters. 

7. Belts kept on skipping, I used to adjust them every week, they worn out pretty fast too. Since then I use 15mm belts, no more 9 or 12mm and it has helped a lot, no offer pulleys for me, seems that I don't need them.

8. Motors keep on failing, I've used all kind of motors but vibrations and bad roads just kill motors there's no way an outrunner motor could hold forever. I've opened motors so many times because of different factors, being rattling the first inconvenience, fit this ice found removing the axle from the can and bolting it back with red loctite and the holding screws have ended with the continuous disassembling/assembling nightmares and rattling

9. Bad connections on the sensor wires, I have fixed sensor wires more than any other wire, because they are very fragile. The solution was to replace the jst 6pin plugs with male and female micro USB plugs, very easy to plug/unplug.

10. Rattling on bearings, just use Zealous bearings and forget about them for a year.

11. Speed wobbles, upgrade your bushings and pivot cups  from day one, use some riptides or anything over 88A and stop adjusting your trucks everyday

12. The dreaded DRV error, once this starts to happen you j if st need to go back to BLDC or replace your DRV. Get 6 DRV chips from mouser.

This was going to be shorter but I wrote too much, I'm sorry guys. 

Please, share your most common issues those that happen all the time and how you plan to fix it.
```

---
## \#2 Posted by: ShutterShock Posted at: 2017-12-27T06:28:16.243Z Reads: 197

```
Maaaaan I have no idea what you're doing or if it's bad roads but that is a laundry list and a half :joy:

I've had no truck issues with the regular TB trucks, however I got riptides for the 218mm ones that I have now. Or anything on this list, except for one VESC randomly dying.

Belts, bolts, etc all good haha  GT2B and Nylock nuts :smiley:
```

---
## \#3 Posted by: scepterr Posted at: 2017-12-27T06:28:56.948Z Reads: 195

```
Thank you for taking the time to list all the issues, I've experienced most if not all at some point. 
I can't recall everything or how i fixed it if I fixed it but I'll go through some here. 

The battery displays most use really aren't meant for the abuse we put em through and die, somebody should make a nice clear potted one, problem solved 😋
The anti-spark switches also aren't meant for the abuse, I only use loopkeys
Motor screws, that was an annoying one, hex cap bolts solved it for me, can torque to the point of tool breaking, no loctite
Haven't had issues with motors failing or sensor wire issues, once it works, it works, for me atleast
Wobbles, definitely proper bushing and pivot to solve

I debated inserts back and forth for weeks with myself and couldn't convince myself to trust them lol, nut and bolt and I'm worry free
```

---
## \#4 Posted by: ShutterShock Posted at: 2017-12-27T06:31:17.165Z Reads: 181

```
Same here, I am a solid believer in the simplicity of the loop key,  I have no idea how some people manage to kill them, but they're definitely better than antispark switches
```

---
## \#5 Posted by: pennyboard Posted at: 2017-12-27T07:35:35.759Z Reads: 159

```
For a power switch I use a $5 toggle switch I bought at Lowe’s. Been using it for over a year at 12s and 100 Amps from Lipos with no problem. Absolutely bulletproof.

Also I seem to have a constant problem with the bolts on my (torqueboards) mounts backing out, even with locktite. I find I’m adjusting those every 2 weeks at minimum. Any advice on that?
```

---
## \#6 Posted by: Mikenopolis Posted at: 2017-12-27T07:38:02.039Z Reads: 149

```
Someone please define abuse of antispark switch. I much rather have my switches rather than a loop key. I though the benefit of loop key is just the lower cost. 

How does a antisprk switch get “abused” and while we are at it the LCD meters. Are we talking about vibration?
```

---
## \#7 Posted by: scepterr Posted at: 2017-12-27T07:40:37.121Z Reads: 149

```
Yeah when I say abuse I mean vibrations, massive g-shock, water resistance is questionable
```

---
## \#8 Posted by: ARetardedPillow Posted at: 2017-12-27T07:42:57.614Z Reads: 145

```
Strong believer in loopkeys, antisparks seem like another way of failure on an eskate
The simpler the better
```

---
## \#9 Posted by: Mikenopolis Posted at: 2017-12-27T07:46:53.756Z Reads: 146

```
The bolt backing out issue is the primary reason I’m aiming to use clevis pins on my next build
```

---
## \#10 Posted by: scepterr Posted at: 2017-12-27T07:52:49.842Z Reads: 148

```
Where I need to use low profile bolts for clearance and torquing will cause stripping I use Loctite 290, it's applied after the bolt is fastened from the open end. 

    Threadlocking adhesive - medium/ high strength. Ideal for locking preassembled fasteners.

    LOCTITE® 290 is a liquid medium/high-strength threadlocker designed for the locking and sealing of threaded fasteners. 
    Because of its low viscosity and capillary action, the product wicks between engaged threads and eliminates the need for disassembly prior to application. 
    The product cures when confined in the absence of air between close-fitting metal surfaces and prevents loosening and leakage due to shock and vibration. The product can also fill porosities in welds, castings and powdered metal parts.


    Your benefits

    Ideal for locking preassembled fasteners, e.g. instrumentation fasteners, electrical connectors and set screws
    Works on metal only
    Proven to be tolerant of minor contamination due to industrial oils, e.g. motor oils, corrosion prevention oils and cutting fluids
    Requires heat for disassembly

http://na.henkel-adhesives.com/product-search-1554.htm?nodeid=8797710385153
```

---
## \#11 Posted by: thisguyhere Posted at: 2017-12-27T08:05:24.622Z Reads: 145

```
[quote="Mikenopolis, post:6, topic:41977"]
Someone please define abuse of antispark switch
[/quote]

the vedder switch uses a small pcb and mosfets to handle all of the current switching your entire board demands. these switches have burned out time and again. a loop key is just a wire, less chance of things going wrong or getting burned out. 

[quote="Eboosted, post:1, topic:41977"]
motor mount bolts kept backing out
[/quote]

what type of hangar clamp are you using? if it's the D clamp where one bolt tensions the entire clamp (ie tb mounts), I've had those go loose on me all the time. 

switched to using two piece clamps (ie enertion, et al.) and they've yet to have come loose. 

[quote="Eboosted, post:1, topic:41977"]
enclosure bolts keep on backing out
[/quote]

clevis pins ftw

[quote="Eboosted, post:1, topic:41977"]
Every time you have a disconnection or signal loss you need to remove the enclosure for inspection
[/quote]

not a single drop out with the 2.4ghz mini. I use psycho's abs enclosures and make sure the receiver is as far away from main power leads.
```

---
## \#12 Posted by: Jammeslu Posted at: 2017-12-27T08:32:17.475Z Reads: 128

```
I have seen something on aliexpress its like a cross thing made out of hard idk the Word for ( water gardening pipe) and you put it between the motor and the motor mount and it helps with vibrations.
Never seen anyone use it why?
```

---
## \#13 Posted by: pat.speed Posted at: 2017-12-27T09:12:01.356Z Reads: 126

```
Do you mean a hose? That could actually work if it was thin enough and nice and soft
```

---
## \#14 Posted by: Jammeslu Posted at: 2017-12-27T09:39:28.518Z Reads: 127

```
No it’s the softer that you put permanently around your busches an the other end to the tap and it drips when you are away
```

---
## \#15 Posted by: Jammeslu Posted at: 2017-12-27T09:40:12.363Z Reads: 120

```
It a bit harder than a bicycle tube I supose
```

---
## \#16 Posted by: pat.speed Posted at: 2017-12-27T09:45:15.320Z Reads: 114

```
Oh yes I know what you are talking about. It's black tubing right? That could work too
```

---
## \#17 Posted by: Jammeslu Posted at: 2017-12-27T10:00:08.558Z Reads: 114

```
https://m.banggood.com/4-PCS-22XX-Series-Motor-Silicone-Anti-vibration-Pad-in-for-RC-Drone-FPV-Racing-Drone-p-1153904.html?rmmds=search

Found something similar not right size but yeah you know what I’m talking about now, this is made out of silicone so there are different materials used
```

---
## \#18 Posted by: Namasaki Posted at: 2017-12-27T14:20:17.209Z Reads: 105

```
Great Topic @Eboosted
I only ride recreationally and not every day and I avoid riding on rough roads so I have very little maintenance.
I do use compressed air to blow off the road dust regularly.
```

---
## \#19 Posted by: Eboosted Posted at: 2017-12-27T14:27:26.115Z Reads: 111

```
Yeah, riding on good roads will definitely keep you out from maintenance, I don't think any esk8 today could hold an abuse of 20-25 miles a day with little to no maintenance.

That's why I think any esk8 company building complete boards will have a hard time with warranties and a bad reputation over time, no matter what these things will break on the hands of anyone with low/none technical knowledge.
```

---
## \#20 Posted by: Deckoz Posted at: 2017-12-27T14:30:57.418Z Reads: 112

```
Hmmm

For me the board should be built and not fall apart. But maintenance...

Bearings I wash and lube every 2 weeks on a Friday when I work from home, this ends up being about 10-14 charges as I ride every day so in the range of 150-250miles my bearings get refreshed

wheel lock nuts, get replaced every time I take the wheels off. I bought a box on Amazon for cheap. I've had wheels roll off and past me. So locknut's get replaced every time(maybe get 2-3 real tightenings on them)

Wheels harder duros get scraped with a razor, softer duros get superglued glued in any cracks or pitting

Belts replaced once every month or two months depending on wear.

Battery inspected once every two months to ensure connections, and balancing

Whole board...wiped down as often as needed to keep it from trailing road grime through my kitchen..

Grip tape...I use a grip tape cleaner. I was replacing my grip every couple months as I move my feet alot and grind in dirt... But since my grip is always clean now it lasts much longer.
```

---
## \#21 Posted by: GrecoMan Posted at: 2017-12-27T14:33:42.360Z Reads: 111

```
Mine can!  

JB welded psycho mount
BKB 6374
DIY 10s6p Pack
Psycho 22” Enclosure
16/36 kit from johnny
97mm clones
TB vesc

I have ridden this thing upwards of 20 miles in 15f weather.  Only thing I have to service every once in a while is the nylock bolts holding the wheels on.  Other than that I can ride for 300-400mi without any sort of maintenance
```

---
## \#22 Posted by: surprisebirthday Posted at: 2017-12-27T14:42:35.791Z Reads: 110

```
I realize this might be a tall ask, but any idea on how much torque (e.g., newton meters) you apply to mount your motors?  I also ordered some hex cap bolts and have a handy torque wrench I'm going to use to tighten it down.  For example, when I built my bike, the handle bars and seat post have a rating in newton-meters to tell you what to set your torque wrench to.
```

---
## \#23 Posted by: Deckoz Posted at: 2017-12-27T14:45:10.190Z Reads: 108

```
I used 30-35ftlbs.  Which is about 40nm
```

---
## \#24 Posted by: Eboosted Posted at: 2017-12-27T14:45:27.043Z Reads: 106

```
Then you must have amazing roads, my roads are not that bad but 20% of my daily commute is unpaved and full of potholes.

I dare someone to ride over my conditions, which are not that bad, with little to no maintenance to their board 😎
```

---
## \#25 Posted by: GrecoMan Posted at: 2017-12-27T14:46:45.384Z Reads: 104

```
hahahaha your funny.  I live in the state that is known for having the worst roads in the US!  I’ll see if I have a gopro video of my roads later and post it

100% of my commute is full of massive potholes, like this one for example:
<img src="/uploads/db1493/original/3X/f/c/fc9460c81ddeb578415af8b83bfe07b07e552cc6.jpeg" width="283" height="178">
```

---
## \#26 Posted by: Deckoz Posted at: 2017-12-27T14:47:35.278Z Reads: 102

```
Bigger wheels play some of a factor in this too..

When my vanguard had 83mm wheels I was tightening things every day.

Since I got the 107s...I haven't touched it unless I needed to to clean or check underneath and enclosure..it's been a few months.

More thane = less loose bolts
```

---
## \#27 Posted by: Eboosted Posted at: 2017-12-27T17:59:13.244Z Reads: 95

```
That's impossible, a city could have maybe 10% like that bit not all 100% of the roads, you would be crazy to ride an eboard through those roads and crazier with hand clone wheels.
```

---
## \#28 Posted by: faithfulpuppy Posted at: 2017-12-27T20:30:17.375Z Reads: 91

```
hoping my 107s solve this, i really just want my board to be reliable above all else
```

---
## \#29 Posted by: scepterr Posted at: 2017-12-27T20:39:10.505Z Reads: 90

```
While on the topic of servicing, does anybody winterize their battery packs? Some thermal insulation?
```

---
## \#30 Posted by: Deckoz Posted at: 2017-12-27T20:44:51.882Z Reads: 90

```
I haven't. But I've considered using lipo warmers. Liions are similar and that they have the lowest IR, and highest current capabilities around 90F.... 

Cold weather really robs the packs of range.
```

---
## \#31 Posted by: Eboosted Posted at: 2017-12-27T20:46:02.898Z Reads: 87

```
I'm runing 107mm they had helped some but the vibrations are still a big issue on bad roads, everything starts to get loose or break

<img src="/uploads/db1493/original/3X/c/7/c77f50aff268bf5be821386932de6bad1756c780.jpg" width="374" height="500">
```

---
## \#32 Posted by: scepterr Posted at: 2017-12-27T20:46:55.715Z Reads: 85

```
Yeah riding around at 0c could easily mean 20-30% less range. I'm thinking just a thermal insulating wrap could have a noticeable improvement, especially if the board was inside and warm, you wanna be able to retain that in the battery
```

---
## \#33 Posted by: faithfulpuppy Posted at: 2017-12-27T20:49:27.852Z Reads: 84

```
the mounts i'm using are pretty sturdy and i doubt they'll fall apart. I've just had one of those builds where something seems to break every few rides.
```

---
## \#34 Posted by: pshaw Posted at: 2017-12-27T21:03:52.195Z Reads: 81

```
Do the anti spark heaven ones blow as well Alan? Thought those were bullet proof....
```

---
## \#35 Posted by: Mikenopolis Posted at: 2017-12-27T21:13:45.671Z Reads: 83

```
those mounting holes has way too much room for adjustment. It reminds me of perforated paper
```

---
## \#36 Posted by: Eboosted Posted at: 2017-12-27T23:37:28.904Z Reads: 74

```
Two of them have shorted mosfets, I've purchased 10 mosfets from Mouser but they are out of stock at the moment, I'll keep them here in case the one I have die.
```

---
