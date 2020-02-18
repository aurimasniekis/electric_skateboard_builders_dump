# First build parts list! (Help me&hellip;)

### Replies: 16 Views: 1642

## \#1 Posted by: nihliphobe Posted at: 2016-07-07T19:35:26.752Z Reads: 140

```
Hey all!
This is my first proposed build, before I started sourcing parts I wanted to poll the community to make sure i'm not doing anything incompatible or missing something crucial. I've based this mostly off of the suggested new builders parts list / other forum lurking.

| deck: Omen Buzzkill (90)
| trucks: caliber II (50)
| wheels: Flywheel clones w/ bearings http://www.amazon.com/Longboard-Wheels-Bones-Bearings-Spacers/dp/B00JFBTDDK/ref=sr_1_1?ie=UTF8&amp;qid=1455717063&amp;sr=8-1&amp;keywords=pro+longboard+wheels+83mm+with+bearings (40)
| Motor: Olinboard co om5065 170kw http://www.ollinboardcompany.com/product/om5065-170kv (73)
| ESC: Olinboard Vedders speed controller http://www.ollinboardcompany.com/product/vedder-s-speed-controller (165)
| Battery: 4 3s 5000mah 20C lipos HobbyKing (96)
| 12S series charger: (50)
| Enertion Single Motor Mount: (60)
| 14/36 Gearing: Enertion 9mm 256t belt, enertion 9mm 14t motor pulley, 
| enertion 9mm 36t drive hub
| Controller: Psycotiller's Winning Mini Thumb Stick Controller (50)
| Pyschotiller Enclosure: (50)

Trying to keep the whole build under $1000, pre shipping I'm at 760 I believe so if there are any suggestions for parts let me know.

Thank you so much, I'm really looking forward to contributing to this forum!
```

---
## \#2 Posted by: sl33py Posted at: 2016-07-07T19:54:31.627Z Reads: 129

```
Looks like a solid build.  Depending on your weight - i might look at the 12mm or15mm wide motor, pulleys, and belt.  More contact area will help avoid teeth skipping on hard braking (and after worn a bit sometimes hard acceleration).
```

---
## \#3 Posted by: Jinra Posted at: 2016-07-07T20:11:44.985Z Reads: 108

```
As @sl33py said, if you're running single motor, step up to a 12/15mm belt. You can run it in a dual diag config later as well if you decide to go dual motor. Also be careful with some clones as they sometimes have thicker spokes which makes it hard to fit pulleys onto them. However, these *should* be fine.

Keep in mind that Enertions wheel pulley needs a modified caliber truck (about 5mm taken off the hangar). If you want to avoid having to do this, get Enertion's trucks as well.
```

---
## \#4 Posted by: nihliphobe Posted at: 2016-07-07T20:19:19.039Z Reads: 99

```
Thanks @sl33py and @Jinra! I'll switch to the enertion trucks and step it up to a 12 or 15 mm pulley.
```

---
## \#5 Posted by: Pablo_702 Posted at: 2016-07-07T20:45:22.193Z Reads: 92

```
what kind of charger is that? 12S $50
```

---
## \#6 Posted by: nihliphobe Posted at: 2016-07-07T20:47:47.914Z Reads: 90

```
I was looking at different ways of charging the batteries and people said that switching between parallel and series for charging was a massive pain. So I looked at just charging them in series. The charger was from ebay that somebody mentioned on here, I might need to bump up that estimate.

If anybody has suggestions for a better charger with this setup that would be very appreciated!
```

---
## \#7 Posted by: Pablo_702 Posted at: 2016-07-07T21:02:41.377Z Reads: 86

```
it was probably me im using a venom dual pro charger that lets me charge up to two 6s at the same time and its $85, i love it im charging them with out removing my enclosure
```

---
## \#8 Posted by: sl33py Posted at: 2016-07-07T22:05:30.871Z Reads: 89

```
12s charging is usually expensive, complex, or both!

I rarely run 12s, but have 3 or 4 chargers (Icharger 306b, iMax B6ACv2, a small el-cheapo for 3/4s at work, and the hobbypartz thunder 1220) to make it somewhat easier.  Most of the time it's easier (IMO) to simply disconnect them - plug into parallel board for charge and balance, then reconnect.  I usually prefer the iCharger

Plug and play simplicity i'd go for true BMS.  My one "12s" charger is a bit odd and fiddly - two separate balance plugs - basically two 6s chargers in one as best i can tell.  Since i've gone away from bigger (and more $) packs (6/8/10/12s lipos), the parallel board works great.  The best i think are the BuddyRC/Paraboard ones - but i've also seen some from HK that already have the XT90 connectors mounted to the PCB (nicer than my xt60->xt90 adapter cables).
```

---
## \#9 Posted by: nihliphobe Posted at: 2016-07-07T22:07:55.767Z Reads: 83

```
Hmnnn, interesting. I originally went with 12s because my campus is quite hilly and I thought i'd need the extra power to chew through the hills on a single motor at this gearing while maintaining the possibility of speed. I was going to look at switching down to a 10s to reduce the complexity of charging but i'll probably just take your advice sl33py and go for a true BMS. 
I'm definitely looking for that plug and play solution. More research!
```

---
## \#10 Posted by: sl33py Posted at: 2016-07-07T22:21:21.008Z Reads: 82

```
More power helps obviously, but it's going to depend on the size of your hills and how much you weigh.

I can make it up some moderate hills and i'm a heavy bastard (265lbs/120kg) - the trick really is to get some running start and keep momentum/rpms up where it can produce power.  Lugging it down or trying to start on a hill is tough!

do you know grade % of your hills?  (there is an app for that btw)  and how much do you weigh?

another critical piece - i think you've looked at least to determine - is gearing.  wheel size, gears, and voltage - i like to target around 20-25mph top speed (stupid fast), and gear as low as i can within reason.

My typical setup is 13/14t motor, 36t wheel on 8s.  With a 190/200kv motor it works well for me.  I've done some at 12t motor gears - but they like to skip a lot with so few teeth engaged.  Not sure if the 12/15mm belts would make a big enough difference to gear this low.
```

---
## \#11 Posted by: nihliphobe Posted at: 2016-07-07T22:25:10.898Z Reads: 74

```
Awesome info, thanks so much sleepy! I don't know the grade of my hills, unfortunately off campus until august. I weigh around 145lbs. Running start huh? I heard you shouldn't push on an eboard, that's gotta be quite the running start! :smile:
 
Gearing wise i'm on the same page, probably 14/36. Bumping the motor up to the 200kv version might well make the 8s feasible. Still shooting for a 20mph weighted top speed, that's my minimum. Everything past that is speed gravy.
```

---
## \#12 Posted by: Jinra Posted at: 2016-07-07T22:27:02.170Z Reads: 72

```
You should hit 20mph on flats no problem. As for kicking, you **should** kick to less stress your components and improve your battery life, especially if you're running unsensored.
```

---
## \#13 Posted by: nihliphobe Posted at: 2016-07-07T23:16:24.254Z Reads: 63

```
That's v. good to know, glad to know I won't be doing any harm if I ever decide to get some exercise!
```

---
## \#14 Posted by: nihliphobe Posted at: 2016-07-08T03:49:13.934Z Reads: 60

```
Based on your feedback, here's my updated list for those who care :)
| deck: Omen Buzzkill (90)
| trucks: enertion trucks (60)
| wheels: Flywheel clones w/ bearings http://www.amazon.com/Longboard-Wheels-
| Bones-Bearings-Spacers/dp/B00JFBTDDK/ref=sr_1_1?ie=UTF8&amp;qid=1455717063&am
| p;sr=8-1&amp;keywords=pro+longboard+wheels+83mm+with+bearings (40)
| Motor: Olinboard co om5065 200kv sensored(73)
| ESC: Olinboard Vedders speed controller 
| http://www.ollinboardcompany.com/product/vedder-s-speed-controller (165)
| Battery: Enertion Space Cell Pro3 http://www.electric-
| skateboard.builders/t/36v-10s-electric-skateboard-battery-space-cell/68 (343)
| Battery Charger: Fast Charger (59)
| Enertion Single Motor Mount: (60)
| 14/36 Gearing: Enertion 12mm 256t belt, enertion 12mm 14t motor pulley, 
| enertion 12mm 36t drive hub (35)
| Controller: Psycotiller's Winning Mini Thumb Stick Controller (50)
| Pyschotiller Enclosure: (70)
I think switching to the 10s spacecell will end up being the right choice in terms of making my charging solution plug and play.
```

---
## \#15 Posted by: Michaelinvegas Posted at: 2016-07-08T03:54:24.791Z Reads: 56

```
Thanks goodness ....a person that take good advise to heart
```

---
## \#16 Posted by: Michaelinvegas Posted at: 2016-07-08T03:55:32.981Z Reads: 50

```
You may want to add any shipping costs to make sure it all works with your budget
```

---
