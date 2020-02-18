# Secondary battery pack

### Replies: 16 Views: 651

## \#1 Posted by: ThorNilsson Posted at: 2018-08-11T00:45:16.296Z Reads: 94

```
Hello guys, I have this idea of a extended battery on the deck hold by Velcro straps (for easy release and mounting when needed) with a plug throught the boards deck to the main power cables.

My plan is that when I have used the main battery I will be able to plug a second battery in to the deck into a standard female battery plug and continue riding. I will probably solder a female conector right to the ordinary power cables. 

My question is what problems will i be facing and do you have any thoughts on improvements or other solutions. Will I for example need a swich for turning the main battery of??

Simple sketch of my idea 
![Snapchat-168696574|690x388](upload://ffw5PpO3TR3pSKF2SL0qEhB2iYT.jpg)
```

---
## \#2 Posted by: Wraith Posted at: 2018-08-11T01:53:47.813Z Reads: 72

```
@TinnieSinker is actually working on this as well! The only thing I can think of is how well it can charge while riding compared to the main battery pack as its going to be smaller
```

---
## \#3 Posted by: strattos Posted at: 2018-08-11T02:07:52.983Z Reads: 67

```
You would need a way to limit your charge current or you would blow/melt something if you just plugged a battery straight in without any charging circuitry.

If I wanted to make a design like this I'd put a loopkey in between the battery and the (charge/spare battery port using an xt90) then use the spare battery as an extended range battery that's external.

And if ya really wanted to you could put a little charge controller in your enclosure to trickle charge your main battery. But this is pointless Imo and is just wasting electricity.
```

---
## \#4 Posted by: ThorNilsson Posted at: 2018-08-11T09:36:43.641Z Reads: 55

```
If I put one on/of switch for the main battery and then plug in the external battery so that only one battery is active at once will that work?
If so do i need one or two switches? 
I mean there are two cables from the main battery so to be 100% sure to not blow anything do I need one for each cable?? 

The position of switches marked with blue
![bild|690x388](upload://4sWZFf5s0uTUvZgFnzsD22nHo9k.jpg)
and i have some sort of battery management board that might be possible to use (I did not make this build)
![P_20180811_101204|375x500](upload://A2fRj2oqJ89AVZjBOXWnk6UvH3m.jpg)
```

---
## \#5 Posted by: Andy87 Posted at: 2018-08-11T09:46:47.809Z Reads: 47

```
If you connect your extanded batter directly to your vesc than use a anti spark xt90. Should work in my opinion. But there is a problem that your extanded battery maybe smaller and with it can’t handle the same current. Means you would need to adjust your vesc settings
```

---
## \#6 Posted by: Newby Posted at: 2018-08-11T09:47:17.928Z Reads: 46

```
No chance mainly because the battery is dictated by it's weakest parralel pack. If you watch this video (https://youtu.be/S919PAzyGxY) you can see that the battery get's half its rated capacity because it can't unleash the last half of the Tesla cells once the voltage fell below it's threshold on one pack. If you disconnect the other battery with a loop key this would work however
```

---
## \#7 Posted by: ThorNilsson Posted at: 2018-08-11T09:48:16.821Z Reads: 43

```
ok, now i understand, is it possible to make different profiles for different power supplies in the BLDC tool??
```

---
## \#8 Posted by: Andy87 Posted at: 2018-08-11T09:50:19.983Z Reads: 40

```
You run single?
Get a Bluetooth module and app like ackmanic.
You can set up different profile or as min change your settings without to connect your laptop.
Easy thing, just don’t forget to make it😉the same with switch off your main battery before plug in your new one
```

---
## \#9 Posted by: ThorNilsson Posted at: 2018-08-11T09:51:42.326Z Reads: 40

```
so this loop key thing, how does it work and is it easy to add to this build?
```

---
## \#10 Posted by: ThorNilsson Posted at: 2018-08-11T09:53:11.259Z Reads: 40

```
and yes single belt motor with a turnigy sk3 6364 motor
```

---
## \#11 Posted by: Andy87 Posted at: 2018-08-11T09:53:43.584Z Reads: 36

```
Definitely just get a Bluetooth. No problem than
```

---
## \#12 Posted by: Winfly Posted at: 2018-08-11T09:55:18.111Z Reads: 36

```
i think the easiest way is to have 2 anti-spark loopkey connectors and only 1 key. so you are guaranteed to disconnect the main battery before switching over to secondary. and +1 to BT module

edit: 
https://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204
```

---
## \#13 Posted by: ThorNilsson Posted at: 2018-08-11T09:59:23.686Z Reads: 33

```
do i even need to get a second on of swich? the regular on of switch is going from the circuitbord on top of the batteries.
```

---
## \#14 Posted by: Andy87 Posted at: 2018-08-11T10:02:17.487Z Reads: 32

```
How @Winfly said the most safe thing would be skip your switch and use just loop key.
If main battery empty plug it out and plug in our extension pack. Use a anti spark key for it and you good to go
```

---
## \#15 Posted by: ThorNilsson Posted at: 2018-08-11T10:05:31.546Z Reads: 32

```
Thanks, will go with the loop key
```

---
## \#16 Posted by: Winfly Posted at: 2018-08-11T10:06:13.629Z Reads: 33

```
you can keep the on/off switch so that you dont need to unplug the main battery loop for regular use. Just make the loopkeys at the + of each battery pack. This way you will only need to touch the loopkey when you swap battery.
![Untitled|690x388](upload://sjMgwy5sfu3aqq5ww7nYgub5B5w.png)
```

---
