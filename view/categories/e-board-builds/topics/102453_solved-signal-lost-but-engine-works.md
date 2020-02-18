# \[Solved\] Signal lost but engine works

### Replies: 7 Views: 170

## \#1 Posted by: anikulin Posted at: 2019-10-02T09:19:42.764Z Reads: 55

```
Hi guys.
I need your advice because really can’t understand what happens.

The expected behavior is: IF signal from transmitter is lost Then ESC must stop the engine.
But in my case it vise versa:  IF signal from transmitter is lost Then ESC starts send power to the engine (please watch video: [Youtube video of wrong behavior](https://youtu.be/lLRN8BM6EIA)).

I thought that problem in the cheap noname ESC from AliExpress ([link here](https://www.aliexpress.com/item/32679463006.html))
But I bought HobbyKing (X-Car Beast Series ESC 1:8 Scale) and behavior the same.

Anybody know why does it happen and how to solve it ? May be problem in the receiver? When the receiver loses a signal, it’s sending some incorrect instructions to the ESC.
```

---
## \#2 Posted by: linsus Posted at: 2019-10-02T10:09:23.182Z Reads: 48

```
[quote="anikulin, post:1, topic:102453"]
engine
[/quote]

is it a 2 or 4 stroke machine? Did you try fill it up on gas? Are the sparkplugs alright? (if its electric its a motor)

Not familiar with those escs, pro tip; buy a vesc

have no idea what remotes u using but normally you have to bind it with the binding loop on the reciever in order to fix the full throttle at disconnect problem. Guessing its a PPM(PWM) remote.
```

---
## \#3 Posted by: anikulin Posted at: 2019-10-02T10:15:20.077Z Reads: 42

```
I'm using this engine "Turnigy Aerodrive SK3 - 6374-192KV Brushless Outrunner Motor"
But in video I'm using noname from Aliexpress. Behavior the same. I don't think that it's engine issue
```

---
## \#4 Posted by: linsus Posted at: 2019-10-02T10:51:24.268Z Reads: 43

```
:see_no_evil:

[quote="anikulin, post:3, topic:102453"]
Turnigy Aerodrive SK3 - 6374-192KV Brushless Outrunner **Motor**
[/quote]

its a motor.. stop the engine talk.

has nothing to do with esc or motor, reciever and remote is the problem.
```

---
## \#5 Posted by: Komamtb Posted at: 2019-10-02T11:58:55.132Z Reads: 39

```
failsafe feature maybe?
```

---
## \#6 Posted by: anikulin Posted at: 2019-10-02T12:15:03.235Z Reads: 35

```
Yes, looks so. I don't see it in my receiver - transmitter.
```

---
## \#7 Posted by: anikulin Posted at: 2019-10-11T07:14:12.966Z Reads: 13

```
OK, guys. The problem solved by rebinding transmitter by this algorithm. It works without standalone fail safe function.
https://www.electric-skateboard.builders/t/solved-board-accelerates-when-signal-is-lost/7588/2

First the remote comes already bind to the receiver, but in some instances the binding process need to be repeated, this is because of the fail safe feature of the receiver that needs to be calibrated. This manifest itself in this situation:

With the board On, if you turn Off the remote, the motors will start spinning without input. This is because the receiver needs to record the NEUTRAL position (mid throttle ) of the remote.

The Binding procedure is as follow:

1).Check and make sure all the wires are connected and that the REMOTE is OFF,insert the bind plug into CH3(Bind) on the RECEIVER.

2).With the REMOTE OFF. Switch on the ESC, to power up the RECEIVER, red LED light will flash.

3).PRESS and HOLD the bind button on the REMOTE and then turn the REMOTE ON.

4).You should notice the REMOTE and RECEIVER LED light go from flashing red to solid red.

5).Once you see a solid red light, the binding process is complete, Then without turning the REMOTE OFF or touching the THROTTLE pull the bind plug out (for the receiver to record the throttle mid point, neutral, to engage the fail safe)

6).Then you can test it again by turning OFF the REMOTE and the RECEIVER LED should flash. By turning the REMOTE ON the RECEIVER LED should go back to solid red.

Before RIDING ,it’s better to test the fail safe function in the RECEIVER ,if the motor didn’t move,so the fail safe function is in good working condition, if the motor is moving,you have to repeat the step No.1- No.6 above"
```

---
