# Vesc brake always at maximum?

### Replies: 9 Views: 601

## \#1 Posted by: Agira Posted at: 2018-01-02T11:19:30.182Z Reads: 102

```
Hi guys,

i stumbled upon an issue with my setup. I cannot set the brake force, whatever number is set the force remain the same. For example i've set the motor min at 5A and the batt min to 0, and when braking the current reach 13A, the same current with much higher brake settings. Same results even setting the brake current with the control tab of bldc Tool.

I'm using an arduino to control the vesc through the RollingGeckos VescUartControl library, more precisely the VescUartSetNunchukValues function. It's the master branch. On the focbox i've flashed the ackmaniac 2.54 firmware. 

Are my config wrong? Or do i understand wrong the brakes behavior? 
Hope you guys can help :)
```

---
## \#2 Posted by: PXSS Posted at: 2018-01-02T12:01:53.552Z Reads: 91

```
Post screenshots of your settings. Are doing this on a bench or actually riding?
```

---
## \#3 Posted by: Ackmaniac Posted at: 2018-01-02T12:13:51.540Z Reads: 84

```
I guess you see the high current only in the moment when the motor comes to a complete stop?
```

---
## \#4 Posted by: Agira Posted at: 2018-01-02T13:43:52.746Z Reads: 73

```
I'm testing on the bech. Is there some other relevant screenshots i should post?
In the last screenshot I've set the current to 2A on the control tab and turn back and forth the wheel.

<img src="/uploads/db1493/original/3X/9/6/962cb7b4db814ade8221ec99dacb48437fc2df49.png" width="690" height="387"><img src="/uploads/db1493/original/3X/4/d/4d136c00dfd4347e38adea834bd61e6b03e2a911.png" width="690" height="387"><img src="/uploads/db1493/original/3X/6/f/6f7e0f62e3d20aca473ba176d663b46bd3cc89eb.png" width="690" height="387"><img src="/uploads/db1493/original/3X/7/d/7dddd1e42f390d922ee41ccada13fd034775010d.png" width="690" height="387">
```

---
## \#5 Posted by: PXSS Posted at: 2018-01-02T13:57:58.909Z Reads: 58

```
Red curve is motor current. You got that set to -30. 
Blue curve is battery current, that stays near zero. 
You probably cant spin it fast enough continuously long enough to produce any significant current back to the battery on the bench. That is more of a while riding kind of test.
```

---
## \#6 Posted by: Agira Posted at: 2018-01-02T14:06:20.079Z Reads: 57

```
But even if I set the motor min to 2A, and using the remote gives just a tiny bit of brake, the brake force remain the same.
I can brake but it always the full power of the brake, I can not adjust it
```

---
## \#7 Posted by: GrecoMan Posted at: 2018-01-02T14:21:29.643Z Reads: 54

```
it’s because your on the bench dude. put your board on the floor and you’ll see how weak and gradual braking is
```

---
## \#8 Posted by: Ackmaniac Posted at: 2018-01-02T14:39:00.995Z Reads: 49

```
Below 3% duty cycle the VESC does a full brake. Doesn't matter which settings you adjusted. Because at this low rpm's it can't detect the motor position.
Just test it riding the board and forget the bench tests.
```

---
## \#9 Posted by: Agira Posted at: 2018-01-02T16:45:24.767Z Reads: 40

```
Oh .. that makes sense. I will test and then report back :grin:
```

---
