# Changing motor spin direction

### Replies: 5 Views: 219

## \#1 Posted by: MrDGOrman Posted at: 2019-03-07T16:15:53.765Z Reads: 76

```
Hi everyone,

I've had a board for a while now. Done some recent modifications which include putting my motor on the other side of the truck.

I need to change the motor direction so naturally I tried changing 2 of the wires and it doesn't change? Ive tried all combinations and the only results I get is either the motor spinning the wrong way, the motor refusing the spin at all, and the motor spinning the correct way but with a horrible clunking noise.

Any ideas why this is happening and how I can resolve it? I'm using a FOCBOX and Nano-X remote with Eskating sensored motor.

Cheers,
Daniel
```

---
## \#2 Posted by: linsus Posted at: 2019-03-07T16:33:39.853Z Reads: 70

```
Only way it didnt change direction is cause you put em back they way they were. You can also change motor direction in the VESC tool. (or you know, with one click on a proper esk8 remote)
```

---
## \#3 Posted by: briman05 Posted at: 2019-03-07T17:00:19.842Z Reads: 55

```
If you change the 2 wires you have to do a motor detection again.  But like  @linsus said there is a part in the vesc tool that reverses the direction
```

---
## \#4 Posted by: MrDGOrman Posted at: 2019-03-08T00:00:22.432Z Reads: 37

```
I ended up connecting the FOCBOX and reversing the motor direction that way. I've colour coded my phase wires so it's probably easier to just change a setting!
```

---
## \#5 Posted by: mynamesmatt Posted at: 2019-03-08T00:01:53.528Z Reads: 37

```
its easier to just switch 2 phases and redo detection. that way you can be sure that nothing will switch back
```

---
