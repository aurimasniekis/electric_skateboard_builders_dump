# Weird noise in my motor, what could have caused it?

### Replies: 38 Views: 855

## \#1 Posted by: atlasdev Posted at: 2019-07-30T11:29:45.236Z Reads: 177

```
After 5 months of waiting for parts I can finally build my board. The problem is that there is some kind of weird noise inside of one of my motors. It only appears on one motor, and if I swap the phase wires the motor appears on the other side. The noise goes away if I brake 100%, or sometimes for a short while if I don't (you can hear it in de video).

This is the noise I'm talking about:

https://www.youtube.com/watch?v=4G7u5KMo12M
https://www.youtube.com/watch?v=ImgXsLI41YE

Here are some of the configurations I got, I think the issue lies at connector 2:

![576-1024|281x500](upload://jakb8pDfHg1byUfA5zo1eVFGoaf.jpeg)

![498-1024|243x500](upload://hliFp9TrM6GvkTib05IeEXWopgA.jpeg) 

![498-1024|243x500](upload://x8Q7N4ngPuS8BQFsqPHJPcFIvJY.jpeg)

![498-1024|243x500](upload://q2E1Ergzdm8MTZpr5MdRRCJjytw.jpeg)

Let's go over every component any try to eliminate as much components as possible:
 - Motors: If I swap the phase wires the issue appears on the other motor. As the motors stay the same but the issue does not the motors are eliminated.
 - Remote: I fail to see how a remote could cause one motor to make a weird noise no matter what position the joystick is in.
 - Sensor wires: I tried to run it sensorless, but I got the same issue.
 - PPM: I'm using UART, and changing to PPM does not change the symptoms.
 - Battery: What the hell does the battery have to do with motor noise?
 - Board: ^ s/battery/board

This leaves the Unity as the only probable cause of this issue.

This all would not have been so bad (shit happens) if there was any support from Enertion whatsoever. First of I turned to the forum, as you guys are awesome. I want to thank anyone who tried to help me, I really appreciate it!

https://www.electric-skateboard.builders/t/noob-question-thread-ask-your-questions-here/9559/7656

The other forum:

https://forum./t/noob-question-thread-ask-your-questions-here/126/1524

https://forum./t/haya-hb83-33-short-board-progress/244/49

I also tagged most of the Enertion guys directly, no response.

https://www.electric-skateboard.builders/t/focbox-unity-support-setup-troubleshooting/77861/2062

I also send a support request 4 (!) days ago, but I have yet to receive a response which is not automated.

![498-1024|243x500](upload://pywV4M6ajpjxqCyfLmtnunqBZOi.jpeg) 

![498-1024|243x500](upload://w4WC9jo4pbPd206C3GnEyeVm36P.jpeg) 

![498-1024|243x500](upload://5RMPLHXcGAZCD60HbLRQ9EMCVhl.jpeg)

I don't think urgent means there what it means here.. I am protected by European law, but I don't feel like going that route. I would much more like to go the route of actually solving the issue. I'll tag them again: @EnertionSupport, @CarlCollins, @adrianenertion, @barajabali or @Deodand. Can anyone tell me what the hell is going on, because I'm so close to throwing in the towel. I just want to ride :(. My support ticket is #82023.

Thanks.
```

---
## \#2 Posted by: venom121212 Posted at: 2019-07-30T12:58:51.406Z Reads: 133

```
One hack around this that may help is to make the observer gain, Flux linkage measurements, etc match eachother. Start with observer gain and make the problem side of the unity match the value of the good one. See if it goes away and report back please!
```

---
## \#3 Posted by: atlasdev Posted at: 2019-07-30T13:06:52.946Z Reads: 139

```
Do you mean copying all values from motor 1 to motor 2? From this image?

[quote="atlasdev, post:1, topic:99392"]
![576-1024|281x500](upload://jakb8pDfHg1byUfA5zo1eVFGoaf)
[/quote]
```

---
## \#4 Posted by: venom121212 Posted at: 2019-07-30T13:08:37.438Z Reads: 123

```
Yes but it depends on which motor side (1 or 2) you think is good. So when you switched the phase wires and the other motor had issues, that side of the unity is most likely the offender. Copy good side values to bad if that makes sense.
```

---
## \#5 Posted by: atlasdev Posted at: 2019-07-30T13:14:20.428Z Reads: 122

```
I'll try that, one more question. Does it make sense to do the calibration once, write down the measurements for motor 1, swap the wires, calibrate again and replace the measurements for motor 2 with the written down values? I think it could improve the accuracy of the values as you would be using two "good" measurements, just both measured with motor 1.
```

---
## \#6 Posted by: venom121212 Posted at: 2019-07-30T13:32:07.552Z Reads: 116

```
I'll answer your question with another question.

If you swap motors and get different results on the same side of the unity using "identical" motors, would that make you any more comfortable?

The results should be very very similar. Try it for science.

I.e.

Motor 1 on Unity Left (L) values =/ motor 1 on Unity Right (R).

Motor 1 on Unity L = Motor 2 on Unity L
```

---
## \#7 Posted by: atlasdev Posted at: 2019-07-30T13:47:51.467Z Reads: 100

```
I tried it, but it didn't seem to do much. What I did notice is that the observer gain was about 450 for motor 2, which is way higher than motor 1.
```

---
## \#8 Posted by: venom121212 Posted at: 2019-07-30T13:49:06.194Z Reads: 96

```
Ok just for clarification, you tried that on unity left or right side?
```

---
## \#9 Posted by: atlasdev Posted at: 2019-07-30T13:50:11.789Z Reads: 100

```
I tried what you initially said. Just copy over the values from focbox motor 1 to focbox motor 2
```

---
## \#10 Posted by: venom121212 Posted at: 2019-07-30T13:50:37.045Z Reads: 98

```
You copied the values over and reran motor detection?
```

---
## \#11 Posted by: atlasdev Posted at: 2019-07-30T13:51:34.008Z Reads: 95

```
No, I just saved them. Motor detection would override the values right?
```

---
## \#12 Posted by: venom121212 Posted at: 2019-07-30T13:53:36.266Z Reads: 87

```
Yes, exactly. How did the observer gain value change to 450 then?

Sorry if I missed something obvious
```

---
## \#13 Posted by: atlasdev Posted at: 2019-07-30T13:55:21.689Z Reads: 86

```
I ran motor detection again before overriding the values. I didn't mention that. This was because I was not completely sure I didn't change anything in the wiring after the last change. That's when the high value appeared.
```

---
## \#14 Posted by: venom121212 Posted at: 2019-07-30T13:57:20.249Z Reads: 85

```
Ahh that makes sense now. How did the resistance, inductance, and Flux linkage measurements look?
```

---
## \#15 Posted by: atlasdev Posted at: 2019-07-30T13:58:25.998Z Reads: 86

```
Mostly the same iirc. Maybe a 5% difference for most values.
```

---
## \#16 Posted by: atlasdev Posted at: 2019-07-30T14:00:29.469Z Reads: 84

```
I also noticed something else, which is what I suspected earlier. The "wrong" motor actually wiggles a bit when it's making that noise.
```

---
## \#17 Posted by: venom121212 Posted at: 2019-07-30T14:02:36.470Z Reads: 83

```
Interesting. I'd guess that's from not processing the input signal smoothly. 

I had a bad Flux linkage mismatch that caused a similar issue but yours look much more normal at around 4 mWb.

I had one at 4 and one at 33 but it responded very similarly to what you're describing.
```

---
## \#18 Posted by: atlasdev Posted at: 2019-07-30T14:08:34.854Z Reads: 95

```
A new measurement made, this is straight from detection. The observer gain is now way less than before. I also noticed that on the focbox had a green led on it, which seems to be responding to the noise. If there is a noise the light becomes less bright, when it stops it becomes normal again. I think this is the signal light. Sorry for the shitty screenshots, I have to borrow a laptop from someone else as mine all run Linux.. 

![57|281x500](upload://cXmg8DyMptbI0ehUHtxvse6nXj6.jpeg)
```

---
## \#19 Posted by: Blasto Posted at: 2019-07-30T15:13:47.482Z Reads: 81

```
if the green light is changing intensity, that mean it is receiving a signal from the remote. Is it possible to use a ppm only remote? In my experience with the photon, well it never left the bench.
```

---
## \#20 Posted by: atlasdev Posted at: 2019-07-30T15:31:09.930Z Reads: 83

```
I don't have a ppm remote, any recommendations for a cheap one for testing? Or is it possible to test it with  an Arduino or something? It did also happen when the remote was not properly set up yet, so I really doubt this is the cause of the issues.

Another reason why I don't think that's the issue is because I read trough the source code of a VESC UART library, and it only references the joystick position to change the speed. As you can see in the second video I change the joystick position a lot, but the issue stays the same. This would eliminate that as the culprit.
```

---
## \#21 Posted by: atlasdev Posted at: 2019-08-02T14:11:07.679Z Reads: 53

```
I just got EXACTLY the same email as 5 days ago. This would be hilarious if this wasn't the thing blocking me from riding my board.. 

![Screenshot_20190802-160549_Spark|243x500](upload://tCynW8noLHKS0FFetLJNbNA3hPl.jpeg)
```

---
## \#22 Posted by: CarlCollins Posted at: 2019-08-02T15:03:32.819Z Reads: 51

```
@Blasto Please see this
```

---
## \#23 Posted by: Blasto Posted at: 2019-08-02T15:34:27.335Z Reads: 48

```
The deadband on the remote is out of bounds.To further prove my point, disconnect the receiver, does the noise go away?
```

---
## \#24 Posted by: atlasdev Posted at: 2019-08-02T15:54:34.087Z Reads: 45

```
I will try that once I have the the chance.
```

---
## \#25 Posted by: atlasdev Posted at: 2019-08-04T11:27:56.312Z Reads: 39

```
I have been able to test this a little more, and I've found that the remote was indeed the issue, at least for one noise. I noticed that there were two distinct noises, one when sitting idle, and one when running on low speed. The first issue has since been resolved with a firmware update, thanks to the quick support of @Wajdi (take note Enertion) . You can hear (and see) the second issue here:

https://www.youtube.com/watch?v=zNHSklOxLt0

You can see the issue at the wheel visible, the other motor spins fine, but this one makes noise and barely moves till I ramp up the throttle. When I feel the motor it feels like there is a pulling it back in the other direction. I don't know what's causing this, it could be the remote or bad calibration or something else entirely. Does anyone know what could cause this? I'm running sensorless here to try an attempt to remove any variables. You can also see a difference in the motor voltages here:

![Screenshot_20190804-130908|243x500](upload://vGSZyAF6R9fxCIwsCpkJcGTAQTs.jpeg) 
![Screenshot_20190804-130844|243x500](upload://syWgLLi2I2r2S9CpnKdM5O05Yi6.jpeg) 
![Screenshot_20190804-130826|243x500](upload://q0bAf9Y2zDfoTxwAktKyHDKOCNy.jpeg)
```

---
## \#26 Posted by: Wajdi Posted at: 2019-08-04T13:20:13.184Z Reads: 29

```
That's not exactly the source of the issue, the deadband on the remote is pretty minimal and response is accurate, the version of the remote you have was one of the very first iterations, latest version have gone through hundreds of changes and improvements.

After he sent me a support request email, we went through the problem and it was a compatibility issue with Unity. We fixed it using a firmware update on the receiver.

@atlasdev The remaining jittering issue is most likely due to your senseless setup, also  when running a dual setup, both motors might not start at the exact time and position, this is usually noticeable on very low RPM.
```

---
## \#27 Posted by: atlasdev Posted at: 2019-08-04T14:44:53.694Z Reads: 28

```
I've also tested the motors in sensored mode, but this didn't change anything, see the video below. You can really see the motor not responding correctly at about 0:06. You hear the other motor spinning up, but the motor in view barely moves. As you can see I swapped the wires since last video, to just make sure again this was not an issue with the motor itself. It also shows again a huge difference in voltage shown in the telemetry data

https://www.youtube.com/watch?v=ObvCXdO6ZtI&feature=youtu.be

![Screenshot_20190804-152648|243x500](upload://n3pC5ob5fCaAvis9MgFR8keMmui.jpeg) 
![Screenshot_20190804-152657|243x500](upload://7SYevXcz58cpY6flHjU35PWOQoe.jpeg)
```

---
## \#28 Posted by: atlasdev Posted at: 2019-08-04T21:50:40.610Z Reads: 24

```
I tried to attach my board to the VESC tool again, and I noticed again that the second motor shows as sensorless. When I change it to sensored and reconnect the board it switches back to sensorless. What could cause this? I tried swapping the wires of the two motors, but the issue stays at motor 2. This means there is nothing wrong with the sensors or the wires to them. 

![20190804_231319|281x500](upload://qrbdV2SjxGnvoX5E7FpDdFwskN2.jpeg)
```

---
## \#29 Posted by: Wajdi Posted at: 2019-08-05T19:27:38.869Z Reads: 20

```
Not sure why the other motor is not receiving correct voltage. The receiver sends a command to the master vesc with the joystick value, master vesc then processes the command and sets appropriate current to the motor. The master motor spins fine, which means that up to this point the receiver has done its job and it is now up to the master vesc to forward the correct commands to the other vesc.

Synchronization problems in dual vesc setups have been around since the very first versions, not sure if anyone has ever looked into this or found a fix.
```

---
## \#30 Posted by: atlasdev Posted at: 2019-08-05T19:45:27.675Z Reads: 18

```
I'm using a Unity here, so synchronisation issues should be minimal (it's using a single SOC). The reason I might expect the receiver to be the issue here is that the previous issue (which has been fixed) also happens on one and the same motor. It's not impossible that it is a synchronisation issue.

@CarlCollins could you weigh in on this?
```

---
## \#31 Posted by: Wajdi Posted at: 2019-08-05T20:09:53.846Z Reads: 18

```
You are correct, it seems like it's only using one micro controller.
After searching around I found that Unity has an extra argument to control the second motor separately, so instead of sending one command and apply it to both motors, they made it so you have to send command for each motor separately ( I don't understand the reasoning behind this design ). Here is where it's mentioned https://www.electric-skateboard.builders/t/focbox-unity-support-setup-troubleshooting/77861/371

That being said, I'm going to apply the changes and send you the update.
```

---
## \#32 Posted by: Wajdi Posted at: 2019-08-05T20:45:14.596Z Reads: 18

```
I spoke too soon, some commands do indeed require both motors to be set in Unity like 
[code]
case COMM_SET_CURRENT:
    ind = 0;
    cmd1 = (float)buffer_get_int32(data, &ind) / 1000.0;
    cmd2 =(float)buffer_get_int32(data, &ind) / 1000.0;
    mc_interface_set_current(cmd1,cmd2);
    timeout_reset();
    break;
[/code]

Where cmd1 is for motor 1 and cmd2 for motor 2,

However the nunchuck command, the one we are using, only requires one value, and Unity should handle controlling the other motor accordingly 
[code]
case COMM_SET_CHUCK_DATA:
    ind = 0;
    chuck_d_tmp.js_x = data[ind++];
    chuck_d_tmp.js_y = data[ind++];
    chuck_d_tmp.bt_c = data[ind++];
    chuck_d_tmp.bt_z = data[ind++];
    chuck_d_tmp.acc_x = buffer_get_int16(data, &ind);
    chuck_d_tmp.acc_y = buffer_get_int16(data, &ind);
    chuck_d_tmp.acc_z = buffer_get_int16(data, &ind);
    app_nunchuk_update_output(&chuck_d_tmp);
    break;
[/code]

The command accepts a joystick value, and Unity should handle controlling both motors appropriately.

Is your other motor still not detected as sensored? Your R and R2 are 0, were you able to do the motor detection?
```

---
## \#33 Posted by: atlasdev Posted at: 2019-08-05T20:48:47.353Z Reads: 16

```
Yes, it's still showing as sensorless. I am able to do the motor detection, but I'm not sure what you mean with R and R2 are 0?
```

---
## \#34 Posted by: Wajdi Posted at: 2019-08-05T20:52:12.464Z Reads: 15

```
On your screenshot, they are highlighted in red.
```

---
## \#35 Posted by: Wajdi Posted at: 2019-08-05T21:06:56.080Z Reads: 17

```
I  suggest you disconnect the receiver, and try to get the motors detected properly with the sensors working.
```

---
## \#36 Posted by: atlasdev Posted at: 2019-08-05T21:17:38.568Z Reads: 16

```
I restarted the tool to get the values, which are not filled in by default. Here is a completely new detection.

![20190805_231551|690x388](upload://kzordABpHnIsc9psU33xuTI0vNf.jpeg)
```

---
## \#37 Posted by: atlasdev Posted at: 2019-08-05T21:50:05.757Z Reads: 16

```
I'm now having bigger issues, the connection to my Unity seems to cut out :(. This is both on usb and Bluetooth. I want to try to update the firmware but, well, my connection cuts out. I'll try again tomorrow, but it doesn't look great..
```

---
## \#38 Posted by: atlasdev Posted at: 2019-08-06T14:56:47.631Z Reads: 15

```
Hi, my unity keeps disconnecting and stops responding to commands. I’m trying to flash the firmware again in an attempt to resolve it, but this keeps timing out. When I start it up the error led flashes once. What could cause this?
```

---
