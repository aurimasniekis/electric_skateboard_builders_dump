# Drive Train Wobble at full gas 12sp5 dual 6355 foc box

### Replies: 16 Views: 407

## \#1 Posted by: Leonardadelmann Posted at: 2018-08-31T11:41:09.370Z Reads: 165

```
Hey! 

Wanted to ventilate a topic which a couple of guys here in Stockholm (me included) are trying to figure out. At this point we got 5-6 easkting dual beasts here in Stockholm. All of them running 12sp5, dual 6355, foc box x2, 15/36 gearing 97mm wheels. 

Even having all belts perfectly tightened, nothing being to loose or to hard we still feel like the drivetrain wobbles whilst giving it the full acceleration on 12sp5. (THINK OF IT AS THE ENTIRE MOTOR SECTION VIBRATING/SHAKING, which instantly dissapears when giving it less then 100% throttle) One of the original owners said he did not experience this kind of wobbles prior to upgrading to 12sp5. 

I'm just curious if there is any solution to this? We've been looking at making these upgrades to the board in hope to solve the wobble issue. Input on this really appriciated. 


These are the upgrades we were thinking about doing: 

Trucks: https://electricboardsolutions.com/collections/trucks/products/caliber-truck-ii-50-with-extended-axle-pre-sale-pair 

Idler pulley: https://electricboardsolutions.com/collections/pulleys-belts-mounts/products/idler-pulley-for-15m
m-belts 

pulley combo: https://electricboardsolutions.com/collections/mechanical-parts/products/pulley-combo 


You would think that these modifications would maybe make the drive train more stable at full gas. Going from 9mm-> 15mm and better optimized belt tension. 


Thanks a lot, 
Leonard
```

---
## \#2 Posted by: Andy87 Posted at: 2018-08-31T12:00:26.729Z Reads: 154

```
[quote="Leonardadelmann, post:1, topic:66646"]
did not experience this kind of wobbles prior to upgrading to 12sp5.
[/quote]
what you mean with it?
what was before 12s? the 10s battery?
Maybe it´s just normal speed wobbles which appear because of higher speed than with 10s.
```

---
## \#3 Posted by: Leonardadelmann Posted at: 2018-08-31T12:04:56.216Z Reads: 146

```
I've been skating all my life, there is a difference between the druck wobbling at high speed due to not being tight enough and the drive train not being stable during 100% acceleration. Having to build 100% throttle gradually because the drive train is wobbling has nothing with speed wobbles to do. This has something to do with the drive train and the increased power to the motors with 12sp5.
```

---
## \#4 Posted by: Andy87 Posted at: 2018-08-31T12:08:17.213Z Reads: 138

```
so good to know about it.
and as I understood there was a 10s battery inside before and with it didn´t appear, right? it´s just not clear about which modification you was speaking.
maybe just I didn´t got it...
maybe @fottaz can recommend what will help to reduce that drive train wobble.
```

---
## \#5 Posted by: Leonardadelmann Posted at: 2018-08-31T12:10:29.498Z Reads: 132

```
I've never owned the board with the 10s config. But one of my friends did. He said himself that riding 10s he did not experience the problem I previously mentioned. After the upgrade to 12s the problem appeared. Which in my eyes is related to higher power to the motor or the drive train (3d printed carbonfiber) not being stiff enough to handle the power the dual 6355's output
```

---
## \#6 Posted by: taz Posted at: 2018-08-31T13:28:18.088Z Reads: 130

```
I have a 12s5p dual beast and was plagued by speed wobbles when I first got the board.
The board now is very stable and allows me to stay full throttle all the time (50km/h) when before I got speed wobbles above 25-30km/h.
Here is what I did:

Got rid of the rubber angled risers. Replaced the with 2x6mm on the front and 2x6mm risers + riser with wire guide on the back.
Install a 5 degree wedge on the front.
Move the rear truck in the further back position.
Change the pivots with Riptide 96A
Change the front bushings to Riptide 88A WFB barrels and the rear to Riptide 95.5A boardside and 93A roadside WFB barrels.

Do all this and you will not believe how much more stable the board is.
The most important changes are the solid risers and the Riptide bushings.
The eskating beast is a fantastic board but with thw stock setup IMO is down right dangerous.
```

---
## \#7 Posted by: Pedrodemio Posted at: 2018-08-31T14:00:24.874Z Reads: 114

```
Are you using ERPM limit? If you are and are hitting it, the PID loop could be unstable  when the input is too high (100% throttle)
Or even the current control loop can become unstable
```

---
## \#8 Posted by: kuphjr Posted at: 2018-08-31T15:11:27.924Z Reads: 106

```
^ This ^

When I first rode my dual motor I though something was wrong with the motors because my speed wobbles were bad at 30+ mph. Then I realized it’s because the stock bushings on the TB trucks were trash at that speed. Needed high quality barrel bushings and it solved everything.
```

---
## \#9 Posted by: fottaz Posted at: 2018-08-31T15:24:07.720Z Reads: 104

```
I would say as the last good guys here, if top speed is a problem about wobbles, tighten the trucks even more, and even change higher quality bushings if calibers one are not enough.
I think I might install higher quality bushings, I think those extra money are worth then.
Also lowering settings can help, if too high.

I don't agree on changing the soft angled risers we install, they absorb vibrations very well. Just to let people know we are installing the rear trucks on further back place of the Evo, to improve stability and motor/wires distance too.
```

---
## \#10 Posted by: thisguyhere Posted at: 2018-08-31T15:29:55.302Z Reads: 103

```
stock bushing on caliber and especially caliber clones are total trash.

i replaced them with [cupped washers](http://www.buzzedtrucks.com/product-category/amishwashers/), [insert bushings](https://www.skatepro.com/en-us/413-30212.htm) boardside, barrel bushing roadside.  hell, upgrade the pivot cup too if you wanna get crazy.

whole board felt better tuned and removed a lot of the slop and wobble.

also vary the duro on front and back trucks and that'll prevent wobbles a bit more.

one last thing, when i was getting wobbles, it turned out of the motor was dying and delivering lessened torque compared to the other motor.
```

---
## \#11 Posted by: Saturn_Corp Posted at: 2018-08-31T16:11:56.049Z Reads: 93

```
OP's not talking about getting speed wobbles, but rather his whole drive system shakes and wobbles at 100% acceleration. 

Or have I just missed the question entirely?..
```

---
## \#12 Posted by: Kug3lis Posted at: 2018-08-31T16:22:18.468Z Reads: 88

```
Yes you are correct, its about drive train vibrating from top speed probably at that RPM the whole drivetrain reaches oscillating frequency and starts to vibrate similar to cars but cars have it at much lower I guess. Try change belts width, and cross bars or etc to make it more rigid I am not belt drive expert.
```

---
## \#13 Posted by: taz Posted at: 2018-08-31T16:32:07.039Z Reads: 85

```
Guys, I have the exact same board and have done all of that before.
I started with tightening the bushings, then changing them, then replacing the rubber riser pads with solid ones. This eventually solved the problem.
The rubber riser pads allow the whole rear truck to move under load and create that instability.
That coupled with the fact that due to the evo's difference in the front and rear angles that requires softer bushings in the front and stiffer in the back leads to that behaviour.
The drivetrain is excellent, the motor mounts are very rigid and adjustable along with all the other items.
I don't agree with Alberto on the fact that the rubber riser pads help to absorb vibrations since I barely noticed a difference when I changed them out.
```

---
## \#15 Posted by: accrobrandon Posted at: 2018-08-31T17:46:09.652Z Reads: 78

```
[quote="Deckoz, post:14, topic:66646"]
When he really needs to be in a perpetual turn/carve and never in the center.
[/quote]

This reminds me of snowboarding... Always 1% on one edge or the other... Never pefectly center because thats when things get scary... And when the edge catches again and youre not ready, or skilled, its face plant time =P
```

---
## \#16 Posted by: zpoole27 Posted at: 2018-08-31T18:01:48.533Z Reads: 77

```
I have a similar issue.

At full speed on 12s5p with dual focbox dual 6355 in FOC mode i get a "wub wub wub wub" affect at top speed. I literally cannot ride past 55kmph because it makes the board wobble.
```

---
## \#17 Posted by: Deckoz Posted at: 2018-08-31T22:20:30.326Z Reads: 68

```
[quote="accrobrandon, post:15, topic:66646"]
Always 1% on one edge or the other… Never pefectly center because thats when things get scary
[/quote]

This.. you said it better.
```

---
