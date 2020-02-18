# Limiting acceleration and acceleration profiles

### Replies: 6 Views: 1529

## \#1 Posted by: Peter1 Posted at: 2017-04-22T08:53:47.357Z Reads: 116

```
Hello everyone!

We are building an electric longboard with a team of university students. Our goal is to make an electric longboard with different driving modes. Because of this, we are working with an Arduino which communicates with the VESC via UART. 

One of the modes that we are using now is just straightforward by using an RC controller. We were also thinking about a way to limit the acceleration of the board (maybe in a different mode, so the user has the option to chose this or not). Furthermore, it is also important to limit the jerk (derivative of the acceleration).

We were thinking of an algorithm for applying this, but it's deffinitely not as easy as it looks. Due to this, I started thinking that we are probably not the first ones to think about this idea. So my question is: is there already a good control mode in BLDC-tool that **limits the acceleration** (**and variation of the acceleration** to drive smoothly)? 

Kind regards, 
Peter
```

---
## \#2 Posted by: Lukas Posted at: 2017-04-22T08:57:50.356Z Reads: 110

```
I think this might be what you are looking for.
https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
```

---
## \#3 Posted by: Peter1 Posted at: 2017-04-22T10:09:12.406Z Reads: 96

```
Thanks, I've read the thread, but I still don't really see how the acceleration is limited? The adjusted throttle valve seems indeed a good idea since it gives more control and will probably give a slower acceleration in the beginning. But still, if I push the throttle for the full 100%, acceleration won't be limited I suppose and the board will still shoot away?
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-04-22T10:54:44.478Z Reads: 87

```
The acceleration is mainly regulated by the Motor Amps. So the normal current control mode works like this. If you want less then simply lower the motor amps. It's not directly controlling the acceleration, so that you would get the same acceleration uphill or downhill. But that doesn't make sense to me.
Acceleration is a speed increase over time. And in theory the VESC already has that for the Nunchuk in cruise control. Because there you can adjust for example that you only allow a speed increase of 3000 ERPM per second. But that's not really usable as your normal riding mode. 
If you simply want more control over the board just use my firmware mod and ride in watt control with a adjusted throttle curve. After you tested that and still see room for improvement or have good ideas then let me know,
```

---
## \#5 Posted by: Peter1 Posted at: 2017-04-22T11:08:02.657Z Reads: 83

```
I was indeed thinking of something like allowing a maximal increase of speed per second. (Just for safety)

But I will definitely try the Watt control. Based on the reviews, it looks very nice!
```

---
## \#6 Posted by: Duffman Posted at: 2017-04-23T14:46:17.138Z Reads: 55

```
There are two more parameters which control ramping under 'Motor Configuration/Advanced':

'Duty ramps step' controls the maximum speed increase per millisecond when using dutycycle control = acceleration

'Max current ramp step' controls the maximum current (torque) increase per millisecond = jerk

Unfortunately these both parameters only work for those two different control methods, so you cannot limit motor speed increase and motor current increase at the same time.

No idea how difficult it would be to change the software to limit both at the same time. @Ackmaniac
```

---
