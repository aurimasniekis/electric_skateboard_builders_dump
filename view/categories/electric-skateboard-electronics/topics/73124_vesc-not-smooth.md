# VESC Not smooth

### Replies: 34 Views: 558

## \#1 Posted by: Anubis Posted at: 2018-11-02T13:16:22.881Z Reads: 149

```
Hey, 
So I'm having issues configuring my vesc to be smooth.
Its very loud (I think without the wheel on it is much louder. Should i have done the motor configuration with no wheel on? It adds resistance and i wasnt sure if it should have been on or not) but you can see the controls are not smooth at all. It detects the remote throw correctly, but then the motor is either on max power or not when I test it
Video: https://www.youtube.com/watch?v=AlNjx6HdpBI note i do press "Write to vesc"

You can see that if i push it up very slowly there is not a linear increase, it just ramps up and stays on full power. There is a lot of throw left in the remote and it stays at the same speed the entire time
```

---
## \#2 Posted by: Acido Posted at: 2018-11-02T13:23:16.938Z Reads: 142

```
if your in foc increase switching frequency
```

---
## \#3 Posted by: spesh Posted at: 2018-11-02T13:24:06.547Z Reads: 140

```
motor detection etc should be done without the belts on
```

---
## \#4 Posted by: Anubis Posted at: 2018-11-02T13:43:22.747Z Reads: 131

```
By what magnitude? I'm new to setting up VESCS
```

---
## \#5 Posted by: Acido Posted at: 2018-11-02T14:19:47.359Z Reads: 116

```
i think the max is 40khz
that sound seems normal to me, its kinda loud try in foc and the thing why your motor does not start with small amount of throttle is because it doesnt have sensors probably
```

---
## \#6 Posted by: Andy87 Posted at: 2018-11-02T14:21:49.738Z Reads: 109

```
Where you have this from?
I thought it’s without load... 🤔
```

---
## \#7 Posted by: Anubis Posted at: 2018-11-02T14:33:08.034Z Reads: 106

```
That isnt really the issue though,  I dont mind noise. The issue is the unusable throttle curve going on. I'll switch up the FOC. The starting smoothness isnt a big issue to me, its just the fact that 10% of the remotes throw is used. The PPM Percentage dosent follow "Duty" at all, what happens is once the remote hits a certain threshold, it just ramps up to 100% power. I want the remote to control the speed of the motors but it dosent
```

---
## \#8 Posted by: spesh Posted at: 2018-11-02T14:39:00.397Z Reads: 97

```
the belt and wheel is a load..
```

---
## \#9 Posted by: Andy87 Posted at: 2018-11-02T14:53:34.464Z Reads: 92

```
🙈🙈🙈🙈
Yes sure...already late here 🙈
Read with belt on... sorry my bad
```

---
## \#10 Posted by: Kug3lis Posted at: 2018-11-02T15:14:39.164Z Reads: 90

```
Did you setup your input source with min max and 0 value?
```

---
## \#11 Posted by: Santino Posted at: 2018-11-02T15:25:06.942Z Reads: 86

```
I had a similar issue, I changed the remote response to .20 and play with the throttle curve to fix it. Sometimes it is cause by the remote, and it is god to check that the trimming are were they supposed to be. I configure my vesc with wheel on it, and on the go, while riding... via UART...It takes some time and patience...Vesc tool is amazing...ones your are done with the learning curve, you are going to love it...Check your motor max amps, and battery regeneration...read the explanation of everything (you have a help button to every part of the set up), go to https://vesc-project.com , documentation, then manuals...
```

---
## \#12 Posted by: Anubis Posted at: 2018-11-02T17:04:44.776Z Reads: 73

```
What do you mean? Did i not do this in the video?
```

---
## \#13 Posted by: Deodand Posted at: 2018-11-02T17:16:55.720Z Reads: 71

```
I will say that it doesn't seem so abnormal for me with no load on it. Keep in mind when using current control its like a torque controller, so even with a slight tap and no rider on board the motors will spin up very quickly. Once your on the board it should feel much more gradual with the throttle. 

Looking at the RT data coming in at the bottom you can see not many motor amps are used to spin up your motor. The duty cycle gauge does not correspond to the command being sent to the motor, it will just try to hit the target amps regardless of speed, if its at max speed then the amps will drop. 

Is it a sensored motor?

Have you ridden it?
```

---
## \#14 Posted by: Anubis Posted at: 2018-11-02T17:17:00.006Z Reads: 70

```
I couldnt find an option called response. I have tried changing my positive ramping to 30 seconds and the issue sticks, as soon as my throttle is past a certain % the motors ramp to max power in under a second. I am a computer programmer and this isnt working and hasnt been for 17 hours by now, I think something must be wrong
```

---
## \#15 Posted by: Anubis Posted at: 2018-11-02T17:18:51.984Z Reads: 70

```
I have not ridden it, I have been working on just this for 17 hours. 

Yes, on videos ive seen, "Duty" corresponds with what percent the throttle on the remote is at, and the motor will catch up or down to where it is when moved. This is what I want, but it is not happening on mine, I am getting this  "Get past x% and then the motor goes to max power and thats it" It doesnt make sense that this would ever be smooth, because the motor literally ramps to 100% power in 0% of the throttle throw at a given point. The shittest chinese ESC is smoother than that
```

---
## \#16 Posted by: Deodand Posted at: 2018-11-02T17:21:46.675Z Reads: 70

```
I think you may have a misunderstanding on how the controller is working, it is impossible for your motor to be at max power with out a load on it. Max duty does not equal max power. The duty cycle isn't what is being controlled by the remote, the motor amps are. 

Is this a motor with hall sensors?
```

---
## \#17 Posted by: Deodand Posted at: 2018-11-02T17:23:16.073Z Reads: 66

```
Perhaps I can explain by example, say I move my throttle to 10% that will correspond to 10% of my boards total **ACCELERATION** not speed. Even 10% of your boards acceleration with no rider on board will be enough to spin up the motors to max speed very quickly.
```

---
## \#18 Posted by: Anubis Posted at: 2018-11-02T17:23:22.882Z Reads: 60

```
Yes but I dont know if the hall is setup properly
Why cant the controller pulselength percent be proportional to the speed of the motor? that is all I want
```

---
## \#19 Posted by: Anubis Posted at: 2018-11-02T17:24:20.306Z Reads: 56

```
Wouldnt that make it impossible to move around slowly? because you can't hold a speed at all? :confused:
```

---
## \#20 Posted by: Deodand Posted at: 2018-11-02T17:25:23.782Z Reads: 57

```
It actually feels very natural once riding the board, kind of like your cars gas peddle. Imagine if pushing in your cars gas pedal halfway made your car immediatley go to half your cars maximum speed as quickly as possible. It would be too touchy.
```

---
## \#21 Posted by: Deodand Posted at: 2018-11-02T17:26:53.256Z Reads: 56

```
There is a duty cycle control mode under app settings> ppm which will work the way you are expecting on the bench but it is pretty dangerous to ride in this mode, typically it is only used in robots or drone applications.
```

---
## \#22 Posted by: Anubis Posted at: 2018-11-02T17:27:27.099Z Reads: 51

```
Thats not what it should do though, it should have a predefined acceleration curve then putting the throttle to 50% should follow that curve until the board is at 50% power? Otherwise people would me mashing pedals to maintain speed
```

---
## \#23 Posted by: Deodand Posted at: 2018-11-02T17:31:33.143Z Reads: 51

```
Current control as you have it setup now will feel very much like the gas pedal in your car, that is what the majority of people on this forum use. Every single one of our boards will spin the motors up to max speed at about 15% throttle when the board is flipped upside-down on the bench. It's just the nature of current control. 

Spinning up motors to max speed is NOT max power because there is no force behind it. Somewhat dangerous (don't try it) but you can try holding one of your motors while you gently press the throttle in, you will feel the force of it increasing/decreasing as you move the throttle.
```

---
## \#24 Posted by: Anubis Posted at: 2018-11-02T17:33:56.607Z Reads: 49

```
Actually as I have you, new issue which might be worse. When i pull the brake to max, the wheel still freely spins and the VESC app live data monitoring crashes without error, and requires a restart to get it back up again
```

---
## \#25 Posted by: Deodand Posted at: 2018-11-02T17:36:27.143Z Reads: 47

```
What is your power source for the VESC? If it is a wall supply and not a battery many don't support sinking current back into them, this causes a large voltage spike at the input voltage which can reset the VESC or even damage it if the supply voltage is very high (48V)
```

---
## \#26 Posted by: Anubis Posted at: 2018-11-02T17:37:23.954Z Reads: 44

```
12S5P Eskating.eu battery. https://eskating.eu/product/flat-12s5p-eskating-electric-skateboard-battery-samsung-30q/

Edit: to clarify it is actually also using a super shitty xt90 to 2x xt90 connector and is connected to 2 fsescs, but I am only trying to get 1 to work, the other dosent have the can bus connected but it is being powered
```

---
## \#27 Posted by: Deodand Posted at: 2018-11-02T17:39:24.944Z Reads: 43

```
OK so its plugged into the battery for this testing? Does the red fault light on your vesc blink when you brake? Does the USB disconnect or the app actually crashes?
```

---
## \#28 Posted by: Anubis Posted at: 2018-11-02T17:40:33.978Z Reads: 44

```
I will make a video, its easiest to see what is going on.
```

---
## \#29 Posted by: Deodand Posted at: 2018-11-02T17:41:32.111Z Reads: 48

```
please film landscape haha, much easier for me to see whats going on.
```

---
## \#30 Posted by: Deodand Posted at: 2018-11-02T17:43:02.001Z Reads: 49

```
I would also encourage you to try a few very slow rides down a hallway or something, if you don't understand how the vesc works it might give you a better idea of how the controls are working in a real application scenario.
```

---
## \#31 Posted by: huntercasillas Posted at: 2019-05-09T05:26:21.844Z Reads: 32

```
Did you ever figure out how to accomplish this? How do you go half speed? I don’t understand this whole current control thing, it’s not like a car gas pedal because you can maintain exact speeds in a car. I want to be able to control my speed based on how far the throttle is pushed forward. Acceleration should be based on how fast you move the throttle.
```

---
## \#32 Posted by: TowerCrisis Posted at: 2019-05-09T06:11:27.044Z Reads: 28

```
Current control is exactly like a car.

If you lift a car up so the drive wheels are free wheeling, don't be surprised when the the idle spins them at 40 mph lol
```

---
## \#33 Posted by: huntercasillas Posted at: 2019-05-09T06:25:56.083Z Reads: 28

```
I have no control of my speed while riding, not only when the board is lifted and the wheels can spin freely. I can’t go half speed it always builds up to max current.
```

---
## \#34 Posted by: Anubis Posted at: 2019-05-09T13:47:59.778Z Reads: 17

```
A given point on my remote is a given current. When I want to stay at 10MPH, and I know that riding at 10MPH has resistive forces of x newtons, I have to find the current which exactly causes an equal and opposite force to appose that, hence I stay at 10MPH. Depending on your throttle curve, your remote may be too sensitive to do this. I have a GT2B casemod which has an INSANE throw, so I can easily maintain any speed. If you have like a nano-x or something, but a very powerful board, you're going to have difficulty getting that sweet spot.
```

---
