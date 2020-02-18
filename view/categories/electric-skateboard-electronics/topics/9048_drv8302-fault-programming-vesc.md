# DRV8302 FAULT Programming VESC

### Replies: 8 Views: 1276

## \#1 Posted by: robskie Posted at: 2016-09-06T11:14:34.954Z Reads: 91

```
Hi guys, I'm giving programming my VESC a shot atm, and whenever i'm at the realtime data tab, and I try to use my remote to power the motor, i get the DRV error. The motor nudges just a little bit, stops, and I can do the same thing around 5 seconds later and the same thing will happen. I was watching the ESK8 support video, he says this might be due to a faulty driver/ VESC, but he didn't really give a solution, what should I do?
```

---
## \#2 Posted by: bigpianist Posted at: 2016-09-06T12:06:45.712Z Reads: 79

```
Hey mate, check your advanced tab for the Max current ramp step. If it's at a value higher than .04, you have the current ramping bug which can kill your VESC. See >>http://www.electric-skateboard.builders/t/vesc-faq-firmware-bug-pre-august-2016-please-upgrade/8018   and      http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262
```

---
## \#3 Posted by: robskie Posted at: 2016-09-06T12:34:42.262Z Reads: 77

```
Tried changing up the numbers to 0,004, it went up to 0.04 like the post said, still get the same error, motor still just nudges and stops working. Anything else I should try?
```

---
## \#4 Posted by: bigpianist Posted at: 2016-09-06T12:35:42.517Z Reads: 72

```
What motor are you using? are trying a motor detection?
```

---
## \#5 Posted by: chaka Posted at: 2016-09-06T12:55:14.250Z Reads: 69

```
Fyi, I have never been able to kill a driver due to this bug.  @robskie you can try checking your phase wires to make sure you have a good connection but it sounds like you might need to replace the drv chip or check for bridged legs. Could also be a bad solder joint somewhere else on the circuit.
```

---
## \#6 Posted by: robskie Posted at: 2016-09-06T13:11:18.134Z Reads: 64

```
http://alienpowersystem.com/shop/brushless-motors/alien-5065-outrunner-brushless-motor-270kv-2200wa/
And it says detection failed when I try to detect the motor
```

---
## \#7 Posted by: bigpianist Posted at: 2016-09-06T14:40:55.752Z Reads: 55

```
Does the motor still move at all? If not you've probably killed you DRV chip by now. It's quite a frustrating issue. 
If your motor does still move but nudges, you may need to change your motor detection settings (higher eprm helped my working one)
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2016-09-06T15:04:27.658Z Reads: 50

```
Do you have any picture ? What type of battery are you using ? What version of the BLDC tool, (have you download it recently, there was problem in the version that was available in July) ? Have you configure the remote ?
```

---
