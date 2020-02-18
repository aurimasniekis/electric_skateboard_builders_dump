# Maytech VESC (4.12) 12S Motor Cutouts at high loads

### Replies: 11 Views: 537

## \#1 Posted by: jnortheast Posted at: 2019-01-16T13:34:22.338Z Reads: 115

```
Hey!
I just built a custom Electric Skateboard with one MOTOR 6355 190KV from  and a Maytech BLDC SUPER ESC 4.12 from Ebay. I had a TORQUE ESC but I blew it when the motor wires came disconnected and shorted, so I ordered another one from  but since they take 7-10 days to ship to Australia, i thought I might try a Maytech VESC from a local ebay seller.
 
So i connected it all up to my 12S lipo (2x ZIPPY COMPACT 2700MAH 6S 25C LIPO in series) and added in a handy loop key switch and programed it the same as i did for my TORQUE VESC with the default Motor Amp limits (60A + -60A) and with Battery Current Max to 35A and Regen at -5A. Connected the controller and set it up the same as i did before and it was done. Then when i rode it, for the first 2 minutes of riding and quickly accelerating the motor would cut out and a red light on the VESC would flash, receiving a FAULT_CODE_DRV upon checking the faults in the VESC tool. The errors generally look like this : 

> Fault            : FAULT_CODE_DRV
> Current          : 49.8
> Current filtered : 44.5
> Voltage          : 46.26
> Duty             : 0.185
> RPM              : 9567.0
> Tacho            : 26135
> Cycles running   : 26523
> TIM duty         : 3154
> TIM val samp     : 1577
> TIM current samp : 10122
> TIM top          : 17090
> Comm step        : 3
> Temperature      : 33.05

The red light would only flash for a second and i would then regain control of the motor, until i would quickly accelerate again and it would happen again. However, it would only happen for the first few minutes of riding, as if it were "warming up" and then it would ride perfect, no cutouts at high load. 
I removed the sensor wire from my vesc and reconfigured the vesc to run sensorless BLDC and it did reduce the occurrence of cut outs interestingly enough, but they still none the less occurred withing the first few minutes of riding.
I then played with different current limits for both the motor and the battery and I think I have found a stable configuration as of my last ride, but im expecting once i let the board cool down again and jump back on it will start cutting out again. 

![image|690x247](upload://6e2u8rc47xNy9CO5FKFtqzJx2uP.png) 

![image|690x463](upload://kXr1lRTqGcYMydV2Fo7hMXpUVxw.png) 

Is there anything in these settings that stands out to any of you guys? 

I've tried moving the remote receiver as to not let the vesc interfere with it and it made no difference, so that rules out controller disconnection. 
I do have the vesc in a zip lock bag with holes in it temporarily velcrowed under my board until i can build an enclosure for it, maybe the lack of air flow is affecting it?
Maybe 12s is too much for the vesc to handle, so that would mean buying two new 5s batteries to build a 10s to see it that is the issue, but i'd rather not spend more on this build. I could try running the batteries in parallel at 6s, but wouldn't I get alot less speed by doing that?
Is it possible that when i shorted the previous vesc i damaged the motor and that is what is causing this issue?

Any ideas or suggestions would be greatly appreciated.
```

---
## \#2 Posted by: tardyparty7 Posted at: 2019-01-16T18:32:57.559Z Reads: 88

```
[quote="jnortheast, post:1, topic:81055"]
I had a TORQUE ESC but I blew it when the motor wires came disconnected and shorted, so I ordered another one from [](http://) but since they take 7-10 days to ship to Australia, i thought I might try a Maytech VESC from a local ebay seller.
[/quote]

this could be the problem, maybe u broke the motor somehow.
```

---
## \#3 Posted by: mynamesmatt Posted at: 2019-01-17T01:56:29.007Z Reads: 81

```
hey bro, it's great to see more fellow Aussies on this forum. 
Now, vesc 4s are known to not be super stable on 12s purely due to their hardware and design. 10s is pretty well their sweet spot. I think the best test (like you said) would be to wire the batteries in parallel to see if the error still occurs. if it doesn't that they vesc can't hack 12s. another good test would be testing continuety between the phases of your motor. (there's a thread on how to do that somewhere on here).
drv error usually means the esc is fucked so
```

---
## \#4 Posted by: jnortheast Posted at: 2019-01-17T04:23:22.028Z Reads: 74

```
Hey @mynamesmatt, Were abouts in Aus are u?
Do you think I would loose much performance going to 6s?
```

---
## \#5 Posted by: MysticalDork Posted at: 2019-01-17T04:31:52.558Z Reads: 71

```
@jnortheast  You will lose half your speed and 3/4 of your power. Current is directly related to voltage, and power is voltage times current. So half the voltage gives you half the current, and thus half the voltage times half the current, gives you 1/4 the power. 

I'd recommend you either get a vesc based on 6.xx hardware, or switch to a 10s battery.
```

---
## \#6 Posted by: jnortheast Posted at: 2019-01-17T04:37:13.668Z Reads: 69

```
@MysticalDork That makes sense. 
Would you recommend a Flipsky 6 VESC - https://flipsky.net/products/fs-esc-6-6
```

---
## \#7 Posted by: MysticalDork Posted at: 2019-01-17T04:53:27.988Z Reads: 70

```
I don't know, I've never used it. I went straight from a stock 4.12 all the way to a pair of trampa vesc6. (which are AWESOME btw, just really expensive) I'd say go for it!
```

---
## \#8 Posted by: mynamesmatt Posted at: 2019-01-17T07:38:51.015Z Reads: 57

```
@jnortheast hey man, I'm down in kenthurst, about 40min nw from Sydney. And yes, with 6s you will lose speed and range. with lower voltage the motors need more current to push the load. If you know someone with a power supply, see if you get the drv error at 34-42 volts. Ik its hard to replicate bc you get the error under load but give it a shot.
If you have higher kv motors handy then plug them in and you should get a bit better performance. something like 270kv would be fine
```

---
## \#9 Posted by: lrdesigns Posted at: 2019-01-17T09:00:42.525Z Reads: 53

```
I have been running maytech 4.12 on 12s for two years without any problems. Though my motors are smaller and my battery amps is only 12amps. So maybe that is it. 

I use BLDC mode. Have quite short wires from battery to vesc. 5065 140kv motors, 2:1 gearing on 97mm wheels. 

Dont use FOC on these it will kill them. 

The fact that the behaviour changes once warmed up makes me think yours might be very slightly faulty, like a bad solder joint on one component. 

That or you're just pulling to many amps. :man_shrugging:

![image|620x374](upload://klfDoeTf2Coq2VFn92bkoMDY3zQ.png)
```

---
## \#10 Posted by: jnortheast Posted at: 2019-01-17T09:16:36.755Z Reads: 48

```
Hey @lrdesigns,
What's the Max speed you have had your board up to with these settings. 
And something fundamentally that I don't understand is how can the motor receive 65A but the battery is limited to 12A? I don't get how these two settings interact.
Cheers :)
```

---
## \#11 Posted by: lrdesigns Posted at: 2019-01-17T09:23:15.251Z Reads: 46

```
45kph. Dual motors by the way so x2 the settings.

At slow speeds the voltage the motor recieves can be quite low. Say 10 volts, the vesc can deliver 50amps to the motor for at total of 500 watts of power. While only drawing only 10 amps from the battery at 50 volts for a total of 500 watts. 

As you speed up it evens out. 

So motor amps has more impact at slow speed.  

Battery amps is kind of like a limit on total system power.
```

---
