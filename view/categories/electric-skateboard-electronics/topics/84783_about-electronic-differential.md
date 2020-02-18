# About electronic differential

### Replies: 5 Views: 264

## \#1 Posted by: jeorghe Posted at: 2019-02-20T12:27:09.605Z Reads: 124

```
Has anyone tried to implement an electronic differential for traction control with arduino or similar? I mean that during a change of direction, one wheel rotates more than the other.
Or does it already exist?
```

---
## \#2 Posted by: Acido Posted at: 2019-02-20T12:40:51.018Z Reads: 120

```
Vesc has traction control when connected with canbus already
```

---
## \#3 Posted by: AlexBE Posted at: 2019-02-21T02:11:39.804Z Reads: 75

```
A few people have talked about it, using an accelerometer to measure board tilt and using that to drive the outside wheel with more torque. With a two wheel drive setup, there is some natural differential action due to the fact that both wheel are driven with the same torque, this means that the outside wheel will naturally spin faster.

Traction control is in the VESC system, but it isn't real traction control. Ie it can only prevent one wheel spinning much faster than the other. It does nothing to stop both wheels spinning. The reason is that this simple form is effective enough.
```

---
## \#4 Posted by: jeorghe Posted at: 2019-02-21T07:55:13.206Z Reads: 56

```
Thanks for the responses, you guess mainly my idea. I have a little of time and I will try wih the tilt sensor.
```

---
## \#5 Posted by: b264 Posted at: 2019-02-21T08:42:37.978Z Reads: 45

```
This is only a thing cars need because they only have one engine.  It's better to have a motor for each wheel, and that renders differentials useless.  If for some reason you had one motor driving two wheels you'd need one, but it'd be far better to put one smaller motor on each wheel.

TL;DR: differentials are going backwards, making it more shitty
```

---
