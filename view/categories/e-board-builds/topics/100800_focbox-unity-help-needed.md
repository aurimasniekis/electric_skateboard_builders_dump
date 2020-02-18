# Focbox Unity Help Needed

### Replies: 10 Views: 171

## \#1 Posted by: achatham Posted at: 2019-08-24T18:14:16.910Z Reads: 60

```
Is there a Focbox app for iPhone? I found the "Focbox UI" app for Windows on GitHub but im not sure if this is what I should be using. If not what should I go with?

Also when I run a motor detection it gives me a "Flux Linage Measurement" error. Read the post on the issue, but didnt help. The test makes a loud beep, halfway spins the motors and then gives a message to hand spin each wheel forward for 15 seconds. I do this and it comes back with the error and red on the ui.

One thing I did that I regret is cut my motor senors so Im running sensorless. Is this causing my issue? Only reason I cut them is because the torqueboard sensor wires on the motors did not match up with the focbox unity input.

https://photos.app.goo.gl/ZF6i2pdTwsnqaXfm7
```

---
## \#2 Posted by: seaborder Posted at: 2019-08-24T20:07:24.632Z Reads: 53

```
try without belts so the motor has no "load". Iam not sure if this is still an issue but just try :)
```

---
## \#3 Posted by: Steven1 Posted at: 2019-08-24T20:54:27.961Z Reads: 44

```
Make sure to give it a good hard spin, that did it for me
```

---
## \#4 Posted by: wenyu007 Posted at: 2019-08-24T21:04:08.621Z Reads: 43

```
On the setup video made by enertion they said that the motor has to be free from everything to be properly calibrated. So take off the belts, and spin the motors by hand. See if that works.
```

---
## \#5 Posted by: SkateYS Posted at: 2019-08-24T22:25:15.314Z Reads: 38

```
Considering how close those bare phase wires are from each other, I doubt you can be sure they never shorted! Not sure why you do it that way but you did not spin the motor hard enough. If the duty cycle at which the calibration is set to occur is high, then the motor has to spin up to that level for it to register. My setup also gave me trouble with the computer software, but the phone app is the best (never tried the iOS version tho). The sensor wires are not the problem
```

---
## \#6 Posted by: achatham Posted at: 2019-08-24T23:01:58.024Z Reads: 34

```
Spinning the motors without the belts did the trick. Thanks guys. 

One other question is do you need spacers between the bearings? Reason I ask is because the wheels little stop when I’m not on the throttle. My previous build spun freely and wasn’t so abrupt in its stop and go.
```

---
## \#7 Posted by: accrobrandon Posted at: 2019-08-24T23:18:25.404Z Reads: 34

```
[quote="achatham, post:1, topic:100800"]
Only reason I cut them is because the torqueboard sensor wires on the motors did not match up with the focbox unity input
[/quote]

Dude, really!? 9/10 sensor wires from the motor dont line up to the esc. U need to add a sensor wire connector. Hopefully you saved what you cut...or left yourself some slack to solder either OE pigtail back on OR if your motors are fairly close to the esc solder on the said wire harness....this is if you want to run sensored.

 https://flipsky.net/products/flipsky-esc-sensor-wires?gclid=Cj0KCQjw9ZDeBRD9ARIsAMbAmoZUggzQnmCZwXfK9oa6tzx3vmsdhGhFfxhzGVgw9Awl7QWmUcsxI9IaAvV5EALw_wcB
```

---
## \#8 Posted by: wenyu007 Posted at: 2019-08-25T00:46:01.910Z Reads: 28

```
yea you need wire adapters, cutting them is not the play haha
```

---
## \#9 Posted by: achatham Posted at: 2019-08-25T01:01:06.438Z Reads: 27

```
Yea and to think I literally cut them today. I’ll probably have to get new motors for sensors bc I cut them so short. Live and learn
```

---
## \#10 Posted by: accrobrandon Posted at: 2019-08-25T01:23:16.105Z Reads: 26

```
Depending on your soldering skills and ability you could reattach at the motor pcb.. Or maybe u got a friend whos more crafty... Otherwise sensorless it is...
```

---
