# Nyko Kama Nunchuck remote Connection Drops Solution

### Replies: 1 Views: 357

## \#1 Posted by: OleksiiF Posted at: 2017-08-23T21:16:48.039Z Reads: 76

```
Hi everyone

About a month ago i broke my GT2B
and after, i started using my Nyko Kama Nunchuck purchased much earlier

And i have some thoughts to share with you, but they may not be 100%  correct, remember it pls

 A lot of riders don't use Nyko Kama due to signal drops. But! I have reasons to think that remote loses connection much less times, than he acts like he loses. Ill explain. I made dozens of experiments and observations of communication between nunchuck(remote)  and receiver.

I think that when remote changes some in-remote parameters, remote send signals to receiver, receiver sends signal to vesc, and vesc doing his job. everything is alright.
But if remote doesn't  changes any in-remote parameters, remote doesn't send any signals to receiver, than,  after 4 seconds, vesc gives no current (0 amps) to motor (and rider thinks connection is dropped)

If you press "C" button, remote and receiver communicating with each other without stopping as long as you hold it.

If accelerometer constantly measures acceleration forces changes(nuncuhck speed ≠ constant), remote and receiver communicating with each other constantly, and everything is alright(vesc gives current to motor).

But! if you move joystick forward too full throttle, remote sends some signals to receiver  to give max amps  on motor, and thats it, no more "throttle" signals! you still hold full throttle. but remote doesn't send anything to receiver. Only accelerometer does. and when you hit max speed And your remote in hand doesn't have any acceleration forces changes(nuncuhck speed = constant), it have no signals to send to receiver. Vesc thinks there is no reason to give any current to motor, it cuts off power, rider experience sudden speed lovering, shakes his hand with nunchuck, trying to stay on esk8, nunchuck (reciever) catches some acceleration forces changes and sends it to receiver, (you still give full throttle), and vesc give you immediate max current on motor. Esk8 changes its speed to fast in short period of time, and rider could fall. and he thinks he has connection problems, but he is not!

if you change settings in BLDC tool in general tub, timeout from 1000 to 3000, than after reaching to top speed, you'll have 7 seconds (3timeout+4recieverConnectionConstantTime) before esk8 starts to messing with current and speed. But when you really lose connection, esk8 will be for 3 seconds uncontrollable, so its not a solution, leave timeout set to 1000

so, what can we do? we probably can not change the way receiver and remote communicating with each other.
we can constantly shake our remote on max speed(well...)
or, maybe anything else? does someone have any ideas?  

Nyko Kama is great remote, and if we could solve this problem, well everybody wins
```

---
