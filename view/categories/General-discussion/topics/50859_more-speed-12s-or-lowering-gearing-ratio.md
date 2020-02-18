# More Speed = 12S or lowering gearing ratio?

### Replies: 18 Views: 738

## \#1 Posted by: Acidfie Posted at: 2018-04-01T13:04:31.038Z Reads: 159

```
Well, this is maybe the 10th thread about the same issue but since i read almost every thread and no one really can answer this question i made a new one.

Currently my board rides about 35kph, or should be. I weigh whopping 200 pounds so torque is needed and fulfilled by dualdrive.

The main question right on here is, where do i make a cut when it comes to adding speed.

Going 12S instead of 10S **OR** lowering my gearing ratio? I do not want to increase wheelsize or buy a motor with higher kV - using 190 right now.

Would it be **more efficient** to go gearing ratio under 2.30:1 with losing torque, or adding 2S to the battery to get higher RPM of the motor and maybe bring the full system to its limits while increasing electrical efficiency through R=U/I?

I hope we can find a solution here since some people want to know what they should do.
```

---
## \#2 Posted by: BoostedBuilder Posted at: 2018-04-01T13:09:18.714Z Reads: 155

```
If you are using a quality VESC, then higher Voltage! It will increase your speed, torque and overall efficiency.

BUT ONLY IF YOU HAVE A QUALITY VESC
```

---
## \#3 Posted by: Acidfie Posted at: 2018-04-01T13:10:03.745Z Reads: 151

```
i do, using the esk8 1.1 (V)ESC and Attila said already 12S won't be a problem.
```

---
## \#4 Posted by: BoostedBuilder Posted at: 2018-04-01T13:12:49.817Z Reads: 152

```
Its not as much the higher voltage but the higher erpm. You should be fine. Go for it!

Are you running FOC?
```

---
## \#5 Posted by: Acidfie Posted at: 2018-04-01T13:14:43.136Z Reads: 152

```
nope, running BLDC mode. FOC and 12S is dangerous for the VESC imho. With limiting the ERPM in the VESC to 60'000. I think its practically impossible to get 60'000 while riding.

How about using motors that are made for 10S, is overvolting motors a big problem? as i just heard about generating heat and bearing failures. my motors are both handwarm after a ride with some hills?
```

---
## \#6 Posted by: BoostedBuilder Posted at: 2018-04-01T13:25:54.840Z Reads: 145

```
Well @Deckoz is running 13s and FOC on all of his builds if I'm not mistaken. So far so good.

On a Maytech or DIY VESC it would most likely damage the DRV but with the ESC 1.1 I think you wouldn't have a problem. I'm running FOCBOX's so not sure, but I don't see any problems.

For the motor, it can't really be made specifically for a certain voltage. A higher voltage should only reduce the heating.
```

---
## \#7 Posted by: Acidfie Posted at: 2018-04-01T13:36:06.986Z Reads: 136

```
well, i will give it a try with 12S, seems more pleasant to me.

i estimated the range with the "how far can i ride calc" - does this sound like the reality?

12S4P = approx. 28km
10S5P = approx. 30km
```

---
## \#8 Posted by: Deckoz Posted at: 2018-04-01T13:40:36.426Z Reads: 132

```
I would say move voltage will get you the gain in speed, as decreasing the ratio will likely only increase your amp draw with no real gains in speed. At least comparatively to 8.4 more volts at full charge...
```

---
## \#9 Posted by: Acidfie Posted at: 2018-04-01T13:56:44.763Z Reads: 128

```
this seems like the best option in this case. i wonder how much the amp draw increases if i lower the ratio.
```

---
## \#10 Posted by: professor_shartsis Posted at: 2018-04-01T20:18:32.022Z Reads: 110

```
increasing the voltage but not raising the amp limit increases the available mechanical power without increasing the motor heating as long as it has enough gear reduction... because the motor can spin with ~20% greater rpm with the same torque... which means ~20% increase in peak mechanical power.

if you increase the motor amp and battery amp limits by ~20% without raising the pack voltage, this also gives you ~20% more mechancal power until the motor is close to no load rpm, (because torque increases by ~20%) but motor heating increases by more than ~20% to achieve this, which means lower efficiency.
```

---
## \#11 Posted by: Acidfie Posted at: 2018-04-01T20:25:31.750Z Reads: 101

```
i will increase the amp limit as well the voltage. so it seems like a good option to get the higher voltage just because of adding some rpm than adding a lower gearing ratio.

so the torque would stay the same if i do not change the ratio but when it comes to higher speeds the motor has the ability to turn fast, means to increase the maximum speed
```

---
## \#12 Posted by: professor_shartsis Posted at: 2018-04-01T20:27:55.134Z Reads: 89

```
increasing the motor amp and battery amp limits increases available torque at the same rpm, but increases heating by a greater amount than it increases torque, which decreases efficiency.

increasing the pack voltage increases peak rpm which increases peak mechanical power without increasing torque, motor amps, or motor heating, but the gearing must be appropriate in order to ensure access to that extra available mechanical power.
```

---
## \#13 Posted by: Acidfie Posted at: 2018-04-01T20:36:39.260Z Reads: 87

```
[quote="professor_shartsis, post:12, topic:50859"]
increasing the pack voltage increases peak rpm which increases peak mechanical power without increasing torque, motor amps, or motor heating, but the gearing must be appropriate in order to ensure access to that extra available mechanical power.
[/quote]

peak rpm is what i want to increase because of the speed, right. i do not need more torque since its enough for me. but with the new battery i even can increase the bat max delivering more power. i think the 36/15 would be a good ratio for this scenario.
```

---
## \#14 Posted by: professor_shartsis Posted at: 2018-04-01T20:39:18.853Z Reads: 83

```
if the motor can spin 20% faster because of a 20% increase in pack voltage, but the motor amp and torque limit is too low to reach the ground speed where the motor is actually spinning 20% faster because of wind resistance, then the extra 20% mechanical power would be inaccessible which would require an increase in gear reduction to access the extra power, or an increase in amp limits to give you enough torque to reach the 20% faster motor rpm (by overcoming the wind drag force).
```

---
## \#15 Posted by: Acidfie Posted at: 2018-04-01T20:43:33.021Z Reads: 84

```
now i get what you mean. so, the question now is, what is more efficient to increase maximum speed. i think going 12S is the way to go, what would you choose?
```

---
## \#16 Posted by: professor_shartsis Posted at: 2018-04-01T21:22:03.626Z Reads: 80

```
if you were to increase the pack voltage by 20%, reduce the # of teeth on the motor pulley by 20%, and keep the motor and battery amp limits the same, you’ll have 20% more torque at the wheel available at all speeds and roughly the same (or slightly increased) top speed, same motor heating, and greater efficiency at the same constant speed (the greater efficiency at same constant speed a result of 20% lower motor amps & motor torque required for the same wheel torque because of the 20% gear reduction increase.)
```

---
## \#17 Posted by: Acidfie Posted at: 2018-04-02T01:00:24.292Z Reads: 62

```
But I need higher top speed which means I need to let the gearing ratio like it is right now.
```

---
## \#18 Posted by: professor_shartsis Posted at: 2018-04-02T02:28:10.930Z Reads: 59

```
in summary...

only changing the gear ratio (same motor amp limit) won’t increase the maximum mechanical power of the motor, but it may make the max mechanical power of the motor more accessible if the current gear reduction happens to be too low to reach a high % of no load rpm factoring the wind drag force.

only increasing the pack voltage will increase the maximum mechanical power of the motor, and assuming the gear reduction isn’t too low this can also increase the efficiency because you can get extra mechanical power without extra motor heating with the same motor amp and torque limit because the motor can turn faster, and more rpm with the same torque and heat means more mechanical power and efficiency.

only increasing the motor amp limit will also increase the maximum mechanical power (by directly increasing the torque- not the max rpm), and combined with lowering the gearing reduction this can also increase the top speed, but every doubling of motor amps and torque leads to a quadrupling of the motor heating rate, so raising the motor amp limit to improve performance rapidly lowers efficiency and increases motor and esc heating.
```

---
