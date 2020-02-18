# VESC PPM input mapping

### Replies: 3 Views: 193

## \#1 Posted by: adeadsquirrel Posted at: 2019-09-22T07:20:45.359Z Reads: 56

```
Using Dual FSESC 4.20 Plus and VX1 remote and running FOC with 2 BLDC motors. 

I go to setup input > Master VESC > PPM RC receiver > PPM mapping. I also turned on RT app data as instructed. When I push and pull the throttle, no data is displayed on the "VESC Tool" and "From VESC" bars on the Pulselength section. Remote, receiver, and motors seem to work fine when I hit the throttle outside of the setup. I keep going to "General" to change "APP to use" to PPM instead of PPM and UART, but it doesn't save that option, if that's a relevant problem. Could be the firmware too. I don't know if I bricked the VESCs, but I have to keep manually rebooting to setup the input when it tells me the firmware is out of date, even though both VESCs are up to date on v3.61. Currently reinstalling VESC tool to hard reset any settings and see how that works out. Anteing else I should be aware of to resolve this issue?
```

---
## \#2 Posted by: pundahh Posted at: 2019-09-22T19:02:37.843Z Reads: 24

```
is your receiver plugged in through uart or ppm? 

you also have to click 'write app settings' in order to save the options.
```

---
## \#3 Posted by: adeadsquirrel Posted at: 2019-09-22T20:22:40.441Z Reads: 21

```
Fixed the problem. I was previously using the reciever cable included with the remote. Switched to the ppm cable with 3 pins coming out of the vesc and it seems to have resolved it. Ty
```

---
