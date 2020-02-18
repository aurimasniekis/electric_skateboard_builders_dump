# First Build Problems- No Speed? Turnigy 245kv Motor Stalling?

### Replies: 11 Views: 192

## \#1 Posted by: ianturner45 Posted at: 2019-06-09T05:51:45.863Z Reads: 48

```
![IMG_3091|375x500](upload://zR0K7YEROcf6v9E9VI8188VBwjH.jpeg) ![IMG_3092|375x500](upload://igM9IkiFGTxYd3BjZNiyj0UobVd.jpeg) 

I am building an electric skateboard for college this summer and I need some help. 

These are the parts I am using:
-Turnigy sk3 245KV
-Samsung 30Q (and two goups of LG HG2) cells in 10s3p configuration
-10s BMS from Mboards.com https://www.mboards.co/collections/diy-supplies/products/10s-bms-battery-management-system
-ESC from Mboards.com (comes with remote) https://www.mboards.co/collections/escs/products/single-belt-driven-motor-esc
-Caliber II trucks 
-Abec 11 83mm flywheels
-32" cruiser deck
-36t wheel pulley
-16t motor pulley

I completed my build today only to find that I could barely pick up any speed. I cannot even ride my board up my driveway. I am not using a sensored motor in my build, however it does start without a push. I am thinking maybe the ESC is not able to supply enough current to the motor but I am not sure, I realized after purchasing it that it's a piece of crap from China. My batteries are soldered together with nickel strips and squished together inside my enclosure. Has anyone had similar problems? Is it my speed controller? Battery? I assume it's not the motor since many people have reported going 20+ mph with the turnigy sk3 245kv. Also my board pretty much has no braking power. I can get going on flat surface to about 10mph but I can barley stop and I have to jump off the board. I am thinking my speed controller is crap but since I have never done this and Mboards isn't responding to my emails I'm not sure what the problem is.
```

---
## \#2 Posted by: Dirt_Bag Posted at: 2019-06-09T07:09:37.524Z Reads: 41

```
Reposted from other forum:


DO NOT USE THAT BATTERY.

Dissasemble it right now. That thing is a massive fire waiting to happen.

If you did any research at all you would know that mixing lithium batteries is a catastrophicly bad idea

That speed contoller is not designed to be able to control a motor like that one. This whole build is future bonfire.

I am not trying to be mean, but this is just dangerous. You will burn down your house at some point if you make things like this. Apart from the mixed battery, there is almost no insulation. I see bare wires and uninsulated parralel groups. 1 mistake and you will have another reason it will catch fire.


Also, soldering batteries heats them up to extremely dangerous levels. You shorten their life and you will possibly blow them up when soldering. The lack of safety on this thing is genuinely terrifying. I honestly think its best to dissasemble this and throw away the battery safely.

Just buy a prebuilt and dont burn you house down. I promise at some point this thing will catch fire if you continue using it.
```

---
## \#3 Posted by: ianturner45 Posted at: 2019-06-09T16:21:40.283Z Reads: 32

```
I realize the battery is dangerous and I did do my research. In fact I got the idea from another forum that mixing batteries was OK. https://endless-sphere.com/forums/viewtopic.php?t=75779 I understand mixing batteries, soldering them, etc. isn't the best idea but I don't see why it wouldn't work. This is not my final setup either, I plan on making a different enclosure with safer wiring. However, assuming that the battery works and is just dangerous, it is just the speed controller that's holding me back?
```

---
## \#4 Posted by: xsynatic Posted at: 2019-06-09T16:36:53.560Z Reads: 31

```
very big yikes.

Listen to what @Dirt_Bag said and prevent being homeless due to a fire in your home or worse.
```

---
## \#5 Posted by: ianturner45 Posted at: 2019-06-09T16:46:40.799Z Reads: 30

```
Got it. I'll disassemble the battery right now. Is the speed controller the issue though?
```

---
## \#6 Posted by: Voxu Posted at: 2019-06-09T16:49:44.626Z Reads: 27

```
Shouldn't be an issue.
```

---
## \#7 Posted by: AlanZhou Posted at: 2019-06-09T17:21:06.047Z Reads: 23

```
The reason the motor is stalling Is case it's 245kv and it's single drive and also because of the esc...
```

---
## \#8 Posted by: ianturner45 Posted at: 2019-06-09T17:29:11.132Z Reads: 23

```
So would you suggest buying a lower KV motor or a VESC or both?
```

---
## \#9 Posted by: AlanZhou Posted at: 2019-06-09T17:31:25.382Z Reads: 24

```
Get a lower kv motor.  190kv and below, and than get a vesc if you can and your exiperence will be much better.
```

---
## \#10 Posted by: ianturner45 Posted at: 2019-06-09T18:06:35.661Z Reads: 21

```
Does anyone have experience using this type of ESC? It's the cheap kind you can get on ebay for $40. I have seen successful builds using this motor so I'm hesitant to buy a different one right now. https://www.electric-skateboard.builders/t/diy-electric-longboard-first-ride-10s-5000mah-lipo-turnigy-sk3-6364-245kv/28492
```

---
## \#11 Posted by: bazis Posted at: 2019-06-09T19:37:15.136Z Reads: 17

```
You can live with 245kv motor. I used it in single drive and get 30km/h on 60% of power. 
Your problems from cheap controller. Get vesc from flipsky. Better [fsesc 6.6](https://flipsky.net/collections/electronic-products/products/flipsky-fsesc-6-6-based-upon-vesc%C2%AE-6-heat-sink?variant=8739267510332)
```

---
