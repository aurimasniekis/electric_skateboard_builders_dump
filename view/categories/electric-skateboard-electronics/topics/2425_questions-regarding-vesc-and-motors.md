# Questions Regarding VESC and motors

### Replies: 6 Views: 1139

## \#1 Posted by: loose_nickers Posted at: 2016-04-18T04:25:33.907Z Reads: 113

```
Hi guys.
As some may have seen my other post, doing a bit of research in regards to potentially building vs buying an electric board.
I've been scanning a few pages on here, as well as various sites regarding motors and motor controllers and have a few queries I'd be keen to see people's answers regarding.

Firstly regarding the VESC as it seems to be the most popular choice/variant.
For starters, the biggest thing I think I've found with this product is availability/supply. As per my original post, looking for something to use everyday as a reliable transport. Having an uncertain availability of a component could be concerning for this.
Also as there seems to be a fairly large demand for VESC controllers, my concern is there seems to be a variety of places manufacturing them and this leads to inconsistencies in quality.  If I couldn't get a replacement from the same place, what issues will I encountered?  I understand open source is good for some, but I see many potential issues here.

2) Being a unit needing precise programming to a motor for use,and apparently temperamental when not precise. This appears to open a large window for failure or poor operation as I've noticed a fair few on here having issues. Are there no pre-programmed/plug-and-play options?

3) Most/a lot of motors I've come across are un-sensored motors. I'm presuming 2 things from this. Firstly, is that there would be no ability for RPM limit programming? Second being from assumption and a couple of videos I have come across, is that low speed control would potentially be jerky or in a way "stepped" speed control. Anyone gone to sensored motors and programmed them for this reason?

4) I am most likely going to run dual motors. I'm yet to come across a motor controller to run 2 motors from the one unit, but rather 2 VESC's either being connected as master and slave via a CAN connection,  or 2 separate VESC's sharing one output from a reciever.
In either case I've seen they still need to be programmed individually and have noticed people with various issues in either situation. 
Additionally, in a video I found on the vedder page, I noticed the motors possibly seemed to be spinning at slightly different rates? Guessing a side effect of running un-sensored motors??

Cheers for any and all feedback guys.  Sorry for all the questions :slight_smile:
```

---
## \#2 Posted by: trbt555 Posted at: 2016-04-18T05:20:40.655Z Reads: 104

```
1) I think all current vendors will honor some form of warranty. I know @chaka will repair your vesc if it fails. Getting a replacement from another vendor shouldn't be a problem, they are compatible if from the same hw version and running the same fw.

2) Firstly there is a motor detection function that will measure the motor parameters for you. The rest of the setup is fairly straightforward. @onloop's vescs come pre-configured for his motors.

3) There defnitely is rpm limiting for unsensored motors, the erpm is calculated by the vesc by measuring the zero crossings of the back emf. This also allows the vesc to accurately determine stator position, which is beneficial to low speed startup performance.
Low speed performance is impressive, I can start from a standstil without a problem.

4) For every person with issues using dual vescs there probably are several people without.

If you wan't plug and play without having to invest time fiddling with settings and finding the optimal setup, I'd say the vesc isn't for you, but if you're willing to put in some effort, the results are impressive.
```

---
## \#3 Posted by: ikjahaa Posted at: 2016-07-29T16:55:45.476Z Reads: 58

```
Would you possibly know how to calculate these rpm limits for the vesc ?
for lets say in my case:
i have a SK3 -245Kv motor, run it in a 6S system.
Motor pully has 15teeth and wheel pully has 36 theeth.

Lets say I'd want to limit my max speed to about 25Km/h
```

---
## \#4 Posted by: Jinra Posted at: 2016-07-29T17:14:09.662Z Reads: 55

```
VESC using eRPM instead of RPM which is typically RPM x 7 for most 50-63mm motors. So find the the RPM you want to limit to and multiply by 7. Put that value into the eRPM max field on the VESC.

Use this calculator to find out your speed/rpm

http://calc.esk8.it/
```

---
## \#5 Posted by: ikjahaa Posted at: 2016-07-29T17:18:06.721Z Reads: 53

```
and min erpm has to be the same number but negative ?
```

---
## \#6 Posted by: Jinra Posted at: 2016-07-29T17:19:33.071Z Reads: 49

```
The number is negative by default to accommodate reverse. If you plan to use reverse at full speed, then yes. Otherwise you could leave it alone or set it to 0.
```

---
