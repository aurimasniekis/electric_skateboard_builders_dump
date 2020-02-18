# Torque converter on a board?

### Replies: 14 Views: 722

## \#1 Posted by: Hummie Posted at: 2018-05-06T19:38:44.407Z Reads: 198

```
Torque converters seem pretty awesome: efficient n quiet.   Why aren't any boards using one?
```

---
## \#2 Posted by: MysticalDork Posted at: 2018-05-06T21:36:07.357Z Reads: 177

```
Because the purpose of a torque converter is to solve an issue that electric motors don't have. Same reason electric cars don't use torque converters.
```

---
## \#3 Posted by: Hummie Posted at: 2018-05-06T21:54:41.087Z Reads: 164

```
Maybe I should say fluid gearbox.  I know a torque converter can disconnect when the vehicle stops moving which wouldn't be a help but a coupling w a 3:1 that was liquid would be cool and quiet.
```

---
## \#4 Posted by: MysticalDork Posted at: 2018-05-06T22:10:34.350Z Reads: 153

```
A torque converter's main function is to remove the need for a clutch between a prime mover and a transmission/gearbox, to allow the prime mover to idle while in gear.

Since electric motors don't need to idle, and thus don't need a clutch, they don't need a torque converter.  

They're inefficient, messy, large and a pain to design.

Gears/belts are cheaper, cleaner, more efficient and easier to design.
```

---
## \#5 Posted by: FredrikHems Posted at: 2018-05-06T22:10:36.370Z Reads: 154

```
I am not totally sure If you and @MysticalDork is thinking the same. If you are, just ignore this:

As far as I know the torque converters job is to make the engine stay in its optimum rpm range, as they put out more torque at higher rpms vs lower. 

However Electric motors dont have this problem as they put out the same torque all over the rpm range, which makes the torque converter unessecary
```

---
## \#6 Posted by: b264 Posted at: 2018-05-06T22:17:27.063Z Reads: 146

```
This reminds me of putting a differential on an esk8.  Cars have differentials because they don't have two engines.  One engine per wheel would be far better and allow maximum power transfer.  They get over this limitation by using a differential so the car doesn't have torque steer as a single-wheel drive.  The other alternative is to reduce the number of rear wheels like the [Polaris Slingshot](https://slingshot.polaris.com/en-us/).

To reduce the number of motors, just to create the problem, so you can solve it by using a differential -- sounds silly to me.

This topic reminds me of that.
```

---
## \#7 Posted by: DeathCookies Posted at: 2018-05-06T22:45:28.764Z Reads: 125

```
Maybe @Hummie want to use it for his hubmotor in some kind of creative way?

[quote="Hummie, post:3, topic:54593"]
but a coupling w a 3:1 that was liquid would be cool and quiet.
[/quote]

i think he wants to try to use a 100kv motor with a 3:1 coupling. that would result in excelent start ups and will overcome the speed limit of a (100kv`*`battery voltage*wheel diameter) motor by 3.
```

---
## \#8 Posted by: b264 Posted at: 2018-05-06T23:05:49.562Z Reads: 115

```
[quote="DeathCookies, post:7, topic:54593"]
i think he wants to try to use a 100kv motor with a 3:1 coupling. that would result in excelent start ups and will overcome the speed limit of a (100kv*battery voltage*wheel diameter) motor by 3.
[/quote]

Then he could use planetary gears - or anything else besides a torque converter?  Electric motors already have full torque all the way down to zero speed ....

This is like adding a clutch when you could just stop applying power to the motor
```

---
## \#9 Posted by: ARetardedPillow Posted at: 2018-05-06T23:16:18.872Z Reads: 103

```
2018 prediction: someone releases a "torque converter" that's not a torque converter, just like someone else released direct drive that's not direct drive
```

---
## \#10 Posted by: Hummie Posted at: 2018-05-06T23:16:31.771Z Reads: 102

```
a fluid gearbox is what Im looking for.   Isnt there a 3:1 fluid gearbox?   a coupling maybe or something.  don't know the terminology.  @DeathCookies no application in mind,  more so a regular pulley board.  If could make a quiet fluid gearbox be pretty cool
```

---
## \#11 Posted by: Pedrodemio Posted at: 2018-05-13T17:33:08.195Z Reads: 62

```
A torque converter only works when you have a speed diferencial between the impeller and the turbine, it wouldn’t convert torque across all the rpm range, the lower the ratio the less multiplication, so when your wheel is stopped and you engage the motor you have maximum multiplication, right as you start to move this drop really fast

And even so the multiplication of most cars is between 1.2 to 1.3, not a lot

For eboard I think the efficiency loss would be to big to make sense, unless we complicate the design and include locking up at higher rpms, most cars do that to improve fuel economy
```

---
## \#12 Posted by: Hummie Posted at: 2018-05-13T18:35:48.367Z Reads: 49

```
ok maybe a torque converter isn't what I was thinking.  isn't there some type of liquid gearing mechanism?
```

---
## \#13 Posted by: Pedrodemio Posted at: 2018-05-13T19:40:12.964Z Reads: 41

```
Yep, basically every hydraulic motor is a fluid gearing, a motor that pressurizes a fluid and that fluid is used to do work, take a look at hydraulic pumps and hydraulic motors
```

---
## \#14 Posted by: Hummie Posted at: 2018-05-13T21:15:31.778Z Reads: 40

```
I'll be searching not that I want to do it, butcan it do a speed to torque conversion like a pulley and 3:1?
```

---
