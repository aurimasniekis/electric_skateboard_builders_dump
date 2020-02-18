# Voltage cut off under load

### Replies: 25 Views: 297

## \#1 Posted by: Jordan12 Posted at: 2019-05-22T18:39:13.262Z Reads: 100

```
Looked around on the forums for help but I could find anything to help.

190kv 
10s4p
Vesc 4.12

At full charge and up to 3/4ths throttle everything is fine. When I hit full throttle sometimes the vesc cuts out, I have to break a little then I can continue riding.
When the battery starts getting lower full throttle doesn’t seem to bother it as much.
I can ride around all day with no issues if don’t go full throttle.

The following faults were registered since start:

Fault : FAULT_CODE_UNDER_VOLTAGE

Current : -0.2

Current filtered : -0.1

Voltage : 8.00

Duty : 0.950

RPM : 10722.7

Tacho : 107023

Cycles running : 0

TIM duty : 4560

TIM val samp : 1200

TIM current samp : 3600

TIM top : 4800

Comm step : 3

Temperature : 56.14

Fault : FAULT_CODE_UNDER_VOLTAGE

Current : 0.6

Current filtered : 0.1

Voltage : 8.00

Duty : 0.950

RPM : 10789.4

Tacho : 120744

Cycles running : 0

TIM duty : 4560

TIM val samp : 1200

TIM current samp : 3600

TIM top : 4800

Comm step : 2

Temperature : 55.61

Fault : FAULT_CODE_UNDER_VOLTAGE

Current : 0.2

Current filtered : -0.2

Voltage : 8.00

Duty : 0.950

RPM : 10663.5

Tacho : 123542

Cycles running : 0

TIM duty : 4560

TIM val samp : 1200

TIM current samp : 3600

TIM top : 4800

Comm step : 4

Temperature : 55.53
**vesc settings**
Motor current 70a
     Max break. -60a
Absolute 130a
Battery 50/-50
Voltage cut off 34-31
```

---
## \#2 Posted by: Jinra Posted at: 2019-05-22T18:41:53.651Z Reads: 86

```
This exact thing happens when I was testing my unbalanced battery. It was due to the BMS freaking out and cutting off load. Are you discharging through your BMS?
```

---
## \#3 Posted by: Jordan12 Posted at: 2019-05-22T18:46:01.787Z Reads: 84

```
Yes I am, the battery was balanced when I got it two days ago
```

---
## \#4 Posted by: Soflo Posted at: 2019-05-22T18:46:46.202Z Reads: 85

```
Cell sag will do that.
```

---
## \#5 Posted by: Jordan12 Posted at: 2019-05-22T18:48:08.464Z Reads: 83

```
Is it common for it to sag that bad to cut off the vesc?
And if so is there a way I set some setting combat that?
```

---
## \#6 Posted by: Jinra Posted at: 2019-05-22T18:51:17.074Z Reads: 75

```
Cell sag does NOT sag that low. This is most likely BMS cutting off due to overcurrent. What pack do you have? @Jordan12
```

---
## \#7 Posted by: AlanZhou Posted at: 2019-05-22T18:52:10.133Z Reads: 71

```
Another possibility is fake cells not being able to handle the amperage and sagging
```

---
## \#8 Posted by: Jordan12 Posted at: 2019-05-22T18:55:40.141Z Reads: 67

```
Lol a nice beauty from China.....
I’m saving up for a nice 30Q I promise
```

---
## \#9 Posted by: Jinra Posted at: 2019-05-22T18:56:34.594Z Reads: 65

```
yea.. you're probably gonna want to limit the current on the vesc to whatever the pack can support.
```

---
## \#10 Posted by: Jordan12 Posted at: 2019-05-22T18:58:27.894Z Reads: 64

```
The battery and motor current?
```

---
## \#11 Posted by: Jordan12 Posted at: 2019-05-22T18:58:44.862Z Reads: 63

```
And any recommendations?
```

---
## \#12 Posted by: Jinra Posted at: 2019-05-22T19:00:10.369Z Reads: 61

```
Just battery current. Also your battery min is WAYYYY too high. What pack do you have 10s?p and what cells?

EDIT: nvm i see it's 10s4p, but would still like to know the cells. 50 amps should be fine for it unless they're fake cells, though they might have included a shitty BMS
```

---
## \#13 Posted by: Jordan12 Posted at: 2019-05-22T19:17:40.093Z Reads: 53

```
I’m honestly not sure why I left it that high.
And I don’t know I’ve been trying to ask them but they just keep saying “it’s a 18650 cell”
.... thanks
```

---
## \#14 Posted by: Jordan12 Posted at: 2019-05-22T19:18:12.864Z Reads: 53

```
I did order a supower bms to replace this one, had issues with a 6s2p battery that wouldn’t fully charge
```

---
## \#15 Posted by: Jinra Posted at: 2019-05-22T19:18:20.142Z Reads: 47

```
yea.. my guess is BMS cutoff, you could bypass discharge, but without knowing the cells, it can be risky
```

---
## \#16 Posted by: Jordan12 Posted at: 2019-05-22T19:25:40.575Z Reads: 44

```
I’ll start with lowering the battery amps see if that helps. 
Resent them a message, probably won’t hear anything back the worst people to contact.
```

---
## \#17 Posted by: Jinra Posted at: 2019-05-22T19:26:34.983Z Reads: 42

```
single motor right? I'd use 30a battery max as a conservative setting.
```

---
## \#18 Posted by: Jordan12 Posted at: 2019-05-22T19:40:21.571Z Reads: 41

```
Yes single motor 

Will do. Thanks for all yalls replies
```

---
## \#19 Posted by: JakeSkate Posted at: 2019-05-22T23:40:15.104Z Reads: 35

```
If you are dead set on not changing battery packs for the moment you might be able to drop some rather large caps in parallel with your pack. I know that the vesc's have their own but some ultra caps might be enough to make the sudden current draw a little less harsh. 

I would say bypass the BMS and just ride with a fire extinguisher if you just want all the current though. :rofl:
```

---
## \#20 Posted by: Jordan12 Posted at: 2019-05-22T23:51:33.394Z Reads: 33

```
@JakeSkate Got a link on how that works? I’d like to learn more about that stuff.
Lowering the current pull from the battery seemed to help. I didn’t fully get on it yet.
```

---
## \#21 Posted by: JakeSkate Posted at: 2019-05-22T23:58:49.343Z Reads: 35

```
Yeah, This image is a decent depiction of what is probably tripping your BMS protection. [Inrush_current](https://www.google.com/search?client=ubuntu&channel=fs&tbm=isch&q=capacitor+high+current+draw&chips=q:capacitor+high+current+draw,online_chips:inrush+current&usg=AI4_-kQtzR_FVyn5neAU_z_5ZZezM-Lszg&sa=X&ved=0ahUKEwjozqbVqrDiAhVQaq0KHQeJABEQ4lYILygH&biw=1366&bih=629&dpr=1#imgrc=2WOf1TC8NbBCuM:)  Basically inrush current is a the sudden current draw that occurs when first applying voltage to the motor coils which act as a dead short to the battery. There is also a ton a current required to get your moving on your board from a dead stop but once you're at speed all your motor is doing is overcoming friction so the current draw is less.

When you toss in that capacitor it holds enough energy that it can "smooth" out that sudden current draw(if it's big enough).

EDIT: if you want to learn more about EE stuff than I would take a look at allaboutcircuits it has some good noncalculus based resources.
```

---
## \#22 Posted by: Jordan12 Posted at: 2019-05-23T00:30:53.885Z Reads: 29

```
Does one need to go one each parallel? I’m trying to find info on them, or coulda few go upstream heading into the vesc? Or do they have to go before the bms?
```

---
## \#23 Posted by: Jordan12 Posted at: 2019-05-23T00:31:07.888Z Reads: 28

```
I’m trying to find a diagram
```

---
## \#24 Posted by: JakeSkate Posted at: 2019-05-23T00:33:21.535Z Reads: 28

```
This is the same concept, the capacitor goes directly across the terminals of your battery.
![](https://usercontent2.hubstatic.com/12189367.jpg)
```

---
## \#25 Posted by: Jordan12 Posted at: 2019-05-23T14:45:36.598Z Reads: 22

```
Well took out the board this morning 
Vesc settings:
Motor 60/-60
Battery 40/-40

Worked great even under full throttle up hills!
I also think I may have set the motor settings too high also just read through my parts again and it said max 65, I had it on 70....
```

---
