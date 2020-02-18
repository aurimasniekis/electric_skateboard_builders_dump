# Controller Opinions

### Replies: 10 Views: 1191

## \#1 Posted by: brandon Posted at: 2016-10-06T15:04:40.495Z Reads: 144

```
So, I'm a cheap ass, and I would much rather design my own transmitter and receiver than drop $50+ on something I can make for pennies (and time, which I have more of then dollars). I plan on 3d printing the housing, and releasing a custom board schematic, as well as inclusding a housing that will work with off the shelf parts, and possibly doing a small run manufacture (read: maybe just a few dozen, I don't have my own printer so the run would be small).

I have only touched the gt2b, but I have looked at every controller on the market. My personal opinion is that a wii nunchuck shaped controller (with the joystick limited to only one axis movement) and the two buttons on the front functioning as a cruise control and a second channel for whatever you want is a solid mechanical plan. As for electronics, 2.4ghz seems like hands down the best solution. Maybe also include a couple pots for adjusting sensitivity of the throttle and brake (though, since I will be writing the firmware, I can create custom curves for these anyways). 

Anyways, I haven't actually finished my board, so I don't have the experience of many of you. I was just hoping to gather any input I can get on design preferences since this is something I would like to provide to the community as a low cost alternative to commercial controllers.
```

---
## \#2 Posted by: Hillso Posted at: 2016-10-06T23:29:48.341Z Reads: 107

```
bluetooth modules are very cheap, but I heard people have problems with bluetooth.
there is got to be a way to make a robust bluetooth controller, because boostedboards remote is bluetooth.
```

---
## \#3 Posted by: brandon Posted at: 2016-10-06T23:42:00.041Z Reads: 101

```
A Bluetooth controller would be no harder than 2.4ghz, but 2.4ghz uses less power, and since I would like the controller to be very small, I think it's the better option.
```

---
## \#4 Posted by: boards Posted at: 2016-10-06T23:53:57.954Z Reads: 98

```
I made a custom remote with a small oled display. I recommend using nrf24s as the new VESC will have one built in.
```

---
## \#5 Posted by: SteveS Posted at: 2016-10-07T00:49:53.529Z Reads: 86

```
I think Boosted has a bad reputation for drops. I experienced a number of them during the 4 weeks I owned one.
```

---
## \#6 Posted by: baxter Posted at: 2016-10-07T13:28:04.485Z Reads: 68

```
For inspiration:

http://www.electric-skateboard.builders/t/contest-nicest-remote-most-wins-ended/9219/
```

---
## \#7 Posted by: baxter Posted at: 2016-10-07T14:23:32.423Z Reads: 63

```
My vote is for @DougM's tubie remote.  Looks like a couple of strategically designed 3d printed plugs at either end of the clear pipe would finish off his design.

Plus, I think there could be more alternatives when it comes to thumb style remotes (as opposed to trigger style).
```

---
## \#8 Posted by: DougM Posted at: 2016-10-08T16:11:44.256Z Reads: 48

```
Thanks @baxter :slight_smile:

If you do use my design don't put the power button next to the enable/disable button - it confuses people.  On the next rev I will have a slider or rocker as a power switch and it will be inset and on the side.

Other than that it's been a great remote.  But it's not for the budget-minded - both the transmitter and receiver board uses XBee, which is rock solid (no BT for me) but it is expensive.  It also has a Teensy 3.2 and an Adafruit 9DOF sensor in it.
```

---
## \#9 Posted by: brandon Posted at: 2016-10-08T16:23:37.930Z Reads: 45

```
I'm having trouble understanding how it works, although @baxter is right, it looks GREAT. Is that button on the top a spring loaded slide pot? How do you apply breaks if you can't pull it up?
```

---
## \#10 Posted by: DougM Posted at: 2016-10-08T17:02:11.687Z Reads: 42

```
It's a tilt-pitch-roll sensor.  The blue button is power, the red button is enable/disable.  Power it up, hold it parallel to the ground, hit the enable button.  Tilt up = go fast; tilt down = brake.

What I found works best is to power it up, push the board until you're moving, tilt it down a little bit and hit the enable button, then you can feel the motor and a little bit of brake engage, then tilt it up and go fast.
```

---
