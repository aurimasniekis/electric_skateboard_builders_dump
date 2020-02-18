# Help me fix my board (please) :)

### Replies: 9 Views: 653

## \#1 Posted by: michichopf Posted at: 2017-04-23T12:28:25.712Z Reads: 99

```
Hey guys. 

Thank you for even reading this, so not to waste more of your time I shall be summary and as precise as possible.

- Board:             Standard Raptor 1.0 Dual drive
- Problem(s):      Sudden loss of motors, 1 spinning slowly only other one dead.
- Found/fixed:     I opened the board and felt a cable was mooving a little too freely,took shrink tube off, saw disconnected wire from vesc. Resoldere it, hope in a functional matter.
- Still not working
- Hooked up to the BLDC tool. checked for error'rs. None found.
- Tried motor detection, motor detection failed (read a bout the r-spec shorting out often, next step taking motor aapart.)

- Pictures : <img src="/uploads/db1493/original/3X/f/a/fa47206026fea3b02e6974aba38ce0c779578584.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/b/e/beeb7732176e536479d0fa1bcf81277b4f699ff4.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/6/4/64882d4b964291fc2742a053c35d838216a619b3.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/d/f/df36db491cf32f7962e4b8dde6e99538f2001e1a.jpg" width="690" height="388">


I believe it to be the motor, since I toock it donwhill a lot, and therefore exeeding the speed I was supposed to on this set up I think. Still If I dont engage the trottel the motor produces current (right?). I mean board goes 40ish and I went 50-60 regularely. If somone has a different Idea, it would be very welcome. Also, will I allways have the risk of blowing my ride, when I go donwhilling with it ?
```

---
## \#2 Posted by: laurnts Posted at: 2017-04-23T17:19:32.057Z Reads: 68

```
The motor in esk8 is most of the time the most reliable things you have. If it went down hard, more or less both motor should have been destroyed at the same time on the same hill.

If you connect bldc tool to each vesc separately and be able to run motor detection for both motor, than your vesc and your motor is ok. Since you stated no vesc error, I assume the vesc are fine.

Hence I really think you have CAN Bus issue. Either the cable unplugged or the connection is not properly connected.
```

---
## \#3 Posted by: michichopf Posted at: 2017-04-23T17:44:26.186Z Reads: 63

```
Yeah. Thought the same at first, but learned in discussion with others that my daily downhill may have fried the motor.
Also I never toock care of the wiring of the r-specc since its prone for damaging itself. Will try thaz. So unplugg canbus and connext every vesc seperately. If motor detection works I guess I know what to fix.
Thx for the help ;)
```

---
## \#4 Posted by: Guacamoleface Posted at: 2017-04-23T19:37:00.085Z Reads: 50

```
Watch out so your motor wires dont connect with eachother(since not fully isolated on the picture), think thats the reason many people burn their DRV's on the vesc!

Did you also check the bldc tool while you were trying to run the motors or did you just power it on?(looking at your picture of the Bldc tool I guess you did)
```

---
## \#5 Posted by: michichopf Posted at: 2017-04-23T19:50:13.873Z Reads: 47

```
you mean the cables soldere to the vesc ? So i should isolate them from eatch other ?

and how do you mean check the BLDC tool ? I am not sure I am following. 

And After taking the motors almost apart, there is so much more resistance on the one with the missing shrink tube. But can only commence tomorrow, I need pliers to take the rings off. 40 minutes of pure anger is neough for today :)
```

---
## \#6 Posted by: Guacamoleface Posted at: 2017-04-23T20:03:34.377Z Reads: 45

```
Nah what i refer to is your cables where the connect between the vesc and the motor, the connectors is exposed - if they touch eachother while power on they might fry your DRV on the vesc.(I always electrical tape them even on temporary connections to check stuff to make sure they dont short out eachother)

And Im pretty sure you did, just me missing that picture but I'll explain anyway.

When the board was hooked up to computer and bldc, did you check your active sampling during(or after) you tried to throttle your motors before turning it off? 
You can either look at the sampling(if fault code goes from NONE to something while using the motors), or type faults(I think) in terminal afterwards.

Im pretty new to this myself but when I got drv error it wouldnt show until I actually throttled my motor.
```

---
## \#7 Posted by: Eboosted Posted at: 2017-04-23T20:11:32.458Z Reads: 42

```
I had that exact problem with both of my builds. 

It happens when one hall sensor doesn't have a good connection or the connection is loose/broken. This cause one motor to spin up slowly and the other to not spin at all. 

Once you connect the bad wire, both motors will spin perfect again. 

If your motor sensors are in hybrid mode on BLDC tool, then you could test my theory by going downhill or push hard and trying to speed up with the remote as sensors only work very low speed.
```

---
## \#8 Posted by: michichopf Posted at: 2017-04-23T20:19:51.046Z Reads: 43

```
well I was under the pressure that my motors are not sensored. I could be wrong.

And @Guacamoleface I actually didnt use the throtel while hoocked up. My bad :( Will try that as soon as my motorsa are back together. Though I am fairly certain that something is wrong with them, the noise and the resitance donßt sound too good.
```

---
## \#9 Posted by: laurnts Posted at: 2017-04-23T20:49:39.947Z Reads: 36

```
Rspec from enertion is not sensored. So hybrid mode is off the hook from testing.
```

---
