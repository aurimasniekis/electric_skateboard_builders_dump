# Electric Motorbike &#124; Range Estimate conflict: VESC vs cal.esk8.today

### Replies: 20 Views: 377

## \#1 Posted by: AjaniBilby Posted at: 2019-08-25T03:44:05.746Z Reads: 126

```
*Pre-cursor: I live in Australia, it gets hot - I want to be able to use this in 40c days if necessary. Thus I'm using a water-cooled motor and ESC. Also, right now this project is all theoretical, and I'm checking the feasibility of the project from a cost, point of view, and whether the result is worth it for me.*

So I've already done a bunch of engineering analysis to work out how much power I need, what gear ratios to allow me to get to highway speeds comfortably (highway speed 100km/h, so the vehicle should be able to do 150km/h, thus I'm not pushing the vehicle to its limits for extended highway use). However trying to calculate the rough range of the vehicle is beyond me, because I'm not sure exactly how many watts the motor will be pulling to maintain 100km/h.
(I know to take everything with a lot of salt because it's almost impossible to know exactly how much wind resistance, final drive, gearing and other inefficiencies will be).

So I turned on online calculators. I was VESC had an online calculator which didn't have anything near the motor I was planning on using, so I modded the webpage to take it. Also, the page only allowed up to 10 cells in parallel, and I was going to have at least 13 so I just multiplied the range by 10/13. (Note 12S13P for the initial build, I will add more packs in parallel as time goes on). VESC gave me a range of 9.9km when riding at ~100km/h.

I then also used the way back machine to use calc.esk8.today which has been referenced elsewhere on the forum. Input the respective numbers and it told me 175km range... Which is just a bit more than a small difference... Hence my confusion.

Can someone give me a better way to get an approximate estimation? Because the fact that there are massive discrepancies proves that something is going seriously wrong in one or both of these calculators.

**Data**  
Gear ratio: 1:6 (motor:wheel)  
Final drive: chain (allows for cheap and easy gear ratio adjustments later)  
Battery: 3.7V 3.4A - 12S 13P  
Motor: [8kW 200kV - 18Nm, 158A](https://flipsky.net/collections/e-skateboard/products/brushless-water-cooling-motor-83100-14s-8000w-for-efoil-ejet-boards-ebike)  
ESC: [FSESC 200A 60V (based on VESC6)](https://flipsky.net/collections/new-accessories/products/high-current-fsesc-200a-60v-base-on-vesc6)  
Weight: 180kg (rounded up a lot, frame, batteries, wheels, rider, motor, all inc.)
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-08-25T04:23:13.458Z Reads: 115

```
@AjaniBilby try this calculator: https://www.ebikes.ca/tools/simulator.html it's built to handle ebikes, with more powerful motors/batteries/controllers than the esk8 calculators do. It's what I use for idiot-checking while I'm building my 20s7p, 7KW ebike.

One thing of note: you're gonna need a lot more power than you think you will to achieve 150km/h - aerodynamic drag increases with a factor of the speed cubed - twice as fast means 8x the power needed.  

I just ran some quick and dirty simulations based on your numbers above, and, well, you're going to need something on the order of 12-20+KW to maintain a speed of 150KPH, depending on the drag of your body position and vehicle. That motor/esc combo won't handle that. Based on some rough guesses (assuming similar drag to a mountainbike rider tucked) with the throttle pinned you'd just barely be able to hit 100kph.
```

---
## \#3 Posted by: MysticalDork Posted at: 2019-08-25T04:27:16.358Z Reads: 106

```
Also, due to the extreme power requirements, 12s is not very suitable - your main battery leads would end up needing to carry 3-400 amps. Much better to use a higher-voltage motor/controller/battery combo to bring those current numbers down out of the clouds. By the way: with those calculations in mind, your cruising (100KPH) range with that battery capacity (1.9KWh) will be somewhere around 22Km. 

These numbers are obviously to be taken with a large pinch of salt, and the efficiency numbers (range and drag) are probably optimistic unless you spend a lot of effort on aerodynamic design. That 9.9km range estimate from earlier doesn't sound that far off. The 175km range assumes a nice, slow, efficent skateboard with low rolling resistance urethane wheels, using ~12Wh/Km. You'd be using more like ~90Wh/Km.

If you slow down, your range will rapidly increase: My ebike has a theoretical top speed of 40-45MPH and at that speed I figure I'll get 20 miles out of it (1.5Kwh battery) but if I drop that down to 25MPH, the range goes up to 60+ miles.
```

---
## \#4 Posted by: Jacobee Posted at: 2019-08-25T04:30:27.623Z Reads: 100

```
I used this calculator which @MoeStooge posted about forever ago (also sorry about the FUB)
http://www.wallaceracing.com/Calculate%20HP%20For%20Speed.php
If you have a 4 ft frontal area and weigh 396.832 lbs (180 kgs) and we assume .9 for a coefficient I f drag (which is medium for a motorcycle according to the website) then you need 7.46 hp which is 5562.921 watts, take your watt hours (1,962.48) and divide it by the watts you get .35277 percent high is the fraction of an hour your battery will last at that speed which translates to 21.16 minutes, at 100 km/h that’s 1.6 km every minute so 33.8 miles. This all assumes the whole time you’re going 100km/h and not taking into account the power used to accelerate to that speed so probably somewhere around 30 miles (more if you aren’t going super fast the whole time)

Edit: also that esc would probably be too small and not powerful enough to handle 5k watts continuous. Maybe it would handle the heat if it was air cooled and completely exposed but I wouldn’t count on it.
```

---
## \#5 Posted by: AjaniBilby Posted at: 2019-08-25T05:09:59.254Z Reads: 85

```
Originally I was going to use [this motor](https://flipsky.net/collections/e-skateboard/products/water-cooling-motor-9097-150kv-for-efoil-electric-bike-electric-skateboard), but then due to some legal reasons with kW/kg power limits I stepped down to the 8kW one because it was the smallest step down I could find that was water cooled.

However, I have since increased the total weight of the bike to be just enough to squeeze an 18kW motor in.
```

---
## \#6 Posted by: AjaniBilby Posted at: 2019-08-25T05:10:47.730Z Reads: 84

```
I forgot to mention a rear wheel diameter of 70cm
```

---
## \#7 Posted by: AjaniBilby Posted at: 2019-08-25T05:16:22.857Z Reads: 87

```
I really want to try out having a water cooling system in my bike, which makes finding an ESC that is also water-cooled hard.

Do you have any recommendations for an ESC (preferably VESC because their software looks nice), what would be able to handle a [motor](https://flipsky.net/collections/e-skateboard/products/water-cooling-motor-9097-150kv-for-efoil-electric-bike-electric-skateboard) of this power?

Side note: I'm tempted to also try the water loop through the battery back as well, obviously I'd have it at the beginning of the loop so I'm not dumping any hot energy from the motor or ESC on the batteries. Any comments?
```

---
## \#8 Posted by: MysticalDork Posted at: 2019-08-25T05:40:55.227Z Reads: 78

```
The most powerful vesc-based controllers I know of is that 200A one you already picked. There are other options, but most don't have nearly as nice of a software experience as the vesc-based ones. I'm using a Sabvoton 72v, 100A controller (the old breadloaf style, the newer ones are more of a square puck - much smaller) and I've been having nightmares with engrish and badly documented hardware and software. It has a reputation as a very solid controller but it's giving me fits getting it set up. It does have the advantage of a nice big aluminum plate that all the fets are mounted to - easy to slap a water block onto for liquid cooling, and they're available in higher current versions - 200A or more IIRC.

Another big name in the ebike world is the Kelly controller - available in sizes from rinky-dink 24V, 10A things, all the way to truly monstrous 144V, 600A and 120V, 800A beasts.
```

---
## \#9 Posted by: MysticalDork Posted at: 2019-08-25T05:42:41.781Z Reads: 79

```
I think one issue you will encounter is that these larger controllers don't handle extreme ERPM very well. With a 150KV and 12s, you're getting close to what they can handle, and you would definitely exceed a limit if you increased your battery voltage without changing your motor KV.
```

---
## \#10 Posted by: AjaniBilby Posted at: 2019-08-27T00:56:01.866Z Reads: 62

```
I did some light research about Sabvoton and Kelly which reminded me that anything higher than a 12s configuration will start getting exponentially more expensive. Because I’ll need a better motor, speed controller, BDSM, and also relays to cut all power from the traction battery in the event of a crash (legal stuff).

This then runs me back to the idea of what if I can have some sort of transmission. Let’s say that I have a magical box with 90% efficiency which can change my gear ratio between the motor and the rear wheel between 1:4 and 1:8 (I can buy dog clutches, gears, shafts to make a gearbox, then investment cast a casing and paws. But that’s another discussion). This solution should allow me to get good torque/acceleration (I’m not aiming anywhere near Zero levels, because that is actually dangerous and it allows you to slip out your bike mid-turn super easy from what I have heard), while also being able to achieve good speeds without getting off the bike and swapping sprockets. If this gear box approach could work, I’ll probably settle for a system that works for now, but design it so I could fit a gear box later in life.

Also using the water-cooled 200A FlipSky VESC, I suspect both the 8kW & the 18kW motors will be held back by the controller. I presume the 18kW would be held back a lot more. Would the 18kW motor give me double the performance of the 8kW in this setup? Because it’s double the price.
```

---
## \#11 Posted by: MysticalDork Posted at: 2019-08-27T01:17:16.500Z Reads: 58

```
I doubt you'll get double the performance unless you have a beefier controller just due to the bottleneck. I think the 200A vesc with the 8KW motor is likely fairly closely matched - You'll need a controller that can handle ~400A at 12s to get that 18KW number. Also, that's BATTERY amps not motor amps. Motor amps may be as high as 1000.

One possibility to avoid this issue is to use multiple smaller motors and controllers, all geared together and sharing the power. Multiple 200A vescs and 8KW motors maybe.
```

---
## \#12 Posted by: AjaniBilby Posted at: 2019-08-27T01:46:00.418Z Reads: 56

```
I did also think of that.
I could possibly have a straight 1:4 motor, then later add a 1:2 geared one connected to the 1:4 (thus 1:8). Then I could do some funky arduino stuff to input different throttles to the two controllers based on speed.

Also one last question. Safety hazards aside.
Is there such a thing as too many cells in parallel? Could you feasibly overload your VESC by the battery alone (presuming you don't do something stupid in the settings)? Also what is the best way to throttle just the amount of continuous amps just in case?
I presume I'd need a DC/DC converted, but most of them are gear towards also outputting low volts.
(FYI I 100% will have fuses as a fail safe, but I'd still like to try and remove the chance of blowing fuses)
```

---
## \#13 Posted by: MysticalDork Posted at: 2019-08-27T04:43:17.824Z Reads: 48

```
There is really no limit to the number of parallel cells. If size/weight/cost was no object, I'd almost suggest getting two Tesla battery bricks (6S, 74P per module - 750A continuous discharge and 5KWH each) or maybe only one and carefully splitting it into two 6S 36P modules to run in series.

Limiting the current draw is literally the vesc's main job - it doesn't need any help from other circuitry.
```

---
## \#14 Posted by: AjaniBilby Posted at: 2019-08-27T05:05:20.526Z Reads: 43

```
I did try looking into buying something semi pre-made, and also cells from Tesla.
But I kept finding things that were 4-8x the price of buying Panasonic 18650 cells and spot welding them together.

Tesla 6S74P seems like it'd end up more Hassel than savings.
Also shipping something like that will probably cost a lot more than the individual cells
```

---
## \#15 Posted by: MysticalDork Posted at: 2019-08-27T05:07:31.342Z Reads: 41

```
Hence why I said if cost was no object. Building a pack from discrete cells is definitely cheaper if you don't count the tools, equipment and time you'll spend.
```

---
## \#16 Posted by: AjaniBilby Posted at: 2019-08-27T05:45:23.063Z Reads: 35

```
MB I was reading that as I was boarding a train. I won't do that again.

It would still be cheaper even if you bought a kit to do it tool less xD.

In the tool-less approach I'd definitely have multiple BDSMs, so effectively separate packs in parallel since I don't quite trust the packs connections
```

---
## \#17 Posted by: AjaniBilby Posted at: 2019-08-27T07:38:11.175Z Reads: 37

```
I just realised something freaky....

The VESC calculator, with you set a lower ratio the torque and top speed are both right... Not one is higher and one is lower... What is this black magic!!! xD
(Even if I adjust the power percent so the speeds are the same in both ratios)

(FYI I have been using 1 as the motor inner-resistance for my calculations on VESC because I have no clue)
```

---
## \#18 Posted by: MysticalDork Posted at: 2019-08-31T02:37:50.512Z Reads: 25

```
The motor resistance is probably in the range of 5-15 miliohms. (0.005-0.0015 ohms.
```

---
## \#19 Posted by: AjaniBilby Posted at: 2019-09-03T07:44:17.281Z Reads: 25

```
I've just realised where my speed limitations are actually at, and that I was using the VESC calculator wrong....

I presumed that when you slide the 'drive power' up till the power & current turn red - that would be the limits of your system. I just clicked that for some reason it's turning red at a higher current value than the Imax I set...

So am I correct that the real limit will be when the current goes above my IMAX, rather than when it turns red?
```

---
## \#20 Posted by: MysticalDork Posted at: 2019-09-05T18:54:52.779Z Reads: 18

```
Dunno, never used the vesc calculator.
```

---
