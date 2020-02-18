# VESC fault code ABS_OVER_CURRENT

### Replies: 20 Views: 524

## \#1 Posted by: affeandersson Posted at: 2019-03-08T22:51:36.925Z Reads: 109

```
Im in the process of building my first electrc skateboard so I am new to this. Everything was working perfectly until I brought the board outdoors for the first test when the motor just would not spin. I took it back inside and the vesc gave me fault code ABS_OVER_CURRENT and i could not get it to work, even after tweaking the current settings (Running in FOC btw). After letting the board sit over night I tried to re-configure the motor and it works perfectly again for a couple of minutes and then the motor stops spinning and i get the same fault code again.

![image|430x257](upload://nm0OA3dbXURCJkmnydl1fkvRbU3.png) 

This is the latest fault code I got and here are my settings:

![image|690x215](upload://idaWlcookRHlSvcE0t2i6Fzo18U.png) 
![image|690x352](upload://6EimzRENDlhu1vM0PNpJjSLRcNv.png) 

Currently i get the fault code while trying to measure the flux linkage, that is why it is set to 100,000 mWb.

Setup:</br>
Flipsky VESC 4.12 </br>
Flipsky 6374 190kv 3250W</br>
12s battry
```

---
## \#2 Posted by: Jarno Posted at: 2019-03-08T22:53:09.089Z Reads: 99

```
What VESC do you have?
```

---
## \#3 Posted by: affeandersson Posted at: 2019-03-08T22:55:34.366Z Reads: 97

```
Sorry, its a Flipsky esc 4.12
```

---
## \#4 Posted by: Jarno Posted at: 2019-03-08T22:59:29.182Z Reads: 94

```
4.12 hardware is not so good with FOC, some faults with bad capacitance choosing and FET choise . 
Go and try BDLC.
```

---
## \#5 Posted by: affeandersson Posted at: 2019-03-08T23:00:39.996Z Reads: 93

```
Im having the same problems with BLDC. I will go test again and come back with results
```

---
## \#6 Posted by: affeandersson Posted at: 2019-03-08T23:04:30.907Z Reads: 94

```
While trying to detect the motor in BLDC:

![image|443x262](upload://rJq12ZE7XO1erx5n51KDLpYASsk.png) 

I still have the same current settings. The motor twitches once and then the vesc blinks red, nothing happens for a couple of seconds then the motor freaks out.
```

---
## \#7 Posted by: pjotr47 Posted at: 2019-03-08T23:07:08.706Z Reads: 91

```
Set absolute max current on 120A and you are ready to go. I had 90A on my focbox and also had over current. After I switched it to 120A (default setting) the fault was gone. 

Btw: run your vesc in blcd
```

---
## \#9 Posted by: affeandersson Posted at: 2019-03-08T23:14:01.018Z Reads: 92

```
And also, according to the real time data, the vesc (or motor?) is drawing ~0.1A while not doing anything... Is that normal? Since i dont remember it doing that in the beginning?
```

---
## \#10 Posted by: affeandersson Posted at: 2019-03-08T23:20:00.314Z Reads: 90

```
@pjotr47 This is in bldc with abs max current set to 120A

![image|430x261](upload://v7TdGTmTMauILWOCT2n8Jr0lFvi.png)
```

---
## \#11 Posted by: pjotr47 Posted at: 2019-03-08T23:59:13.496Z Reads: 79

```
Do you have a fault code while motor detection?
```

---
## \#12 Posted by: mynamesmatt Posted at: 2019-03-09T00:11:59.794Z Reads: 75

```
then try absolute max at 130 or 140a
```

---
## \#13 Posted by: affeandersson Posted at: 2019-03-09T05:42:28.365Z Reads: 72

```
Yes that one is from the detection
```

---
## \#14 Posted by: affeandersson Posted at: 2019-03-09T05:43:30.061Z Reads: 72

```
Is it really that easy? Sounds like I could just set it to 200A then?
```

---
## \#15 Posted by: Andy87 Posted at: 2019-03-09T06:18:07.169Z Reads: 73

```
I would first check my connections.
Abs overcurrent can come from a bad solder join or one of your plugs or bullet connectors not 100% plugged in.
Also check the pcb of your vesc. 
Can you se find some lose connections?
Have a special eye on the legs of the capacitors. If there is something lose, broke it might be the reason.
```

---
## \#16 Posted by: pjotr47 Posted at: 2019-03-09T10:58:26.943Z Reads: 71

```
Oh if that abs over current happens while detection, I think your drv is fried
```

---
## \#17 Posted by: CarlCollins Posted at: 2019-03-09T15:06:50.517Z Reads: 67

```
Try this 

Unplug both of the motors if dual setup
 Swap them, plug them back, make sure joints and connectors are properly connected
Set the values to lower, your ESK calculator for that 
Perform detections, and throttle check then 

ABS_Overcurrent occurs when one or more motors are faulty or values are not accurate for the setup.
```

---
## \#18 Posted by: sayekim Posted at: 2019-03-09T23:46:50.380Z Reads: 60

```
You have it set to 120 and it went 123 so yeah the fault gets triggered. 

Of course you should only be reaching these amps when under load on take off usually. 

Ate you running dual motors? Which firmware version are you running?
```

---
## \#19 Posted by: affeandersson Posted at: 2019-03-14T07:10:57.880Z Reads: 55

```
But wouldn't I be getting a DRV error also then?
```

---
## \#20 Posted by: Bataleon Posted at: 2019-06-22T09:41:12.673Z Reads: 34

```
Did you have any luck solving this @affeandersson? My VESC has the exact same problem: applying any throttle results in the motor stuttering once or twice, then the red LED blinks and a `FAULT_CODE_ABS_OVER_CURRENT` is logged. Motor detection also fails. I've tried a few different motors with the same result.
```

---
## \#22 Posted by: affeandersson Posted at: 2019-06-22T09:56:54.598Z Reads: 32

```
Nope. I contacted Flipsky on facebook but they where not much of help so ended up upgrading to a VESC 6.6 instead and didnt have any problems yet..
```

---
