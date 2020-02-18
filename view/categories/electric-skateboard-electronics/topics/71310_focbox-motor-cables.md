# Focbox motor cables

### Replies: 20 Views: 454

## \#1 Posted by: JensSjogren Posted at: 2018-10-15T15:44:38.908Z Reads: 158

```
So i just picked up my focboxes that im going to use on my trampa build. First thing i noticed is that the 3 motor cables is 14 awg. From what i understand i need 10-12 awg for my 80 amp motors running on 12s li-ion. I want my total peak power to be around 130-140 amps. Will theese 14 awg motor cables be a bottleneck for my setup? My torqueboard vescs has 10 awg motor cables.

Thanks in advance for any help given!
```

---
## \#2 Posted by: Kug3lis Posted at: 2018-10-15T15:49:35.554Z Reads: 156

```
First question will the focbox itself would handle 130-140 amps :laughing:
```

---
## \#3 Posted by: wafflejock Posted at: 2018-10-15T16:13:08.228Z Reads: 150

```
https://sciencing.com/cable-length-vs-power-drop-12184174.html

Yeah would really be curious if you're pulling that much power anyhow I mean is this thing going up a 45 degree incline with a 300lbs gorilla on it or what? (hitching a car for towing?)  Typically I pull around 10A at 40V or 400W at 'peak' on a regular cruise, have seen it get up to 20A or so but in what world do you need 130-140A at 50V or 5000W+ of power.
```

---
## \#4 Posted by: Kug3lis Posted at: 2018-10-15T16:14:36.728Z Reads: 144

```
I have seen max like 50A with my current setup coming from battery

EDIT: single motor... I am even using MR60 connector but now will need to switch back to bullets as 80mm motor wire is bit bigger... and later on to 8mm for ARC200 testings...
```

---
## \#5 Posted by: wafflejock Posted at: 2018-10-15T16:15:11.250Z Reads: 142

```
Yeah if I was intentionally speed running or testing acceleration I could see it getting higher (or if I weighed more) but that is a lot of juice :)
```

---
## \#6 Posted by: wafflejock Posted at: 2018-10-15T16:16:50.177Z Reads: 140

```
Long story short is shorter cables will have lower resistance just because of the length (more length of wire is more resistance, but also more length of wire is more surface area and mass to dissipate/consume the heat).  The amount of amps a given thing can sustain depends in part on how long you're sustaining that peak amps and how many watts of heat it is bleeding off.
```

---
## \#7 Posted by: JensSjogren Posted at: 2018-10-15T17:14:16.975Z Reads: 117

```
Well with total peak power i am of course refering to both of my motors and focboxes, so 65-70 amps per focbox. The focbox is rated for 60 amps continious right. The evolve GT is supposed to peak 80 amps and my build is a lot more beefy than an evolve so this isnt strange at all to me :) 

The purpose of the board is to run in mountainbike tracks so i want to be able to pull a lot of power when i need it
```

---
## \#8 Posted by: barajabali Posted at: 2018-10-15T17:54:53.372Z Reads: 106

```
Make sure you use some additional cooling
```

---
## \#9 Posted by: Kug3lis Posted at: 2018-10-15T18:04:57.540Z Reads: 105

```
[quote="JensSjogren, post:7, topic:71310"]
evolve GT is supposed to peak 80 amps
[/quote]

Are you kidding bro? :D
```

---
## \#10 Posted by: JensSjogren Posted at: 2018-10-15T18:12:52.940Z Reads: 106

```
According to evolve atleast. Saw that on a evolve weekly episode (dont remember which one). Anyhow it may of course be over exadurated from their part
```

---
## \#11 Posted by: wafflejock Posted at: 2018-10-15T18:21:23.972Z Reads: 103

```
Okay well what I'm saying is it just depends on how long you are pulling how many amps to determine how many watts are getting lost in heat.  It isn't exactly like a pipeline width since the added heat from the current will increase the resistance typically and will therefore be a bit of a feedback cycle the longer you are heating the wire the more resistance you're adding the more you're heating the wire.

If you want to assume you have continuous 130A through a wire at a given voltage then you can calculate the voltage drop, but if you sustain that load you'll continue to add heat and increase the resistance until you melt the conductor.  Also things we haven't discussed yet but are relevant the battery amps vs motor amps (typically you'll have much higher motor amps than battery amps due to the duty cycle, the voltage is on off, on off with the BLDC motor so you'll have bursts of high amperage as voltage is applied to the coils.

Assuming 50V and 14AWG (2.525 ohms per 1000ft) and assume 6 inches of phase wire then we take .5ft /1000ft * 2.525 = 0.001263 or 1.263 milli-Ohm.  At 130A you'd have 130^2 * 1.263 mOhm ~= 21W bled off in a wire (let me know if I botched the math somewhere or used the wrong equation here... very possible).

https://www.calculator.net/voltage-drop-calculator.html?material=copper&wiresize=8.286&voltage=50&phase=dc&noofconductor=1&distance=1&distanceunit=feet&amperes=130&x=105&y=27

Anyway all the calc and numbers aside getting some real world data on the temp and actual amp draw will help more than any amount of academic argument :)
```

---
## \#12 Posted by: JensSjogren Posted at: 2018-10-15T18:22:27.370Z Reads: 96

```
https://youtu.be/hIEj9ylmKRI

1:55
```

---
## \#13 Posted by: Kug3lis Posted at: 2018-10-15T18:25:49.816Z Reads: 95

```
Fcking no shit i never seen more than 30a on remote :D maybe he is talking in total not single motor :D
```

---
## \#14 Posted by: JensSjogren Posted at: 2018-10-15T18:27:06.821Z Reads: 94

```
Thanks for the info, i am of course not expecting 130a cintinous. However i want to be able to get that huge burst for a second or two. Basicly the 14 awg should be fine? 😅. Im going to connect 10awg from the 3.5mm bullet connectors since that is the cable that i ordered. Or maybe even resolder and put 10awg from the focboxes directly
```

---
## \#15 Posted by: JensSjogren Posted at: 2018-10-15T18:28:20.954Z Reads: 93

```
Dude, that is what i said all along. Total amps for both vescs and motors
```

---
## \#16 Posted by: Deodand Posted at: 2018-10-15T18:56:27.528Z Reads: 92

```
Burst current really doesn't matter for wire gauge unless it's something absurd (2000 amps or something). For wire gauge what matters is continuous pull, it will take your wires a few minutes to heat up and become damaged. 14 AWG is plenty for phase wires, the resistance of the internal FETs is going to be much higher than this short length of wire, thus the FOCBOX will thermal throttle before your 14 AWG wires get anywhere close to melting (unless you liquid cool or something). Most wire amp ratings you read online are for building codes where the wires sit inside insulated walls next to potentially combustible material. They are very conservative, like you can usually multiply that number by 3 and still not run into huge problems for the short wire runs in eskate applications.
```

---
## \#17 Posted by: JensSjogren Posted at: 2018-10-16T11:19:45.710Z Reads: 67

```
Got it! Thanks for the detailed answer! :)
```

---
## \#18 Posted by: Goonman Posted at: 2018-10-16T14:30:18.445Z Reads: 55

```
Evolve GT only pulls max 40amps constant.
```

---
## \#19 Posted by: JensSjogren Posted at: 2018-10-16T14:45:05.947Z Reads: 52

```
Well as previously mentioned i was talking about peak/burst or whatever you want to call it.
```

---
## \#20 Posted by: Goonman Posted at: 2018-10-16T23:42:21.964Z Reads: 40

```
Yes I read that. Total maximum number recorded seen verified at any moment in time (resolution of about one sample per second) on my evolve gt is 40amps at 40v 1600w. It uses 14awg battery wires. 40amps through 14awg wire gets hot (measured 80deg C) quickly. So I know it's all relative because hot to touch isn't necessarily too hot for the wire. But bigger wire is better. 80amps peak for one or two seconds through 14awg ok whatever but how are you going to control that?
```

---
