# Electronic Q for noobs

### Replies: 6 Views: 582

## \#1 Posted by: lamjiasheng Posted at: 2017-05-21T05:49:08.423Z Reads: 99

```
What ESC/BATTERY/MOTOR match for
-25mph
-15miles

Can u guys tell me what to look for when matching these parts :)
```

---
## \#2 Posted by: saul Posted at: 2017-05-21T07:11:33.221Z Reads: 91

```
there are more than a few ways to get what you want. its really a question of $$ and builder skills.

heres my usual rec
http://esk8.today/guides/build-guide/
```

---
## \#3 Posted by: Nordle Posted at: 2017-05-21T07:29:25.330Z Reads: 86

```
Straight answer to your question:
"..depends on wheel size"
```

---
## \#4 Posted by: Eboosted Posted at: 2017-05-21T18:45:40.294Z Reads: 59

```
Here is the most common setup for your requirements

10S4P battery on Samsung 30q
6374 190kv motor
97mm wheel size
15/40T pulleys
Vesc (I'll still call it that way forever)
```

---
## \#5 Posted by: sl33py Posted at: 2017-05-21T20:05:51.686Z Reads: 49

```
I typically would work backwards from battery (# Series) to ESC (that can handle that voltage/# S).  

Deck and wheels - i like bigger wheels... but not every deck will clear even 83mm wheels (my recommended starter setup).  So **first determining deck you like** and then fitting wheels that you can squeeze in with *minimal* risers.  (again my preference - i like to keep deck height lower for pushing and more stability).  So a typical top mount deck you'll probably need 1/4-1/2 risers (i do like 1/8 shock pads for helping absorb vibrations/bumps a bit).  If you go with a symmetrical deck like a vanguard - you can probably fit 97's w/o issue.  I'd still suggest 83mm as a start.  If on a budget some 83mm clones are hard to beat for the $.  If down the road you want softer thane get legit flywheels (if you can find).

So in my theoretical build i'd have 8-10s (lipo - li-ion is a lot more $ and more voltage sag than nicer lipo) - VESC - 83mm wheels.  And 190-200kv motor tops to avoid 60k ERPM issue w/ VESC 4.xx.

Then you just need to figure out gearing for your speed wanted.

83mm - 190kv - 10s - 15/36 = 26/27mph
same - 8s - 22mph

If you want more hills i might go to 40t wheel gear (DIYes 12mm or 15mm wide from @Titoxd10001):
83mm - 190kv - 10s - 15/40 =  24mph

If you are on a budget, and especially if you a lighter rider - a single motor setup should work well unless you have big hills or want to accelerate like a bat outta hell.  I'm a big guy and ride single setups regularly just fine.  I might walk up some steeper hills and go slower up others...

The "build guide" @saul posted is a good start.  One clarification/edit i'd suggest is regarding dual motors:
[quote]
Booster Build #3:

Dual motors mean double the torque, **_higher top speed_**, and more hill climbing ability.[/quote]
Not totally true.  On the flats dual motors will not get you a faster top speed - your speed is limited by voltage/kv and gearing.  one motor or two will have the same speed.  Getting quickly to that top speed (acceleration), and going uphill will benefit from a second motor.

**AND an obligatory caution especially for a new rider:**

**Ride within your skill level.**  If you are a long time downhill ninja - cool.  "25 mph" sounds like a *great* idea... but if you don't have appropriate skills - it's stupid fast and _bone breaking speed._  **Wear appropriate gear for the speed you intend to ride.**  Downhill folks wear leathers for a reason.  **A helmet really should be a must regardless of speed.**  /soapbox

My long-winded .02

HTH - GL!
```

---
## \#6 Posted by: sl33py Posted at: 2017-05-21T20:27:54.473Z Reads: 30

```
in my long winded reply - i didn't comment on range...

Again i suggest lipo over li-ion to start.  Yes li-ion are sexier...  slim... and safer (given reasonable precaution).  But they are more $, have more voltage sag (depending on battery chosen, and # parallel to distribute amp load), and heavier Wh to Wh.

Starting and wanting the lightest, most powerful battery w/ minimal sag - i still think quality lipo is a great start.

Range = 10Wh = 1km (flats w/o racing).  so with your goal of 15mi (24km), you want a 240+Wh pack.  If you really *need* the full 15mi range i'd build in a bit extra personally.

To determine Wh:  Take your pack voltage (10s for simplicity = 42v) x Ah (mAh/Ah 5000mAh=5Ah) = Wh.  So a 10s(42v) x 5Ah = 210Wh.

HTH - GL!
```

---
