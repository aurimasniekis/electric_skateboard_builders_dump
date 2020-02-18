# VESC Order of Operations &amp; Hall Sensors

### Replies: 18 Views: 2061

## \#1 Posted by: Snow4us Posted at: 2017-10-05T21:49:36.631Z Reads: 185

```
Hi,  I just blew out a Maytech 50A VESC attempting to finish my 12s build with Carvon V3's.  I wanted to make sure I do everything properly so I don't fry another speed controller.  A few questions about the process in general:

-The V3's have Hall sensors, to use them, do I plug the sensor cable into this port on the VESC?  Is it okay to have this plugged in the entire time while I set up the motors?

https://i.imgur.com/BR1hkzv.jpg

A few questions about setup and order of operations:

-I would like to use FOC, do I need to do anything with BLDC under motor configuration? (ie motor detection.)  Is it alright to go straight to R & L measures as long as FOC is selected in Motor tab?

-I am connecting via canbus, does the slave still need to be set up to receive ppm, or just the master? (also I learned the hard way that I need to set up each motor individually BEFORE connecting via canbus)

-If I have setup everything correctly, will the motors spin together via the arrow keys if I have the master connected and 'disabled' selected as the control mode?

-I come from the multirotor world and am used to having to change the phase wires around.  Is this necessary with eSK8?
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-10-06T02:58:34.622Z Reads: 152

```
FOC isn't recommended with maytech vescs in less you "upgrade" them by adding the components that maytech leaves off when they ship. They try to save money by using cheap parts and leaving parts off, and that makes them tend to fry DRV chips like no tomorrow.


If you do go with FOC, you should do all the motor detection in both the BLDC and FOC tabs and write the settings both times just to be sure. 


You only need to set up the ppm stuff on the master vesc.

You may have to swap phase wires, yes. If you do, remember to redo the hall sensor detection and save the settings after swapping phase wires, because otherwise you'll confuse the hell out of the vesc.
```

---
## \#3 Posted by: Mikenopolis Posted at: 2017-10-06T03:08:35.234Z Reads: 150

```
[quote="MysticalDork, post:2, topic:34884"]
swap phase wires, yes. If you do, remember to redo the hall sensor detection
[/quote]

Hmmm I wonder if that's how I killed one vesc and not the other
```

---
## \#4 Posted by: MysticalDork Posted at: 2017-10-06T03:19:01.550Z Reads: 140

```
It's possible. If you don't redo the hall detection, the vesc will think the motor is spinning one way and the halls will tell it it's trying to spin the opposite way because you swapped phases, and it'll just sit there and rattle and make angry sounds without spinning. Took me a while to track down what caused it.
```

---
## \#5 Posted by: ARetardedPillow Posted at: 2017-10-06T07:19:18.285Z Reads: 127

```
Youre better off using maytech vescs as door stoppers
```

---
## \#6 Posted by: Snow4us Posted at: 2017-10-06T15:41:57.634Z Reads: 122

```
[quote="MysticalDork, post:2, topic:34884"]
You may have to swap phase wires, yes.
[/quote]

How will I know if a swap is needed?  WIll the motor spin backwards when I hit the right arrow key?

[quote="MysticalDork, post:2, topic:34884"]
remember to redo the hall sensor detection
[/quote]

I have not heard of a sensor detection process in BDLC, I thought all you had to do was select hall sensor in FOC tab.  Where is the hall sensor detection conducted in BDLC?

[quote="ARetardedPillow, post:5, topic:34884, full:true"]
Youre better off using maytech vescs as door stoppers
[/quote]


Thanks for the information, I'm disheartened to hear that Maytech ESCs are such crap. I reached out to Carvon before beginning my build and they recommended I use ESCs from Psycotiller.  Bummer that they would recommend such crappy speed controllers for their new motors.  SHould I just return the new ESC I ordered and buy more capable VESCs, or do you think I have a good chance of success is I proceed with caution and double check all my work?
```

---
## \#7 Posted by: MysticalDork Posted at: 2017-10-06T15:48:14.701Z Reads: 104

```
If you're using sensors, you have to do the sensor detection, whether you're using BLDC or FOC. If you're willing to do a little bit of easy SMT soldering, I'd keep the maytech vescs and just add in the missing parts. 

I'd hook up the vesc to your remote and test the rotation there. I never really messed with the keyboard control.
```

---
## \#8 Posted by: ARetardedPillow Posted at: 2017-10-06T16:01:10.350Z Reads: 98

```
If you can, you should add in the missing parts but if you dont have the equipment for that you should def return those maytech vescs and get some quality vescs, maytech vescs have a bad rep and i wouldnt trust them when im going 25 mph on an eskate
```

---
## \#9 Posted by: Snow4us Posted at: 2017-10-06T17:12:19.785Z Reads: 100

```
[quote="MysticalDork, post:7, topic:34884"]
If you're using sensors, you have to do the sensor detection
[/quote]

How do you do sensor detection in DLDC tool?

[quote="ARetardedPillow, post:8, topic:34884"]
get some quality vescs
[/quote]

Any recommendations?  I'm hoping this board will be a rocketship with the 12s and dual V3s,  don't really want to risk substandard components.

[quote="MysticalDork, post:7, topic:34884"]
If you're willing to do a little bit of easy SMT soldering, I'd keep the maytech vescs and just add in the missing parts
[/quote]

[quote="ARetardedPillow, post:8, topic:34884"]
If you can, you should add in the missing parts
[/quote]

I can't find any threads or guides about upgrading the Maytechs.  What missing parts would I need?  I feel relatively comfortable with doing some basic soldering.  Replacing the DRV is above my ability level tho.
```

---
## \#10 Posted by: gogomrrobot Posted at: 2017-10-06T17:19:31.067Z Reads: 85

```
OT: Can you include a full sized photo of your build. I see a deck with those little freebord or binding inserts... would like a full view.
```

---
## \#11 Posted by: Snow4us Posted at: 2017-10-06T18:34:30.522Z Reads: 83

```
Here’s the full view. 

<img src="/uploads/db1493/original/3X/e/b/eb53b1306baf26c785fe1389c319d55f11052d60.jpeg" width="375" height="500">
```

---
## \#12 Posted by: ARetardedPillow Posted at: 2017-10-06T18:41:10.278Z Reads: 82

```
If you cant replace the drv, most likely you arent able to upgrade the vesc, i would suggest ollinvesc to be the best choice but those are 170 bucks per vesc, but you might have some trouble with shipping though, ive waited over a month and still havent received my vesc
```

---
## \#13 Posted by: Snow4us Posted at: 2017-10-06T20:45:56.012Z Reads: 71

```
I just dont have a heat gun, so would struggle with anything that has + and - underneath.  Any idea what people are saying about the Focbox vs Ollin VESC?  

Also, still confused as to how to 'do' a sensor detection.  I cant find anything on here, just posts about people saying that they got a detection failure or fault.  Any info on that process?
```

---
## \#14 Posted by: Snow4us Posted at: 2017-10-06T22:39:43.243Z Reads: 70

```
Really torn on if I should return the new Maytech VESC and get something better.  I live in the UT mountains and winter will be here in weeks :sweat:
```

---
## \#15 Posted by: MysticalDork Posted at: 2017-10-06T23:14:11.097Z Reads: 72

```
This is the tab where the detection is done. http://www.electric-skateboard.builders/uploads/db1493/optimized/1X/aa42f2525c52a702e51e32b3bd142d5e413afc24_1_690x407.png
```

---
## \#16 Posted by: Snow4us Posted at: 2017-10-09T07:19:35.059Z Reads: 66

```
[quote="ARetardedPillow, post:8, topic:34884"]
If you can, you should add in the missing parts
[/quote]

[quote="MysticalDork, post:2, topic:34884"]
FOC isn't recommended with maytech vescs in less you "upgrade" them by adding the components that maytech leaves off when they ship.
[/quote]

The only thread I could find about Maytech's missing parts was [this thread](https://www.electric-skateboard.builders/t/vesc-hall-sensor-connection/32867/18)  @darkkevind was missing C37, C51, and C14.  I got the new Maytech 50's in from @psychotiller and none of those are missing.  Is it safe to run sensored FOC if all those components are present?  Are there other components that are typically missing that I should look for?  I would really like to get full use from the Carvon motors and a quiet FOC ride.
```

---
## \#17 Posted by: psychotiller Posted at: 2017-10-10T16:09:25.410Z Reads: 55

```
Run sensored BLDC and you will have no issues. Also, you will have access to way more functions with 2.54 including cruise control.
```

---
## \#18 Posted by: Donson Posted at: 2017-12-02T22:43:24.616Z Reads: 45

```
i blow up one to..... but o order 3 drv83020 or so... can someone help me?
```

---
