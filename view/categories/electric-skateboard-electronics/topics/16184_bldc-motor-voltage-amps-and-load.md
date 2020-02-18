# Bldc motor voltage, amps and load

### Replies: 18 Views: 3906

## \#1 Posted by: aethyr Posted at: 2017-01-16T18:29:20.061Z Reads: 139

```
Hi,

I've just upgraded my son's e-scooter to a bldc motor setup. Here are my components:

sk3 149kv motor, torqueboards esc, 6s lipo battery, Sprocket gearing ratio 1:3.63

The scooter ran, a bit roughly here and there (throttle mapping issues from the hall effect voltage to servo pwm signal arduino controller I built) but it ran for multiple short runs.

But since I had originally intended this scooter to be 12s (48v), after successful runs at 6s, I added another 6s in series to get to 12s. The motor fried up within a few seconds.

My question is this: Does a motor pull the same amps at a given load regardless of voltage? So at 6S if it was pulling 60 amps at a given load, will it pull 60 amps at 48v too? Or does a motor behave as watts vs load? I guess it seems strange to me that at 48V the motor nearly instantly burned up when at 24V the scooter ran ok, albeit a bit hot.
```

---
## \#2 Posted by: DeathCookies Posted at: 2017-01-16T18:47:29.825Z Reads: 131

```
The higher the voltage the less the amperage! So on 12S it would draw less current than on 6S. Less current means that it wont get as hot as on 6S too.

Strange that it burned out because my SK3 149KV motor is just running fine on 12S
```

---
## \#3 Posted by: Hummie Posted at: 2017-01-16T18:49:10.408Z Reads: 130

```
the motor sees it all as amps.  there's no free rides on voltage.  but with higher voltage there will be more amp flow.   Also moving the no-load speed further (double) the distance, makes the motor more inefficient at lower speeds
```

---
## \#4 Posted by: aethyr Posted at: 2017-01-16T19:00:48.380Z Reads: 121

```
I'm confused. DeathCookies is saying that amps should decrease, aka its watts vs load. But Hummie, are you saying with higher voltage, amps will _increase_?

There was definitely something more going through however. The 3 motor wires from the esc were all melted as well, so I don't think it was faulty motor per se.
```

---
## \#5 Posted by: Hummie Posted at: 2017-01-16T19:08:22.568Z Reads: 115

```
please find the answer and tell us!  it's a reoccurring question.

ill add this to the confusion.  losses in the esc with higher voltages and I've read there's similar losses in the motor as well.  don't know the details and am curious.

https://www.rcgroups.com/forums/showthread.php?2046097-DJI-Propulsion-System-for-Multirotor-***Developer-and-Owner-Thread*****/page249#post30680333
```

---
## \#6 Posted by: Ackmaniac Posted at: 2017-01-16T20:39:45.062Z Reads: 104

```
That really depends on what the torgueboard Esc is controlling. PID, duty cycle, current. 
But the best guess is that you run it now with double the power and that the motor was not made for that and melted or fried or whatever you want to call it.
```

---
## \#7 Posted by: IDVert3X Posted at: 2017-01-16T20:46:21.162Z Reads: 105

```
For the same motor, higher voltage equals to higher current. Thats why we use high-kv motors on lower voltage and low-kv motors on higher voltage. Low-kv motor requieres more voltage for the same RPM, but draws less current. High KV motors requieres less voltage for the same RPM, but draws much more current. KV depends on winding thickness.

Also, the higher the load, the higher the amps for the same RPM.

Hope this explains it.

And one more thing, motor is inductive load, not resistive, just keep that in mind while doing the math.
```

---
## \#8 Posted by: Hummie Posted at: 2017-01-16T21:00:38.501Z Reads: 98

```
Could either of u succinctly explain how efficiency is affected by the voltage.  The effective voltage changes based on pwm so why is running high voltage inefficient in the motor and esc.   I read about increased ability to magnetically saturate as well from higher voltage while I'd always understood inductance and the field strength to be determined by amps
```

---
## \#9 Posted by: raphaelchang Posted at: 2017-01-16T22:53:57.347Z Reads: 94

```
I think this can be better explained with motor curves. This curve shows the values when **effective voltage (PWM and battery voltage) is fixed** and you vary the load on the motor.

<img src="/uploads/db1493/original/3X/7/8/78ed1663885d68d785dc3db3189e84e7c4ecc4f4.png" width="504" height="288">

**Current is always proportional to torque**, with no exceptions. It is also proportional to [effective voltage - back EMF], and back EMF is proportional to the actual speed. This is why in the graph, as RPM goes up, current/torque goes down. For a higher KV motor, the slopes in the graph would be different. All of the slopes would be steeper, and the speed curve would have a higher y-intercept (free speed) and lower x-intercept (stall torque). Because the amps/torque curve is steeper, **higher KV motors require more current for the same load**.

Now suppose we double the battery voltage, doubling the effective voltage. All the slopes in the curve stay the same, but the axis values are doubled. For example, the 12000 rpm point becomes 24000, and the 0.6 oz in point becomes 1.2 oz in. Because current is proportional to torque, the **stall current doubles when the voltage is doubled**. If you double the input voltage, your motor will also be capable of twice the torque and therefore twice the current. So if something goes wrong in the ESC, it will cause much more damage to the motor at a higher voltage.

Here is where it gets confusing. If we overlay the original curves on top of the new curves (double voltage) and pick a point on the x (torque) axis, we see that with double the voltage, the motor is spinning faster when delivering the same torque/drawing the same current. This makes sense from a power perspective, we have double the electrical power, so we should have more mechanical power (torque * speed) too. Now, as a thought exercise, suppose we change the gearing (which preserves mechanical power) so that the speed is halved, and the torque is doubled. But the load is still the same, so the system doesn't need twice the torque that we just gained. So the operating point on the motor curve moves to the left, because the motor is now only delivering half the torque is used to before the gearing change. We didn't change the mechanical power, but we halved the current, so **by increasing the voltage, less current is required to produce the same power**. Moving left on the curves also tends to mean better efficiency, so increasing the voltage also helps with the [mechanical power / electrical power] ratio.

Hope this wasn't too confusing.
```

---
## \#10 Posted by: Hummie Posted at: 2017-01-16T22:58:25.789Z Reads: 80

```
By increasing the voltage less amps are needed for the same power IF a gear is used and the motor is spun faster no?   But how to figure most efficient voltage If the load is fixed and the gear ratio is fixed?
```

---
## \#11 Posted by: raphaelchang Posted at: 2017-01-16T23:29:12.173Z Reads: 81

```
If you fix the load, your current is fixed. Therefore, any change in voltage will change the electrical power and speed of the motor at that load. Efficiency is [mechanical power / electrical power]. Both powers increase when you increase the voltage, but usually mechanical power increases more (if you look carefully at the speed curve when you shift them up by increasing the voltage). This is why increasing voltage increases efficiency.
```

---
## \#12 Posted by: Hummie Posted at: 2017-01-16T23:37:37.176Z Reads: 76

```
For a given load the current would be fixed ok but if u add battery voltage and don't increase the speed?
```

---
## \#13 Posted by: raphaelchang Posted at: 2017-01-16T23:57:27.591Z Reads: 82

```
If you look at the curves, the speed will have to increase when you increase the voltage at a fixed load. Current is proportional to [applied voltage - back EMF], so if applied voltage is increased but current is fixed, back EMF (speed) has to increase as well.
```

---
## \#14 Posted by: Hummie Posted at: 2017-01-17T02:32:16.613Z Reads: 82

```
I mean if the pack voltage is increased how will it effect the motor efficiency.. but now in this simulatior
http://www.ebikes.ca/tools/simulator.html

 I'm seeing that the motor almost never sees the pack voltage when looking at the motor amps and battery amps in the bottom center.  I thought the vesc, since it seemed to get to 100% duty cycle early as it increased speed, it was having the motor exposed to the full pack voltage once it got to 100% duty cycle.  and that would be inefficient maybe as it would spend more time in rpms possibly much slower than the no-load based on the pack voltage.  and it's said you should ride roughly 85percent of the no load for optimum efficiency.  
and that logic follows what the simulator shows as the high rpms are the most efficient regardless of the motor amps and pwm bringing the effective voltage down
 

I thought that outrunners were most efficient running at high speeds.  Is this just because with the increased speed there's less torque/amps needed to produce the same power?  Is this idea based on a fixed power output and its more efficient to put it out at higher speed.    maybe that's all it means.

any light you can shed is appreciated.  or I'll have to get my iphone chip going and do some tests.  probably will anyway..  have to try 6s vs 12s and running a consistent 10mph and see what temp and range I get.

im more concerned with motor efficiency as the vesc seems to have no problem doing anything and the losses there I assume are pretty small.  if its not getting too hot to run it's good and never happened to me.
```

---
## \#15 Posted by: raphaelchang Posted at: 2017-01-17T04:02:52.825Z Reads: 66

```
These curves describe the motor values **at a fixed applied voltage**. As soon as you change the pack voltage or duty cycle, the curves will change. Think of them as spinning a motor at a fixed voltage, and gradually increasing the load on them until the motor can't spin anymore. If you know what speed you usually want to ride at and the typical load, you can choose your voltage such that that operating point is 85% of no load speed (i.e. you know KV, so you can calculate the no load speed, and use 85% of that to match your desired speed, and make sure that point on the curves matches your typical load).

Because of the geometry, outrunners have more torque and less speed (lower KV) than inrunners (think of it like gearing). I don't know if they're more efficient at high speeds. It is definitely more efficient to run at higher speed and lower torque; this is why gearing down makes it more efficient.
```

---
## \#16 Posted by: aethyr Posted at: 2017-01-17T07:14:44.755Z Reads: 59

```
Thank you, so I wasn't quite at stall, but I kicked forward on the scooter about 1-2 mph, but I'm guessing that's still near stall, which, if I understand correctly, at 48V, I did in fact double the current from 24V, which means I quadrupled the wattage. I think this definitely explains why my motor and wires nearly instantly fried.

I think I may need to go with a smarter ESC like the vesc. My only concern is the 60A limitation.

DeathCookies - are you running a TB esc or a vesc on your 12S sk3 motor?
```

---
## \#17 Posted by: DeathCookies Posted at: 2017-01-17T07:25:53.346Z Reads: 59

```
VESC! Imo there is nothing better for esk8
```

---
## \#18 Posted by: aethyr Posted at: 2017-01-19T20:28:18.739Z Reads: 48

```
Hmm, the VESC probably limited the current so that it wouldn't blow the motor. Looks like I'll have to go VESC.
```

---
