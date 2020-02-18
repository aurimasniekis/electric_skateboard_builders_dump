# Servo Y connector completely powering second esc

### Replies: 8 Views: 980

## \#1 Posted by: stuxtruth Posted at: 2016-08-18T00:32:57.336Z Reads: 96

```
Can someone tell me how to use a remote with two ESCs. I used a servo y connected to bridge both ESCs to Channel one on my reciever. Even when I unplugged the xt60 the esc was still being powered.
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-18T00:40:02.683Z Reads: 94

```
Not sure what you mean. Are you talking about the servo cable or the power cable? servo cable doesn't supply power to the ESC. The ESC supplies power to the receiver, and you have to cut one of the positive leads on one of the servo cables since you don't need two sources of power on 1 receiver.
```

---
## \#3 Posted by: stuxtruth Posted at: 2016-08-18T00:53:30.578Z Reads: 85

```
For some reason it was completley powering my esc lol. I had the power cable out... the fan was going full blast. But yea cutting one of the red wires did the trick.Thanks!
```

---
## \#4 Posted by: VladPomogaev Posted at: 2016-08-18T01:08:37.558Z Reads: 76

```
Yeah that happens. It's perfectly fine actually, except you won't be able to power the motor on the second ESC.
```

---
## \#5 Posted by: stuxtruth Posted at: 2016-08-18T01:20:14.701Z Reads: 68

```
https://youtu.be/qxIYb9Y-R8E
```

---
## \#6 Posted by: Namasaki Posted at: 2016-08-18T05:07:26.670Z Reads: 59

```
I've known for some time that your not suppose to feed 5v to the receiver from 2 esc's or vesc's.
But, frankly I don't see why since dual  5v supplies would be in parallel and it should be no different than connecting dual  5v batteries in parallel. Can someone give me a good reason for this?
```

---
## \#7 Posted by: Jinra Posted at: 2016-08-18T05:09:02.033Z Reads: 56

```
I actually don't see a problem either except it's feeding double the current from the ESC to the receiver, which may or may not be bad for it depending on the receiver.

What's happening with @stuxtruth, I believe, is that the fan is powered by the 5v terminal and the 5v from 1 ESC is also powering, in parallel, the fan on the other ESC.
```

---
## \#8 Posted by: Namasaki Posted at: 2016-08-18T05:41:04.155Z Reads: 52

```
Theoretically, if you power the receiver by 2 bec's, the current that the receiver pulls should be divided by 2
Wonder if anyone has every done it and what the outcome was. 
I'm not willing to risk trying it with my Vesc's or Receiver but it would be nice to know for sure 
and think of the advantage,
If the 5v supply fails on one esc, the other will keep things going.
```

---
