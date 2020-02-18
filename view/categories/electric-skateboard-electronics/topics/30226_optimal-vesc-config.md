# Optimal vesc config

### Replies: 5 Views: 480

## \#1 Posted by: florensvb Posted at: 2017-08-10T08:06:49.806Z Reads: 108

```
Hey guys,

I have read tons about how to configure the vesc and I can say that I have achieved that, because my build runs well. But anyways, some things remain not too clear to me:

For example I know that my motor has max 60 amps, so is it wise to set it to 60 or should i go a bit lower for safety? I also know that my motor is rated at max 8S (which I have), so i am worried that if I set it to 60 amps and i have a full battery pack going down a hill, it will hit ERPM and blow my foxbox?

Also, i don't seem to be able to figure out what the max charging of my battery is for the regenerative breaking settings. 

_Motor:_ [Electric-skateboard-motor-5065-260kv](diy-electric-skateboard-kits-parts/electric-skateboard-motor-5065-260kv/)

_Battery:_ [Zippy-flightmax-8000mah-4s1p-30c](https://hobbyking.com/en_us/zippy-flightmax-8000mah-4s1p-30c.html?___store=en_us) 

Do you think battery sag is a problem with 8S2P?

I do not have a BMS.

And i use the FOCBOX as a controller. 

I am just interested in your opinions, as to what you think are the optimal settings for 
_Motor Max, Motor min (regen), Batt min (regen)_ and also what do you guys suggest as a _Battery cutoff end_ in order to preserve battery life but still get a descent mileage in? 

Thanks so so much! :kissing_smiling_eyes:
```

---
## \#2 Posted by: Der6FingerJo Posted at: 2017-08-10T10:52:32.680Z Reads: 87

```
I'm not too sure about the particular motor, on 10S with my SK3 motor I barely hit half throttle when cruising at 15 to 20 km/h so I just keep it at 60A and don't go crazy on the throttle all the time. 
I also use lipos without BMS and I make sure to never start my ride downhill when fully charged. Generally regenerative braking isn't an issue as long as you can monitor your voltage during the ride. 
If I start downhill I charge them to only 4.10V per cell so that  i won't overcharge while breaking on the first part of my ride.  Depends on your chargers abilities though, I use an ISDT 500W charger.
I mostly cut off at around 3.7 to 3.8V per cell and have my bat min set to -10A with 5000mAh cells.
```

---
## \#3 Posted by: florensvb Posted at: 2017-08-10T13:23:44.201Z Reads: 71

```
Thanks a lot for your input! Unfortunately my charger does not let me choose the voltage. 

I do have a battery indicator, but it shows in %, not in V. 

Isnt 3.7V like half the charge? I thought it should be set to like 3.3V - 3.4V ? I mean isnt it empty really quick from 4.2 to 3.8 Volts?

Also, what is the difference between motor min and batt min? 

Cheers!
```

---
## \#4 Posted by: florensvb Posted at: 2017-08-10T15:00:50.316Z Reads: 54

```
Oh you probably mean _battery cutoff start_ instead of _battery cutoff end_ ?
```

---
## \#5 Posted by: Der6FingerJo Posted at: 2017-08-10T15:09:03.563Z Reads: 49

```
Basically yes, however ending your trip at 3.7V is playing it safe. But i wouldn't go lower than 3.5V for maximum battery health.

Theoretically Lipos can go down to 3.3V per cell or so, but it's only healthy for them if you discharge at a slow rate. Since E-boards do draw a bit i'd recommend 3.5V. 

As for battery indicators, monitoring individual cells would be the best thing. But a real voltage number to read out would also be ok and it's what i use. You could use a little lipo checker for this.
```

---
