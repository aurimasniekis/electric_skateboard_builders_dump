# Vesc Reverse and Remove Three Red Flashing Lights

### Replies: 7 Views: 560

## \#1 Posted by: IsTalo Posted at: 2017-07-16T02:58:41.742Z Reads: 66

```
Hello Guys, so, my board is almost done, but there are some things that I think would make it better, like the capacity of using it with reverse... but the tutorials I saw telled me to use "Current No Reverse with brakes" and there is no option like "Current with Reverse" and I don't know how to configure DutyCicle, I really want some help, tomorrow I post my configs. When I use dutycycles the motor get crazy and when I brake and turn the trigger back it start going full throttle, help mee

Another issue is that red light blinking, because I really don't like to wait that 3-4s to start using my board, would there be a way to remove that?
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-16T03:10:08.397Z Reads: 63

```
"Current" is the mode you want for reverse. The blinking lights is part of bootup and will likely be done before you even put your board down
```

---
## \#3 Posted by: IsTalo Posted at: 2017-07-16T03:11:03.855Z Reads: 61

```
Fine, but I like DutyCycle because it have a acceleration wave better than Current, or is it something only in my mind?
```

---
## \#4 Posted by: Blasto Posted at: 2017-07-16T03:15:51.710Z Reads: 58

```
Current control is the reason the vesc is so nice, current is constant and the duty cycle is dependent.

In duty cycle mode, the duty cycle is constant and the current is dependent... meaning the current can be potentionally infinit, busting the hardware. (Main reason why you are hitting a cutoff limit)

Duty cycle mode is mosly used in robotics, for a skateboard, current control is the way to go
```

---
## \#5 Posted by: IsTalo Posted at: 2017-07-16T03:17:55.712Z Reads: 58

```
Oh, that is a good explanation, you convinced me, another thing that I want to ask in the same threat, sometimes when my motor goes one direction the Belt go to the outside of the pulley, when I go to the other direction it goes to the inside of the pulley, what can it be?
```

---
## \#6 Posted by: Blasto Posted at: 2017-07-16T03:25:54.492Z Reads: 56

```
Tbh, the only reason i see for going in reverse is for deerping around.

But to answer your question, most likely your wheel pulley is not perfectly true with the motor pulley. To a certain degree this could be hard to obtain.

I always ask myself, is it good enough for the girls i go out with?
```

---
## \#7 Posted by: IsTalo Posted at: 2017-07-16T03:38:35.963Z Reads: 54

```
The girls call me Nerd because I build an Esk8 and still building a drone... But maybe some girl see a potential in it hahah

Yeah, maybe the wheel pulley is a bit different of the motor pulley, also because it is 3d printed, but Thx anyway
```

---
