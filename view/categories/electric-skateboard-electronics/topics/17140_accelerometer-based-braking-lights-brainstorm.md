# Accelerometer based braking lights &ndash; BRAINSTORM

### Replies: 4 Views: 580

## \#1 Posted by: 3sly Posted at: 2017-02-03T10:24:56.767Z Reads: 104

```
Hey guys,

Have been messing around with the idea of building some arduino based braking lights that don't require a manual input to be activated.

How cool would it be when you put an all-in-one unit (like those little lights you can buy) on your bike that automatically detect a strong enough deceleration to activate a braking light. Would it be possible to differentiate between a braking deceleration or a deceleration due to e.g. the start of a hillclimb (which also isn't a bad idea to activate braking lights for)

Or am I looking for a too complex solution and is it maybe possible to tap the signal from the vesc and see when the controller is in the minus range (that way you have a 100% accurate braking signal)

If so then this might be a new project.

Thoughts, inputs,... I'm curious to know!

Dries
```

---
## \#2 Posted by: lowGuido Posted at: 2017-02-03T10:50:48.120Z Reads: 98

```
Not trying to disrespect your idea. But isnt it overly complicated?
There is already a brake signal going to the esc. Hook it up to lighting kit. Job done.
```

---
## \#3 Posted by: eitan Posted at: 2017-02-03T10:54:35.408Z Reads: 98

```
VESC supports regenerative breaking, correct? Then another solution might be the inputs to the batteries. 

```
if (battery is charging and the e-board is switched on) {
 breaklight = true
}
```
If I understand correctly, this would only work in cases where the discharge functionality of the BMS is being used (rather than circumvented, as is the case in some builds).
```

---
## \#4 Posted by: 3sly Posted at: 2017-02-03T11:22:41.701Z Reads: 93

```
@lowGuido. True, exactly my thought. I'm probably going to end up doing it that way. It seemed an interesting idea though to make an aio package that you can stick on any moving object and can sense strong enough decelerations. I might end up experimenting with it. I was just wondering what the implications would be. My thought would be that it might trigger too quickly on irregular terrain and the difficulty of distinguishing between a meant deceleration and an environmental one.

@lowGuido @eitan, isn't there an even easier solution to that? Isn't there a possibility to just tap of the signal of the remote receiver. And calculate when it is pulled backwards.
```

---
