# Arctic Fox Remote Bluetooth 5

### Replies: 5 Views: 539

## \#1 Posted by: Sindre Posted at: 2019-04-30T09:39:46.213Z Reads: 141

```
I thought i could share my progress so far.

![white%20controller|407x500](upload://xyk1dUDYPLAyQUVbPFKG1kIdt92.png) 

Inspired by Adafruit, and SolidGeek:
https://learn.adafruit.com/bluefruit-nrf52-feather-learning-guide?view=all#downloads
https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543

![DSC02161|690x460](upload://vy7e6oIydIqLgsOApMakCnWVDvW.jpeg) 

Pcb is compadible with Arduino IDE and can be programmed over usb, jtag or over bluetooth.
Arduino compadible CODE can be found here:
https://github.com/Heplaphon/MountainX-Remote
https://shop-us.segger.com/J_Link_EDU_mini_p/8.08.91.htm

Follow setupguide from Adafruit:
https://learn.adafruit.com/bluefruit-nrf52-feather-learning-guide?view=all#arduino-bsp-setup

![Front|256x500](upload://uzpANwZXJvs7T0yhH5mhiOnoMQ5.png) 
![Back|236x500](upload://5WfcB0GmdOxk1ygNlhXdJJKNiDC.png) 

3D model of PCB can be found here:
https://github.com/kattemjau/MountainX-remote/tree/master/3D%20model

![controller%20wood|492x500](upload://pGLOZccPf8M9X54IuRQBi37qqKl.png) 

3D model of remote can be found here:
https://github.com/kattemjau/MountainX-remote/tree/master/3D%20model/V2

Images can be found here:
https://github.com/kattemjau/MountainX-remote/tree/master/Images

Note that V3 of the PCB have not yet been tested.


Features:

3 Hall sensors for more accurate readings, 
Nordic NRF52 Bluetooth 5, Arm Cotex m4,
Oled screen with telematry from Vesc: Speed, distance, battery voltage, error codes e.t.c, 
Remote battery reading, 
1A Fast charger, 
Long battery life, 
Dual battery to prevent battery disconnect due to shaking, 
Spring loaded knob and trigger, 
Deadmans switch, 
Opensource reprogrammable firmware with arduino IDE, 
Connects with up to 20 clients, long range and high bandwidth,


Its hard finding a good remote, so I started making one on my own, based on the FireFly remote. I had a couple of shady Chinese remotes, and heard about people having issues with evolve gen1 remotes. So this is a remote with a ARM Cortex m4 cpu with 3 hall sensors for a more accurate reading. It has full integration with the vesc, so its possible to get speed, distance, battery voltage e.t.c on the oled screen.

![Mechanics|351x499](upload://vCU4nN9dZ0rM35BpKIn61FlBB2v.png)
![image|360x500](upload://jWEVHaTd5vFMYne7nn8TwTUPPhR.png) 

Mechanic provides a tactile feel and a glove fiendly design. The design is really crude but feels comfortable in your hand. The 3D model needs some redesigning before finished version. Made in Fusion360.

All files can be found on the github: 
https://github.com/kattemjau/MountainX-remote
```

---
## \#2 Posted by: zsanderson61 Posted at: 2019-06-24T13:17:34.271Z Reads: 74

```
Do you have any working photos of version 3?
```

---
## \#3 Posted by: Sindre Posted at: 2019-06-24T13:55:39.228Z Reads: 71

```
Thanks for the intrest. Pcb's are ordered and I am awaiting them. I have alot of other projects atm but I will post updates when there is progress but it might be a while. V2 is working for its purpose, althought software is not yet on point
```

---
## \#4 Posted by: Deodand Posted at: 2019-06-24T22:18:47.635Z Reads: 55

```
Is Arctic (you are missing a C) intentionally misspelled?
```

---
## \#5 Posted by: Sindre Posted at: 2019-06-25T07:13:34.642Z Reads: 34

```
Hehe, its not intended. Ty for pointing it out
```

---
