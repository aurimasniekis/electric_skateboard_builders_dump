# Is my sensor broken, how do I check that? It runs fine in BLDC, just a bit of expected cogging

### Replies: 7 Views: 141

## \#1 Posted by: Narnash Posted at: 2019-03-27T10:56:49.045Z Reads: 52

```
Hello community, 

I hope you can help me with a little problem I have lately on my eMTB. 
My problem at first was overcurrent errors according to my metr module, to fix that I checked all obvious connections (battery, motor bullets, solder joints on the dual ESCape) no broken connection found. 

After that I tried 1 motor at a time to found out that only the right side (2WD, FOC sensored) made problems, on the bench with no load it runs fine though on both sides. With a bit load with my hand the right motor was stuttering, on flat ground short jitter than over current error.

My next step I took to fix my problem was recalibrating the motors with the VESC Tool, again 1 motor was fine the other didn't calibrate . Than the same thing in sensorless, worked not on the first try but got it calibrated. I tried it on the ground again, with the same result -> overcurrent error.

My last attempt that for the time being worked or worked arround was to switch to to BLDC mode and upping the motor max. current a bit (to 200A) even though it already was at 160A. It basicly worked since then as expected some cogging jitter cuz BLDC than it's fine. A push and it works flawlessly I drove about 60km since than with that setup no big complants just a bit louder or better a bit different in sound as my chain is a tad loud anyway and the cogging from standing still which is espacially annoying uphill because you can't really push to spin up the motors in these cases ("pushing" is hard/weird anyway with straped on bindings and heelstrap :sweat_smile:).

TO GIVE SOME MORE INFO ABOUT MY SETUP:

I have a...
2WD Trampa eMTB
10S8P top mounted Samsung 30Q battery.
dual ESCape in an enclosed and water tight box but I didn't really drove on wet weather/ground anyway.
Unik Polaris 6374 150KV sensored motors.
10 : 42 chain gearing.

I have this setup since maybe a half year, due problems in my family and a broken elbow (2nd test ride ...) I only got maybe 250km so far on this thing.

I really would like to get sensored FOC back again. My first conclusions by my fixing tryouts are that a fatal failure by either ESC or motor is kinda unlikely, it still sounds for me like a loose connection or broken cable to be honest. I can also imagine that the sensor may or may not be broken (don't know if the Polaris is coated) I also don't really know how to check if the sensor is broken.

I don't know what would you suggest or can you even give me a solution by my error describtion :heart_eyes:
**What should I try next? How can I check the sensor on the faulty side? Do I have to open that motor? **

Thanks for any help!
```

---
## \#2 Posted by: Dirt_Bag Posted at: 2019-03-29T04:14:05.782Z Reads: 26

```
thats a strange issue, make sure you are testing without your belts/wheels connected, sensor detection with drag leads to weird errors. also, check and make sure the motor can isn't able to rotate on the shaft, and the 2 are solidly joined and not slipping. other than that im really not sure. hope this helps
```

---
## \#3 Posted by: threebysix Posted at: 2019-03-29T04:19:24.718Z Reads: 23

```
try swapping the motor around to see if you still get the same problem. If you swapped the motor around and that "bad" motor still causes over current, then you know it's the motor. After the swap if the "bad" motor does not cause any over current but the "good" one now does, then it could be the ESC.
```

---
## \#4 Posted by: Andy87 Posted at: 2019-03-29T06:08:54.245Z Reads: 19

```
i would next check the jst plugs for the sensor wires.
I think you have there an adaper from 1.5 to 2mm jst as well. did you swap that cable as well? maybe one is bad. check also the crimp contacts and if they sit full into the jst plug.
after that i would open up the motor.
It´s not a big thing on the polaris motors.
just remove the circle clip and take off the bell.

To be sure that you don´t have issues with your windings, you can also measure the resistance of your windings. all combinations should have the same resistance. you could do that before open up the motor as well.
```

---
## \#5 Posted by: Narnash Posted at: 2019-03-29T11:26:45.802Z Reads: 9

```
I already swaped the leads on both motors and on both ESC sides the "right" motor always failed to "perform as expected", though sensorles FOC calibration fails most of the time, but when it works the motor don't has enough torque on the ground stutters->overcurrent as I described.
```

---
## \#6 Posted by: Narnash Posted at: 2019-03-29T11:31:06.960Z Reads: 9

```
I will try that next, thanks.

 I don't really have a problem with opening the motor by iself but open the chain, heating the sprocket and reassembly is a bit annoying and dirty.
```

---
## \#7 Posted by: Andy87 Posted at: 2019-03-29T11:38:36.923Z Reads: 9

```
Totally understandable 😅 same issue here. 
Check the other things first and maybe you lucky to find the fault somewhere there.
```

---
