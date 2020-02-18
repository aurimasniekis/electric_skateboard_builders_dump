# What causes VESCs to be fried in FOC vs. BLDC?

### Replies: 6 Views: 824

## \#1 Posted by: SOICDIP Posted at: 2017-12-24T14:10:16.461Z Reads: 192

```
Hey all, I've been reading about numerous reports about VESCs being fried in FOC mode, and if the damage isn't permanent, people suggest others to switch to stick to BLDC mode. 

[quote="elkick, post:9, topic:5263, full:true"]
VESC failures with FOC are not a manufacturing issue. 

It's a combination of motors (some fail, some don't under FOC), parameters in BLDC tool, cables (shorting them, length), bad solder joints due to vibrations, switching between FOC and BLDC with no reset to default values, using 12s sometimes causes that as well, and so on. Already wrote the in the FOC thread.
[/quote]



In this thread, everyone says it's user error (disconnected motors, long battery wires, not resetting parameters after switching from BLDC to FOC) but seems to me there are way too many VESCs being fried while in FOC mode.

[quote="JohnnyMeduse, post:3, topic:15651"]
I'm sorry but I don't think they have FOC in mind... since they clearly don't recommand to use it... It is not that you can't (any vesc can) it's just that you need to be more careful and know what you are doiing.  Also, The only VESC on the market right that as been design with FOC in mind, is the VESC-X from Enertion.
[/quote]



Also, why does Maytech not recommend FOC mode in its VESCs? I thought the BOM was very similar among VESCs.
```

---
## \#2 Posted by: FredSaberhagen Posted at: 2017-12-24T16:15:09.960Z Reads: 178

```
In BLDC you are slamming the FETs on / off as fast as you can.  This is a good idea, because FETs may be very low resistance when all the way on - but while they are transitioning from on to off (or vice versa) they are spending some nanoseconds in the "ohmic" region meaning they are dissipating a fuck lot of power.

Now for FOC you're kind of gently turning them on/off with an analog knob not a digital on/off switch.  This feels a lot smoother, sounds quieter, but is gonna burn off more power as heat across all your FETs.

So why is that burning up a DRV chip?  Well on a VESC all your FETs are right next to your DRV.   And your DRV itself has a lot of hot shit going down (for example, sourcing and sinking all that current to/from the FET gates) and that got less efficient as well!  

You can run a big ass FET hotter than the fires of hell and damnation... because literally all it is is a big chunk of metal.  The DRV Chip has a bunch of sensitive ICs including a bunch of analog circuitry, it straight up does not like to be hot.  FOC makes the DRV hotter from the outside and inside.  Thus, fried
```

---
## \#3 Posted by: ugothakd Posted at: 2017-12-24T16:58:59.991Z Reads: 156

```
I don't know if I buy that... To replace a drv chip hot air soldering is the preferred method, and that doesn't destroy the drv chip when the temps are much hotter than the fets usually ever get
```

---
## \#4 Posted by: emepror Posted at: 2017-12-24T17:53:34.589Z Reads: 150

```
Hot air soldering is a specific temperature for a short amount of time when the devices is off.

That being said FOC is more efficient vs BLDC (if its implemented properly) so technically the heating of the device is lower. It's a much more complicated operation to perform though, you cant just time the on off switch, now your creating a full sine wave with the FETs to drive the motor. 

I have a feeling that the reason FOC is much harder on the VESC is due to components, Board should be a bit bigger, more caps and larger traces. Thats just a quick potential reason.
```

---
## \#5 Posted by: SOICDIP Posted at: 2017-12-25T01:52:15.099Z Reads: 120

```
[quote="FredSaberhagen, post:2, topic:41816"]
In BLDC you are slamming the FETs on / off as fast as you can.  This is a good idea, because FETs may be very low resistance when all the way on - but while they are transitioning from on to off (or vice versa) they are spending some nanoseconds in the "ohmic" region meaning they are dissipating a fuck lot of power.

Now for FOC you're kind of gently turning them on/off with an analog knob not a digital on/off switch.  This feels a lot smoother, sounds quieter, but is gonna burn off more power as heat across all your FETs.
[/quote]

So if I'm reading you correctly, BLDC mode runs cooler because the PWM states either create an on or off state for the MOSFETs, whereas FOC mode puts the MOSFETs into the linear (triode) region to provide a smooth sine wave to the motor. 

That'll definitely run the FETs hotter, but it's interesting to see why people say FOC mode is more efficient. Seems like there would be a lot of loss in the FETs.

Is heat the only thing killing the DRV8302, or does FOC mode present a heavier load to the DRV? Higher transient voltages as well maybe?
```

---
## \#6 Posted by: FredSaberhagen Posted at: 2017-12-25T15:38:52.035Z Reads: 94

```
I haven't measured it so I'm not sure what the effect on voltage would be.  However meperor is likely also correct, but in a secondary or even tertiary sense... Your IC has some standoff voltage on all it's little switches - maybe that's 75V in perfect conditions - as you heat up your system it becomes harder to hold off voltage (Vds or drain-source voltage)  once you can't hold off that high voltage, that can cause a kaboom!

I think people thinking about efficiency gains in FOC are maybe thinking they get a little torque boost at lower speeds?  Due to gradually dialing in FETs vs. slamming them on/off.  Reason being trying to slam a FET on/off results in a very high di/dt - and change in currents is opposed by inductance, which your motor has lots of :slight_smile:

And yes remember the DRV Chip is dumping like 1A into the gate of your FETs, while also sinking 1A from those other FET at the same time- that gate current is totally passing through the DRV package - you want to minimize that duty cycle if you want to keep temps low!  What makes a FET efficient (low resistance or Rds_on) is simple - how big is your gate geometry?  You pay for space on a wafer basically.  Now imagine how big the FETs are *inside* the DRV chip.  They're fuckin tiny!  So they have a high resistance  (10s of mohm or more) and generate lots of heat.  Keep that duty cycle low OR try to pull heat out of that system some how
```

---
