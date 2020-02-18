# Building battery pack

### Replies: 16 Views: 1028

## \#1 Posted by: pengy Posted at: 2017-09-28T16:27:51.758Z Reads: 205

```
Hey everyone,

I'm about to build a 6s battery pack (for now)..
Out of 18650 3300mah batteries.

The packs will be connected also with balance wires, so I will charge it with a balance charger.

I have 12 18650 batteries and my plan is to connect every two batteries together in parallel to form 1s out of 2 batteries.
And then each set of two to another set of 2 in series.
So I will have 6s Battery pack eventually with 6600mah.

The question is, if this is indeed the recommended way to do this for the cells to be properly balanced, or there is a better way.

Thanks.
```

---
## \#2 Posted by: UniqueSnowflakeN27 Posted at: 2017-09-28T16:32:30.452Z Reads: 195

```
What cells exactly? Can they output 20A+?

6S2P won't be very good. I ran a 6S4P for a summer but even with the 4P the voltage sag was too much at times. That's not even mentioning the poor range you'll get out a 2P.

Are you asking if BMS is the way to go? Yes, most people agree that's the best. Some people don't. Do some more research if you're not sure.
```

---
## \#3 Posted by: MysticalDork Posted at: 2017-09-28T16:40:54.154Z Reads: 181

```
That's the correct way to do it, but like @UniqueSnowflakeN27 said, 6s2p of 18650s will be pretty weak and not great range, even if they're 20amp cells, which they probably aren't (I've never found 3.3ah 20a cells, they're all lower than that.)
```

---
## \#4 Posted by: pengy Posted at: 2017-09-28T16:41:12.004Z Reads: 174

```
This is the kind: LG HG2 3000mAh 18650 30A High Drain INR Battery
I know it may be not idle and the range probably won't be amazing nor performance, I am planning to get some more batteries of the same kind to form a 9s and maybe add another parallel, will have to see what is the range I get out of it.
But for now for completing the initial build I was thinking I'll do with 6s2p.
```

---
## \#5 Posted by: pengy Posted at: 2017-09-28T16:44:18.638Z Reads: 156

```
As for the charging I have a BMS as well, but heard some bad reviews about it.. And I needed a high amp power supply anyway so decided of buying the Imax b6 hobby charger.

I'm just trying to prevent unbalanced batteries in the future so didn't know if the connection I'm planning is going to be optimal for that.
```

---
## \#6 Posted by: MysticalDork Posted at: 2017-09-28T16:47:46.282Z Reads: 145

```
It will work, as long as you hook up the balance leads to the balance charger. If you're planning to go up to a 9s pack in the future, make sure to pick a motor with a kv low enough to work at 9s without exceeding 60k erpm.
```

---
## \#7 Posted by: pengy Posted at: 2017-09-28T16:58:43.371Z Reads: 142

```
Great,
I guess I will try a few variations, I think a very high top speed is not important to me, I will probably prefer a good at least 10 mile range which now probably I'll get less. I don't know what to expect with my setup yet. The motor I have is a Turnigy 6374 149KV, I don't remember the wattage but remember it was more than enough to handle also 12S. It will be connected to a 1 to 3.4 gear ratio if I'm not mistaking, so I'm expecting to get at least get a good enough torque for cruising.

But yeah I wish I'd know what to expect in terms of range and speed.
```

---
## \#8 Posted by: MysticalDork Posted at: 2017-09-28T17:05:10.877Z Reads: 130

```
What size wheels are you planning on using? With that we can figure out your speed.
```

---
## \#9 Posted by: pengy Posted at: 2017-09-28T17:05:41.011Z Reads: 129

```
That would be great :slight_smile:
82mm
```

---
## \#10 Posted by: MysticalDork Posted at: 2017-09-28T17:14:43.427Z Reads: 122

```
With those numbers you can expect about 8mph and 7 miles of range. The 1:3.4 gear ratio is a little low for 6s, you can increase the speed significantly by going with a different gearing.
```

---
## \#11 Posted by: MysticalDork Posted at: 2017-09-28T17:20:46.706Z Reads: 116

```
This is all according to calc.esk8.today go there, and you can plug in your numbers and tweak things until you find a combo you like.
```

---
## \#12 Posted by: UniqueSnowflakeN27 Posted at: 2017-09-28T17:21:22.028Z Reads: 110

```
Personally I would never "upgrade" a battery like you're suggesting. The cells should be married - meaning they should have the same brand, same model, same voltage and used for exactly 0 cycles before.

If you ride for a year now with the battery and then upgrade it to 9S the cells will differ in quality. Making it an unstable battery.
```

---
## \#13 Posted by: pengy Posted at: 2017-09-28T17:39:24.464Z Reads: 108

```
That's a good point actually, but I think there should be something like a month max between the new batteries and older ones as I want to see it working first, plan my upgrade and then wait for the new batteries to arrive.
And during this time not to use it much.
```

---
## \#14 Posted by: MysticalDork Posted at: 2017-09-28T17:40:23.122Z Reads: 104

```
If it's that short of a wait, I'd just wait and build the damn thing once.
```

---
## \#15 Posted by: pengy Posted at: 2017-09-28T17:45:13.441Z Reads: 109

```
Well I became a little paranoid with this project as my VESC was short circuited and had so much delays with parts.. I just want to get it assembles at least :). I am taking into consideration only to test run it once and wait for the new batteries to arrive to complete the build. Also I'll have a good idea as of what I'm looking for more, speed or range. Or both..
```

---
## \#16 Posted by: pengy Posted at: 2017-09-29T18:51:57.885Z Reads: 99

```
Took your advice and will make the board 8S2P. According to the calculations on these sites:

http://esk8.today/2016/12/28/how-far-can-i-ride/

http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":8,"motor-kv":149,"system-efficiency":85,"motor-pulley-teeth":16,"wheel-pulley-teeth":48,"wheel-size":83}|

My speed should be:
14.29 mph - 23 km/h
Which is OK I think..
And with distance of 10.66 Miles or 17.15KM 

Thanks for the advises.
```

---
