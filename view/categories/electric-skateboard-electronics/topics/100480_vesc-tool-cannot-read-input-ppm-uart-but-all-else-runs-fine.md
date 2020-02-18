# VESC Tool cannot read input (ppm/UART) but all else runs fine

### Replies: 8 Views: 288

## \#1 Posted by: Fungineers Posted at: 2019-08-18T05:07:36.247Z Reads: 72

```
Hey guys!
So Ive been running my VESC without a problem. It uses PWM from an arduino and all was good until recently it just decided to not accept PWM anymore (update: tried UART, doesnt accept that either). 
I checked the input port and the SIGNAL port is receving from the Arduino alright, but the VESC tool seems to be in full brake mode all the time. See picture below:
![image|690x372](upload://k89KbYIp1gZheAwsAWrmjXRVDHS.png) 

Has anyone had a similar problem? The motor is fine it runs on detection and when run manually from the toolbar at the bottom of the VESC tool (duty cycle, current run options).

So the problem is definitely at the input from ppm/uart, basically any communication. Any help is appreciated.
Experts: @trampa @longhairedboy @chaka
```

---
## \#2 Posted by: trampa Posted at: 2019-08-19T06:44:33.015Z Reads: 54

```
Try to use a simple PPM remote to check things. 
Sometimes going back two steps in the Wizard and then going forward again also helps.
Can you check if the arduino sends appropriate signal output. ?
```

---
## \#3 Posted by: Fungineers Posted at: 2019-08-20T03:50:15.511Z Reads: 35

```
Hey thanks for replying!
The arduino is sending the correct pulses. Even with the arduino and motor disconnected, vesc tool is reading full negative throttle when ppm is enabled. 
Here's what Ive tried so far: 
- Tried communicating on UART since I thought ppm is the issue. Was getting nothing from the vesc, in or out, even though there was voltage on the tx rx pins. This lead me to believe maybe the hardware is the issue. 
- Which lead me to doing a reflashing of firmware uaing the stm utility. The firmware was fine but same issue persisted. 
- Then I took out the old stm chip and transplanted a new one. Ran a new firmware upload. Still same issue! 
Im really stumped at this problem. Im starting to think it is the vesc tool that is the problem?
```

---
## \#4 Posted by: trampa Posted at: 2019-08-20T09:10:41.261Z Reads: 28

```
What HW do you use? Which mode do you run? *Current no reverse with brake* is the default.

Frank
```

---
## \#5 Posted by: Fungineers Posted at: 2019-08-20T09:41:17.840Z Reads: 28

```
Frank, 
Using HW4.12, FW 3.57
Running 'Current' mode, but after this bug, all modes stopped working. Tried Duty cycle mode, and all other variations. 
The input from 'Vesc tool' just remains at a constant -300% (as shown in the picture above). When I try to set the max min center limits, it says 'Activate RT app data', even though the RT app is active! It seems like it just cant read realtime data from the vesc (regardless of it being ppm or uart) but can put out data from the computer (USB) to the vesc and motors just fine. Could it be a short? A bad cap? Maybe the vesc tool itself?
```

---
## \#6 Posted by: Fungineers Posted at: 2019-08-20T09:42:13.353Z Reads: 25

```
@SwarleyAUS
```

---
## \#7 Posted by: trampa Posted at: 2019-08-20T09:58:41.920Z Reads: 23

```
[quote="Fungineers, post:1, topic:100480"]
So Ive been running my VESC without a problem
[/quote]
Sounds like a HW matter. This is third party HW and if it fails to work as intended, you have to contact the vendor.
```

---
## \#8 Posted by: SwarleyAUS Posted at: 2019-08-28T05:57:21.933Z Reads: 13

```
@Fungineers as suggested, the best idea is to confirm everything you have designed is working. I.e. verify arduino is correctly outputting RC-compliant PWM (not true PWM) (either with oscilloscope or feed the output into another Arduino), cables providing good connection, etc.

I've never seen the VESC say it is receiving -500% throttle. I think my VESCTOOL differs from yours though, I don't believe I see the VESC Tool bar graph. Should this graph not be ignored though? All you care about is what the From VESC graph shows, no? 

Regardless, if those numbers for Min, Max and Center are live data, the VESC is receiving out of bounds PWM data. You still using the Servo library?
```

---
