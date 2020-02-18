# First build. help

### Replies: 8 Views: 637

## \#1 Posted by: astread Posted at: 2016-12-28T18:47:41.587Z Reads: 73

```
Hey guys. I've been riding a magneto board for a year now, it's been great but I'm hungry for more speed. I've looked around for other boards but nothing seems worth the price.. so I want to build one.
I've got a few decks in mind and gone for the space cell pro 3 which comes with the controller and the housing for it. I would preferably want a single motor as I can get more range but what do I get? I want as little labour as possible so kits would be nice but not necessary. I'm looking for a top high speed (at least 22mph) which is the reason for me building a board. Also what vesc would work best?
I live in a flat land area so I won't be climbing any hills.
Any other help/ tip would be appreciated 
Thanks
```

---
## \#2 Posted by: Iceni Posted at: 2016-12-28T19:09:13.485Z Reads: 73

```
With the space cell a motor around 200kv will be the sweet spot.
For single motor setup a 6374 size is what most people would recommend.

Depending on where you live (EU/us/aus) you got different options when it comes to vendors. 
For EU I'd recommend www.esk8.de, they got both the motors and good quality vesc.
You also have www.alienpowersystems.com, not sure if they have the vesc though.

If you're in the US you got either www. or www.ollinboardcompany.com
Ollin propably has the most well built vesc on market.

For Australia you got www.enertionboards.com
But you know about them already seeing as you got the space cell ;)
```

---
## \#3 Posted by: sl33py Posted at: 2016-12-28T19:56:43.878Z Reads: 63

```
Welcome to the forum and this sounds like a fun project.

I would double check your weight - just to confirm a single motor will work ok for you.

Yes a single will give you more range, but be slower accelerating (likely not an issue - a single is a LOT of fun), and much harder to go up hills (also sounds like not an issue for you).

Where do you live?  That will help steer us recommend suppliers near you (as @Iceni mentioned already).

VESC should work really well for this.  I too would suggest a bigger 63mm motor likt eh 6374 - anywhere from 149kv - 200'ish kv.  

For a kit, i personally prefer DIYes setup with his aluminum wheel gears, then enertion's next.  As a kit you get everything that works together correctly.  No guessing or waiting to get the right length belt etc.  The enertion one does require you to use their modified trucks, or to modify you Caliber II's to get the wheel gear to fit correctly.  You need at least a dremel and some time to cut away the aluminum on the hanger to fit.  

Speed will absolutely be dependent on gearing.  Check out some of the calculators that are all over the place.

A quick check of a "standard" setup (gearing wise) - using the SPACE cell 3 (10s3p) =

83mm wheels, 190kv motor, 10s, 15/36 (motor/wheel gearing):
<img src="/uploads/db1493/original/3X/9/e/9e7a24b64ebeb40df7c205de74a1adb609e838ee.JPG" width="690" height="179">

26mph is really really scary fast depending on your skill and board and surface you'll ride...

You could gear down a little to get more torque and startup speed... or increase to 40t on the wheel gear (drops almost 2mph exactly to 24mph).

149kv same setup = almost exactly 22mph (says the calc - usually pretty accurate from my tests).  170kv might be a good "sweet spot" setup too.

I usually target a top speed of 25mph and that's plenty fast for me.  but i'm not a downhill guy and don't need top speed - instead i want torque and hill climbing ability.

HTH - GL!
```

---
## \#4 Posted by: astread Posted at: 2016-12-28T20:16:12.964Z Reads: 51

```
A lot info here, thanks! 
I'm a light guy around 150lbs so a single motor would be fine. 26 mph seems good, but would increasing the kv of the motor massively decrease range? As I also don't want the range of the boosted board.
I'm located in UK, around London but I don't mind waiting a while for shipping if it would be worth it.
```

---
## \#5 Posted by: Hummie Posted at: 2016-12-28T20:31:44.327Z Reads: 48

```
Increasing the kv won't decrease range if you add to the gear ratio
```

---
## \#6 Posted by: Iceni Posted at: 2016-12-28T21:29:49.660Z Reads: 45

```
The benefit of ordering from esk8 or alien is you don't have to pay import duties since it's within EU which will otherwise add to the cost.

I have a space cell with a dual 240kv motor setup, and I get roughly 15km range.
I wouldn't recommend using 240's, since with a 13/36 gearing it still does 30 mph, and that my friend is not a speed you want to go on anything but a perfectly paved road :P
```

---
## \#7 Posted by: astread Posted at: 2016-12-28T21:51:32.739Z Reads: 44

```
I'm a little confused, the space cell says it can only take motors with a max of 2400w however I see 6374 motors with 3200w?
```

---
## \#8 Posted by: Iceni Posted at: 2016-12-28T22:18:04.000Z Reads: 39

```
The space cell is limited to 60 amp output I believe. 
Which is plenty of power, especially for a single drive. 
The watt rating on the motors are their maximum tolerance before they burn up, and running them with less is no problem, though you need to limit the amp draw in the vesc firmware to not pull more than the battery can deliver.
```

---
