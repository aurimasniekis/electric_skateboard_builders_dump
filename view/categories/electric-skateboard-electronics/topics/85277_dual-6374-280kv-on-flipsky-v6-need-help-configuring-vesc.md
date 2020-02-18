# Dual 6374 280kv on flipsky v6, need help configuring vesc

### Replies: 1 Views: 168

## \#1 Posted by: mattfrancis Posted at: 2019-02-24T22:49:36.393Z Reads: 54

```
Hey guys, I need help configuring my vesc v6 with heatsink from flipsky. I have two 6374-280kv sensored motors. I'm running a 12S 20ah lipo, flipsky's nano-x receiver, and their bluetooth module. I can't get the bluetooth to work at the same time as the receiver. 15T motor pulley and 66T wheel pulley on 203mm wheels. 

The closest I got was having all the telemetry on the phone, but it causes one motor to stop when it connects to bluetooth. So I'm not sure why it's doing that. Both escs are on the latest same firmware. I did the motor set up for the master esc as a BLDC motor since I'm on 12S and set the baudrate to the specified one on flipskys site under the uart tab for bluetooth. I configured the slave esc to just copy the master (BLDC), but I keep getting a hall sensor error 255. So I swapped the hall sensor wires and kept getting the same error. 

Then I configured them as FOC, then redid the motor setup and set it as BDLC (saw somewhere online this was a trick). Now both motors turn, but the wrong way. When I swap motor direction in firmware to the correct way, the vesc shutsdwon. Tried old school wire swapping and it didn't like that either. So I'm not sure what to do. I want my bluetooth to work so I can get voltage / telemetry on my phone while I'm riding, also I want the smoothness of a sensored start. I also want to make sure I don't burn up my vesc. 

Any help is appreciated!
```

---
