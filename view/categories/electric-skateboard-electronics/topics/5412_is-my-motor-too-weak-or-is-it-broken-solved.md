# Is my motor too weak or is it broken? SOLVED

### Replies: 5 Views: 1185

## \#1 Posted by: edwardlui531 Posted at: 2016-07-01T08:06:07.684Z Reads: 153

```
I just got my first ever vesc hoping it will solve my jittering problem
 so I just follow online tutorial on setting up the vesc
it still jitters a lot when I feather the trigger 
video is showing how there is no torque on current mode
duty cycle mode actually give me decent torque but it seems to be braking when I don't pull the tiger. 
Is there more I need to config if I want to use current mode?
I am running 6s and I am not sure what kv is the motor, is there a way to find out using bldc tool?
Sorry about my disgusting finger nails. 
https://youtu.be/A0XGKK-CsRU
```

---
## \#2 Posted by: treenutter Posted at: 2016-07-01T14:36:23.544Z Reads: 121

```
@edwardlui531 In my experience with VESC, that is normal behavior. The motor toggles like that at low speed. I believe it does this on sensorless motors so that it can find it's starting point before more torque is added to achieve a smooth start (this is a rudimentary and potentially inaccurate description). Have you tried it off of the bench yet?
```

---
## \#3 Posted by: edwardlui531 Posted at: 2016-07-01T16:40:05.373Z Reads: 105

```
I tried it off the bench and the torque is so weak it won't go from standing still. I am going to try riding with duty cycle now.
```

---
## \#4 Posted by: Blasto Posted at: 2016-07-01T18:09:57.364Z Reads: 97

```
In the video that happens because you are bench testing and probably are sending a 4-5A max command to the vesc, meaning it will stall pulling a max of 4-5A. In real life, if you are full throttle and sending a 30A command, believe me you won't be able to stall the motor, you'll polish your finger

duty cycle mode can lead to the death of your vesc.

keep it in current control, make sure all you setup setting are good, motor max-min, batt max-min-absmax, your max erpm at 70000.

in your case stick with

motor max: 60A
motor min: -60A
batt max: 30A
batt min: -20A (or less)
absolute max: 120A


Max ERPM: 70 000

set your battery cutoff start and end.

in the app configuration, set to "current no reverse with brake"
```

---
## \#5 Posted by: edwardlui531 Posted at: 2016-07-01T22:03:59.854Z Reads: 79

```
Huge thanks to Blasto who sold me his vesc and walk me through the vesc setup. Will do more config later on when I fix my motor.

As for the solution, I just crank up the startup boost on the advance tab on motor config
```

---
