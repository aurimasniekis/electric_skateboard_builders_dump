# Electronics schematics

### Replies: 12 Views: 617

## \#1 Posted by: Jammm Posted at: 2018-09-22T20:12:18.967Z Reads: 146

```
Hello !

I would like to use 2 6s lipos in series with this BMS : http://www.batterysupports.com/44v-48v-504v-12s-100a-12x36v-lithium-ion-lipolymer-battery-bms-p-393.html

This is the schematic that comes with the BMS : http://i1098.photobucket.com/albums/g378/lilianleung/LOGO%20Connecting%20Chart.jpg~original

This is my schematic : 
![Electronics%20scematic|260x500](upload://vAxammqli2bRYv651fSRTrG3WiF.jpeg) 

Is this right ? Please do not hesitate to correct my schematic
```

---
## \#2 Posted by: rich Posted at: 2018-09-22T20:23:52.371Z Reads: 123

```
![correct|260x500](upload://178DYGKkP5O55Amirg3qzzX0BxU.jpeg)
```

---
## \#3 Posted by: laurnts Posted at: 2018-09-22T20:25:04.324Z Reads: 108

```
Switch is only installed to the positive or the negative side only (never both). As far as I recall, there is no antispark that connect to both positive and negative.
```

---
## \#4 Posted by: rich Posted at: 2018-09-22T20:35:37.549Z Reads: 100

```
He is not talking about an antispark loopkey, every antispark switch needs both.

@Jammm don't connect both "0", only the positive balance wires for this BMS then you are good 2 go :sunglasses:
```

---
## \#5 Posted by: Jammm Posted at: 2018-09-22T20:46:22.121Z Reads: 101

```
Alright thank you very much, i'll make sure to post here once i've got all of my components !
```

---
## \#6 Posted by: b264 Posted at: 2018-09-22T20:50:49.446Z Reads: 102

```
[quote="laurnts, post:3, topic:68889, full:true"]
Switch is only installed to the positive or the negative side only (never both). As far as I recall, there is no antispark that connect to both positive and negative.
[/quote]

The new 3D Servisas (@Kug3lis) antispark switches have positive and negative, and some hobbyking ones do also

@Jammm you need to pay attention to which lines are thick (10AWG or 12AWG) and which are thin (20AWG or 22AWG).   Also, take a look in the [Beautiful Diagrams](https://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179) thread

I know for sure the wires going to the charge jack don't need to be 10AWG and really shouldn't be in case there's a short, you want the wire to be able to melt and fuse away hopefully
```

---
## \#7 Posted by: Namasaki Posted at: 2018-09-27T04:18:19.539Z Reads: 73

```
If you haven't already purchased the BMS, you might consider getting a Bestech bms with built in anti-spark 
E-switch.
```

---
## \#8 Posted by: Jammm Posted at: 2018-09-27T04:34:30.245Z Reads: 69

```
I haven't purchased it yet.

I know it sounds lazy, but do you have a link to such a BMS ? I can't find one on the bestech website
```

---
## \#9 Posted by: Namasaki Posted at: 2018-09-27T04:41:24.237Z Reads: 70

```
This is the one I use. It is 80A continuous 240a peak.
You can buy direct from Bestech (min order qty is 2)
http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html

Or you can buy one from @JLabs

https://buildkitboards.com/collections/parts/products/bestech-bms?variant=7201537687582

I have been using this bms on my builds for about 2 years now and they have been rock solid dependable.
```

---
## \#10 Posted by: Tilt Posted at: 2018-10-11T16:34:26.164Z Reads: 58

```
@Namasaki If this BMS has a max continuous discharge of 80A, but my twin motors are 50A each, shouldn't I want a 90A or 100A BMS to fully utilize my motors' power?
```

---
## \#11 Posted by: Namasaki Posted at: 2018-10-11T19:12:41.975Z Reads: 53

```
The current values on the battery side of the Vesc are different than the values on the motor side of the Vesc. 
I run dual Vescs set to 50a batt max each and dual motors with motor max at 80a each with the 80a bms which btw can handle current bursts up to 240a supposedly.
```

---
## \#12 Posted by: Tilt Posted at: 2018-10-12T06:26:55.803Z Reads: 41

```
Thank you Namasaki! Pardon my ignorance, but how do the VESCs put out 50A each if the BMS can only put out 80A? 

Also, Lucy sent me this. 12s, 80A out, 15A in. My only question left is about the 50.4v...it says it's 44.4v but then on the same spec sheet says its 50.4v. Does that matter? Is this BMS what I would need? 

![Screenshot_2018-10-11-21-11-44|281x500](upload://bHDo20oZ7fUYFWzdwv54y6ATKjm.png)
```

---
