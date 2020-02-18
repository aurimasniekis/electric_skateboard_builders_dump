# Short Circuit? My fuse fries at start up!

### Replies: 14 Views: 877

## \#1 Posted by: Vaulter92 Posted at: 2016-09-29T08:20:49.720Z Reads: 93

```
Hi guys...
Yesterday evening my board was suddenly slowing down and stopped even though my cell voltages have still been at 3.7 volts. So I charged everything again and wanted to start up today.
I have a 40 amp fuse installed which gets fried 2 seconds after the start up of the esc.
I am using a 6s setup, a trackstar ESC and a turnigy 6354 esk3 motor.
I think I might have a short but I am not sure. 
The problem occurs with 2 different battery packs which are both fully charged and balanced.

How do I determine if I have a short in the motor?
I checked my cabeling and it seems to be ok....no difference to the day before yesterday as I can recall...
```

---
## \#2 Posted by: TarzanHBK Posted at: 2016-09-29T08:45:58.105Z Reads: 88

```
at 6s you´re using much more than 40amps! get rid of that fuse!
```

---
## \#3 Posted by: Vaulter92 Posted at: 2016-09-29T08:48:19.311Z Reads: 84

```
But that worked for weeks. furthermore when I start up the ESC there is no load, right.
```

---
## \#4 Posted by: TarzanHBK Posted at: 2016-09-29T08:54:36.507Z Reads: 80

```
perhaps you didn´t draw more than 40 all the time. Just try it without fuse and check all your cables and stuff.
```

---
## \#5 Posted by: Vaulter92 Posted at: 2016-09-29T09:20:57.183Z Reads: 73

```
So, I disconnected the fuse and connected the track star (only) to a 3S battery. 
The track star started to smoke... So I guess there is a short circuit inside the ESC
```

---
## \#6 Posted by: Vaulter92 Posted at: 2016-09-29T10:23:07.859Z Reads: 71

```
Update: Seems to work again... more or less. Have 6s connected but the speed seems more like 3s. Does anyone here have experiences with the trackstar?
```

---
## \#7 Posted by: lowGuido Posted at: 2016-09-29T10:59:40.542Z Reads: 71

```
don't try it without the fuse. if the fuse is burning up there is a problem. solve the problem first.
check your ESC for a short
```

---
## \#8 Posted by: PB1 Posted at: 2016-09-29T12:17:31.301Z Reads: 67

```
Sorry @TarzanHBK, but the advice to try without a fuse was bad advice. 

A fuse is there to protect from overload. If it blows - there is too much current, overload. 
This normally means there is a problem. 

When the fuse blows without pulling the throttle it's probably not the motor. 
So probably ESC or BEC or receiver. 

Sorry, no experience with the trackstar.
```

---
## \#9 Posted by: TarzanHBK Posted at: 2016-09-29T12:25:07.534Z Reads: 66

```
a 40amp is definitely too low for a 6s system. And normaly you don´t use a fuse there. If just from a standard connection on startup without load causes smoke on the esc, i´d say that there is a big problem with it!
Like i said before, check everything and measure everything, before you fire up more things @Vaulter92! Sorry if i wasn´t clear that you do that before you try to connect something again to a smokin esc.
```

---
## \#10 Posted by: SORRENTINO Posted at: 2016-09-29T13:10:10.391Z Reads: 63

```
Use a multi meter to try and find the short. Definetely a short somewhere hence your fuse blowing. Most people build whats called a smoke stopper. It will light up if something is shorting. This way you dont ruin your electronics on new builds. I build mini drones so im accustomed to making sure there are no shorts anywhere.<img src="/uploads/db1493/original/3X/b/8/b8f96fedcef565bb55cd0bbbb108eea818cf7bb0.jpg" width="666" height="500">
```

---
## \#11 Posted by: SORRENTINO Posted at: 2016-09-29T13:17:00.208Z Reads: 62

```
EASY WAY TO CHECK MOTOR SHORT


So you overheated the wire by pulling too many amps and suspect the wire shorted to the stator. A clear indicator of this is that the motor will draw huge amps. Hopefully your ESC will cut out quickly or you are in danger of damaging your ESC and Battery. To test if your motor is damaged do the following:

    Setup a continuity meter or "Ohm Meter". Normally they will beep or show continuity when you touch the two leads to each other.
    Disconnect the motor from the ESC.
    Optionally remove the bell from the motor so you have easy access to the stator.
    Hold one meter lead to any of the three leads coming from the motor.
    Hold the other meter lead to the stator. The stator is the metal plates that the wire is wrapped around. Touch the side facing the magnets.

If you meter beeps, or shows continuity - you have a fried motor. You can fix the motor by rewinding it. But this requires knowledge of how to wind motors, time and materials to wind.
```

---
## \#12 Posted by: DeathCookies Posted at: 2016-09-29T13:18:31.580Z Reads: 61

```
Does it not burn when a ESC pulls much current on initial connection?
```

---
## \#13 Posted by: SORRENTINO Posted at: 2016-09-29T13:26:31.813Z Reads: 56

```
Your esc should not pull many amps at all when starting up. Its either your esc or motor. Most likely your esc imo since you should see smoke from the motor if the motor is shorted or see your windings burnt.
```

---
## \#14 Posted by: Vaulter92 Posted at: 2016-09-29T22:41:46.334Z Reads: 42

```
It's definitely the esc. The fuse was burned when the motor was disconnected. I'm running with half speed now and the switch that came with the esc can turn it on but not off. I find that very strange. Thank you guys for your comments. I will probably try to get a replacement from hobbyking.
```

---
