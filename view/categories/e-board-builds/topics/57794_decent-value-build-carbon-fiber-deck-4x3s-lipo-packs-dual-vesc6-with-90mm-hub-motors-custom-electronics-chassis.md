# Decent value build: Carbon fiber deck &#124; 4x3s lipo packs &#124; Dual Vesc6 with 90mm hub motors &#124; custom electronics chassis

### Replies: 11 Views: 671

## \#1 Posted by: rbstv Posted at: 2018-06-04T16:42:25.302Z Reads: 197

```
Hey guys, I haven't been active on this form before, but thought I'd make a post and share a build that was completed several months ago. It is my first build and I'm quite happy with it for now.

The specs are:
Carbon fiber deck https://www.hi5ber.com/incisor
4x 3s 4500mAh RC lipo packs
2x Vesc6
2x Maytech Hubs http://www.maytech.cn/en/mto91hbm-nh/8803.html
typical PWM transmitter/receiver

max around 50km/h
goes about 20km but haven't bench-marked precisely.

The design goal is an optimal bang for buck dual hubs setup. The total cost ended up around $1200 dollars, but can easily go below $800 if I chose a less fancy deck and ESC.

The VESC6's were a bit pricey but definitely runs smooth without problems, I was a beta tester and mostly expertise in electronics so this is something I'm willing to splurge on. If I build another, I would consider using another ESC another my friend is working on that can drive 2 motors for $100: https://odriverobotics.com/#features

The battery configuration is designed to be as cheap as it gets, 4x3s RC lipo packs in series. Cost $120 total.
There is no BMS, the VESC already takes care of over current and low voltage protection. To charge it, I bought four low current 3s chargers for $6 each https://tinyurl.com/ybr7yej4. They are low current enough to charge through the balance ports without needing to unplug each battery to charge, and the balancing is a plus.

Not so worried about bending the batteries in this arrangement since a carbon fiber deck has zero flex. 

The design was made to fit this battery -> https://hobbyking.com/en_us/turnigy-battery-nano-tech-4000mah-3s-25-50c-lipo-pack-xt-60.html?___store=en_us
but recently hobbyking stopped shipping batteries to japan, so I had to find a chinese equivalent in the same form factor. From a past project, I found these nano-techs to be very slim for a 3s (20mm) and did not puff up much with age. 

The chassis is custom made, designed for 3D printing, the filament used costs around $20 excluding trial iterations during design. If anyone else wants to use it here's the link : https://cad.onshape.com/documents/02d850ea504003ff8ec3647a/w/247ca65aba941cf1eb0a8ab4/e/7696919bd0aa67d72aa20b4e
One notable thing is that the battery compartment is designed to "slide out" which provides the mechanism to access the balancing ports to charge as well as swapping the battery packs on the go.

I was a bit worried about the quality of the chinese hubs knowing there will not be any manufacturer support. but TBH I've had no problems with them so far. The 800W max per motor is a bit lower than I'd liked, but I guess that is the trade-off for the full enclosure causing worse heat dissipation. They haven't been over heating on me since I find myself rarely needing to max throttle. I chose them mainly because they were cheap and has a low 60KV ideal for a 12s build.

![2501387487940744344|375x500](upload://1HvTwaFJlJQMDW4bSw4gOaoBP7a.jpg)![4181253589518535863|666x500](upload://A20pvhOVdZNCl4JygrtXzOLw5VE.jpg)![3590385262633990604|375x500](upload://boRYyTLwTLgfNIZ76JEf4EnYdZ.jpg)![3914195972621096017|375x500](upload://jNA8s4A4aBUA5Ev6uJi2Vczu61U.jpg)![Screenshot from 2018-03-23 03:13:06|690x377](upload://xbU9zOVOTj7KBNglhGOBtX76BfS.png)
```

---
## \#2 Posted by: Lionpuncher Posted at: 2018-06-04T17:58:51.399Z Reads: 137

```
The build looks great! Curious to hear your thoughts on those hubs a year from now. 
Have youu weighed the board? Looks like it would be fairly light. Very COOL!
```

---
## \#3 Posted by: baxter Posted at: 2018-06-05T01:28:15.629Z Reads: 119

```
You (or your friend) might like to create a new thread on this forum for the Odrive speed controller design?

It’s always nice to hear about new options for Esk8 speed controllers 😀.
```

---
## \#4 Posted by: rbstv Posted at: 2018-06-05T04:47:22.092Z Reads: 111

```
AFAIK currently it's more geared towards 3D printer and robotic arm applications. The hardware is up to spec but it won't be plug and play for electric skateboards ATM since there needs to be firmware for smooth throttle, coasting, battery management, drivers for various remote input sources etc. Sensorless FOC current control is implemented though, and field weakening is on the feature list. It is open source, so if I decide help development for esk8te integration I will probably make another post.

Actually I attempted this a while back, but put the project on hold since there's a lot to do to catch up to the VESC and I didn't have so many free weekends to spend on engineering.

https://www.youtube.com/watch?v=vvgma1lW7A0&feature=youtu.be
```

---
## \#5 Posted by: goldrabe Posted at: 2018-06-05T04:59:08.495Z Reads: 102

```
Wow someone from Japan too!
I literally thought i am the only e-skater here.  Where are you located?
I have the Maytech Hubs too, but replaced them with different hubs because of over heating and bad Urethane.
Nice build by the way, have you had any incidents with the police so far?
```

---
## \#6 Posted by: rbstv Posted at: 2018-06-05T05:24:19.001Z Reads: 94

```
Hmm so the hubs seems to be very slightly off balance when spinning at high speeds, and there is a little bit of vibration when max throttle free spinning. I haven't driven other hubs of the same size before so not sure if other's are way better in this aspect. When I ride it it's not noticeable at all, considering there's way more vibration's coming from the road.

The entire board and wheels feel very stiff by design, this is fine since back streets in tokyo are fairly well paved, but I can imagine designing in more flex next time for bumpier conditions.

The total weight is relatively light compared to other boards of the same specs, but I was hoping it wound end up lighter since I did shell out for a CF deck. In total it's about 7kg.
Motor 1kg X2, trucks + front wheels 1.2kg, vescs 0.2kg x2, deck 1.6kg, batteies 1.3kg, chasis, wires, etc
```

---
## \#7 Posted by: rbstv Posted at: 2018-06-05T05:33:29.923Z Reads: 86

```
cool, I'm around East Side Tokyo, what about you? maybe pm me n we can meet up if you like or something

They sell chinese Eboards at donquixote these days, I've seen a few salary men kicking them around b4 haha

I mostly ride really late at night so there's no cars or people around usually. And I just get off when there's police around. It's a relatively stealthy build usually they don't notice unless I dart it. 

As I said, no problem with the hubs so far, though they are a bit massive IMO considering I was designing for weight as well. probably get a set of hummies next if they wear out (I've hand a 300 doller deposit with him for over a year now lol)
```

---
## \#8 Posted by: madcowswe Posted at: 2018-06-15T04:34:17.898Z Reads: 64

```
Hi, Oskar here, creator of the ODrive.
I don't mean to hijack this thread, but I thought I'd say Hi due to the explicit invite ;D

It would be cool to see ODrive used in EV's (skateboards, bikes, etc), and I'd love to help that happen. @rbstv is right, the focus has been on robotics, but nothing is stopping us to cater to Esk8 also. Especially if we can engage, excite and help independent firmware development of the required features.

Any recommendations on how I can find and engage devs? Any recommendations on a board I can test on that is nice and doesn't require too much time to get going, that either doesn't come with a controller, or where the controller is easy to rip out?

Cheers!
```

---
## \#9 Posted by: Anubis Posted at: 2018-06-15T06:23:16.321Z Reads: 52

```
Kind of looks like you made your own predator banshee, looks good man :smiley:
```

---
## \#10 Posted by: baxter Posted at: 2018-06-15T09:48:37.490Z Reads: 49

```
Hi Oskar,

The best advice I can give is that you should start a thread and share your design! I am sure that people who are technically competent (I am not) would be more than willing to give feedback/assist you in developing and testing your ODrive, or some other similar ESC design prototype if you think that might be appropriate.

The biggest issues we have in the community when it comes to speed controllers are cost and reliability, especially when it comes to handling potentially high currents (up to 80A continuous).  There are the cheap and nasty chinese made speed controllers from E-bay and Aliexpress which can be unreliable, and there are the super expensive ones, like the Vesc 6.x sold by Trampaboards. While the Vesc 6 might be reliable, coming with all the bells and whistles (like traction control), they are also prohibitively expensive for your average e-board builder (£300 each!).

At the moment the Vesc 6.x tends to be the benchmark of esk8 speed controllers.  There have been a number of members of this forum who have developed their own clones using the v6 design, and had a measure of success selling them. There are designs such as the Focbox and Focbox unity which have been derived from Vesc 4.x designs, but there aren't many options when it comes to an affordable alternatives in the market, at least ones designed for esk8 which are reliable.

If there was a speed controller (or even a dual speed controller) which was as reliable and customisable for 10S-12S voltage, but more affordable than a Focbox, I dare say it would become VERY popular in the esk8 community.  

The good news is that the esk8 community are always willing to try out new things!  

Looking forward to your thread! :smiley:
```

---
## \#11 Posted by: rbstv Posted at: 2018-06-16T05:32:00.554Z Reads: 39

```
Lol Oskar how did you find this? I see your doing pretty well these days.
```

---
