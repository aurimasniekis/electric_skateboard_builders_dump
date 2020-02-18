# More speed and torque. Solutions?

### Replies: 12 Views: 789

## \#1 Posted by: Klaxs Posted at: 2018-05-04T09:13:34.322Z Reads: 166

```
Hello everyone. I have a query about a very economical configuration that I have made. I have an 8" mountainboard and I have mounted an Esc + a 7s 1p battery that I had from a old skate with a hub motor. It is a Esc very similar to the ones sold in Diyeboard. To have more power I have added 4 units in series. 18650, total 11s1p, the engine is a 6368 190 kv sensored and the pulleys are 60-20 teeth, and I get a speed of about 25 km / h on the flat.The problem comes when there is an inclination, even if it is small, with a road of 3% inclination the speed is reduced to 10 Km/h and I do not know what would be the solution to obtain high speeds in mountainous or with high inclinations

I have tried other configurations of pulleys, 60-15 and 60-12 but the speed and torque is even lower.

What solution would you do? Thank you very much and sorry for my English.
```

---
## \#2 Posted by: linsus Posted at: 2018-05-04T09:19:33.508Z Reads: 158

```
[quote="Klaxs, post:1, topic:54359"]
engine
[/quote]

*Motor

Need more cells in parallell, you dont have sufficient battery config to draw any big currents. Voltage sag on a 1P must be horrid as well.
```

---
## \#3 Posted by: rich Posted at: 2018-05-04T10:15:57.832Z Reads: 149

```
Like @linsus said 1p is not a good idea except you want to use the cells as a mobile cooker for boiling water for your tea. 

For 8" pneumatics you need at least 4p, better 5-6p (good cells). But even a 5p with bad cells is a bad battery with a lot of voltage sag. Or get lipos, that's cheaper and you won't get problems with power output.

Is your ESC rated for 12s?
```

---
## \#4 Posted by: Klaxs Posted at: 2018-05-04T11:10:52.649Z Reads: 132

```
Thank you very much. I thought that adding batteries in parallel only serves for the distance that can travel. I'm not sure if my ESC supports this amount of voltage. I have detected difference in speed and torque when I have gone from 7s to 11s

I will try to add 11s2p for the moment and I will expand what is necessary.

I attached you to my ESC, it's really bad ... 

![IMG_20180504_130339|375x500](upload://dl7spuIF5X1fxtUl3SsRkQ21kr2.jpg)
```

---
## \#5 Posted by: professor_shartsis Posted at: 2018-05-04T11:57:31.272Z Reads: 109

```
[quote="Klaxs, post:1, topic:54359"]
I have an 8" mountainboard and I have mounted an Esc + a 7s 1p battery that I had from a old skate with a hub motor. It is a Esc very similar to the ones sold in Diyeboard. To have more power I have added 4 units in series. 18650, total 11s1p, the engine is a 6368 190 kv sensored and the pulleys are 60-20 teeth, and I get a speed of about 25 km / h on the flat.
[/quote]


@Klaxs by my calculations, to have a top speed of only ~25km/h (15mph) on the flats with your setup you must only be getting roughly max ~5a battery amps or ~15a motor amps through the controller to your single motor at 25km/h (15mph). take a look at yellow line bottom left chart (vehicle thrust minus wind drag force), red line bottom right chart (5a battery amps) and blue line top left chart @ 15mph (15mph - ~15a motor amps). the chart represents 5a software battery limit only but you would reach the same top speed if your controller has a ~15-20a software motor amp limit instead.

https://image.ibb.co/hascDn/5a_battery.jpg

the solution for greater speed appears to be using a controller and battery pack that can safely output more than ~15-20a motor amps and more than 5a battery amps. for example, if you look at the following chart, i'd imagine you'd reach ~48kph (30mph) with a controller and battery with software allowing 60a battery amps and 60a motor amps such as a vesc with 60a battery limit and 60a motor limit settings.

this chart shows the same board but with 60a software motor amp limit & 60a software battery amp limit vesc controller settings:

https://image.ibb.co/gcm167/60a_60a.jpg

also if you will be using only one motor perhaps consider switching to 3.75:1 (60t wheel 16t motor) gear reduction instead of 3:1... this will improve your top speed, thrust/acceleration and efficiency:

https://image.ibb.co/eRQNUS/375_to_1.jpg
```

---
## \#6 Posted by: michaelcpg Posted at: 2018-05-04T12:57:42.205Z Reads: 81

```
Like others have previously said, unless you want to destroy your battery rather quickly, you need much more than 1P or even 2P. At a basic level, think of adding batteries in parallel as a way for your battery to be able to provide more torque (where as adding batteries in series increases top speed) and also reduces the overall stress on your battery 

You could go 2P if you really wanted to which would improve performance to some extent but you'll still fairly quickly ruin your battery and then have to start over again with buying a new battery. 

Better to invest a bit more now and get a decent sized battery that can provide a reasonable amount of current which will improve your range, hill climbing ability and battery cycle life significantly.

As a reference, I'm using a 10S9P pack with 8" wheels and dual 170kv 6374 motors with a 10/50 gearing ratio. My board has easily been able to climb any hill I've ridden it on and I live in a very hilly city :)
```

---
## \#7 Posted by: professor_shartsis Posted at: 2018-05-04T20:55:21.953Z Reads: 63

```
[quote="michaelcpg, post:6, topic:54359"]
As a reference, I’m using a 10S9P pack with 8" wheels and dual 170kv 6374 motors with a 10/50 gearing ratio. My board has easily been able to climb any hill I’ve ridden it on and I live in a very hilly city :slight_smile:
[/quote]

@michaelcpg looks like about ~29mph top speed & 111lbs peak thrust w/ 90a motor limit & 60a battery limit per motor?

https://image.ibb.co/dYwptn/170kv_5_to_1.jpg
```

---
## \#8 Posted by: michaelcpg Posted at: 2018-05-05T00:41:57.978Z Reads: 47

```
My real world top speed is around 35km/h in FOC. I expect that if I was running in BLDC mode the top speed would be closer to 40km/h
```

---
## \#9 Posted by: professor_shartsis Posted at: 2018-05-05T00:55:31.063Z Reads: 45

```
@michaelcpg what are your motor and battery amp limit settings?
```

---
## \#10 Posted by: michaelcpg Posted at: 2018-05-05T00:59:16.597Z Reads: 45

```
Battery 40A max, -13A min. Motor 80A max, -80min on each VESC
```

---
## \#11 Posted by: professor_shartsis Posted at: 2018-05-05T01:09:41.367Z Reads: 47

```
[quote="michaelcpg, post:8, topic:54359, full:true"]
My real world top speed is around 35km/h in FOC. I expect that if I was running in BLDC mode the top speed would be closer to 40km/h
[/quote]


that makes sense. the chart predicts a bit more than 40km/h top speed in BLDC mode, but it also doesn't factor any rolling resistance, drivetrain loss or iron loss (only wind and copper loss which are the 2 biggest).

40a battery limit & 80a motor limit (~99lbs peak thrust & ~28mph/~45kph predicted in BLDC mode):

https://image.ibb.co/eXFKtn/40a.jpg

@michaelcpg if we assume the pack's voltage sag is 34v and the motor winding + vesc resistance is 0.16ohm the prediction is almost exactly 40km/h top speed.

https://image.ibb.co/hJRER7/34v.jpg
```

---
## \#12 Posted by: Klaxs Posted at: 2018-05-08T19:06:14.310Z Reads: 23

```
I'm thinking of buying this battery for my configuration. Do you think it will be enough to have more speed and torque? Do you know another place to buy a low cost battery? Thank you very much to all

http://www.diyeboard.com/10s3p-samsung-lg-18650-lithium-battery-pack-p-631.html
```

---
