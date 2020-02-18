# Tessie &#124; Tesseract &#124; Caliber &#124; 6355 Dual Rear &#124; 10s4p &#124; 190 kv &#124; VESC &#124;

### Replies: 16 Views: 908

## \#1 Posted by: kiwi_skate Posted at: 2018-07-23T02:28:42.264Z Reads: 252

```
Hi everyone

I've been doing lots of reading as I plan my first build.  Where I am coming to at the moment is set out below but i still have some decisions to make and hopefully you guys can help!

- Loaded Cantellated Tesseract for the deck
- Caliber II 44 deg trucks (as the tesseract adds 3 deg on truck angle)
- 85mm wheels in the first instance to help avoid chance of wheelbite - might increase size later
- 10s4p (20700 cells) likely battery set up for space, weight and budget constraints - gives a high voltage to help reduce current, but leaves a bit of headroom before the VESCs max out on voltage
- Dual rear set up with 6355 motors to fit on the calibers
- VESC - ideally with a heatsink, or i'll attach my own - 4.12 version from hobbyking or similar
- I'll likely run in BLDC mode to avoid any potential implications of FOC with the 4.12 VESC
- i'd like to target a max speed of 50km/h and will probably cruise most of the time up to around 35 km/h.
- I'd like it to pull / accelerate well right through the range of speeds

My use will mostly be on the flats, but we do have a few hills on the cycle ways and paths ill be using - so needs to be a combination of hill climbing / speed - a set up that is good for both but not excellent at one i guess.

I weigh about 90kg, so with the board im guessing will be a 100kg being hurtled around.

I am now struggling with what kv motor shall I select.  I have looked at the calculators and with have two scenarios below which id love to get some of your feedback on that target a 50km/h top speed. Which one will be easier / less strain on the electric gear? I've tweaked gearing for each kv option to target 50km/h.

Calculator: https://vesc-project.com/calculators

Calculator: http://calc.esk8.it

1) 6355, 230kv motor, 85mm wheels, 14 motor pulley teeth, 36 wheel pulley teeth (2.57:1 ratio). (I think this calculator is for a single motor - so current would halve to each motor). ERPM at 57k. Motor rpm 8280.

Calculates current of 51.9 A at full throttle on flat (~50km/h)
Calculates current of 55.4 A at half throttle up a 20% gradient (25km/h)

2) 6355, 190kv motor, 85mm wheels, 17 motor pulley teeth, 36 wheel pulley teeth (2.12:1 ratio). (I think this calculator is for a single motor - so current would halve to each motor). ERPM at 47k. Motor rpm 6840.

Calculates a current of 52.4 A at full throttle on flat (~50km/h)
Calculates current of 55.6 A at half throttle up a 20% gradient (25km/h)

So if I tailor the gearing for a 190 or 230 kv, it looks like the current demand is the same - so i could go with either kv motor and gearing to target the 50km/h target and have the same hill performance?

Are there any other considerations I should assess in this decision of motor kv? 

Thanks everyone!

Sam
```

---
## \#2 Posted by: chris.hunt Posted at: 2018-07-23T03:12:55.945Z Reads: 221

```
not sure if you've purchased anything yet but this auction on eBay looks like a good deal those mounts alone are worth like $100 or more I believe and the trucks and pulleys make it a steal

https://www.ebay.com/itm/DIY-Electric-Skateboard-kit-Dual-Motor-Mount-with-Wheels-Never-Used/113161562448?hash=item1a58f46950%3Ag%3A8VMAAOSwyjNbU6Y8&LH_PrefLoc=1&_sop=1&_sacat=0&_nkw=electric+skateboard+parts&LH_ItemCondition=3&_from=R40&rt=nc
```

---
## \#3 Posted by: kiwi_skate Posted at: 2018-07-23T10:10:56.162Z Reads: 201

```
Been doing a bit more reading and found this link. Has a bit more info but still not sure if there is a performance difference between 190 kv and 230 kv that are geared to go the same top speed. Is one more efficient? Do they have different torque curves?
https://www.electric-skateboard.builders/t/who-has-experience-low-kv-vs-high-kv/17177?u=kiwi_skate
```

---
## \#4 Posted by: boardman Posted at: 2018-07-23T20:14:58.144Z Reads: 155

```
I would go with the lower kv which would lead to a power Erpm. I think if you look into vesc discussions you'll see that vescs are rate for about 60k eprm max.
```

---
## \#5 Posted by: kiwi_skate Posted at: 2018-07-24T01:55:41.075Z Reads: 157

```
Hi - thanks for the reply.

Looking at Ben Vedder's post on choosing the right kV again:

http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/

I've seen the target is to set up the battery voltage, gearing and kv to hit your planned maximum speed with a motor rpm of 8,600 rpm, and this will hit the target of max 60k ERPM.

So if I say - ~50km/h max speed, 16t motor pulley, 36t wheel pulley and 10s set up.  At full charge, voltage might be up to 42v, so I want a kv of 8,600/42=205 kv (max to not exceed the 60k ERPM).  This gives an ERPM of right on 60k ERPM.

After a bit of riding, might be back down at nominal voltage for 10s at 37v - which if using a 205 kv motor gives me an ERPM of around 50k ERPM.

So, I'm currently concluding:

- 100kg (rider plus board)
- 16t motor pulley, 36t wheel pulley
- 10s4p battery pack with 20700 cells
- dual 6355 motors at 200 kv
- 85mm wheels
- max speed ~50km/h
- max ~20% gradient hills possible (will find out i guess????)

Anyone around this weight and use this set up?

Thanks
```

---
## \#6 Posted by: Wraith Posted at: 2018-07-24T02:32:40.813Z Reads: 141

```
you mentioned the tesseract adds 3 deg on the angle so going with the Caliber II 44 deg will actually give a total of 47deg when mounted w/o any risers? 

How high off the ground is it with that setup? curious as I'm planning out my truck setup on my tesseract build too!
```

---
## \#7 Posted by: kiwi_skate Posted at: 2018-07-24T09:29:03.200Z Reads: 124

```
Thats what ive read about the truck angle.

I havent got the trucks or wheels yet but will let you know. Board arrived today.
```

---
## \#8 Posted by: Wraith Posted at: 2018-07-24T09:30:18.259Z Reads: 125

```
cool great to hear! looking forward to hearing back from you and seeing photos with it!
```

---
## \#9 Posted by: kiwi_skate Posted at: 2018-07-24T09:31:44.162Z Reads: 134

```
![1532424567278-408468085|280x499](upload://4WzLnRRBqvTE3BRhCxJg6hdMXDB.jpg)

![1532424621783363848108|690x387](upload://x4m1X3LgQEiC1ZOnJjmnkcJ0uWz.jpg)
```

---
## \#10 Posted by: Wraith Posted at: 2018-07-24T10:26:36.816Z Reads: 125

```
Hows the angle with the trucks?
```

---
## \#11 Posted by: Luuke Posted at: 2018-07-24T11:11:47.568Z Reads: 124

```
I have the same board with 44° Caliber II.
With my 90mm Wheels I need 1/2" riser and the right bushings.

I use a 170kv mono drive with 10S and 20T - 36T what leads to 50km/h max. speed (loaded)
```

---
## \#12 Posted by: Wraith Posted at: 2018-07-24T12:05:01.583Z Reads: 119

```
Is it riding too low for your enclosure with  44deg trucks?
```

---
## \#13 Posted by: Wraith Posted at: 2018-07-24T12:05:57.303Z Reads: 121

```
That makes me think that 50deg is where its at for me if I go with an altar wedge enclosure from @psychotiller
```

---
## \#14 Posted by: kiwi_skate Posted at: 2018-07-24T12:21:20.756Z Reads: 119

```
What motor mounts did you go for?

Looking around on available sites i'm leaning towards just getting the motors, VESC, mounts and pulleys from DIY electric.  Im in New Zealand and they do free shipping on orders over 300 and seem to be fairly reasonably priced.

Why did you go for a sealed motor on your build? Do they overheat more easily?

Your soldering skills on your build looks epic!
```

---
## \#15 Posted by: Luuke Posted at: 2018-07-25T15:26:30.867Z Reads: 101

```
I am using the hobbyking mounts. But you have to file down a little to fit to the caliber profile.
Back then I tought, that I need/want a sealed motor. meanwhile I am not sure about that any more.
The sealed one is heating up, but I can not compare to other motors. But the temperature of the focbox is higher then the motor, so that is the limiting factor here.
```

---
## \#16 Posted by: kiwi_skate Posted at: 2018-07-31T12:13:03.469Z Reads: 90

```
![IMG_20180801_000624|280x499](upload://8JaTCwhb2SR6YvfIqKPVB0JsM55.jpg)

I have laid out the main components on my deck with some old trucks I had lying around. Im thinking the layout above will mean my custom enclosure can be shaped similar to the board itself so it kind of matches. Also makes use of the flat are behind front trucks without getting into the wheel wells. Using 20700 cells for good capacity.

Or this option below. Any thoughts from your experience?

![IMG_20180801_000556|280x499](upload://gzb8fVpL6NcFqwXMashwbN4qggq.jpg)
```

---
