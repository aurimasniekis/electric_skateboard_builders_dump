# Fully 3D Printed 8S3P 270KV 4250 Dual Motor Setup

### Replies: 13 Views: 1212

## \#1 Posted by: gazwoo123 Posted at: 2017-08-09T04:34:46.123Z Reads: 204

```
Hey Guys,
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Just wanted to post up my build and get some feedback. Long time reader, first time posting. So I wanted to get  a board that was pretty lightweight, has decent range and decent speed. I am targeting 25km range and 30-35km/h. Currently I am upgrading to a 8S3P battery (max 60A but I’m limiting to 45-50A just to be safe) with custom 270KV 4250 sensored motor setup and is geared 1:3.2 (15T to 48T). The mounts, pulley and casings are all 3D printed.  

This is my old version below which is using 6S battery with 350KV motor. Should all look the same on the outside, but battery is thinner but longer. 

<img src="/uploads/db1493/original/3X/c/c/cccd7fe6718f6a50c04d386af9fec451da061fd5.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/7/e/7e10e577648a3e7f4c306dd876d9ff934654f39c.jpg" width="374" height="499">

<img src="/uploads/db1493/original/3X/a/a/aad311061e9af3d40f61a3d3085ecc86dfd064f1.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/e/2/e2e9628f524f4ab7f2f276d2e1017f801058a427.jpg" width="375" height="500">

Anyway, I recon the dual motor kit is close to ready so if anyone is interested in one check it out on my website here <a>www.savage17.com.au</a> . 

Will try post a more detailed build log on a regular basis there soon as well.

A few things need advice on as I try move to a production ready model:
* Anyone know a Chinese supplier for quality custom Li-Ion battery packs?
* Anyone know a cheap supplier to get a 48T pulley injection moulded or CNC’d?
* Anyone know a cheap supplier to get casings vacuum formed?

Other than that I think I am pretty close unless anyone else has anything else I should consider?
```

---
## \#2 Posted by: gazwoo123 Posted at: 2017-08-09T05:03:34.109Z Reads: 178

```
Probably should have put more details about the upgrade. So below is:
* New battery pack using Samsung 25R in  8S3P (seeking alternatives like 30Q or LG HG2)
* Custom built 4250 270KV sensored motor
* Custom built wireless transceiver for wireless remote to the longboard (same board on both ends). It is an integrated ATTINY + NRF24L01 all in one board designed from scratch (only 19mm x 29mm) with built-in 1S Lipo recharging.

<img src="/uploads/db1493/original/3X/e/5/e557d8a4f7f9a529ebb4ae1ab47b4baa0b26675e.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/d/e/de1685be4d93b0d1ac7f9b69fc9f10083fe5c2f1.jpg" width="375" height="500">
```

---
## \#3 Posted by: trancejunkiexxl Posted at: 2017-08-09T06:01:10.383Z Reads: 155

```
very nice dude... sick
```

---
## \#4 Posted by: Crossfire Posted at: 2017-08-09T07:52:05.002Z Reads: 142

```
Nice!
With what filament did you print those parts? I'm in the same boat, I've tried colorfabb's HT and Extrudr Green Tec so far and both can be easily used in those applications beside PETG or ABS.
```

---
## \#5 Posted by: gazwoo123 Posted at: 2017-08-09T08:02:37.117Z Reads: 138

```
Oh sweet, I haven't tried those filaments. I'm currently using Protopasta Carbon Fiber PLA. Super stiff and great layer adhesion. It's a bit expensive but super strong and prints easily. The stiffness is the key, because all the other filaments I have tried allows the motor mount to bend too much under the strain of the belt tension.
```

---
## \#6 Posted by: Crossfire Posted at: 2017-08-09T09:23:26.602Z Reads: 130

```
I'm trying to avoid PLA as much as I can, but reinforced with CF it could do the trick. Especially that Green Tec prints better than PLA at 200C and it's sturdy as anything. For enclosures temps are not that problematic but for mounts where motors can easily get very hot it's mandatory to get good materials which can withstand the temps over 100C. 
Yeah, bending under belt tension is a problem. I've made my mounts way thicker because of it.

Do you get any vibrations on the motor because of the printed pulley - on the bench for example when accelerating? My printed pulley adds some under slight acceleration (probably resonance) but then rings out quickly. I'm quiet pleased with 3D printed parts for casual abuse.
```

---
## \#7 Posted by: gazwoo123 Posted at: 2017-08-09T09:34:47.175Z Reads: 121

```
Well the CF PLA seems to be working fine, and my motors have never gotten close to that hot. As far as it adding vibration I don't believe so, it could be that your pulley is off centre? (I have had issues with that in the past). I will probably move back to Aluminium pulleys because the teeth aren’t printed very well even with 0.3mm printer nozzles (for HTD-3M). As for enclosures, I'm hoping someone can tell me on here a good supplier that will build vacuum formed enclosures for me.
```

---
## \#8 Posted by: Crossfire Posted at: 2017-08-09T09:56:42.487Z Reads: 115

```
Exactly. 
I'm leaning toward the aluminium pulleys for the wheels as well. My pulley is screwed into the Kegels, tight enough. But when you rotate it on the truck it has a slight wobble. So basically that's what is causing  those vibrations.
Teeth were printed quite good, no problems after 50km so far.

You can easily print VESC enclosures, why not. I'm using 2x4S atm and I've printed that one too because it's big enough for my 20x20 printer.
```

---
## \#9 Posted by: TONY888 Posted at: 2017-12-02T17:03:53.531Z Reads: 85

```
really nice done！are those 4250  motor powerful enough for going up hills？im sure they are going tosave a lot of weight though，interesting in buying  of those motors for my super light build！any specs？weight especially，and how many kw？
```

---
## \#10 Posted by: Jammeslu Posted at: 2017-12-02T23:35:24.367Z Reads: 71

```
What enclosure are you using for the 8s3p
```

---
## \#11 Posted by: gazwoo123 Posted at: 2017-12-03T03:38:19.182Z Reads: 57

```
The motors themselves seem plenty to get me up hills (I weigh 70kgs) with 1:3.2 gearing. The motors weigh around 270g and probably good up to 1kw each. I only have a few for prototyping so if there are more people interested I can get more of these made.
```

---
## \#12 Posted by: gazwoo123 Posted at: 2017-12-03T03:38:55.880Z Reads: 58

```
The enclosure is a 3d printed one I made
```

---
## \#13 Posted by: Jammeslu Posted at: 2017-12-03T10:29:37.724Z Reads: 46

```
Pm sent about it
```

---
