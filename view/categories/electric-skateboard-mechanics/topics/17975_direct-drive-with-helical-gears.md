# Direct drive with helical gears?

### Replies: 18 Views: 2190

## \#1 Posted by: michaelcpg Posted at: 2017-02-20T06:50:01.298Z Reads: 336

```
Has anyone tried this or does anyone sell them? I've seen a few threads of people using gears on, mostly on mountain boards, but I'm curious as to why so few people seem to use direct drive systems for their motors. 

I hear that it's a bit noisier but I like the idea of not having to worry about dealing with belts, particularly because mine seem to always end up either being too tight or otherwise end up being able to slip on the odd occasion when braking heavily.
```

---
## \#2 Posted by: chuttney1 Posted at: 2017-02-20T07:23:34.898Z Reads: 333

```
It's more about preference. Destroyed belt, easy replaycement. Broken tooth on gears, expensive. Helical gears are slightly more costly to make than straight cut gears but much quieter. Nothing is stopping you from making helical gears should you decide.
```

---
## \#3 Posted by: Alextech Posted at: 2017-02-20T07:29:36.415Z Reads: 322

```
Helical Gears if properly Meshed and shim. Yes, But if not then they can be louder.
```

---
## \#4 Posted by: benwong Posted at: 2017-02-20T07:45:20.239Z Reads: 314

```
@michaelcpg

@captainjez - He is the one who using helical gears on JedBoard~~ :v:
```

---
## \#5 Posted by: michaelcpg Posted at: 2017-02-20T08:09:54.382Z Reads: 298

```
Cheers, didn't realise he was on these forums :p
```

---
## \#6 Posted by: captainjez Posted at: 2017-02-20T09:12:40.293Z Reads: 289

```
Right here :) Happy to answer any questions :)
```

---
## \#7 Posted by: TarzanHBK Posted at: 2017-02-20T09:29:46.409Z Reads: 283

```
also @esk8 and @Nowind are producing them
```

---
## \#8 Posted by: captainjez Posted at: 2017-02-20T09:31:01.834Z Reads: 277

```
Those are spur gears, not helical.
```

---
## \#9 Posted by: HTownBomber Posted at: 2017-02-20T13:07:21.187Z Reads: 272

```
I hate to get all semantical and shit, but if it has any gears or other reduction, it's not direct-drive by definition.
```

---
## \#10 Posted by: TarzanHBK Posted at: 2017-02-20T13:31:57.035Z Reads: 259

```
you´re right! I just saw gear-drive :monkey:
```

---
## \#11 Posted by: captainjez Posted at: 2017-02-20T13:45:38.147Z Reads: 261

```
Direct drive in this instance refers to the fact the wheels are driven directly off the motor without the use of a belt.
```

---
## \#12 Posted by: HTownBomber Posted at: 2017-02-20T14:18:22.010Z Reads: 259

```
I hear you and I understand the distinction. The correct terminology would be inline helical/spur/planetary/hypocycloid drive. Or geared hub if it's inside the wheel. Direct drive, by definition, means no gearing at all and the motor output shaft drives the wheel without reduction. But I digress. 

I've done a good amount of reading on geared hub and mid-drive setups, mostly on Endless Sphere. You can get monster torque and power from a high-revving motor, particularly when you're gearing down like 8:1 or higher. That kinda reduction just isn't possible with belts unless you have multiple stages. High kV motors are more efficient with less cogging. One of the more extreme examples is the Tangent Motors mid-drive ebike setup with a beastly little Astro Flight 32xx inrunner mated to a cycloidal gearbox at 40:1 reduction, where it drives a chain. Insane torque. 

As we push the limits of belts and move to bigger wheels, we get into territory of e-scoots & trikes. Those guys have been monkeying around with inline gearing for years. 

I would love to see somebody mate esk8 wheels to the output shaft of a cycloidal drive. Maybe it'll be me...
```

---
## \#13 Posted by: DaveMess Posted at: 2017-02-20T14:33:56.536Z Reads: 249

```
The biggest reason I'd say not to use gears is because you want the belt to fail. So say you're riding along and your wheel loses traction on something and then quickly regains it, jerking your drivetrain. That belt is actually going to absorb some of the shock from that. With gears, there is a direct, unforgiving connection between your motor and your wheel, so if something causes your wheel to lock up suddenly, it gets transmitted directly to your motor shaft and bearings. With a belt, some of that shock will be absorbed by the flex of the belt, reducing the impact on your motor and pulleys. Also, the belt creates an intentional failure point. If the shock is too great the belt will snap instead of breaking something more expensive like your motor shaft or pulleys/gears. Tldr belts are your friend.
```

---
## \#14 Posted by: captainjez Posted at: 2017-02-21T02:14:00.701Z Reads: 224

```
This is why we built a traction control system into our drivetrain to handle events such as wheel slippage without it affecting the ride and handling. We have custom made motors with additional internal reinforcement along the shaft to ensure the additional forces don't but undue stress on it.

Bottom line is if a belt breaks and you're riding along you've lost all control. Our gears are engineered to last for years.
```

---
## \#15 Posted by: DaveMess Posted at: 2017-02-21T02:26:15.371Z Reads: 224

```
Right, that sounds very well engineered, but for the typical Joe Cool with an SK3 and a HK ESC (or any other ESC, does the VESC have traction control???) That's not going to be ideal. Definitely good advertising for your boards, however. I'd like to have that technology.  🆒
```

---
## \#16 Posted by: captainjez Posted at: 2017-02-21T02:37:02.972Z Reads: 223

```
We've spent a great deal of time on gear engineering and consulting with folks who are specialists to ensure what we are doing will work long term. They're probably way over engineered, but we'd rather release a product that will work without issue. 

Our traction control systems are built using a number of onboard sensors, not just from the motors themselves.
```

---
## \#18 Posted by: Hummie Posted at: 2017-03-06T16:14:27.307Z Reads: 187

```
how would other sensors help traction if they aren't in the motor
```

---
## \#19 Posted by: captainjez Posted at: 2017-03-06T21:07:16.941Z Reads: 181

```
Using various sensors we can know the state of the board at all times. Is it on an incline or decline, how much weight is on each side of the board, etc. This let's us do things like adjust acceleration and braking curves in realtime, as well as subtle changes to how our traction control works based on where weight is shifted on the board.
```

---
