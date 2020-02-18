# VESC FAQ &#124; Duty Cycle VS Current Control &#124; PPM settings

### Replies: 9 Views: 11351

## \#1 Posted by: onloop Posted at: 2016-02-04T02:39:19.752Z Reads: 1069

```
**Vesc PPM Control Modes**

 - Disabled: Nothing at all, motor is off. 
 - Current: Torque control. This is what Vedder prefers since it feels most natural for him. No hobby grade
   ESCs have current control. 
 - Current no reverse: Save as above but no reverse function. Note that centring the now will give half
   throttle. 
 - Current no reverse with brake: No reverse, but centre is
   zero torque. Reversing will brake, but not change motor direction.
 - Duty cycle: Duty cycle or voltage control. What most hobby ESCs use.
 - PID speed control: The throttle command is interpreted as a speed set
   command and closed-loop control is used to maintain that speed. “PID
   max ERPM” sets what max throttle should be interpreted as.

<img src='/uploads/db1493/original/2X/d/dbe11884d7695e61de4d24c4a06031740a0c0936.png'>

**What control modes are you using on your eboards?**
-----------------------------------------------------


----------


I have been using **current control no reverse**, it works fine. However, when coming to a slight hill if you don't increase your throttle position you will slow down because the load on the motor increases but you are are not increasing the current. I am curious to see how this will behave when approaching a hill with cruise control activated whilst using current control.
As I now have a remote controller that has a cruise control function i plan to try the duty cycle option to see what result is more desirable.
```

---
## \#2 Posted by: laurnts Posted at: 2016-05-12T01:16:14.967Z Reads: 853

```
Duty Cycle control the speed of the motors without taking into account the current needed to push the load. So it's a very good option in controlling speed of motor if the load is light. In steep hill climbing from eboard perspective, you will need to climb the hill at high speed due to the low speed of duty cycle also output very low amps.

Current Control does similar job to the way cars work. It control the currents flow instead of the speed. With just a slight of throttle the motor will spin at maximum rpm immediately. When load is added, the motor rpm will slow down. This allow you to steep climb hill at quite low speed as the power flow of your board is in you hand. The disadvantage of current control is if you maintain your throttle and the road suddenly goes down hill, you will accelerate. At some point it could be dangerous in dual drive motor when one wheel is loosing traction, the wheels that looses traction will spin at max rpm immediately and when it has traction again might cause a slight drift movement.
```

---
## \#3 Posted by: brakkeh Posted at: 2017-04-15T11:33:19.103Z Reads: 564

```
Is it safe to use current mode as a brake. 
So if you go forward and then put the remote in reverse, will it brake safely?

thanks
```

---
## \#4 Posted by: Alanhunt123 Posted at: 2017-04-17T14:43:30.663Z Reads: 526

```
I have only used current control with braking, and it feels very natural to me, should work fine. Good luck!
```

---
## \#6 Posted by: KrisKraanen Posted at: 2018-11-08T16:35:17.574Z Reads: 183

```
i want to accelerate and brak but then if im standing still i also want to reverse how do i do this so when im still going forward not immidiate reverse but first brake and when the throttle is centered again then i can apply reverse
```

---
## \#7 Posted by: StefanMe Posted at: 2018-11-08T16:39:52.606Z Reads: 175

```
Sounds like the ackmaniac thing...
```

---
## \#8 Posted by: KrisKraanen Posted at: 2018-11-08T16:50:46.089Z Reads: 170

```
ackmaniac?
```

---
## \#9 Posted by: Deodand Posted at: 2018-11-08T17:00:38.990Z Reads: 163

```
The described behaviour isn't implemented in vesc FW. I started implementing it on the FOCBOX Unity, but came across some behaviour questions during implementation that I still need to tackle. 

1) Say I am going forward up a hill, I pull the brake and my board comes to a stop then begins to roll backward as I'm holding the brake in. In this instance I guess the board should stay in brakes mode? 

2) Say no throttle is applied and I am moving in reverse when I pull the throttle backward does it then continue to push me in reverse? Does the forward throttle then become brake? Or is it a timeout window on the reverse functionality i.e. pull in the brake release it check if speed is 0 or reverse then switch the backward throttle to reverse mode. 

3) if you fully brake then press in the throttle into reverse a second time to enter "reverse mode"  release the reverse throttle does it switch back to brake again?  Or is it now locked into reverse mode until velocity becomes greater than 0 again (or some threshold) 

Need to investigate what feels intuitive. A non-intuitive control interface is bound to piss people off and throw them from the board potentially injuring them.
```

---
## \#10 Posted by: KrisKraanen Posted at: 2018-11-08T18:19:55.065Z Reads: 147

```
i actually want duty cycle with brak don't need reverse that bad
but on duty cycle the motor is braking all the time i only want it to break when i pull back on the trigger
```

---
