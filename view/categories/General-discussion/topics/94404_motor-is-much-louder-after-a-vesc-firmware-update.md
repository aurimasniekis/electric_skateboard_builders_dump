# Motor is much louder after a vesc firmware update

### Replies: 8 Views: 309

## \#1 Posted by: The_Strij Posted at: 2019-05-20T08:27:33.911Z Reads: 115

```
Hello all! I am fairly new to this so any help will be great!
I am running a 12s2p battery with a 4.12 vesc and a 190kv torqueboards motor. Everything has been running smoothly until I updated the firmware on the vesc to 3.57. I'm not sure which it was on previously but the vesc tool app told me to update. After that the motor is lurching on start from standstill and is making a high pitch noise when running that it didn't previously. Any ideas?
```

---
## \#2 Posted by: McErono Posted at: 2019-05-20T08:30:30.754Z Reads: 114

```
Sensors ok? Sounds like you've been in FOC mode and now BLDC mode?
```

---
## \#3 Posted by: The_Strij Posted at: 2019-05-20T08:32:26.545Z Reads: 109

```
Which sensors? Like the hall sensors?
```

---
## \#4 Posted by: McErono Posted at: 2019-05-20T08:33:36.692Z Reads: 106

```
Yes. Sensored FOC mode would start smooth and quiet. BLDC unsensored louder and stutters from standstill.
```

---
## \#5 Posted by: The_Strij Posted at: 2019-05-20T08:37:42.917Z Reads: 102

```
When I run the motor detection it says "Hall sensors" under the sensors area. Do I need to change a setting manually?
```

---
## \#6 Posted by: bluegreen Posted at: 2019-05-20T08:50:48.914Z Reads: 91

```
When you reinstalled the firmware, did it do a motor detection? If it did so with the belt connected then this could be the problem. Motor detection should be run without the belt.
```

---
## \#7 Posted by: egzplicit Posted at: 2019-05-20T09:23:38.458Z Reads: 80

```
You are running BLDC and not FOC. It happened to me the other day, upgrade firmware, redid motor detection via wizard but for some reason it was in BLDC mode. Cogging from stand still and sounded like a rocket.

Check via the VESC Tool and make sure both vescs are running in FOC.

Not sure why the wizard leaves the control mode to BLDC...
```

---
## \#8 Posted by: The_Strij Posted at: 2019-05-20T18:25:53.266Z Reads: 43

```
That did it! Turns out I was in BLDC mode not FOC.
```

---
