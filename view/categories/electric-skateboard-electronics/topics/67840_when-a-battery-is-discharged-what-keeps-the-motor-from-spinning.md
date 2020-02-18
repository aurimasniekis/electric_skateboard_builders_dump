# When a battery is discharged what keeps the motor from spinning?

### Replies: 12 Views: 237

## \#1 Posted by: Harp Posted at: 2018-09-12T20:30:16.176Z Reads: 102

```
When I'm riding my longboard and suddenly the motor stops providing force I know that it's out of battery. In this state what about the battery keeps the motor from running? Is it the because the voltage or the current is low?
```

---
## \#2 Posted by: dareno Posted at: 2018-09-12T23:25:46.059Z Reads: 78

```
:notes:There may be trouble ahead...........:notes:
```

---
## \#3 Posted by: AlexBE Posted at: 2018-09-12T23:28:52.747Z Reads: 77

```
The BMS (battery management system) has detected that the voltage is too low and turned off the switch between the motors and your board. Most likely.
```

---
## \#4 Posted by: Harp Posted at: 2018-09-13T00:12:58.630Z Reads: 71

```
are you ok
```

---
## \#5 Posted by: dareno Posted at: 2018-09-13T00:18:44.689Z Reads: 68

```
Li ion/lipo batteries have a low voltage cut off because if they discharge too much they are history.  Your esc and indeed the bms will cut off the battery to protect from this.  Please excuse my humour it is not sometimes in sync with the rest of humanity.   What board do you have?
```

---
## \#6 Posted by: TowerCrisis Posted at: 2018-09-13T00:24:48.181Z Reads: 64

```
Electrically speaking there's nothing stopping the motor from spinning. It will continue to slowly decrease in speed until the battery is at 0V and the motor won't have any electricity.

But draining the battery to 0V will destroy it. It will not be able to recharge.

SO lipo batteries can only be operated in the 3.3V - 4.2V range. Your electronics in the board will not power the motors (or possibly will shut off completely) once the cell voltage has reached 3.3V (or whatever they specify, it varies)
```

---
## \#7 Posted by: Harp Posted at: 2018-09-13T00:30:55.524Z Reads: 56

```
It's a custom build. Turnigy G160 motor, FVT 120A ESC, and an 18 V battery
```

---
## \#8 Posted by: TowerCrisis Posted at: 2018-09-13T00:41:25.438Z Reads: 53

```
You should probably get one of these and program it https://hobbypartsusa.com/lcd-program-card-for-fvt-car-esc-s.html/

I can't seem to find what the default cutoff voltage is for that ESC. If it's too low then that could be a problem, you don't want it lower than 3.2V. If it is below 3.2V you're currently over discharging your cells.

I'll keep searching for the defaults online.. Will post back with results


It looks like by default you can only use 50% brakes.

It's got a 9% deadband by default, which is way too high for our usage.

It also is unable to properly determine what cell count your battery is using. 18V isn't within any of the voltages it can use to guess what cell count. You need to program it in.

It's possible that this motor controller is running your battery beyond dry, or it has lots of capacity left even after it shuts off. But you have no clue unless you use a programming card to input the data yourself.

I wouldn't ride with this for an extended duration without recharging, and I'd NEVER run it dry without knowing what it's doing. Please get a program card for it.
```

---
## \#10 Posted by: Harp Posted at: 2018-09-13T23:27:17.272Z Reads: 25

```
The batteries that I’m using are Li-ion batteries so how would I know what to set as the cutoff voltage? Specifically, they’re power drill batteries. The reason I’m using them is that I had them lying around and I knew it would be easy to strip the charger and have it built into the longboard. Do these batteries have their own cutoff system built in?
```

---
## \#11 Posted by: TowerCrisis Posted at: 2018-09-14T00:20:02.189Z Reads: 22

```
I'm very unsure of that.

I know that lion drills will shut off instantly once they reach cutoff voltage. The control circuitry could be inside the drill, or it could be the battery. Look up the specs and details of your battery.
```

---
## \#13 Posted by: Harp Posted at: 2018-09-14T01:40:09.885Z Reads: 19

```
I couldn’t find anything about the control circuitry on the batteries but that might not matter because apparently, the programming software for this ESC supports lion batteries. This was stated in a configuration video: https://youtu.be/8gfUVjBnxKk?t=6m53s

Would this mean that the ESC will know the cell count for this lion pack and be able to accurately cutoff based on the voltage/cell.

Sorry for all the replies but this issue has been bugging me for a while.
```

---
## \#14 Posted by: TowerCrisis Posted at: 2018-09-14T01:52:35.203Z Reads: 18

```
have you programmed it or is it all the default settings?

If it's the default there may be problems. Just make sure you program it yourself and verify settings.
```

---
