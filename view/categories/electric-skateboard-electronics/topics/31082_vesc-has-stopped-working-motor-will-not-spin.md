# VESC has stopped working. Motor will not spin

### Replies: 6 Views: 940

## \#1 Posted by: repfea Posted at: 2017-08-20T04:37:29.101Z Reads: 126

```
Hi, I recently purchased my VESC from @chaka



----------
**The Problem**
I used it for approximately 6 or 7 rides and then I went into the BLDC tool to change the remote control max and min settings. Since I did not want the motor to spin, I unplugged one of the motor wires. Now it will not spin the motor at all. The VESC will still connect to the computer.

                                                                            
**Other information**

* I have tried both my Turnigy SK3 motor and my maytech motor so I do not think the motor is the problem.

* In the BLDC tool the VESC is getting signal from my remote.

* The VESC appears to boot up normally (blue and green lights are solid and red light flashes a couple of times and then turns off) 
* There is around 9 volts between the 2 motor wires on the VESC even hen there is no signal from the remote  

I do not want to void my warranty from Ollin Board but maybe I should reflash the firmware?
Thanks! :slight_smile:
```

---
## \#2 Posted by: darkkevind Posted at: 2017-08-20T07:00:06.889Z Reads: 115

```
Have you tried rebooting it? Have you tried writing the default config to it?

To not have the motor spin you need to set the current to disabled whilst you adjust the settings, then back to whatever your previous option was to write config.

Please check YouTube for "VESC settings" videos.
```

---
## \#3 Posted by: chaka Posted at: 2017-08-20T20:56:13.156Z Reads: 91

```
Do as much as you can to rule everything else out before sending it in for warranty/repair work. Be careful to upload the correct firmware and you shouldn't have any problems with reflashing using the bootloader. 

Double check all your connections and be sure you did not short anything or have a poor connection somewhere.
```

---
## \#4 Posted by: repfea Posted at: 2017-08-22T05:47:49.365Z Reads: 68

```
@chaka okay in BLDC tool i re-uploaded the firmware but that did not fix anything. Would giving the VESC throttle with one of the motor wires unplugged really mess it up?
Who should I contact about sending it back to be fixed and is there a was to expedite the process because it took a long time for me to receive it. 
Thanks!
```

---
## \#5 Posted by: chaka Posted at: 2017-08-22T13:15:07.831Z Reads: 66

```
Unplugging one of the wires can cause problems if it allows the phase wires to short circuit. It did work prior to you removing the phase wire so something did happen, our VESC's do not spontaneously fail. We test them rigorously to make sure our customers get a stable working motor controller. As long as the pcb is salvageable we will repair it! 

Send the motor controller to:
Ollin Board Company
PO Box 1340
Elephant Butte, NM
87935

Please be sure to add your personal information and a brief description of your build.
```

---
## \#6 Posted by: repfea Posted at: 2017-08-24T22:18:12.810Z Reads: 50

```
@chaka Okay I mailed it to that address (even though it is different from the address on your website) 

Is there someone specific that I should email the tracking number to and be in contact about the repair process??
Thanks!
```

---
