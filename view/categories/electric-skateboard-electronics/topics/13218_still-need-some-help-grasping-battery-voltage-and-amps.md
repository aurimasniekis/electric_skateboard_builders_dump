# Still need some help grasping battery voltage and amps

### Replies: 5 Views: 814

## \#1 Posted by: thefoolio Posted at: 2016-11-17T04:47:20.314Z Reads: 85

```
First of all, I love DIY projects and i'm good at the mechanical side of things but this battery thing has got me kinda stuck. I read the sticky on batteries and from what I can gather is that voltage is muscle/power which would allow for more torque and amps is energy/stamina and it allows the e-board to run longer before needing to charge. I bought [this](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html) motor that says it has a voltage of 10s lipoly, which I assume means I can use up to a 10s lipo battery. It also indicates that it has a max load of 65A and this is the part i'm a little stuck on. I figure that 65A is 65 amps max and I wouldn't want the motor to be running at max load at all. So if I were to have a 6s 45C x 4.5Ah battery which is 202.5Ah capacity and I use 20Ah continuously just cruising I should in theory get about 100 mins (1hour and 40mins) of run time? and if I want to get more time would I connect two of them in parallel to increase the capacity? I also ran a esk8 calc and got [this](http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":6,"motor-kv":190,"system-efficiency":80,"motor-pulley-teeth":13,"wheel-pulley-teeth":36,"wheel-size":83}|).

I think I confused myself again, thanks in advance for any input.
```

---
## \#2 Posted by: FredSaberhagen Posted at: 2016-11-17T05:18:59.812Z Reads: 79

```
I think you learned your math from the same place as those chinese kickstarters.  Pop some Adderall and let's get ino it!  This shit is confusing.  

Where you wrote 202 Ah I think you mean watt hours.  You want to know how much ENERGY you have (for example a Joule is a watt-second)  Divide by watts spent to get time capability.

Also watt hours = voltage * amp hours.  45C just means you can pull max 45 * battery capacity  (in this case 4.5ah) so you could pull around 200A from the pack (good luck with that -disregard C rating - 200A will melt your wires, your esc, and your face like that guy in the indy Jones movie that didn't close his eyes)

Actual watt hour calc would be voltage (6S = 6*3.7V or 22V) * capacity ( 4.5Ah ) = closer to 100Ah ... I mean watt hours lol.

So 100 watt hours you're burning 20amps cruising, OK how much POWER - it would 22.2V * 20A = say 400W cruising.  100wh / 400W means you have about 1/4 hr or 15 min. 

Gonna be the most fun 15 minutes you have all day. At 20 MPh you'll have 4 or 5 Mile range.
```

---
## \#3 Posted by: NickTheDude Posted at: 2016-11-17T05:24:20.776Z Reads: 73

```
Alright, so first and foremost, your motors need to output power in order to push the deck and yourself. Power is measured in Watts, and W = V * A.

To measure capacity, we use watt hours. A single watt hour is enough to sustain a full watt for a full hour. Wh = Ah * V. A general assumption is that 10Wh will give you 1km of range.

So in your 6S 4.5Ah battery you have 22.2 * 4.5 = 99.9 watt hours, and therefor roughly 10km of range.
```

---
## \#4 Posted by: thefoolio Posted at: 2016-11-17T05:45:23.794Z Reads: 65

```
I've seen you edit your reply about 3 times now and I'm cracking up. First I really appreciate the help. I'll make sure to close my eyes so my face doesn't melt or I can cap it with a vesc (I believe). I was honestly only thinking in amps/milliamps but now with the watts i completely understand. I've always been good at building stuff but I've never added electronics to a build. thanks again for the help.
```

---
## \#5 Posted by: thefoolio Posted at: 2016-11-17T05:47:41.429Z Reads: 58

```
Thanks for the reply. I didn't realize I could measure it in watts. This helps me understand it now.
```

---
