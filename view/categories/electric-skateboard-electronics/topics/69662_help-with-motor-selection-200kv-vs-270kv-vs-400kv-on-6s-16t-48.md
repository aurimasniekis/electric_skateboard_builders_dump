# Help with motor selection (200kv vs 270kv vs 400kv on 6s 16T/48)

### Replies: 14 Views: 446

## \#1 Posted by: Plonvick Posted at: 2018-09-30T21:10:13.354Z Reads: 95

```
I'm currently building a 1 motor, 6S longboard with 70mm wheels and am second guessing my motor choice. I purchased a 5065 200Kv motor from banggood and plan on using it with 16T on the motor and 48T on the wheel.

The motor hasn't arrived yet, but I now realize it will be way too slow. If I was to replace it with another 5065 motor (keeping wheel size and gears the same) would you do 280Kv or 400Kv?

I am looking to get around 20 miles per hour but don't want to be without torque. Thanks for the help!
```

---
## \#2 Posted by: rojitor Posted at: 2018-09-30T21:27:30.367Z Reads: 90

```
You can't use above 300kv. I'd stick to 200. Torque is better than top speed.
```

---
## \#3 Posted by: Plonvick Posted at: 2018-09-30T21:43:08.085Z Reads: 86

```
You think 200kv at 6s will still be ok with my 3:1 gear ratio? I was under the impression that it would be really slow, but I guess not. 

Thanks!
```

---
## \#4 Posted by: mccloed Posted at: 2018-09-30T22:47:00.265Z Reads: 82

```
Yes. You will be pretty slow on 6s and 3:1. When I used to run 6s on 245kv motors I had 20t motor pulleys and 40t wheel pulleys on 83mm wheels and would get a top speed of 25mph on hobby esc's. Looks like you'll only be getting 10mph with 70mm wheels and a 3:1 gear ratio. Check out this calculator: http://calc.esk8.it/#{%22batt-type-lipo%22:1,%22batt-cells%22:6,%22motor-kv%22:200,%22system-efficiency%22:85,%22motor-pulley-teeth%22:16,%22wheel-pulley-teeth%22:48,%22wheel-size%22:70}|
```

---
## \#5 Posted by: Jmding Posted at: 2018-10-01T03:39:17.602Z Reads: 67

```
Depends on what parts you are fully committed on using.  You generally want to go as high voltage as practical (I dont see any reason you wouldn't upgrade to 10s or 12s assuming you are using hobby lipo batteries).  You also want to go as high Kv as possible without breaking 60k erpm, and adjust your gearing to reach the desired top speed of 20 mph.  Motor Kv is proportional to max current capability, which is proportional to max torque at the wheels (assuming you adjust your gearing to trade that extra speed for torque). 

To be honest, given how cheap used Boosted v1's are, I think its a better idea to just buy one of those for around $600.  You wont save any money going DIY, you wont end up with nearly as polished a product.  And unless you do a lot more reading and get to the level where you can draw the torque curve of the drive-train configuration you're planning to use, you almost definitely wont end up with more performance than a used Boosted without spending at least 1k.
```

---
## \#6 Posted by: dareno Posted at: 2018-10-01T04:45:14.724Z Reads: 58

```
[quote="Jmding, post:5, topic:69662"]
To be honest, given how cheap used Boosted v1’s are, I think its a better idea to just buy one of those for around $600. You wont save any money going DIY, you wont end up with nearly as polished a product.
[/quote]

Now go and wash your mouth out with soap
```

---
## \#7 Posted by: Plonvick Posted at: 2018-10-01T23:53:14.638Z Reads: 46

```
Does anyone else care to weigh in?
```

---
## \#8 Posted by: J0ker3366 Posted at: 2018-10-02T00:05:23.758Z Reads: 45

```
@Jmding is right. Unless you're willing to upgrade to 10s or 12s, buy a boosted. From my experience with the liftboard prebuilt I had, 6s4, I do believe it was a 5055 200ishkv (don't quote me on that), would get me 16mph for 16miles. After building the current board I have, 12s, Lipo, 6374 195kv, Focbox (you can quote me on that), 35mph is so much more enjoyable.
```

---
## \#9 Posted by: J0ker3366 Posted at: 2018-10-02T00:07:36.221Z Reads: 44

```
You could definitely go for the 200kv with 16/36 10s and you'd have a blast
```

---
## \#10 Posted by: Holyman92 Posted at: 2018-10-02T00:33:32.809Z Reads: 40

```
im going dual 280kv 8072 motors lol, but i like climbing anything life throws at my board and going fast
```

---
## \#11 Posted by: Plonvick Posted at: 2018-10-02T23:23:40.647Z Reads: 25

```


Very cool! Good luck with that build
```

---
## \#12 Posted by: b264 Posted at: 2018-10-02T23:25:21.669Z Reads: 22

```
ALWAYS use the lowest kv you can.  

You can always increase the size of the motor pulley or reduce the amount of current you're sending to the motor.  You can usually NOT do the opposite.
```

---
## \#13 Posted by: Jmding Posted at: 2018-10-03T01:22:48.874Z Reads: 22

```
b264, low Kv motors cannot handle as much current, and so after gearing they are actually less capable of putting down torque to the wheels.  I agree that you shouldn't use motors with extremely high Kv in that using really small motor pulleys is a bad idea, but in general you want to go with higher Kv motors and adjust the mechanical gearing to compensate.

Especially since he is running a low voltage system, he will need to use as high a Kv motor as practical in order to squeeze out that extra current capability and keep total power as high as possible.  The below is the table of max currents from the factory that makes the SK3 motors.  These are the motors we buy as sk3 50xx motors.  Switching from a 4035 310 Kv to 375 Kv increases max current, and therefore max power, by 17%.  That said, 375 Kv is probably going to require a giant wheel pulley that wont fit, but the general principle still applies when comparing a 200 Kv motor to a 300 Kv motor..

![image|690x360](upload://mbejC1lqnZn1nknjGntvyXFIxqx.jpeg)
```

---
## \#14 Posted by: Plonvick Posted at: 2018-10-03T01:54:51.321Z Reads: 21

```
Thanks! That's very helpful
```

---
