# Trouble going uphill with 200+ lbs

### Replies: 11 Views: 1422

## \#1 Posted by: Fetteperson Posted at: 2016-09-21T08:15:22.200Z Reads: 142

```
To my setup:

Battery:
 2x 6s 8000mah 25-50C in series

VESC:
Motor/ Batter Max: 50amp
Everything else pretty much default.
Transmitter calibrated.

Motor:

EMAX GT5345/08
KV: 190
Diameter: 63mm
Lenght: 71mm
Watt: I don't know, but similar have 3300W

Gear:
Pulley: 15/40theet
Wheel: 97mm

Now my problem is going uphill when I am driving (200lbs). It just doesn't have enough power, but when my friend (130lbs) is on the board, there is no problem going uphill.

Before I had the VESC, I had a regular 120a ESC with a 6s setup. With that I had no problems going uphill.
Otherwise the board is really fast on flats 40+ km/h.

What can I do? I don't really want a dual-motor setup (expensive). I will change 
gear ration to 10/40, but I guess this won't be enough. Do motors with 
same watt have different power in real-world? Does anyone with 200lbs+ 
have experience. Do I need to change some settings on the BLDC tool?
```

---
## \#2 Posted by: DeathCookies Posted at: 2016-09-21T08:27:02.677Z Reads: 134

```
[quote="Fetteperson, post:1, topic:9928"]
I will change gear ration to 10/40, but I guess this won't be enough.
[/quote]

Dont do it because then the belt will always skip![quote="Fetteperson, post:1, topic:9928"]
Do motors with same watt have different power in real-world?
[/quote]

Normally not. [quote="Fetteperson, post:1, topic:9928"]
Do I need to change some settings on the BLDC tool?
[/quote]

You can set up motor max to 85A. ([Information](https://www.amazon.de/GT5345-Brushless-8S-12S-6V-44V-Au%C3%9Fenl/dp/B00DK9L0ZW))
```

---
## \#3 Posted by: Fetteperson Posted at: 2016-09-21T08:45:16.217Z Reads: 128

```
I don't really understand what the different between battery max and motor max is. Doesn't 85A motor max damage the VESC, which is rated at 50amp constant?
```

---
## \#4 Posted by: sl33py Posted at: 2016-09-21T08:48:12.942Z Reads: 127

```
What @Deathcookies said.  I'm a big guy too.  You can't compare yourself w/ a 130lb buddy...  Will need a lot different setup for same hill ability.

first - 9mm, 12mm, or 15mm belt currently?

I don't see any issue w/ your batteries - try the VESC settings adjustment DC recommended, but i'm thinking you'll need to re-gear.  Or get smaller wheels - or both.

on 9mm i would not go under 13/14t - 13 might be pushing it.  12 or 15mm belt should be fine w/ 13t.  40t is pretty big, but if you have flywheels i might also look at the printable 42/44t wheel gears to gear down further.

GL!
```

---
## \#5 Posted by: DeathCookies Posted at: 2016-09-21T08:55:43.690Z Reads: 121

```
[quote="Fetteperson, post:3, topic:9928"]
Doesn't 85A motor max damage the VESC, which is rated at 50amp constant?
[/quote]

Well, i dont think so because it can handle 50A at 12S from the battery?

@all
Is my assumption actually correct?
```

---
## \#6 Posted by: Jinra Posted at: 2016-09-21T08:58:11.083Z Reads: 114

```
the VESC can take up to 240a burst current, 50a constant. This is also current supplied by battery. Motor current tends to be higher than what the battery is supplying. The extra amps should get you up to speed on hills, then decay to a lower continuous current.
```

---
## \#7 Posted by: Fetteperson Posted at: 2016-09-21T09:12:56.152Z Reads: 104

```
i use 15mm belt. shouldn't I get the biggest gear ration possible to have maximum torque? Becasue my speed on flat is fast enough, I don't care if it would be a little less.
```

---
## \#8 Posted by: Fetteperson Posted at: 2016-09-21T09:15:02.799Z Reads: 100

```
so I don't risk, damaging the vesc for longer hills? The Vesc will still only get the 50amp from the battery? Or how is it possible that the battery is giving 50amp max, but the motor is pulling 85amp max?
```

---
## \#9 Posted by: DeathCookies Posted at: 2016-09-21T09:36:19.821Z Reads: 98

```
If you want this information then just search in this thread:
http://www.electric-skateboard.builders/t/hummie-vs-devin-volts-conversion-to-amps/6910

But i think nobody from this forum can you tell this correctly...

Setup motor max to 85A and battery max to 50A. Than you are safe. Do not forget that you will reach these max values  only if you are starting from standstill on a hill or when you go with a very high speed uphill.
```

---
## \#10 Posted by: Kaly Posted at: 2016-09-21T09:49:10.026Z Reads: 96

```
@Fetteperson beside  fallowing @DeathCookies advise, when ever tackling a hill try to get some speed  before reaching the base of the hill and maintain the momentum, the system have more torque at higher speeds.
```

---
## \#11 Posted by: Bender Posted at: 2016-09-21T12:16:41.965Z Reads: 90

```
Also lowering your wheel diameter increases your torque, so some smaller wheels will help.
I'm 220lb and don't have problems with hills with a 12s single drive, but I'm on 76mm wheels, 13/36 gear ratio

I think I'm going dual on my next build with 97mm wheels
```

---
