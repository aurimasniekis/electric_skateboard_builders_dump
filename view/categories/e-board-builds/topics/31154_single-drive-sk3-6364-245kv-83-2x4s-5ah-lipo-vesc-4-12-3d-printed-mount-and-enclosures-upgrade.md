# Single drive Sk3 6364 245kV &#124; 83 2x4S 5Ah Lipo &#124; VESC 4.12 &#124; 3D printed mount and enclosures&#124; upgrade

### Replies: 5 Views: 650

## \#1 Posted by: Crossfire Posted at: 2017-08-21T10:22:59.375Z Reads: 122

```
Hi folks,
I've been around some time, reading and studying your awesome builds.
I've pulled the trigger in July and this is what I've came up with.

Motor: Turnigy SK3 6364 245kV
Board: Murksli Slider
Trucks: Paris 180mm
Batts: 2x4S 5000mAh Lipos
Charger: ISDT SC-620 with parallel charging DIY cables, charging time 35min @10A
VESC 4.12
Motor mount: 3D printed with XT-CF20
Enclosure: 3D printed with GreenTEC
Wheels: Orangatang Kegels 83mm

Top speed: 30+ km/h
Range: 14 km, 16km/h average

http://imgur.com/a/L6Y0E

Now, while I find my setup to be perfectly fine in terms of overall performance, I'm looking for a slight (few hundred $) upgrade:
Motor: 190 kV sensored 6374
Battery: additional 4S so 3x4S - 12S setup
Wheels: ABEC11 97mm, 75A
ESC: Focbox (because of, you know, FOC)
Trucks: Caliber II 50 or TB 218mm

What do you guys think? Should I go for even lower kV motor like 170 or 149 kV? Sensored? 
I'm quite set on 97mm wheels, Kegels are great but roads to my workplace are 40% rough. Need a smoother ride.

Paris trucks have some long-term limitations (too much hassle) for my 3D printed mounts so basically upgrading them to better profile is a no brainer. 218mm will give me even more options for the future (2x6374 anyone?), but raw Calibers just look so nice.

What do you guys think? What's rational upgrade and what's not? Any hints and experiences are welcome.
```

---
## \#2 Posted by: pat.speed Posted at: 2017-08-21T10:35:01.764Z Reads: 107

```
Sounds great. The torque boards trucks are a must if you want to go dual 6374. Maybe just add a 2s lipo so it is 10s otherwise you might get quite close to the erpm. Or you could lower the kv your choice
```

---
## \#3 Posted by: Crossfire Posted at: 2017-08-21T10:56:31.184Z Reads: 103

```
It's easier to add another 4S lipo and to charge 3x4S lipos in parallel @15A than charging 2x4S and then additional the 2S :slight_smile:
12S with 190kV motor calculates it to 59k erpm, so still in the ballpark.
Maybe changing the wheel pulley from 36 to 40T will be good for acceleration too.
```

---
## \#4 Posted by: pat.speed Posted at: 2017-08-21T11:08:02.911Z Reads: 99

```
Yes I know it is not over the erpm normally, but if you go full throttle down a hill you may hit the erpm and fry the Vesc. I think there is a setting to limit this though in the Vesc tool. I see what you mean about the charging now and yes 12s would be easier
```

---
## \#5 Posted by: Crossfire Posted at: 2017-08-21T11:58:57.401Z Reads: 90

```
That is correct...luckily I don't go full throttle down the hill...I'm all regen in that scenario :slight_smile:
Limiting it to 60k erpm is correct way. I have it set at 100k atm which is default value.
```

---
