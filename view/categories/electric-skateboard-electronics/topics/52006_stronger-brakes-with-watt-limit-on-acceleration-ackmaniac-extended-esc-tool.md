# Stronger Brakes with Watt Limit on Acceleration? (Ackmaniac Extended ESC-Tool)

### Replies: 9 Views: 990

## \#1 Posted by: skatardude10 Posted at: 2018-04-12T04:39:05.686Z Reads: 168

```
Hey guys! 

Tonight i've been tooling around with [my new build](http://www.electric-skateboard.builders/t/lbl-build-longboard-larry-stingray-tb-218-tb-6374s-190kv-tb-mounts-chibattery-10s4p-dual-focboxes-done-omg/50610/25), and I have some questions... please bear with me... 3 main issues (1 - watt limit limiting brakes 2 - no brakes past speed limit 3 - battery regen limit not hit until last moment).

Here are the configurations I have - *thus far*...
![Screenshot_20180411-220319|281x500](upload://i8Oz3ilbe4Dd9WQWOxIswBSH6x.png)

1. Stronger brakes: How do I get stronger brake force when setting a wattage limit? The wattage limit seems to apply to both acceleration and brake force... and since I have my setup geared for speed, even 20 watts gets you going pretty quick! But then it's difficult to slow down- not exactly beginner friendly. Fine for me, I can foot brake or slide, but I want my friends to be safe too...
* I've tried turning off my wattage limit, and only limiting battery and motor amps, and that just feels crazy, almost too powerful and unpredictable, even down to 1 amp max battery and 20 motor amps... huh.

2. Setting a max speed seems to have some effect... but unfortunately it seems to disable 95% of the brake power if you happen to go faster than the speed limit set in the app.
* For example, I set 10mph... feels somewhat fast in a tight neighborhood... but the moment I coast a bit faster downhill, the brake force stops and comes back on once I am going less than around 10mph... so I just leave this pretty high (around 30mph) and don't have the issue of the brakes cutting out past the speed limit. 
* I'd rather if it would brake to keep the board at the speed limit.

3. I notice that when I set a lower wattage limit, not only does it seem to limit the brakes, but it also limits the battery regen, way below the setting I have it set to... **until** the last moment... right before stop the brakes lock up much harder and the regen amps jump to the regen setting (jump to -8A from -0.5A to -1A) before the board comes to a halt. i'd love it if not only the board would brake harder when setting very low wattage limits, but also regen to the limit i've set. 

Is there an ERPM or some other settings I need to change to fix these things? I guess I could also add this, but it might go without saying: On the faster modes not limited by wattage, braking is great... everything is great. @Ackmaniac I figure you are the guy to tag...

Thanks!
```

---
## \#2 Posted by: Eboosted Posted at: 2018-04-12T04:47:08.415Z Reads: 147

```
When you select beginner mode and pull the throttle a the way in, both wheels spin at the given limited speed or only one?
```

---
## \#3 Posted by: skatardude10 Posted at: 2018-04-12T04:50:20.175Z Reads: 146

```
Both spin at the same speed (slow on beginner / very fast on performance / etc).

I did have to figure this out earlier though, remembering that my BT module was connected to master and to check to connect by can to ID1 (slave).
```

---
## \#4 Posted by: Eboosted Posted at: 2018-04-12T04:57:37.775Z Reads: 150

```
I wouldn't limit the power of the board on each mode, I'd deselect the limit max Watt checkbox and limit the acceleration by adjusting the motor max and battery Mac current, I'd also limit max speed on each mode as needed. 

For all modes I'll leave brakes at -65A motor min and -12A battery min, considering you have a 10S4P battery pack of 25R or 30Qs

Test it and keep us posted
```

---
## \#5 Posted by: skatardude10 Posted at: 2018-04-12T05:20:47.765Z Reads: 138

```
Okay, I just tried your suggestion.

First of all, -12 and -65 works to brake *muuuuch* better, thank you! This setting is nearly perfect. 

But the problem still seems to persist for (attempted) slow modes. 

1. Tried limiting Motor and Battery Current to 15 and 12 respectively, to match -12 battery regen, with -65 min motor... but min motor only ever went to -15... not any stronger than the opposite of my max motor unfortunately. This was with watt limit disabled and no speed limit.
* Batt regen stats were better... as they weren't limited by watts now, but still no stronger than the inverse of motor max.
* watt limits do the same thing it seems, limiting the max brake power to the watt limit instead of the max amp limits set.

2. Tried 65 motor max and 40 batt max, -65 motor min and -12 batt regen *but with a speed limit* of say 8mph. It would end up going much faster than 8mph due to the acceleration, but not brake at all, no regen, no nothing once I got past 8mph... so I can't limit it via speed limit for now.

Anyways... slow modes aren't working out, but the faster modes are great. I just need to remember to set all my speed limits to the max, otherwise I am going to be going *faaast* with no brakes past the speed limit.

*If only* I could set my throttle curve values in ESC tool like you can in BLDC tool, making the max throttle say 70% at 100% throw... things would be real easy right now setting throttle curves for each mode with the same settings across the board pretty much. Is there a way to do this in ESC tool? All I see is the ability to change the brake and accel curves, limited to 0 at one and and 100 at the other, and 50 in the middle regardless of the curve values. I could change my puleslength values, but then it would persist across all my modes unlike throttle curves defined in the app.

Side note: The heatsinks seem to be working. Temps rarely go above 45 and almost never above 50. I figured all those 120+ amps and such high speed gearing would heat these things up. Can't wait to push this thing up some hills and see how hot it gets.
```

---
## \#6 Posted by: skatardude10 Posted at: 2018-04-13T07:11:07.459Z Reads: 107

```
is -12 batt min safe on each of two VESCs for 25r in 4P configuration? My math has me worried: 4A max fast charge per cell x 4P = 16 / 2 VESCs = -8 each. 

I do a lot of braking, and because of my gearing I don't have a TON of torque to work with, so braking down from 35-40mph tends to take a while. 

Because of this, today I saw many long periods of -24 amps going back to the battery. Is this really safe? Charging 10S4P at 24 amps for 10+ seconds at a time, many times in relatively quick succession ?

I changed it back to -8 until I get confirmation that this is either safe, or dumb.
```

---
## \#7 Posted by: Eboosted Posted at: 2018-04-13T22:04:08.641Z Reads: 91

```
Even -16A (-8A each VESC) is safe for short periods of time.
```

---
## \#8 Posted by: Ackmaniac Posted at: 2018-04-20T20:34:11.960Z Reads: 83

```
I am glad you reported your problem very detailed. Because that made me have another look at the code and i found a issue. The problem was that above the max speed limit the slave motor brakes were disabled. I fixed it in the Ackmaniac-Tool Version 3.101. 
Thx again for the details which let me find the bug.

Here you can find more information.
http://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116/294?u=ackmaniac
```

---
## \#9 Posted by: skatardude10 Posted at: 2018-04-21T05:52:54.564Z Reads: 69

```
Yay! Thanks for the work man, this is great :sunglasses: :smiley:
```

---
