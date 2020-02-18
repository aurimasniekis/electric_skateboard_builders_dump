# Unknown hall error: 255 on sonsorless motor

### Replies: 6 Views: 306

## \#1 Posted by: JasperM Posted at: 2018-08-01T05:59:48.024Z Reads: 68

```
I have had some problems with my battery a while ago but I can't see any serious damage to cells and have reconnected everything and ran motor detection, it detected the motor but also says 'Unknown hall error: 255.'

I am running an SK3 in sensorless mode, am I missing something?

Thanks in advance for any help.
```

---
## \#2 Posted by: Rod12579 Posted at: 2018-08-01T07:34:54.906Z Reads: 56

```
Had this same thing happen to me but using a TB 6374 motor running in bldc, I contacted TB & they told me this was normal but yet it was only happening on one motor.🤨...the motor did run fine in BLDC... but I was unable to get a sensor detection in FOC on that same motor (failed) I ended up replacing the motor because I wanted to run FOC & sure enough the new motor had a good sensor detection in FOC  I didn’t try it in bldc yet so I suspected the old motor had a faulty sensor not sure if this is your same issues but try the sensor detection in foc & see if you get any sensor reading.
```

---
## \#3 Posted by: dareno Posted at: 2018-08-01T07:38:30.728Z Reads: 55

```
I had a similar thing too, motor locked and when I ran detection came up with unknown hall error. I'm running sensored.  disconnected the sensors set unsensored in the vesc tool and now its running fine.  The detection still came up with hall error though.
```

---
## \#4 Posted by: Silverline Posted at: 2018-08-01T08:11:17.951Z Reads: 43

```
Sk3 is without sensors. So you can't detect something that is not there. You need to run bldc or foc detection and choose "sensorless"
```

---
## \#5 Posted by: JasperM Posted at: 2018-08-01T08:12:47.733Z Reads: 37

```
I have selected sensorless but it still says the error.
```

---
## \#6 Posted by: Silverline Posted at: 2018-08-01T08:13:21.252Z Reads: 37

```
That is Strange :-/
```

---
