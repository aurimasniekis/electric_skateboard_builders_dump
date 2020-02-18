# Hub motor building question

### Replies: 6 Views: 1330

## \#1 Posted by: Trans-amers Posted at: 2017-01-25T01:16:22.920Z Reads: 167

```
After my first build, I decided to get serious to my build for my daily commute, which includes a 3 mile hill trip( YES the whole trip is a slope) The trip has a 11% slope and road here in the uk are quite broken compare to road in us. I am a a 67kg asian which means dual 6355 is quite enough for me. I do carry equipments so the load is 80kg at most.

OK off to the topic lol
I always liked the design of carvon hubs and I wished that i can build one like them. I do have access to milling machines and welding machines which helps. The plan is here:

* dual alien 6355 60kv

* gt front truck strut (303mm according to the official website)

* avenue trucks

* mbs 100mm wheels

The mounting is actually quite easy. A modified pulley(without the gear part) frjunior@JuniorPotato93 is needed to mount on the motor with bearings from the motor. There are 4 mounting holes on the outerside of the alien motor, which can be used to hold the wheel. 
**THE PROBLEM IS**:

* With a 10s build, the speed is 41.85km/h or 26mph which is ridiculously fast to me, yet I heard that **loaded top speed is halfed**?.

* 12s 123A 26650 70A or 10s 2.7ah 35C ? Also I dont really find anywhere that i can buy chargers and bms (for both lips or li-ion) here in the uk.

* Where can i buy gt front truck here in the uk? I have no idea where to get them. They are never on the uk site.
```

---
## \#2 Posted by: HTownBomber Posted at: 2017-01-25T14:06:10.290Z Reads: 121

```
Interesting idea.

26mph should be the weighted (loaded) top speed according to [http://calc.esk8.it/](http://calc.esk8.it/) (assuming 70% efficiency).

Problems you might run into:

* Outrunners are more efficient at higher KVs. When you get down under 100kv, it means lots of really thin copper windings, introducing significant current losses and translating to more heat.  It won't have nearly the same low-speed torque as a belt-driven setup.  3 mile hill climbs might burn those motors out.
* It appears that the drive mechanism is weight-bearing in your setup.  The wheels will be pushing up on the outside of the motor can at an angle.  What's to keep it centered?  a couple little grub screws fixing the shaft to the can?  Or are you gonna extend the motor shaft out through the wheel?  If not, the motor can will tilt and your magnets will hit the stator.
```

---
## \#3 Posted by: Hummie Posted at: 2017-01-25T20:10:15.390Z Reads: 93

```
heat to torque is proportional regardless of the kv.  a low kv wont spin as fast and reduce the overall possible power as speed x torque is power and a hub motor is a slow turner without a gearing to take advantage of greater speed
```

---
## \#4 Posted by: Trans-amers Posted at: 2017-01-26T00:45:52.499Z Reads: 81

```
I'd never know out runners are more efficient at higher kVs! thank you!
So I might just have to switch back to a belt drive system then.

For the design of the motor, I will take he motor apart, remove the shaft as well as the inner bearings of the motor, mill the truck to fit the inner diameter of the motor, also weld a mount at the end to screw in the motor. **The connecting part between the wheel and the motor will be a pulley like design to fit the core of the wheel hub, a base to fit the four acres to the out runner, as well as a hole at the centre of the connector( between four screw holes) to fit the removed motor bearing.**

As it seems possible, you are absolutely right with the concern that the the out runner might dislocate due to shear stress. I would fit a sk3 6374 with two bearing at both end but they only have a 149kv motor. Anyway I'm now changing back to a **belt drive system** :) 
like this:
http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":12,"motor-kv":130,"system-efficiency":80,"motor-pulley-teeth":15,"wheel-pulley-teeth":40,"wheel-size":100}|
```

---
## \#5 Posted by: Trans-amers Posted at: 2017-01-26T00:57:07.578Z Reads: 72

```
So I guess without meeting the highest speed, the torque will not be the highest, right?
```

---
## \#6 Posted by: Hummie Posted at: 2017-01-26T05:53:03.287Z Reads: 67

```
I imagine if u got any motor and spun it at max speed and added a gear u would get max torque.
```

---
