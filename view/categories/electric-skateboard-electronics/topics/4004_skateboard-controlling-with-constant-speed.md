# Skateboard Controlling with constant speed

### Replies: 12 Views: 1856

## \#1 Posted by: John12121 Posted at: 2016-05-30T12:49:06.026Z Reads: 131

```
Hey there! 

I have built a very short electric skateboard using a brushless hub-Motor with hall sensors. It's not supposed to go 50km/h or so. It is just for slow cruising and therefore about 16km/h are enough for me. 

It is very hard to ride because it is so short that when you try to accelerate, it's hard to keep standing. 
My target is now to not make the board accelerate itself but to simply push the skateboard like an normal skateboard and to use the motor to keep the speed constant from that point on (even if I'm for example going uphill). 

My plan is this:
- Use a normal ESC to controll the motor
- Use an arduino to read the hall sensors and thereby calculate the speed at which the board was accelerated by pushing
- Use arduino to write the according throttle-value to the ESC to keep the speed constant
- Use a remote control button to control when I wnat to slow down

My questions are now:
- Is there an easier way to do this?
- Do you see problems here? 
- Do you have suggestions for the remote control? I simply need an easy remote-control-button, but it is very important to have a stable remote connection. 
- Can I simply use any 433Mhz Remote like for garage doors or so? Or do I have to fear someone else to steer my skateboard if he/she has the same 433Mhz remote?

Thanks a lot in advance!!!
Regards, John
```

---
## \#2 Posted by: psychotiller Posted at: 2016-05-30T13:08:55.043Z Reads: 119

```
@lowGuido did this using the nunchuck/c button I believe and from what I read it worked quite well.
```

---
## \#3 Posted by: DeathCookies Posted at: 2016-05-30T13:20:56.295Z Reads: 117

```
[quote="John12121, post:1, topic:4004"]
My target is now to not make the board accelerate itself but to simply push the skateboard like an normal skateboard and to use the motor to keep the speed constant from that point on (even if I'm for example going uphill).
[/quote]

When you are accelerating by push kicking you cannot hold the same speed downhill. The board does not know if you are going downhill or just pushing. My idea would be that it would accelerate downhill but then you would use the brake do decelerate (hold the same speed)
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2016-05-30T15:50:33.995Z Reads: 101

```
[quote="psychotiller, post:2, topic:4004, full:true"]
@lowGuido did this using the nunchuck/c button I believe and from what I read it worked quite well
[/quote]

As @psychotiller said....

Let's go to @lowGuido's video tape 👇🏻

  http://www.electric-skateboard.builders/t/low-guidos-hack-board-for-science-now-with-hub-motors/870/42?u=michaelinvegas
```

---
## \#5 Posted by: lowGuido Posted at: 2016-05-31T10:52:33.908Z Reads: 77

```
Super easy. VESC and a gutted nunchuck.  You dont even need arduino VESC has it built in.
https://youtu.be/jzwtTf7k4yQ
```

---
## \#6 Posted by: John12121 Posted at: 2016-06-01T08:29:06.965Z Reads: 66

```
Thanks for all the replys! The video looks really good!

But couldn't this also simply be done with a "normal" ESC with governor mode? Governor mode is normally for helicopters to keep the speed of the rotors constant. But couldn't that simply be used for making a skateboard go with constant speed?
```

---
## \#7 Posted by: flatsp0t Posted at: 2016-06-01T08:31:13.545Z Reads: 65

```
No, because you have different loads.
if you reach a hill, a normal esc will keep the power and you slow down.
The vesc will increase speed to keep measured RPM
```

---
## \#8 Posted by: lowGuido Posted at: 2016-06-01T08:41:40.772Z Reads: 62

```
what he said.... 
there is constant speed, and then there is constant RPM. 2 different things.
```

---
## \#9 Posted by: John12121 Posted at: 2016-06-01T09:07:55.562Z Reads: 59

```
[quote="flatsp0t, post:7, topic:4004"]
if you reach a hill, a normal esc will keep the power and you slow down.
[/quote]

But this is only correct for a normal ESC without governer-mode, isn't it? 
According to [this](http://wiki.rc-heli-fan.org/index.php/Regler/Steller) (sorry, the link is in german), the  ESC should automatically increase the Ampere, if the RPM drops to keep the RPM constant.
```

---
## \#10 Posted by: flatsp0t Posted at: 2016-06-01T09:18:46.555Z Reads: 55

```
I need to think about it for a moment. German is no problem as i am from Germany.
```

---
## \#11 Posted by: John12121 Posted at: 2016-06-02T07:18:51.287Z Reads: 47

```
Already some thoughts? 
Does someone know governor mode?
```

---
## \#12 Posted by: lowGuido Posted at: 2016-06-02T08:45:57.848Z Reads: 43

```
I don't know.. sounds like you might have to give it a shot..
```

---
