# Custom VESC 6 for robot

### Replies: 9 Views: 331

## \#1 Posted by: b4zz Posted at: 2019-01-02T15:39:35.756Z Reads: 120

```
I'm currently in the proces of customising a VESC 6 design for usage in a robot. The idea is to create a Dual VESC eventually. But first I would like to design a single Vesc to test. 

Maximum motor current will be around 20 amps and 10 amps continuous. I've left out the NRF24L01P and MPU9150 since we won't be needing those. Eventually all communication will go over CAN, but for now I left the ppm(or pwm) input for testing purposes. 

Below you'll find the schematics. I've designed the PCB as a two layer pcb and made the design in Eagle, if there is any interest the brd and sch can be shared. 

Could the more advanced designers take a good look and let me know if there are any weaknesses or point of attention in the design?

**Board design**
![Dual_motor_controller_v2|690x444](upload://lVb4AKI0iVQ7zA11uJfmENJml72.jpeg) 

**MCU**
![CAN|690x487](upload://anV2HWIVBDsV2534C9ip3c24Mdn.jpeg) 

**DRV8301**
![drv8301|682x499](upload://zQ3NmHDwbAyZlhfs3txR8IxvDXF.jpeg) 
**Motor FETs**
![Motor_fet|690x354](upload://ffqpglnSW8knTwLWdX83UzPziWu.png) 
**Can COMM**
![can|482x353](upload://86dEoVIijfVe5A25ZKqNRYWMMK6.png) 
**Hall COMM**
![hall|690x466](upload://yfglQjcIu0eNE3fk9q9kMbyhoac.png) 
**External connections**
![ext_comm|473x500](upload://r3NvxzpNVEFV7MBbZajFrzhAqDs.png)
```

---
## \#2 Posted by: Skunk Posted at: 2019-01-02T15:57:19.788Z Reads: 103

```
Robots you say?
@DerelictRobot
```

---
## \#3 Posted by: b4zz Posted at: 2019-01-03T09:32:30.648Z Reads: 65

```
Yes it's a self driving robot, the Vesc will be used to control overboard wheels ~350watt.

And the used mosfets are: NVMFS5C604NLAFT1G since they have more than enough current capability while still remaining quite small, and are easier to solder than the direct fets.
```

---
## \#4 Posted by: b264 Posted at: 2019-01-03T10:50:43.969Z Reads: 52

```
What supply voltage will this be operating at?  What are the reliability requirements?
```

---
## \#5 Posted by: b4zz Posted at: 2019-01-03T11:00:15.929Z Reads: 47

```
A 7S12P battery will be used to power the system, so 21-29,4V. 

Tha system should be very reliable since it will be eventually used in a production environment.
```

---
## \#6 Posted by: b264 Posted at: 2019-01-03T11:08:29.814Z Reads: 42

```
What firmware will be used?  Will it be custom and closed or a GPL Vedder variant?
```

---
## \#7 Posted by: mishrasubhransu Posted at: 2019-01-03T11:13:27.884Z Reads: 39

```
As someone who first stated using VESCs on robots(then esk8), I wonder what is the reason for making your custom VESC: reduce cost, gain design experience(& hence potential for improvements), improved specs?
```

---
## \#8 Posted by: b4zz Posted at: 2019-01-03T11:33:40.182Z Reads: 36

```
At first Vedder's variant will be used for testing, later this will be customised to suit our needs.
```

---
## \#9 Posted by: b4zz Posted at: 2019-01-03T11:34:28.930Z Reads: 35

```
Mainly to create a Dual VESC that will be integrated with the controller board already in the robot. This will reduce costs and build time.
```

---
