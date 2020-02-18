# Some beginner questions about VESC and Motors

### Replies: 3 Views: 495

## \#1 Posted by: jet Posted at: 2017-05-29T17:12:05.055Z Reads: 88

```
Hi guys, I'm new here and am just doing some research at the moment, but these are a few things that I've not been able to figure out yet.

I believe that I've read about some people using 2x VESC, why would you need more than 1? Do you need 1 for each motor if you are running 2 motors? How do you program them if you're using more than 1, do you have to program them separately, are they able to communicate with each other to share controls? What about the crazy people using 4 motors, do they have to use 4 VESC's?

Do VESC's work the same with both geared and hub motors?

What do the numbers mean on geared motors such as 6374-170 and 5065-270?

I've seen some bigger geared motors that extend past the halfway point of the trucks, obviously you can't run two of these together on the same side of the board, the 2x geared motor builds use 2x smaller motors. What's the difference? is 1 big motor more powerful than 2 smaller motors?
```

---
## \#2 Posted by: wmj259 Posted at: 2017-05-29T17:21:02.607Z Reads: 88

```
You got it right, you.  Need a Vesc for each motor.  For those crazy people that have 4 motors, yes they have 4 Vescs. 

To use two Vescs you can get a splitter cable called a CANbus cable. You plug the receiver , Rx, into one vesc and link the two Vescs using the CANbus cable. When programming there is an option for using more than one Vesc in the software. 
To use more than two Vescs gets a little complicated, as you need more CANbus cables and splitters.

For motors. 
The first pair of numbers you see, are the approximate size of the motor can, the cylinder, I suppose. Sometimes instead they are the size of the magnetic stator inside  so it can vary. 
The second pair of numbers, (usually three digits in most esk8 cases),  is the Kv rating. Lower the number means more torque, higher the number means more speed.
When you see people with two motors it's usually a smaller pair 6350-6360s, if they are on the common caliber Trucks. If they are on MTB trucks then they can use the bigger full sized motors, 6374
```

---
## \#3 Posted by: jet Posted at: 2017-05-29T17:29:02.609Z Reads: 80

```
Thank you for the help :D
```

---
