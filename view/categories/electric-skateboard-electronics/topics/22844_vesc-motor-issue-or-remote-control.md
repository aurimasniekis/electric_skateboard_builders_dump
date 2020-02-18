# VESC, Motor Issue, or Remote Control?

### Replies: 10 Views: 702

## \#1 Posted by: zblad Posted at: 2017-05-11T18:09:41.338Z Reads: 82

```
Hello,

I am working on an electric mountain board and I am using a sk3 213kv motor, a VESC, an 8s battery, and an old traxxas rc remote.  I did the motor detection and all went well but for some reason and only sometimes when I punch it full throttle my motor like jumps or cogs.  The motor isn't hooked up to anything just mounted up to spin so there is no load on the motor.  It only seems to do this usually if I spin the motor up then brake and then punch in full throttle.  I don't think I will ever punch it full throttle when riding but I don't think it is supposed to do this.

Thank You
```

---
## \#2 Posted by: TarzanHBK Posted at: 2017-05-12T14:27:00.024Z Reads: 55

```
hook it up on your bldc tool, go to terminal and type in "faults" and see what problem your vesc has.
```

---
## \#3 Posted by: zblad Posted at: 2017-05-12T19:21:56.878Z Reads: 45

```
Alright I'll try it tonight thanks
```

---
## \#4 Posted by: zblad Posted at: 2017-05-15T13:18:10.084Z Reads: 39

```
Alright so I did this and didn't get any faults, But before I did this I realized the VESC was setup for dual motors over can so I disabled that for now beings I only have a single motor right now.  I am thinking it had something to do with that.  My next question is when I use some electric skateboard calculators online it says I should be getting around 20mph.  I am only getting 10mph right now.  I am thinking it is either because I have a single motor or my battery might not be able to output the amount of amps needed.  The battery is two 4s batteries in series to make 8s.  I took the battery out of a broken hoverboard and read the specs and the max output is 10 amps so in series should be 20 amps which isn't very much?
```

---
## \#5 Posted by: TarzanHBK Posted at: 2017-05-15T13:35:51.271Z Reads: 34

```
sounds like you took the vesc from another system and plugged it in your own and took a run.
Vesc is not plug and play and you have to set it up from the beginning for every motor - battery combination. So make sure all your settings are right.
The next thing is that if the battery is only capable of 20A max, you should leave a bit room and set it up right, also in the vesc settings, to make sure that you don´t stress and kill it as soon as you go for a ride.
```

---
## \#6 Posted by: zblad Posted at: 2017-05-15T13:41:40.080Z Reads: 31

```
it was a brand new VESC from diyskateboards.  I went through a couple videos on setting amps and voltages and my receiver up.  Not sure how I missed the dual motor check box.  As for the battery do you think 20 amps is enough to get the power needed for an electric mountain board or should I order a battery that can handle at least 60+ amps?  to me 20amps max isn't very much and im wondering if that is what is limiting my board to only 10mph.
```

---
## \#7 Posted by: TarzanHBK Posted at: 2017-05-15T14:09:06.334Z Reads: 29

```
In my opinion you need at least 2 very good vesc that can handle the amount of power you need to have fun with a mountainboard.
Post screenshots of your vesc settings.
```

---
## \#8 Posted by: zblad Posted at: 2017-05-15T14:11:56.292Z Reads: 29

```
will do on my lunch
```

---
## \#9 Posted by: Montiey Posted at: 2017-05-15T15:54:06.881Z Reads: 29

```
Might want to hold on that...
That's normal from my experience. Without FOC it is hard for the VESC to smoothly accelerate the motor, and so if you apply too much current, the electric RPM will exceed that physically capable of the motor, so the VESC has no choice but to advance the phases anyways and you'll loose traction. If it works normally other than that, I wouldn't worry about it. You could try using FOC, but I can't recommend that since I have not used it myself.
```

---
## \#10 Posted by: zblad Posted at: 2017-05-15T17:26:09.097Z Reads: 25

```
Here are my current settings...
<img src="/uploads/db1493/original/3X/2/f/2fae447b99c4875075f3f01426ea1cfbbe9205cd.PNG" width="690" height="392"><img src="/uploads/db1493/original/3X/1/e/1e04d2676e6e7261cf96237b1bbab76932964a2c.PNG" width="690" height="414"><img src="/uploads/db1493/original/3X/9/0/9078cadb95d3f87ec5c0d9a6dabef5b44817e994.PNG" width="690" height="413"><img src="/uploads/db1493/original/3X/6/c/6c03280768121d92ac45f9527fbf9e26029a86eb.PNG" width="690" height="415"><img src="/uploads/db1493/original/3X/a/1/a118a8c5c6e6e1d4b76b4a602aff11fa19172ff5.PNG" width="690" height="403"><img src="/uploads/db1493/original/3X/e/d/ed3674959421cba23c2f0c04a27e396fcaaef127.PNG" width="690" height="406">
```

---
