# VESC Static Spark? One VESC not working

### Replies: 11 Views: 1324

## \#1 Posted by: Eckles Posted at: 2017-01-03T04:57:17.826Z Reads: 131

```
**Board Info**: Dual Motor x2 170 KV 
                 x2 VESC 4.12 
                 Li ion 12s3p Battery
                 VESC Firmware 2.52 (With Ackmaniacs BLDC Throttle Control Mod)

My board was working great until yesterday when one of my motors cut out and I couldnt get it running again. I got home started testing, after running motor detection I think that my Intergrator Limit and BEMF coupling values were wrong on both VESCs/Motors (This baffled me because im almost certain I set them correctly on initial setup).
<img src="/uploads/db1493/original/3X/1/6/1682f0f35919e41559c7f7cdad2409d8cb8557ac.png" width="689" height="278">

I didnt think the board would even run with wrong values but anyway im still a novice really. My MASTER VESC seems to be fine with both motors detected and are responding normally via Remote Control but when I press Right on the keyboard either connected motor will stutter and barely spin (due to the incorrect values maybe?).  
With my SLAVE VESC neither motor is detected and I get the "Bad Motor Detection Result" message, after typing "Fault" into the TERMINAL page I get "FAULT CODE NONE" and typing "Faults" it tells me "No Faults Registered Since Startup". So, the LED lights all function as normal on SLAVE VESC the only thing is when I move it I hear the sound of spark but I cannot see where its coming from. This spark has also interfered with my battery indicator (blinks stating 0%). After rebooting the SLAVE VESC battery indicator returned to normal (84%). All my other BLDC settings look correct for my setup...
<img src="/uploads/db1493/original/3X/c/7/c706d9c445399b2624cd67fe81a519dd74f71042.png" width="689" height="278">
<img src="/uploads/db1493/original/3X/d/c/dc61edc5e039ac044b283536d3cea95ed16ffccb.png" width="689" height="278">

Here are pictures of the SLAVE VESC , I cant see any differences to the MASTER VESC...
<img src="/uploads/db1493/original/3X/7/8/78919df7d4d6731fe02e7bdbc88a38b58ec58c59.JPG" width="690" height="388">

Ive tried to give as much info as possible to see if anyone can help determine the cause of this and perhaps confirm if this VESC is beyond repair.

Thanks
```

---
## \#2 Posted by: Iceni Posted at: 2017-01-03T12:23:12.529Z Reads: 92

```
If you hear a sparking sound when moving the vesc it might be the cables from the battery coming into contact with something. 
Check the soldering on the capacitor PCB and where the wires go onto the vesc. 
Will propably have to remove the heat shrink.
```

---
## \#3 Posted by: Ackmaniac Posted at: 2017-01-03T12:56:31.736Z Reads: 90

```
First of all your settings are way to high. You have a 12S3P Li-Ion Battery so they can only give 60A (20A a cell) continuous. 
But each of your VESCs is setup to 60A. You should set them to 30A max battery each. And also adjust the max watts setting according to that. So it should only be half the value. Because when both VESCs draw max power from the battery the amps get summarized.
Next thing is that you didn't do the motor detection on the slave VESC. Could be that it got killed by that.
But it also could be that the motor detection get's disturbed by the remote signal.
So you always have to disable the remote in the application settings by set the crontrol mode to disabled (as in the picture) when you want to do a motor detection. An the slave VESC gets the signal by the master. So you have to disable the control mode at the master. Then switch to the slave and do the motor detection there.
<img src="/uploads/db1493/original/3X/7/d/7d0874ece04e3670ca539ab267a0f2579f590298.png" width="683" height="500">
1. First read the configuration.
1.Select Disabled in your control mode. If you use the Nunchuk do it in the Nunchuk tab, if you use PPM do it in the PPM tab. If you have a dual setup and the 2 VESCs are connected by CAN then set it to disabled at the Master.
2. Write the application settings.
3. Change to the motor configuration
4. Read the configuration
5. Do the Motor Detection.
6. If the motor detection was successful click the apply button
7. write the configuration
8. do step 3 - 7 for the slave
9. go to the masters application tab
10. read the configuration
11. select your wanted control mode
12. write the configuration

So the best is disable the remotes control mode. Do the motor detection's on both VESCs and then do the rest.
```

---
## \#4 Posted by: Eckles Posted at: 2017-01-03T16:18:07.736Z Reads: 77

```
I will have a look when I get home, it does seem that the sound of the spark is coming from that end of the VESC
```

---
## \#5 Posted by: Eckles Posted at: 2017-01-03T16:20:03.857Z Reads: 78

```
Ok man, Im out right now but I will go through the steps when I get home, thanks for the help
```

---
## \#6 Posted by: cmatson Posted at: 2017-01-03T22:28:57.647Z Reads: 75

```
I had the sparking issue on my VESC, and it turned out that one of the contacts for the battery were coming off the board, so it would effectively "spark" making a popping sound.

https://www.youtube.com/watch?v=SKjD6C49k3c

https://www.youtube.com/watch?v=NKJ95Hi1aEI&t=65s
```

---
## \#7 Posted by: willpark16 Posted at: 2017-01-03T23:18:52.399Z Reads: 69

```
I messaged u
```

---
## \#8 Posted by: Eckles Posted at: 2017-01-08T17:27:03.633Z Reads: 62

```
 I managed to pinpoint the problem as a bad contact on the cable from the capacitors going into the VESC. It had come loose and under vibration would disconnecct causing a spark then would reconnect once repositioned, I re-soldered this contact and the disconnection problem stopped.

My problem still is doing a motor detection, I keep receiving "Bad Detection Result Recieved" message. When I type "Fault" or "Faults" in the terminal page it tells me "No faults registered since startup" or "FAULT_CODE_NONE". On top of this the LED lights are functioning as normal and when I use the directional keys within BLDC Tool the lights change accordingly but with no movement from the motor.

I have tested this motor on my MASTER VESC and it works fine so it rules out motor troubles. I then re-flashed the firmware on the SLAVE VESC but im still unable to run a motor detection. When I "Activate Sampling" in the Realtime Data tab I get seemingly normal responses in the graphs but nothing from the motor.

After re-flashing the firmware all my settings are Default Settings for VESC 4.12/Firmware 2.52.

Is there something more I can do to figure out the problem? Anyone got suggestions as to what this is?
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2017-01-09T01:52:43.515Z Reads: 56

```
do you have any picture of your connection ? also, Firmware is suppose to be 2.18...
```

---
## \#10 Posted by: Eckles Posted at: 2017-01-10T18:50:37.671Z Reads: 48

```
I believe it upgraded after downloading the Throttle Mod (see above) I could try reflashing back to 2.18 but I dont think thats the problem, the Throttle Mod was working great (really improved the ride) for over a month. Is there any other way to check for faults other than the terminal page? Could something fry without showing a fault? 
p.s I will do the pictures as soon as I get home. Gonna have to say goodbye to the heatshrink :cry: haha othwerwise the pics are useless
```

---
## \#11 Posted by: ivandeleon120 Posted at: 2017-04-20T09:57:07.008Z Reads: 30

```
I am having a problem with my VESC.

I am using a 12s3P battery and 5563 dual motors. Results that I disconnected one my vescs since I was having issues with my BMS. After solving the issue with my BMS the VESC didn't turn on at all. I connected it to my computer and was not detected. There are no damages on the motor driver itself neither on the MCU. It only gets hot by the usb port. Sadly, I only rode my electric skateboard for a weekend.
Anybody has had this issued? did you have to replace something? I've checked the BOMs and I can get the parts if you ever had this type of issue.

Thanks
```

---
