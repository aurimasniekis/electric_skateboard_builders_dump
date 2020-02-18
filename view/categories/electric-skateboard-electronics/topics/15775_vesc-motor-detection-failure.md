# VESC motor detection failure

### Replies: 1 Views: 622

## \#1 Posted by: Eckles Posted at: 2017-01-08T01:47:52.952Z Reads: 77

```
Hey guys, quickly let you know my setup:
 **12s3p Li-ion** 
 **x2 170kv Motors**
 **x2 VESC 4.12**
  So my board was working fine but I had a problem where my SLAVE VESC kept cutting out during use, I managed to pinpoint the problem as a bad contact on the cable from the capacitors going into the VESC. It had come loose and under vibration would disconnecct causing a spark then would reconnect once repositioned, I re-soldered this contact and the disconnection problem stopped. 

My problem still is doing a motor detection, I keep receiving "Bad Detection Result Recieved" message. When I type "Fault" or "Faults" in the terminal page it tells me "No faults registered since startup" or "FAULT_CODE_NONE". On top of this the LED lights are functioning as normal and when I use the directional keys within BLDC Tool the lights change accordingly but with no movement from the motor.

 I have tested this motor on my MASTER VESC and it works fine so it rules out motor troubles. I then re-flashed the firmware on the SLAVE VESC but im still unable to run a motor detection. When I "Activate Sampling" in the Realtime Data tab I get seemingly normal responses in the graphs but nothing from the motor.

  After re-flashing the firmware all my settings are Default Settings for VESC 4.12/Firmware 2.52. 

Is there something more I can do to figure out the problem? Anyone got suggestions as to what this is?
```

---
