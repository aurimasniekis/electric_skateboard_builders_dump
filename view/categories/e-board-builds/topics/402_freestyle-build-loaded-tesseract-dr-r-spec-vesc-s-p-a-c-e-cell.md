# Freestyle build &#124; Loaded Tesseract &#124; DR R-SPEC &#124; VESC &#124; S.P.A.C.E CELL

### Replies: 12 Views: 3337

## \#1 Posted by: Moja Posted at: 2015-11-03T09:02:17.787Z Reads: 243

```
 I've been assembling this board for a while, I wanted to make the best board I could for use as practical transport around the city with some freestyle jibbing abilities along the way. 
 I've made it so its easy to swap out batteries and access the VESC's to change settings with BLDC, the pelican case is water tight and the clip stays shut not problem. Velcro is awesome and simple, the battery has velcro underneath and the elastic velcro straps keep it secure over harsh bumps. 
 I went all out with hot glue to keep all the electrical components secure, I even added some glue to the soldering connections in the SPACE cell. I've been able to do ollies and acid drop curbs no problem, I intended to make the electrical components solid enough that I could smash the board against a wall for a good while. I intend to incorporate the fuse into the SPACE cell so it's still accessible, it looks a bit messy at the moment.
 I am using a Nyko Kama nunchuck and I also have a GT2B receiver so I can choose what I prefer at the time. I feel like the nunchuk is great for using the board as transport as it's got a great form factor and the cruise control it brilliant. However if I want to ride aggressively the GT2B's throttle feels much more safe and it fills your hand well. 
 I'm not getting as much range as I had hoped at the moment, seems to be around 30 minutes ride time when Im riding it aggressively. Im getting top speeds around 35kph with the 13t pulleys. 
 I would like to add headlights and brake lights, potentially indicators controlled by the Nyko Kama nunchuk. And maybe even an iphone mount on the nose so I can use google maps getting around the city or potentially even use an Android device hooked up to the VESC as a HUD reading speed and motor info.

Thoughts and suggestions?

Parts:

 - Caliber 33 degree trucks
 - Swiss ceramic bearings 
 - Abec 11 90mm 75a flywheels
 - Loaded Tesseract board 
 - 2x Enertion R-SPEC 2.0 190kv motors 
 - 2x K2 Gold & Carbon Limited Edition
 - 2x VESC 4.7
 - S.P.A.C.E cell 
 - 1020 Pelican case ESC housing
 - Nyko Kama nunchuk controller
 - Flysky GT2B
 - 13t pulleys 

<img src="/uploads/db1493/original/1X/3fed590d28dade27d692673ee1dc8cf05f40e875.JPG" width="690" height="460"><img src="/uploads/db1493/original/1X/cb2f44e272029dd0578f907b056b19b6611f940c.JPG" width="690" height="460"><img src="/uploads/db1493/original/1X/aecdc9c72ce6b5985eb9a7b06af34b85ef00daa4.JPG" width="690" height="460"><img src="/uploads/db1493/original/1X/66b8f79ef494c4cad38f43be0afa8d6d3f3683a2.JPG" width="690" height="460">
```

---
## \#2 Posted by: onloop Posted at: 2015-11-03T10:43:25.843Z Reads: 235

```
Awesome build... I like it that you are thinking about durability so you can do tricks.. I see that as an emerging trend with eboards.

In terms of top speed it seems about right.
<img src="/uploads/db1493/original/1X/b244a718d4a524630a46c7ad7c2db660598fbc32.png" width="281" height="500">


You will need to go to 14t pulley to reach 44km/h at full battery charge. Or 15t to get 48km/h at full battery.. I use 15t. I also get better range too. But my testing is in areas with very few hills of steep gradient.

In terms of only lasting 30min per charge it seems really low. 

What is the terrain like? What is your riding weight?
```

---
## \#3 Posted by: onloop Posted at: 2015-11-03T10:50:40.270Z Reads: 211

```
Sorry that last calculation was wrong, i wrote 160KV instead of 190kv
<img src="/uploads/db1493/original/1X/ffae84864233cb592b6ed557cb883752f3f80ec8.png" width="281" height="500">

You should be going much faster... something is not right
```

---
## \#4 Posted by: Moja Posted at: 2015-11-03T10:52:47.679Z Reads: 204

```
I weigh about 80 kilos and I'm riding up and down lots of hills with lots of accelerating and braking. I've got some 15t pulleys that I'll switch over too, I expect that when I am just cruising Im going to get much better range. Its riding like a dream though, loving the slow speed control with cruise control for my film work, just need to try and tweak the motor setting to try and get smoother performance form stationary and whilst changing direction at slow speeds so I can get smoother tracking shots. Any suggestions?
```

---
## \#5 Posted by: onloop Posted at: 2015-11-03T11:17:09.315Z Reads: 202

```
honestly i don't think you can avoid the slight stuttering that the motor tends to do before starting from a complete stationary position. one slight touch of forward momentum and it (stuttering) will disappear. I know this might not be ideal with bulky camera gear mounted on you but as a skater you are probably naturally pushing off with a start anyway?

is the start better with the GT-2B due to the more responsive throttle control?

you should play around with the start up boost settings and see if it helps.. default is 0.01, try 0.02, 0.03, 0.04 etc
```

---
## \#6 Posted by: Moja Posted at: 2015-11-06T08:18:18.572Z Reads: 193

```
Managed to get pretty decent results by tweaking those setting, once the motors are moving slightly the slow speed control and torque is great. I've been riding with 60am output on the motor so I'll do some more speed and range tests with things tuned up as see what I get.
```

---
## \#7 Posted by: Moja Posted at: 2015-11-06T08:21:55.578Z Reads: 186

```
BTW I kick flipped this setup first try a few days ago and and my mate Dan who runs Fiik did a 360 flip on his new single drive hub motor setup last week. Sorry to beat you to it Jason!
```

---
## \#8 Posted by: onloop Posted at: 2015-11-06T14:32:44.072Z Reads: 184

```
nice... but without video it didn't happen!
```

---
## \#9 Posted by: treenutter Posted at: 2015-11-06T14:43:55.414Z Reads: 184

```
@Moja @onloop This note is from [Vedder's page][1] about startup boost in VESC: "The range is 0.0 to 1.0, where 1.0 is full throttle (which you shouldn’t use.). A sane range is up to 0.15 or so."


  [1]: http://vedder.se/2015/01/vesc-open-source-esc/
```

---
## \#10 Posted by: dacc34 Posted at: 2015-11-20T18:14:37.753Z Reads: 174

```
How tall are those risers? I'm thinking of getting the same deck and trucks for my build.
```

---
## \#11 Posted by: siggs3000 Posted at: 2015-11-20T22:37:08.265Z Reads: 175

```
I have a Tesseract as my main (non-powered) ride and it's my absolute favorite board ever. This must be one awesome e-board!
```

---
## \#12 Posted by: willpark16 Posted at: 2016-06-04T20:44:15.792Z Reads: 118

```
how is this board doing?
```

---
