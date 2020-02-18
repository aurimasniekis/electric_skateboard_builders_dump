# Freewheel spinning on a Mellow Drive

### Replies: 8 Views: 1537

## \#1 Posted by: Mellow Posted at: 2016-12-11T09:36:23.634Z Reads: 207

```
Cogging being a sine wave function (repels and attracts equally) normally shouldn't impede how long a motor might spin freely, but does affect behavior at lower speeds, usually more only noticeable when not loaded. Still, we've optimized as much as we could while modeling for performance and efficiency. 


https://youtu.be/GcLAvYbbnzM

Bearings are grease-filled and were cold when we filmed. ;-)
```

---
## \#2 Posted by: Hummie Posted at: 2016-12-11T17:41:14.992Z Reads: 177

```
Nice. Is the easy spinning (lack of cogging) through electrical actions in the esc or
Solely due to the orientation of motor parts?
```

---
## \#3 Posted by: Rollbrett Posted at: 2016-12-19T11:51:09.816Z Reads: 135

```
Thats an interesting question and I hope Mellow will give us an answer soon.
Though I think it's most likely trough electrical actions.
"Almost all the techniques used against to cogging torque also reduce the motor counter-electromotive force and so reduce the resultant running torque." - Wikipedia
As a decent amount of torque is required for hubmotors I'd guess the minimal rolling resistance is not due to the orientation of motor parts. Instead they probably loop the generated electricity back into the motors. 

Does the VESC have a similar feature?
```

---
## \#4 Posted by: ccostel Posted at: 2016-12-20T12:29:03.956Z Reads: 113

```
[quote="Rollbrett, post:3, topic:14497"]
probably loop the generated electricity back into the motors.
[/quote]

Hmm this is quite an interesting way of doing it.
```

---
## \#5 Posted by: Mellow Posted at: 2016-12-21T19:23:32.206Z Reads: 102

```
Cogging is higher when the Drive is on, as in the video. We don't actively reduce it, but were thinking about it. We modeled different magnet widths in order to retain high torque - our priority.
```

---
## \#6 Posted by: Hummie Posted at: 2016-12-21T20:04:09.883Z Reads: 94

```
modeling magnet widths!  if you're going solely for highest torque wouldn't you go with full magnet fill and the thicker and stronger the better?  creating the strongest field you can?  Id think trying to be more efficient instead of going for max torque would be more unknown and require using modeling smaller magnets to maybe create a more sine wave.  Or higher temp magnets for a more continuous power ability.  I thought magnet width choice mainly had to do with the shape of the tooth, and with your smooth board tooth being compete ..sounds good for torque and a sine wave maybe for efficiency?  I'm likely oversimplifying.   Did you look into using a hallbach array?
in your modeling for max torque what part shows the losses most?  I recently read the point at which magnetic saturation of the tooth happens is at a much higher field strength than we would be using.  it happens literally on the end of the tooth I've seen in images.  very nice how you have a lot of tooth I imagine.  So instead of with magnetic saturation and it's increasing hysteresis more so the losses are ....mainly just copper still even at highest torque?  

especially with the slow turner you have 12x14, id think your biggest goal would be to get as much copper in..maybe at the expense of the iron.  ?
```

---
## \#7 Posted by: Mellow Posted at: 2016-12-22T15:54:31.831Z Reads: 74

```
@Hummie Since building a motor is always a give/take affair (increase here, leads to decrease there), modeling is the fastest way to target the desired specs while making sure what is given up falls within tolerances.

Magnet max temp is same as yours: 150C. - we didn't want to go higher and settle for less magnetivity. Concerning losses, for us, the thermal bottleneck in the system isn't the motors, but battery and control electronics. 

You really should come and visit us in Muenchen!
```

---
## \#8 Posted by: Hummie Posted at: 2016-12-22T17:26:07.202Z Reads: 64

```
Thanks if they were giving away tickets I certainly would.  There's s toy convention coming up in Germany which id also like to see. If you can spend some on a tix to San Fran u can stay for free at my place. Come in a month and hopefully will have more exciting motors for you to try

I'm surprised ur bottleneck isn't the motors.
```

---
