# Arduino powered controller to switch between two motors

### Replies: 11 Views: 533

## \#1 Posted by: Snowi Posted at: 2017-08-13T18:29:07.981Z Reads: 85

```
So I have two motors. I am trying to use my arduino powered controller to, in a click of a button, turn off one motor and turn on the other or use both motors at the same time. Is there any way I can do this?

This is completely experimental. I have never seen anyone do this. If you guys have, please link the thread in the comments.
```

---
## \#2 Posted by: wafflejock Posted at: 2017-08-13T18:59:59.321Z Reads: 82

```
A few threads have brought this up, basically it isn't worth it to shut one off you still have drag and the off motor is acting as a generator at that point, surprisingly using mixed kv motors both on can work though and might be worth playing with.
```

---
## \#3 Posted by: JLabs Posted at: 2017-08-13T19:07:54.955Z Reads: 78

```
I wonder if there is any way to just have one motor drive and have the other regen power and only use it for braking (this 'mode' would only be used when lightly cruising, but when you need to climb hills you can switch the second motor back on).
```

---
## \#4 Posted by: Der6FingerJo Posted at: 2017-08-13T19:33:30.974Z Reads: 73

```
If you use ppm control for your ESC you could just set up 3 modes:
1: Send ppm out of both arduino pins you set up for the motor outputs
2: send ppm out of only one pin and set the other to neutral
3: send full ppm out of one output and only pwm under 1500 for braking out of the other output pin
```

---
## \#5 Posted by: Snowi Posted at: 2017-08-15T03:31:51.497Z Reads: 51

```
@wafflejock @JLabs the second motor acting as a generator would be interesting... i'll prob develop that once I get my skateboard to run.

@Der6FingerJo what is ppm? i see it around the forums, but couldnt find what exactly it is.
```

---
## \#6 Posted by: Der6FingerJo Posted at: 2017-08-15T05:02:21.353Z Reads: 41

```
It's the signal you use to control the VESC and goes to the white cable coming out of it. You can generate it with the service library of the Arduino 
But I'd suggest you read up on the theory of the VESC before programming your own control :slight_smile:
```

---
## \#7 Posted by: pennyboard Posted at: 2017-08-15T06:52:15.884Z Reads: 36

```
[quote="Der6FingerJo, post:4, topic:30508, full:true"]
If you use ppm control for your ESC you could just set up 3 modes:
1: Send ppm out of both arduino pins you set up for the motor outputs
2: send ppm out of only one pin and set the other to neutral
3: send full ppm out of one output and only pwm under 1500 for braking out of the other output pin
[/quote]


I think this is the best way to do this sort of thing. If your controller has a spare switch on it (as in a second channel, like on the winning nano), wire the white wire of that channel into the read-in of an arduino. Then wire each ppm to a transistor, like this one, http://uk.rs-online.com/web/p/bipolar-transistors/4859749/, and have an analog read pin from the arduino control each transistor. Then program the arduino to shut one motor off when the channel 2 it's reading in is activated, and turn that motor back on when the channel 2 is off. It takes some learning on the arduino and coding to do this but it shouldn't be too difficult.
```

---
## \#8 Posted by: Der6FingerJo Posted at: 2017-08-15T07:16:34.309Z Reads: 31

```
Actually when you use the servo lib you could just set up 2 VESC outputs on your pwm pins, so you could do all the switching on the software side of things. Going neutral(1500us) sounds better to me when you don't want to  use the motor than fully cutting the signal. This way you can still have failsafe in the VESC itself and possibly switch control faster, I don't know how fast the VESC detects the pwm signal after it has been completely cut. 
The Transistor idea would work with 2 anti spark switches to fully disconnect one VESC from the drivetrain, however if the motor of that VESC spins and generates current it could potentially damage the hardware.
```

---
## \#9 Posted by: pennyboard Posted at: 2017-08-15T07:21:41.733Z Reads: 30

```
How would you do the switching on the software side of things without input for the remote though? I'm assuming the remote has only 1 channel that can be used for user input and that channel is either on or off. It could be different for different remotes though.
Cutting off the vesc from the ppm would be the same as going neutral though. It'd be equivalent to just turning off your controller, and leaving the vesc on, so the motor spins freely (relatively speaking, as it is still going to see mechanical resistance to turning from the belt). That would leave the vesc on and so any back emf would just be regenerated into the battery from that vesc
```

---
## \#10 Posted by: Der6FingerJo Posted at: 2017-08-15T10:47:45.208Z Reads: 25

```
With only one spare channel you would probably have to set up cycling between the riding modes or play around with tapping and holding the button to go back and forth. 
When you physically disconnect the ppm from the VESC you would have to disable it's built in failsafe of setting a predetermined brake of the signal should fade. If you keep the signal connected and switch it to neutral though, you can keep the failsafe functionality. And it would be simpler than using the transistors.
```

---
## \#11 Posted by: pennyboard Posted at: 2017-08-15T14:12:10.517Z Reads: 22

```
Yeah I suppose you should do that, it may be difficult to know which mode you're on if you're just flipping a switch. I think the best option is to do a Gt2b mod like I've seen a few times on here, which a screen or leds to indicate which mode you're in, since that controller comes with more than one spare channel I think. 

There's a way to program the VESC to go into neutral if it loses the ppm signal, I know I have mine set up that way. I just think generating the ppm signal through an arduino seems like it might affect the responsiveness of the remote
```

---
