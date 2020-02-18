# Benefits of sensored BLDC?

### Replies: 11 Views: 332

## \#1 Posted by: Jake2k17 Posted at: 2018-11-07T01:43:46.868Z Reads: 109

```
As the title states, is there any benefit to this? I have dual Torqueboards VESC and I don’t want to use FOC with them, would sensored bldc be any better that bldc without sensors?
```

---
## \#2 Posted by: b264 Posted at: 2018-11-07T01:48:11.043Z Reads: 108

```
You can start without kick-pushing.  It's also one more thing that can fail.  It's your choice, pick your poison
```

---
## \#3 Posted by: Jinra Posted at: 2018-11-07T01:55:41.126Z Reads: 101

```
Anything can fail, but more often that not it's because of shoddy craftsmanship
```

---
## \#4 Posted by: Jake2k17 Posted at: 2018-11-07T01:58:30.591Z Reads: 97

```
I can start without kick pushing without sensor wires already...
```

---
## \#5 Posted by: Jinra Posted at: 2018-11-07T01:59:42.069Z Reads: 95

```
Then don't worry about it, but when you find yourself cogging you'll know why
```

---
## \#6 Posted by: xilw3r Posted at: 2018-11-07T06:24:09.547Z Reads: 74

```
I read multiple times how shitty sensor wires shorted and killed the DRV. So as @Jinra says, craftsmanship is key. Especially if you want to try and install them yourself.

My board is so heavy and with such shitty bearings that cogging is really the last thing i would notice :D
```

---
## \#7 Posted by: Andy87 Posted at: 2018-11-07T06:28:19.633Z Reads: 74

```
sealing the sensors is easy and cheap to do and would solve the problem of shorting.
```

---
## \#8 Posted by: Jake2k17 Posted at: 2018-11-07T16:13:36.841Z Reads: 57

```
Ok that makes sense, I’m using bkb motors, which are sealed. Is there any set up I need to do with the sensors or can I just plug them in?
```

---
## \#9 Posted by: Andy87 Posted at: 2018-11-07T16:41:51.711Z Reads: 53

```
When you go through the motor wizard you need to choose hall sensors and do a detection run
That’s all.
Which esc you have?
If you have a escape you need to change the sensor wire order. 
With focbox or Flipsky you can just plug them how they are.
I don’t have bkb motors, so if they like maytechs you need an adapter from 1.5 to 2mm jst
```

---
## \#10 Posted by: Jake2k17 Posted at: 2018-11-07T16:45:19.681Z Reads: 52

```
I have dual TB Vesc, and I have TB sensor adapters which fit
```

---
## \#11 Posted by: C23 Posted at: 2018-11-07T17:40:08.308Z Reads: 42

```
I would not use a sensored setup.  This is because the sensor wires on the TorqueBoards motors break really easily.  The braided sleeve on my got a tear in just a few hours of riding.  Of of course the wires are still fine, but I would just recommend against it.  It is just something else to fail.  Plus, the circuitry for the sensors is in the back of the motor, and it could get wet and malfunction.  Uncensored works really well with vesc.  Yes, for the first .5 km/h there may be some pulsating, but at hardly any speed at all, the motor gives the vesc enough feedback for it to operate really smoothly, depending on your gear ratios.  And, even if you don't want to give it a little push with your foot, just use full throttle at first, it isn't that jerky.  But who am I to say either way; the sensored setups do feel really smooth.  If you were to let someone else try your board, they would probably appreciate the sensors.
```

---
