# Please remind me about braking going downhill with the vesc

### Replies: 22 Views: 1993

## \#1 Posted by: Hummie Posted at: 2016-10-13T17:49:41.046Z Reads: 218

```
as long as I dont go over my max voltage cut-off by riding downhill and braking with a full charge I'm good right?   Maybe I should up this limit a bit. 

  as long as I stay under the max erpm of the esc which would be my kv times voltage x 7 I'll have brakes right? 
 Otherwise no brakes in the first situation or esc death in the second?

definitely thinking I feel safer with a kv that's on the higher side for this reason.  Couldn't be worse than losing brakes going down a hill at full speed.
```

---
## \#2 Posted by: chinzw Posted at: 2016-10-13T18:04:13.588Z Reads: 210

```
Just keep your batteries undercharged to about 4.1 and you should be fine.
```

---
## \#3 Posted by: Hummie Posted at: 2016-10-13T18:06:35.450Z Reads: 205

```
but if I go faster than the no-load speed?  or is it just the erpm limit I need to worry about?

i need to be reminded of the exact details...I'm always remembering I dont know this when going downhill fast.
```

---
## \#4 Posted by: SORRENTINO Posted at: 2016-10-13T18:19:18.019Z Reads: 197

```
Just don't go faster then your max speed you can reach on your board lol
```

---
## \#5 Posted by: Hummie Posted at: 2016-10-13T18:23:34.656Z Reads: 188

```
but I want to!  
as it is now I'm only using 9 cells and a max speed of 24mph when powered.  

what are the solid facts?
```

---
## \#6 Posted by: chinzw Posted at: 2016-10-13T18:32:13.374Z Reads: 183

```
Im guessing you need to stay below the max ERPM (i think its 100.000)
```

---
## \#7 Posted by: Jinra Posted at: 2016-10-13T18:41:38.532Z Reads: 180

```
try it and find out :)
```

---
## \#8 Posted by: Hummie Posted at: 2016-10-13T18:52:12.499Z Reads: 169

```
@jinra lets meet up again and you can try it for me.   come over and see my battery
```

---
## \#9 Posted by: Jinra Posted at: 2016-10-13T18:55:16.200Z Reads: 169

```
Sure, once I finish my second build
```

---
## \#10 Posted by: stealth71 Posted at: 2016-10-13T18:59:00.257Z Reads: 162

```
eRPM changes with voltage?  I just peg the throttle and hold on.

Downhill longboarders go downhill with no brakes regularly.
```

---
## \#11 Posted by: Jinra Posted at: 2016-10-13T19:01:11.213Z Reads: 159

```
[quote="stealth71, post:10, topic:11068"]
eRPM changes with voltage?
[/quote]

Yep, higher voltage higher speed.
```

---
## \#12 Posted by: stealth71 Posted at: 2016-10-13T19:03:11.227Z Reads: 158

```
Sorry I should have said.  Does max eRPM change with voltage?
```

---
## \#13 Posted by: Jinra Posted at: 2016-10-13T19:06:16.483Z Reads: 153

```
Max erpm of what? the motor, the controller? The motor has no max so it'll increase linearly with additional voltage.
```

---
## \#14 Posted by: Hummie Posted at: 2016-10-13T19:10:40.053Z Reads: 151

```
 I go down steep busy hills with stop signs at the bottom. san francisco city.   without brakes I'd be dead quickly

higher voltage allows you to increase your rpm and also the erpm.  

but I still havent heard an answer.  Looking for the speed limits for the vesc.  I know it will cut the brakes off after the high voltage cut out,  so going faster than the no-load speed based on the kv and voltage, but I forget anything else.
```

---
## \#15 Posted by: Jinra Posted at: 2016-10-13T19:15:59.093Z Reads: 144

```
For me, I run 200kv. Overvoltage cutoff is 57v. I'd have to be going 80,000 erpm in order to hit that cutoff. That's 50 miles an hour!
```

---
## \#16 Posted by: Hummie Posted at: 2016-10-13T19:27:35.062Z Reads: 145

```
direct drive
90kv x 50 volts (full charge) is maybe 4500 rpm.  x7 equals 31,500.   so I'm good on keeping under the erpm but what about voltage spikes?  If i get above my no-load speed going downhill and then brake I'll have an even greater voltage spike than the 57v cut-off maybe?
I'm confused by the voltage spike.  I thought the voltage sent from the motor was determined by the speed of the motor yet you can have a high voltage spike braking when youre going slowly
```

---
## \#17 Posted by: Jinra Posted at: 2016-10-13T19:29:42.804Z Reads: 136

```
I believe voltage spikes only occur in the battery (don't quote me on this). Keep in mind your hub motors should have higher erpm due to additional pole pairs.
```

---
## \#18 Posted by: Hummie Posted at: 2016-10-13T19:30:47.652Z Reads: 136

```
its still 14 magnet and 12 teeth.  feel good with the erpm but the voltage spike at even slow speeds is higher than I'd thought
```

---
## \#19 Posted by: Jinra Posted at: 2016-10-13T19:36:39.359Z Reads: 132

```
The spike is actually beneficial in order to regen your batteries as anything lower than the current working voltage of your batteries would be lost as heat instead of regening.

If you're working with 40 volts, you need to have a BEMF of 40+ volts in order to regen or the energy will be lost as heat.
```

---
## \#20 Posted by: Hummie Posted at: 2016-10-13T19:39:28.885Z Reads: 129

```
ok. so it has to be higher than the battery, which makes sense, but how does it get higher as I thought the voltage was tied to the speed, just as it is when the motor is being used as a motor and not a generator?

that's the last question
thanks
```

---
## \#21 Posted by: Jinra Posted at: 2016-10-13T19:41:32.367Z Reads: 120

```
I'm unsure as to that. We know voltage spikes when braking, I'm just not sure why it spikes. I'm thinking the spike is the reason we're able to regen given the higher voltage compared to the battery.

Another instance of reaching a higher voltage than the battery is when going fast downhill or when your battery is at a lower voltage, or both.
```

---
## \#22 Posted by: TarzanHBK Posted at: 2016-10-14T08:54:21.156Z Reads: 94

```
also keep in mind that the vesc could lose the motor for a few milliseconds if you go over 60.000erpm and probably will lose it going over 100.000erpm. The result is a stuttering motor which can throw you off the board, depending on how much the motor stutters (Not to mention a DRV Error). If you limit the motor to 60.000 you shouldn´t be able to exceed that with throttle, but i´m not sure what happends if you exceed that going downhill without throttle...
for safety reasons i would do the math on how fast i can go to not exceed 60.000 and stay under that speed :monkey:
```

---
