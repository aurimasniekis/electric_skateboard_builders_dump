# Esk8 Dyno testing

### Replies: 31 Views: 2627

## \#1 Posted by: Blasto Posted at: 2017-02-24T03:58:17.813Z Reads: 400

```
This is still work in progress, but the objective here is to able to get some consistent data out of a esk8 setup without any terrain influence.

<img src="/uploads/db1493/original/3X/0/e/0e656624775ea6287b517f4c18217e8fa62035b1.JPG" width="666" height="500">


currently i'm running in to a few challenges:

1- my flywheel is not big enough to consistently measure the torque of a system, currently a system is able to hit max speed within 100ms. My data acquisition is at a 20ms rate. _I will be adding a bigger steel fly wheel machined out of steel_

2- I'm not able to load up my system  enough to get a max current output of a motor. _I will be adding 2 36T pulley on each side of the drum to put 2 6374 slave motors with a pair of vesc to control the slave current ressistance_

3- Get a better material to adhere to the drum, the current one got folded by the R2 ghost hubs

<img src="/uploads/db1493/original/3X/1/6/1609aacf7ccafaf409a70d5e579d3c713a275d28.JPG" width="375" height="500">

image R2 G hubz

I am using a few methods for data acquisition. 

on the input of the dyno I have a EloggerV4 from eagle tree, this module is used to measure the **input voltage, output current and RPM of the drum**

I am also using @Ackmaniac APP for data acquisition for redundancy.

The drum is a 62mm diameter 13" long aluminium cylinder.

initial result with the R2 ghost 90mm hubz, I shorted one of the hubz as a slave and used only one driving hub... but I need a bigger load, still has plenty of power to go by 

<img src="/uploads/db1493/original/3X/e/c/ec8c81af5c5fa9ed959d9f111f6068985f99c7de.png" width="690" height="409">
```

---
## \#2 Posted by: Okami Posted at: 2017-02-24T07:57:12.672Z Reads: 358

```
Nice work! I bet there are many of us waiting for the progress in this field! :)
```

---
## \#3 Posted by: Blasto Posted at: 2017-03-05T18:39:36.031Z Reads: 328

```
Found some nice material for a flywheel, a nice 35Kg steel chunk, it has some gravity to her

<img src="/uploads/db1493/original/3X/e/a/ea88ead2728050d226db016834f3f72e3f16a24b.JPG" width="666" height="500">
```

---
## \#4 Posted by: Okami Posted at: 2017-03-05T20:52:43.200Z Reads: 308

```
Good.. we will need some more detailed review once you have collected some good data from real e-boards!
```

---
## \#5 Posted by: jaykup Posted at: 2017-04-11T18:03:32.569Z Reads: 298

```
Is this project still active?  It seems very interesting!
```

---
## \#6 Posted by: Blasto Posted at: 2017-04-11T18:04:28.280Z Reads: 303

```
Yes still alive, slightly on the back burner... so many projects
```

---
## \#7 Posted by: Blasto Posted at: 2017-04-16T01:16:49.633Z Reads: 301

```
Big ass fly wheel added, not as big as originaly stated, but it's good enough for the girls i go out with

<img src="/uploads/db1493/original/3X/f/d/fd69967e697804db94f0f6c6b851362ede0db942.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/8/d/8d60fe2b9894334315c9ec397a9c2f6b3739d592.JPG" width="666" height="500">

First run for the giggles

http://www.youtube.com/watch?v=0MoMY3g11y0
```

---
## \#8 Posted by: onloop Posted at: 2017-04-16T01:31:50.229Z Reads: 286

```
Haha... awesome!...

Need some straps..... or just stand on it ;)
```

---
## \#9 Posted by: Blasto Posted at: 2017-04-16T01:44:12.091Z Reads: 287

```
Sone static pics of the setup

<img src="/uploads/db1493/original/3X/f/b/fb942662912556055d5a3f7a9f0a57101df5a1f6.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/6/2/62e3ae23b2155672d4d6fa531baa440f46b0ae70.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/1/d/1dfc0be017eebe2269d98e91e20f61dcfb709457.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/4/d/4d0f564688255603bd7604772247ddb71a06f228.JPG" width="666" height="500">
```

---
## \#10 Posted by: jaykup Posted at: 2017-04-17T14:46:35.954Z Reads: 252

```
This is awesome!
```

---
## \#11 Posted by: Okami Posted at: 2017-04-17T14:58:10.707Z Reads: 250

```
Cool update.. post some power output data once u get something..

IT does look like you gonna need some sort of clamp to hold the boards down.. the ''wheel well'' (u shape thing) looks like wont hold the boards in place :D 

/ if that was even meant for such purpose //
```

---
## \#12 Posted by: jaykup Posted at: 2017-04-17T15:35:24.170Z Reads: 250

```
Try these clamps - they would be perfect for this type of application.

We use them all the time in manufacturing

https://www.grainger.com/product/3CXV4?gclid=CL-Z-I_nq9MCFZCFswodfAMJdw&cm_mmc=PPC:GOOGLEPLAA-_-Hand%20Tools-_-Clamps-_-3CXV4&AL!2966!3!50916772317!!!s!71849729719!&s_kwcid=AL!2966!3!50916772317!!!s!71849729719!&ef_id=WPTfJgAABE3xAS-I:20170417152838:s

probably need a bigger version.
```

---
## \#13 Posted by: Okami Posted at: 2017-05-17T19:14:15.795Z Reads: 234

```
@Blasto Could u describe the 'process'' a bit more?

I want to know how to build a dyno.. and how hard it might be? Im seeing a lot of mechanical work involved but did you write the software itself?

How do you do the measurements?

I would really love to test some motor outputs soon,.. so this info would be kind of crucial. 

--

When you can, please take up some evolve 5065 motors and try to push them to the max.. lets see how much can they actually deliver..
```

---
## \#14 Posted by: Blasto Posted at: 2017-05-17T19:25:07.587Z Reads: 226

```
My main issue at the moment is to find the time to use it.....

To get the torque output of a given system, I use @Ackmaniac's app for the data acquisition on the master VESC.

The data will contain the following information:
-Pack voltage
-Pack current
-ERPM
-time stamp

What I still need to calculate is the moment of inertia of the flywheel, to which i did not have time to do yet... 

with all that info, I should be able to get a nice torque curve.


the second system, I connect the dyno slave motor to the system, using another vesc for the data acquisition (or eagle tree) and apply a constant load on the system. I still haven't figured it out yet, but hopefully i'll be able to get the efficiency of a given system.

hope that is unclear enough for now haha.
```

---
## \#15 Posted by: Okami Posted at: 2017-05-17T19:47:31.346Z Reads: 210

```
Ok, at least now I kind of get that there are 2 methods for testing this.

Im more interested in this 'slave' motor thing.

I can only imagine that the Rspec motor you have there is the one who is the 'slave' and it is also connected to vesc, where you see all the data..

Then, you just make the motors 'compete' against each other and measure the values in between..

Though there are still a lot of unclear parts about this.. and im also not sure can you get reliable results in the method I described (one motor against the second one)
```

---
## \#16 Posted by: Pedrodemio Posted at: 2017-07-17T19:39:46.641Z Reads: 200

```
The best way to do the second way and get efficiency is to use an strain gauge or a torque wrench so you can measure the mechanical torque at once

This way you can set the ERPM on the slave VESC and them set a current on the master,this should provide a nice diagram of torque and efficiency like those that @Mellow do

https://www.instagram.com/p/BN1uG-8A1jL/?taken-by=the_endless_engineer
```

---
## \#17 Posted by: Cobber Posted at: 2017-07-18T12:06:05.614Z Reads: 191

```
would be cool if you/someone with a rig like this could attend the las vegas esk8 con... even if i can't make it... would love to see what is what measured by a quantitative tool...
```

---
## \#18 Posted by: evoheyax Posted at: 2017-11-13T23:48:20.003Z Reads: 177

```
@Blasto is this still going?

Really interested in it now. After SPD2, I realized how weak most hub motors really are. Would love to show the numbers hummies motors put out vs the raptro 2 hub motors vs carvon v3/v4 vs other cheap hub motors.
```

---
## \#19 Posted by: pbrink Posted at: 2018-05-08T03:18:35.786Z Reads: 151

```
Any update on this?? Very interesting.
```

---
## \#20 Posted by: MoeStooge Posted at: 2018-05-08T05:13:14.717Z Reads: 152

```
Was discussing this very topic a week ago with @psychotiller.. With the speeds and power were making it's getting to a point where road testing the limits of a high performance vessle is becoming more hazardous than necessary..  Along with the WR board taking shape so is a prototype for a stand on Fluid Dyno.  The layout will be a simple hydraulic pump plumbed to a resivour with a ball valve for pressure regulation. The pump will be driven by a small barrel, floated and then attached to a one Foot moment arm that will push on a scale.. the setup will strap the board down and the operator will weight the board, regulate the fluid back pressure, read torque output on the scale and be able to sustain loads over time to exploit performance weakpoints without sacrificing skin and blood..  I think this may also be a good test tool for diagnossing speed wobbles under load.
```

---
## \#21 Posted by: Scoo_B_SK8 Posted at: 2018-05-08T05:52:21.779Z Reads: 146

```
i just spent last hour researching Dyno setups to better understand this setup after reading through this topic earlier when @pbrink asked about it .  i get what dyno's do just not how they specifically worked to collect data. was gonna @MoeStooge ya, cause thought about your rocket ship.  also looked like something fun & interesting to put together, and now you just :exploding_head: all over again.

some details/schematics (even hand drawn) of any eSK8 dyno would be sweet to see or knowing @MoeStooge style,  it'll just appear.

anyways AWESOME stuff!
  i'll figure it out someday :wink:
```

---
## \#22 Posted by: E1Allen Posted at: 2018-05-08T06:10:42.211Z Reads: 142

```
@MoeStooge 

Are you more concerned with the motors and ESC or the drive system as well?

Considering they are RC motors I've seen motors run with large propellers for testing.  That would test the motor ESC and batteries if you're able to data log.

I've seen a car alternator being used as well to provide resistance.
```

---
## \#23 Posted by: pbrink Posted at: 2018-05-09T03:15:37.095Z Reads: 139

```
A friend in college built a dyno for the SAE Baja kart. He used on of these dynos with a roller setup. May be of interest to you all. 
https://www.dynomitedynamometer.com/kart-dyno/kart-dyno.htm
```

---
## \#24 Posted by: Cobber Posted at: 2018-05-09T03:38:08.574Z Reads: 142

```
When ever I think of a eSk8 dyno I think of using a set of "track bicycle roller(s)" as a base. Track side we used these to warm up/cool down between sprint events...

random internet video

https://youtu.be/XgJprqwSQog
```

---
## \#25 Posted by: MoeStooge Posted at: 2018-05-09T12:17:54.831Z Reads: 136

```
Upsides of the double roller is it takes up less room than a barrel and stabilizes the rear axel.   In my mind the barrel roller would allow for rear axel instability.  Would give the operator a chance to work on speed wobbles without getting thrown to the ground at 40+..   Hmm ?maby a hybrid with a small removable roller in front of the barrel..  either way the WR board is going on a Cycle Dyno for some comparative baseline #s for the toolbox.
```

---
## \#26 Posted by: Scoo_B_SK8 Posted at: 2018-05-09T12:34:12.237Z Reads: 132

```
outside the box... how fast can you get a tread mill going? (of course with a few mods)...

-would allow the rider some sway left and right 
-would introduce incline / decline 
-handle(s) would give rider quick safe bailout option

transferring balance/weight of rider instead of fixed position
```

---
## \#27 Posted by: psychotiller Posted at: 2018-05-09T14:53:31.263Z Reads: 126

```
Yeah, I like the idea being able to move around on a belt but having the handles for emergencies
```

---
## \#28 Posted by: lock Posted at: 2018-06-02T03:39:54.226Z Reads: 109

```
These mini dynos are pretty cute.

https://www.instagram.com/p/BjevyXLAHuA/

Not sure if BajaBoard's one is actually a dyno with any sort of resistance/power measurement; it kind of looks like just a set of rollers.
```

---
## \#29 Posted by: lrdesigns Posted at: 2018-10-24T02:13:39.144Z Reads: 77

```
![please-sir-may|500x300](upload://xkZJ5rFQfYnWOaKzrelece0zbMh.jpeg) 

DYNO TESTING?
```

---
## \#30 Posted by: PumpkinEater Posted at: 2019-06-17T00:51:57.881Z Reads: 34

```
I'm gunna pick this up. A regenerative dyno is perfect for this.
```

---
## \#31 Posted by: Okami Posted at: 2020-02-12T17:40:45.254Z Reads: 9

```
Damn, seems like this thing got put off for a while.

Or whoever made one is using it but just havent published it online.

How do commercial board makers test their boards? I think I saw some vibration etc stands in some videos, not sure about dynos..
```

---
