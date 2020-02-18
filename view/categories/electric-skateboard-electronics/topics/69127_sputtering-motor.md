# Sputtering Motor

### Replies: 36 Views: 406

## \#1 Posted by: Jcullinan09 Posted at: 2018-09-25T02:32:16.584Z Reads: 94

```
Im running 10s5p 30Q's, Dual FocBox, and 6374 190kv from Torqueboard. 

From BLDC tool when I perform a motor detection the motors detect just fine. However when trying to operate the motors from the remote, I'm just getting a sputter. 

Anybody have any ideas? I am using PPM and UART with one vesc as the master and the other slave. 

Here are my settings on BLDC. I'm not sure whats happening. 

![27%20PM|690x420](upload://j2WY7apOhT1X72bkk7dLlkAtTzj.png)
```

---
## \#2 Posted by: Andy87 Posted at: 2018-09-25T05:12:32.650Z Reads: 73

```
Did you setup it with sensors or sensorless?
Does the studder already happen on the bench or only loaded?
```

---
## \#3 Posted by: Jcullinan09 Posted at: 2018-09-25T05:18:26.454Z Reads: 70

```
Thanks for the response.
I have each motor's sensor wires connected to the vesc, and in BLDC tool I have the sensor mode type selected as Sensored. 

The studder happens on the bench when throttling with the remote. I haven't throttled with load, figuring the motors aren't turning on the bench they probably wont spin with load. However motors will run when I hit "start detection".
```

---
## \#4 Posted by: dareno Posted at: 2018-09-25T05:19:50.884Z Reads: 63

```
Is that split ppm or can bus?
```

---
## \#5 Posted by: Andy87 Posted at: 2018-09-25T05:21:54.366Z Reads: 63

```
If you do motor detection, can you look the results of you hall sensors? Maybe they failed?
Did you try to set up your focbox in FOC?
Maybe there you don’t get that problem
```

---
## \#6 Posted by: Jcullinan09 Posted at: 2018-09-25T05:26:42.698Z Reads: 58

```
@dareno Right now the two VESC's are connected via canbus. Should or would it make a difference to have them connected via split ppm. If so how do I do that?
```

---
## \#7 Posted by: Jcullinan09 Posted at: 2018-09-25T05:28:43.574Z Reads: 58

```
@Andy87 After I do a motor detection, where could I look to see if a hall sensor failed? I don't think I want to try setting up in FOC mode because I want to use a bluetooth module which requires UART.
```

---
## \#8 Posted by: dareno Posted at: 2018-09-25T05:29:28.929Z Reads: 54

```
No man thats cool you just said ppm and master slave.  With split you have to set up as two masters.
If you are using canbus make sure you keep them both powered with the canbus connected.  V IMPORTANT.  

[quote="Jcullinan09, post:1, topic:69127"]
I am using PPM
[/quote]
this just threw me for a minute.
```

---
## \#9 Posted by: Jcullinan09 Posted at: 2018-09-25T05:33:35.628Z Reads: 50

```
@dareno I thought setting up in ppm and master slave was only as simple as going under app configuration and general tab, then selecting "send status over CAN" then naming the " controller ID" of each vesc a different number ie) 1 and 2.

I don't think I set them up correctly then...? How would I go about getting it to work like I thought it would?
```

---
## \#10 Posted by: Arzamenable Posted at: 2018-09-25T05:34:12.495Z Reads: 51

```
When you hit write motor app, there will be an error about halls being out of range
```

---
## \#11 Posted by: Jcullinan09 Posted at: 2018-09-25T05:36:13.533Z Reads: 50

```
Motor app?![42%20AM|690x415](upload://rWylWPq7j75AG8OWP2KXRxjzc9A.png)
```

---
## \#12 Posted by: Arzamenable Posted at: 2018-09-25T05:38:45.178Z Reads: 44

```
I don’t want to confuse you, I haven’t used bldc tool in awhile. I use vesc tool and a red error will pop up: “bad detection results”

Edit: sorry, I’m making this worse. In AM if you don’t get this figured out, I’ll find an old computer image with bldc tool and try to walk through.
```

---
## \#13 Posted by: Andy87 Posted at: 2018-09-25T05:39:32.143Z Reads: 46

```
Looks good so far.
It’s the right down window under detection results.
Scroll a bit down and there it’s written when your sensors failed
```

---
## \#14 Posted by: Andy87 Posted at: 2018-09-25T05:40:21.632Z Reads: 45

```
You can use your uart also in FOC.
It does not make any difference.
```

---
## \#15 Posted by: dareno Posted at: 2018-09-25T05:42:17.880Z Reads: 44

```
First of all use hybrid mode it works better for everyday use.  It basically removes sensors after 6kmh or so which is what you want.  When you do the detect on each motor make sure that you hit apply and get the green write ok notification and the big window will have the results.  when you hit apply it will send those findings to the vesc.
```

---
## \#16 Posted by: Jcullinan09 Posted at: 2018-09-25T05:42:53.727Z Reads: 41

```
Is there any difference in any of the Vesc tool programs? Or is the platinum/gold/silver/bronze just a way to pay it forward for the developers of the programs?
```

---
## \#17 Posted by: Andy87 Posted at: 2018-09-25T05:44:24.894Z Reads: 43

```
Yeah looks like he didn’t push apply after motor detection.
There still written the stock values in the right upper field.

@Jcullinan09 did you push apply and write to the vesc after motor detection?
```

---
## \#18 Posted by: dareno Posted at: 2018-09-25T05:44:57.858Z Reads: 43

```
Its a conscience thing this whole set up is the brainchild of Ben Vedder and its good to give back. I love vesc tool for ease of set up but you will have to update the firmware before you can use it and I was trying not to make this more complicated for you.
```

---
## \#19 Posted by: Andy87 Posted at: 2018-09-25T05:44:59.572Z Reads: 43

```
No difference
```

---
## \#20 Posted by: Jcullinan09 Posted at: 2018-09-25T05:46:06.207Z Reads: 44

```
@Andy87 I did in previous attempts before deciding to try and ask for help. Let me apply it once more just for good measure. I don't think it'll make a difference.
```

---
## \#21 Posted by: Andy87 Posted at: 2018-09-25T05:48:01.654Z Reads: 36

```
Ok.
Did you make the detection with or without belt attached?
```

---
## \#22 Posted by: Jcullinan09 Posted at: 2018-09-25T05:48:39.829Z Reads: 34

```
With the belt attached. I reckon it should not be though
```

---
## \#23 Posted by: Andy87 Posted at: 2018-09-25T05:49:49.912Z Reads: 34

```
I never understood that hybrid mode.
Always thought that even in sensored mode the sensors will not give any values after a rpm of 6000
```

---
## \#24 Posted by: Andy87 Posted at: 2018-09-25T05:51:00.187Z Reads: 35

```
I made mine with and without.
Both where working, but it’s recommended to do it without load.
Maybe your belts overtide?
Just guess what else it could be
```

---
## \#25 Posted by: dareno Posted at: 2018-09-25T05:59:02.589Z Reads: 34

```
tbh I used bldc tool for my first set up and that was the advice I got at the time. I assumed that the sensored in bldc was sensored all the time unless configured with hybrid otherwise why have it?  I now use vesc tool which is either sensored or not and is just so much easier to configure that I don't use the other tool at all anymore.  Oh and I don't use sensors either anymore so......
@Jcullinan09  try vesc tool because once you use it you won't look back.  It has wizards to guide you through the whole process.  
 https://www.youtube.com/watch?v=qpovd2XRKqc&t=887s
watch this video man it helps
```

---
## \#26 Posted by: dareno Posted at: 2018-09-25T06:00:50.053Z Reads: 33

```
definitely without the belts and always make sure your belts are loose, not so they skip but as loose as you can get them without.
```

---
## \#27 Posted by: Jcullinan09 Posted at: 2018-09-25T06:06:04.058Z Reads: 32

```
I don't know what box I checked, but now I can't even get a motor detection without belts on. Im just left sputtering with no load. But thanks for the heads up on Vesc tool. Im going to look in to it.
```

---
## \#28 Posted by: Andy87 Posted at: 2018-09-25T06:06:36.234Z Reads: 33

```
Honestly I think the wizard of the vesc tool is not the best.
There some things which just get skipped.
Maybe I just didn’t understood but the ppm wizard for example don’t give you to configure ppm+uart. After the wizard you need to add this under the settings. The same with the max erpm limit at the motor wizard. It’s nowhere mentioned while setup.
Besides it’s for sure more comfortable tool.
```

---
## \#29 Posted by: Andy87 Posted at: 2018-09-25T06:07:30.220Z Reads: 34

```
Can you move your motor by hand?
You hear something scratching inside?
Maybe magnet became lose?
```

---
## \#30 Posted by: Jcullinan09 Posted at: 2018-09-25T06:08:54.242Z Reads: 33

```
Yeah, I can move the motor by hand just fine, and nothing sounds unusual. I think its just a setting from BLDC tool.
```

---
## \#31 Posted by: Andy87 Posted at: 2018-09-25T06:11:29.550Z Reads: 34

```
If you want to use the vesc tool you also need to update your firmware.
Just as additional info.
```

---
## \#32 Posted by: Jcullinan09 Posted at: 2018-09-25T06:13:53.792Z Reads: 32

```
So the 2.18 firmware, won't work for Mac OS? 
If you have the file of the firmware I might need could you private message it to me, or post it here? 

If you don't that's fine, and ill just have to do some digging on my own.
```

---
## \#33 Posted by: Andy87 Posted at: 2018-09-25T06:23:56.252Z Reads: 34

```
So you need the Mac version of the vesc tool?
Unfortunately I don’t have the original version vor Mac, but you can find the ackmaniac version here
https://www.electric-skateboard.builders/t/ackmaniac-3-10-version-for-mac/69096?u=andy87
It’s the same interface just with a bit more explanations and the firmware is adjusted more for Esk8.

The firmware laying in the software folder.
So after you opened the vesc tool just go into the firmware section, select the right fw for your hw (focboxes should be 410,411,412) and upload it.
I would also disconnect the CAN while uploading.
Shouldn’t be an issue but I would have a mixed feelings while flashing new fw.
```

---
## \#34 Posted by: Jcullinan09 Posted at: 2018-09-25T06:25:01.641Z Reads: 32

```
AWESOME Thanks!
```

---
## \#35 Posted by: pat.speed Posted at: 2018-09-25T06:40:41.483Z Reads: 30

```
also make sure to not power only one focbox at a time when connected with can. It will kill the can chip and even drv. 

Either power both at same time or disconnect can wire will doing powering one at a time
```

---
## \#36 Posted by: Jcullinan09 Posted at: 2018-09-25T20:29:24.253Z Reads: 17

```
Hey guys,
I've been trying to understand the VESC tool, and when doing a motor detection, results are getting better, but not nearly where they should be. I've got a screen recording that shows just whats going wrong with the motor detection, you can hear the sound in the background of the motor stuttering in the second half of the video.

https://youtu.be/4qdq7n3mYV4
```

---
