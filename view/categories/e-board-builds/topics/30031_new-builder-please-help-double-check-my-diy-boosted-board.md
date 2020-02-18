# New builder, please help double check my DIY boosted board

### Replies: 17 Views: 812

## \#1 Posted by: cryo Posted at: 2017-08-08T05:05:31.987Z Reads: 125

```
Haven't yet ordered any parts, I am a first time builder. Would like all of your opinions regarding my build. 

I weigh 140lbs and live in hilly san francisco. I wanted something as close to the boosted board as possible with more range. will these parts work for me?

Parts: 
Loaded Vanguard Flex 1
Orangatang 80mm kegels with bones red bearings
caliber II trucks 10" 50 degrees and some 1/8 risers
2x 5s 8000mAh 30c zippy flightmax (in series)
2x Turnigy Aerodrive SK3 - 5065-236KV Brushless Outrunner Motor
2x 16/36t pulleys
2x hd 265 belts
2x DIY motor mounts
2x VESC
supower 60A 37V BMS
random enclosure
various nuts and bolt
```

---
## \#2 Posted by: torqueboards Posted at: 2017-08-08T05:07:47.502Z Reads: 117

```
Everything looks good but I'd advise against the 5065 SK3 motors as they have 6mm motor shaft. In the past I was able to snap a motor shaft. Since your using our DIY motor mounts as well the 63mm motor mount is much easier to use since you have a better clearance for the motor pulley and your hex key tool for easy adjustment. Using 50mm, you'll have to take off the pulley to secure the "motor" which is inconvenient IMO. Also... forgot the 50mm SK3 don't fit our mounts as they use an even shorter bolt spacing for their motors.
```

---
## \#3 Posted by: cryo Posted at: 2017-08-08T05:14:19.246Z Reads: 104

```
Thanks for looking it over. I did not catch that the diameter of the motors was 6mm so thanks for that. Would this motor fit the mounts https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-213kv-brushless-outrunner-motor.html?
Really trying to find a motor around 230kv as suggested from a thread i saw to complement my 10s battery.
```

---
## \#4 Posted by: torqueboards Posted at: 2017-08-08T05:25:47.306Z Reads: 98

```
If your using VESC, you want to stick to 190KV but SK3 190KV is fine. I think it's 192kv.

But just know, you might not be able to fit dual 6364 on a regular 180mm Caliber Truck. You would need something like our **[218mm Trucks](diy-electric-skateboard-kits-parts/torqueboards-218mm-trucks/)**.
```

---
## \#5 Posted by: Ishayc Posted at: 2017-08-08T06:32:42.231Z Reads: 95

```
I'm using a vesc and 6364 Tacon 160 245kv.
I'm using it with 6s battery and the torque is great even on stiff hills.
You will not be able to mount 2 motors on the rear, you will have to go diagonal, which is a great setup(at least for me) or change your trucks.
```

---
## \#6 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-08T06:35:52.861Z Reads: 94

```
What's your budget?

I'm building a Boosted clone as well and have already ordered all the parts. Mine won't be geared for hill climbing as much as yours, but there's still some things I think you should change. 

Here's some:

1: Why flex 1? I'm using a flex 3, and I weigh about the same as you do.

2: Don't use lipos. If it's within your budget, get someone to make you a custom 10S4P pack out of Samsung 25R or 30Q(?) cells.

3: You can get a cheaper BMS and just bypass it for discharging.

4: Look into buying an enclosure from @Eboosted! In my experience making enclosures for flexing decks is hell. Outsource that which you can not do yourself.

5: Look into buying the whole drive train from diyelectrics(torqueboards). I bought a "Single mechanical kit" from him about a year or two ago and it's been working great. Well worth it.
```

---
## \#7 Posted by: cryo Posted at: 2017-08-08T06:54:29.142Z Reads: 89

```
@UniqueSnowflakeN27 trying to keep it under $850 but im already well over. flex 1 just because I'd rather not have my board bending as much. As for the battery I just dont want to use a battery unless its made by me and I don't have access to a spotwelder, plus its more expensive. @eboosted makes some damn nice enclosures but cant afford it atm. My initial goal was to build a boosted board for less than its retail cost but im fast approaching it lol. its a shame but i might have to do without a loaded deck.

@Ishayc do you think 50mm motors can fit dual rear? I also cant seem to find any 50mm motors with 8mm shafts and less than 230kv.
```

---
## \#8 Posted by: Ishayc Posted at: 2017-08-08T07:01:52.105Z Reads: 86

```
it's not the diameter of the motor, it's the length.
You can use 6355 motors like:
diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/
```

---
## \#9 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-08T07:10:09.000Z Reads: 88

```
[quote="cryo, post:7, topic:30031"]
I just dont want to use a battery unless its made by me
[/quote]

Why not? You're obviously willing to use lipos that I assume you haven't built yourself.
```

---
## \#10 Posted by: cryo Posted at: 2017-08-08T07:16:54.130Z Reads: 82

```
caliber specs hangar width at 185mm. is it really not enough for two 6364 motors? 

how the hell does boosted fit them :sweat:

probably gonna ditch caliber altogether. @torqueboards can u confirm if your v4 motor mounts will fit the 218mm trucks you also sell?
```

---
## \#11 Posted by: cryo Posted at: 2017-08-08T07:23:10.210Z Reads: 79

```
@UniqueSnowflakeN27 i guess assembled is the more correct term? I doubt anyone on this site can make lithium ion or lithium polymer batteries (safe ones anyway.:yum:) But as for wiring them up in series and such I'd rather do it myself  or not at all. I know there are users on here who can do it better and are more knowledgable than me but I still wouldn't trust it unless they were a company(samsung, zippy). Idk im weird like that. Its a moot point anyways since its out of my budget.
```

---
## \#12 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-08T07:34:46.602Z Reads: 77

```
Ok, whatever floats your goat :slight_smile:

Yesterday I saw a thread about an ebay seller selling some *really* cheap genuine 18650 batterypacks, wired with BMS and everything. They were only like 10A cells but if combined to a 12S setup they would be plenty. Might be worth looking in to!
```

---
## \#13 Posted by: Ishayc Posted at: 2017-08-08T07:37:31.128Z Reads: 70

```
check the discharge current before running and buying the pack.
```

---
## \#14 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-08T07:38:38.238Z Reads: 70

```
Definitely! But there was actually a guy in the thread who had been using it for a while without any problems.
```

---
## \#15 Posted by: cryo Posted at: 2017-08-08T07:39:11.142Z Reads: 65

```
will do. what motor(s) did you end up going with if u dont mind me asking? having trouble finding smaller width motors with the correct specs because the one i was originally looking at doesnt fit on caliber trucks with dual setup.
```

---
## \#16 Posted by: torqueboards Posted at: 2017-08-08T07:43:00.591Z Reads: 70

```
@cryo - You can use our Dual 6355 190KV on 180mm Trucks or our dual 6374 190KV on our 218mm trucks. Our motor mounts will fit both.
```

---
## \#17 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-08T07:46:12.260Z Reads: 71

```
[This dual hub motor kit from Torque boards.](diy-electric-skateboard-kits-parts/electric-skateboard-hub-motor-dual/) But I won't be climbing hills really. If you're in San Francisco you're probably better of with a belt drive system geared for torque.
```

---
