# R-Spec Motor Repair/solder joint testing

### Replies: 17 Views: 1579

## \#1 Posted by: Fababuba Posted at: 2016-04-27T15:31:05.138Z Reads: 96

```
I bought a r-spec 6355 a while back and completed my board recently. After about a 5 mile test run it stopped spinning. I thought one of my bullet connectors might have come loose as my vesc seems to be fine. The motor neither spins nor makes any noises when I press the throttle, any ideas? I was thinking I had a bad solder joint either on the vesc or motor but even so it should still be touching under the heat shrink, right?
```

---
## \#2 Posted by: treenutter Posted at: 2016-04-27T15:50:03.553Z Reads: 93

```
@Fababuba [quote="Fababuba, post:1, topic:2658"]
it should still be touching under the heat shrink, right?
[/quote]

nope, a bad join can disconnect even if the heat shrink is intact. In this case pics of the relevant parts of your build would help everyone on the forum to answer your question.

Possible issues: motor connectors disconnected, bad solder joint somewhere, controller's receiver disconnected, controller's battery dead, battery disconnection, vesc threshold exceeded (temp, voltage).
```

---
## \#3 Posted by: Hummie Posted at: 2016-04-27T16:41:16.171Z Reads: 89

```
There are so many ways to make ur board not go.   Do u have a multimeter?  That'll clear up the simpler problems
```

---
## \#4 Posted by: Fababuba Posted at: 2016-04-27T18:40:36.278Z Reads: 80

```
Ill post pics of my setup when I get home and I have a multimeter but I'm not too sure how to test the motor and vesc with it.
```

---
## \#5 Posted by: Fababuba Posted at: 2016-04-28T02:35:09.717Z Reads: 69

```
<img src="/uploads/db1493/original/2X/a/aa423e921f63e9093090186c7cc44131713cceee.jpg" width="689" height="390"><img src="/uploads/db1493/original/2X/b/b407179be94d0ac046e42296cf6bae8a8c6af69c.jpg" width="689" height="390">
I had each motor wire individually wrapped in electrical tape and heat shrink, just took it off to make sure the solder joints were still connected. Under the white pvc cover is a space cell.
 
https://drive.google.com/file/d/0Bw8ImCZYazEZWGtkSXFhRjhuRzA/view?usp=sharing -test video/ the vesc responds to the transmitter but the motor is completely unresponsive.
```

---
## \#6 Posted by: treenutter Posted at: 2016-04-28T02:44:13.771Z Reads: 66

```
@Fababuba did you modify any of the settings in bldc tool? Is it possible that you disabled the controller app? On the PPM tab make sure that you've chosen on of the non-disables options. Also check that you've chosen PPM in the general tab.
```

---
## \#7 Posted by: Fababuba Posted at: 2016-04-28T02:52:39.295Z Reads: 66

```
Yup I checked all of that a PPM, current no reverse with brake, the plusewidth display also works. Everything was working fine for a good 2 miles until suddenly it stopped responding. I live in Chicago so everything is pretty flat and i'm pretty sure i never even got full throttle so I don't think I overloaded it.
```

---
## \#8 Posted by: treenutter Posted at: 2016-04-28T03:27:44.641Z Reads: 63

```
@Fababuba Have you checked the soldering of the motor wires on the VESC, under the heathshrink?
```

---
## \#9 Posted by: Fababuba Posted at: 2016-04-28T22:45:55.003Z Reads: 58

```
@treenutter Yes, it's not the best soldering job but all 3 wires are connected.
```

---
## \#10 Posted by: chaka Posted at: 2016-04-28T22:53:13.327Z Reads: 59

```
I see this all the time! Uninsulated phase connectors :fearful: 

Mind your connections guys!

Edit: just read that you removed it for the photos but it looks like it is powered up?
```

---
## \#11 Posted by: Fababuba Posted at: 2016-04-28T23:27:56.906Z Reads: 55

```
@chaka Its powered up but I made sure the connectors never touched. Do you know how to test if I shorted out the motor or if its something else?
```

---
## \#12 Posted by: chaka Posted at: 2016-04-28T23:57:50.214Z Reads: 56

```
Do you get 3 red flashes from the vesc when you try to run the motors? If you do then you have a drv8302 fault.
```

---
## \#13 Posted by: Fababuba Posted at: 2016-04-29T02:39:35.694Z Reads: 51

```
Nope, no red flashes at all.
```

---
## \#14 Posted by: Fababuba Posted at: 2016-04-30T15:26:16.999Z Reads: 49

```
@Hummie Can you briefly explain how to test the motor and Vesc with the multimeter? Is there a way to test if the Vesc is actually delivering power to the motor?
```

---
## \#15 Posted by: Hummie Posted at: 2016-04-30T15:35:29.334Z Reads: 48

```
I don't know much and others here would likey be a better help but did you try the motor testing on a pc since this happened?  Id try that first.  If nothing there then put ur multimeter up to the three phase wires (each possible combo of two wires) and see what u get.   I'd think the motor would at least stutter if it was damaged.  I'd be strange for the motor to completely die like that.
```

---
## \#16 Posted by: Fababuba Posted at: 2016-05-01T00:47:47.843Z Reads: 46

```
Pretty sure at this point I've tried just about everything it and I can't get it to work. Neither the vesc nor the motor show any signs of damage. 

Edit: I actually found a single charred wire in the motor windings. 

@onloop Do you have any ideas about troubleshooting it? Can I get a warranty? Even though its been over 60 days it has less than 5 miles on it.
```

---
## \#17 Posted by: Fababuba Posted at: 2016-05-01T21:09:41.388Z Reads: 38

```
After some more testing the motor might actually be fine. Even though the Vesc seems to be working properly it shows no output current when I use the multimeter. It' not my solder joints as I tested the Vesc board itself. Any one have any ideas about what might have caused a vesc to just stop working?
```

---
