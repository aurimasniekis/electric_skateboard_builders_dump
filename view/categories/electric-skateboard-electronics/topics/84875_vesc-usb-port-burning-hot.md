# VESC USB Port Burning Hot

### Replies: 38 Views: 433

## \#1 Posted by: J_Dizzle Posted at: 2019-02-21T02:12:10.416Z Reads: 114

```
99.9% of my build done, Vescs programmed, everything working, then I went to the bathroom and came back and found that the USB port on both vescs were burning hot, as they burned my finger. There are no leds on either Vesc and the motor doesn’t spin but the light on my receiver lights up so I know they are getting power. Any thoughts?
```

---
## \#2 Posted by: J_Dizzle Posted at: 2019-02-21T02:18:04.641Z Reads: 111

```
Also I am now noting that the drv chips on both vescs are hot, $&@#!!!. But that still doesn’t explain why the vescs don’t power on or connect to Vesc tool. They are both 4.12 from @torqueboards
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2019-02-21T02:26:02.675Z Reads: 107

```
Is the bleu light on ?
```

---
## \#4 Posted by: J_Dizzle Posted at: 2019-02-21T02:33:18.716Z Reads: 104

```
No, no lights at all on the Vesc... I believe I will be needing your repair service lol
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2019-02-21T02:34:29.340Z Reads: 99

```
Yes It is most likely the can transceiver who blowup
```

---
## \#6 Posted by: J_Dizzle Posted at: 2019-02-21T02:42:52.584Z Reads: 98

```
Ok, here is a pic, the three circled components are the ones that get really hot. I can pick out the drv chip but I’m assuming that the top chip is the can transceiver?
![image|375x500](upload://qJeTm5dFjaHW29RA8h53Gzg959y.jpeg)
```

---
## \#7 Posted by: b264 Posted at: 2019-02-21T02:43:54.132Z Reads: 94

```
It sounds like a short on your 5V power supply rails
```

---
## \#8 Posted by: b264 Posted at: 2019-02-21T02:44:11.902Z Reads: 94

```
The top chip is the MCU
```

---
## \#9 Posted by: b264 Posted at: 2019-02-21T02:44:45.414Z Reads: 92

```
What brand is the VESC?  Where did it come from?
```

---
## \#10 Posted by: J_Dizzle Posted at: 2019-02-21T02:51:49.185Z Reads: 91

```
Torqueboards, 4.12. I was using it with canbus, but there were no sparks or signs of anything going wrong
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2019-02-21T02:52:26.114Z Reads: 88

```
Short is on the 3.3v, the mcu is not powered by the 5v...

To be sure you can you check this

https://www.electric-skateboard.builders/t/no-power-to-enertion-vesc/7600/8?u=johnnymeduse
```

---
## \#12 Posted by: J_Dizzle Posted at: 2019-02-21T17:20:02.261Z Reads: 73

```
Thanks for the info, is there anything that could be causing this that could be an easy fix, cause tbh I’m pretty much out of funds :man_facepalming: 

I’ll tag @b264 also because he was here earlier too
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2019-02-21T17:33:17.567Z Reads: 69

```
You can always remove the 2 CAN transceiver chip and use split PPM configuration.
```

---
## \#14 Posted by: J_Dizzle Posted at: 2019-02-21T18:11:39.387Z Reads: 67

```
@JohnnyMeduse
 Sweet! So I would de solder the can trasciever and run the vescs in ppm? Are there any side affects or error codes I should know about?

Edit: where is the can transceiver on the Vesc? lol
```

---
## \#15 Posted by: JohnnyMeduse Posted at: 2019-02-21T19:54:22.145Z Reads: 57

```
![Inkedbb55b289e203a3c5e0bb1caf1ff2f0a4a5be8cbc_LI|375x500](upload://uDSGTVI0krcjBWymkUIJMJOagp1.jpeg) 

This one in yellow, 

No there should not have any error code after.
```

---
## \#16 Posted by: J_Dizzle Posted at: 2019-02-23T02:21:40.112Z Reads: 36

```
Hello, sorry to summon you again @JohnnyMeduse but I removed the can chip from both vescs and one works fine, but the other I programmed regularly and it barely stutters and the yellow led on the bottom flickers really fast. Any thoughts on that?
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2019-02-23T02:23:52.851Z Reads: 36

```
That really weird, it could be that something else as been damage... Can you post pic or video of it?
```

---
## \#18 Posted by: J_Dizzle Posted at: 2019-02-23T02:43:22.120Z Reads: 35

```
@JohnnyMeduse
 It won’t let me upload a video from my phone, but here is a photo
![image|375x500](upload://chXEZOWA1BhiqwdXvcdv7Od5V0k.jpeg) 

It never turns off it just goes bright then dim
```

---
## \#19 Posted by: JohnnyMeduse Posted at: 2019-02-23T03:04:12.710Z Reads: 34

```
Does the motor run, does the vesc look like it work fine or it is just doing this all the time? Because it is the signal light if it sends a command to the drv the light should brighten, then dim down, and when your programming a Firmware it should flash. 

[quote="J_Dizzle, post:18, topic:84875"]
It won’t let me upload a video from my phone
[/quote]
You need to upload it to youtube first, then post the link.
```

---
## \#20 Posted by: J_Dizzle Posted at: 2019-02-23T03:29:15.936Z Reads: 28

```
So... the problem just randomly fixed itself lol case closed I suppose
```

---
## \#21 Posted by: JohnnyMeduse Posted at: 2019-02-23T03:31:02.936Z Reads: 28

```
I guess... but it is still weird, just be cautious at first :confused:
```

---
## \#22 Posted by: J_Dizzle Posted at: 2019-02-24T19:42:24.950Z Reads: 20

```
This is fucking pissing me off now. So I have a brand new @torqueboards vesc, and it out of the blue blows the can transceiver on both of my vescs. I know that it is easy to make the mistake of connecting CAN wrong, but I connected the can cable to both of my vescs, and powered them on both at the sames time, just like you are supposed to. As seen above, I removed the transcievers off both vescs, and are running them in split ppm. cool. however before I can even get off the bench, I'm finding that the BRAND NEW vesc is smoking from the 3 pins for the servo cable. 
I'm tagging @torqueboards cause I feel like I got a faulty vesc etc... but we can take that to pm I suppose (trying to abide by new rules)
Again @JohnnyMeduse I hate to bug you, but any idea about this new problem?
```

---
## \#23 Posted by: JohnnyMeduse Posted at: 2019-02-24T19:46:01.415Z Reads: 19

```
could you post some closeup picture of it?

Also, what firmware are you using?
```

---
## \#24 Posted by: torqueboards Posted at: 2019-02-24T19:46:30.442Z Reads: 20

```
You can program a dual vesc setup and just connect the canbus afterwards that way you don't damage the can transceiver. Just remember which one is master. Send us an email. We'll replace it.
```

---
## \#25 Posted by: JohnnyMeduse Posted at: 2019-02-24T19:49:24.440Z Reads: 19

```
I guess you didn't read the thread Dexter, Can is ALREADY blown. And now look like it has issue with the PPM... it is probably gonna be a dead MCU.
```

---
## \#26 Posted by: J_Dizzle Posted at: 2019-02-24T19:50:50.821Z Reads: 19

```
[Uploading: 24334EA1-75C0-4355-BAF2-CE0D18B3485D.jpeg...]() [Uploading: CBF77C91-2678-4D35-9FAA-8AC65CFB49B5.jpeg...]() [Uploading: 12B6AB6A-90F2-4A90-AA91-B288FFC94B48.jpeg...]() 
I’m using Ack 3.103 on both 
@JohnnyMeduse
```

---
## \#27 Posted by: torqueboards Posted at: 2019-02-24T19:51:03.127Z Reads: 19

```
Thanks Johnny. @J_Dizzle Email me and we'll get you squared away.
```

---
## \#28 Posted by: JohnnyMeduse Posted at: 2019-02-24T19:54:07.588Z Reads: 19

```
maybe you could try to switch FW... sound like I could have something to do with the MCU. Maybe try the old 2.18 or the new Vesc_tool from vedder.

Doesn't look like the picture upload properly
```

---
## \#29 Posted by: J_Dizzle Posted at: 2019-02-24T19:56:12.091Z Reads: 18

```
Yeah the pics are loading I will try again but there are not visible burn marks or anything. It doesn't smoke when I connect it to power, there is no response when I do that it is when I connect the servo cable then it starts smoking from right there
```

---
## \#30 Posted by: JohnnyMeduse Posted at: 2019-02-24T19:59:12.069Z Reads: 17

```
I just remember a little detail, If you use split PPM make sure that the 5V (or red cable) is only connect to one VESC
```

---
## \#31 Posted by: J_Dizzle Posted at: 2019-02-24T20:00:03.877Z Reads: 19

```
:man_facepalming:
I guess that would be the problem, so if I snip the red (positive) then it may work?
```

---
## \#32 Posted by: JohnnyMeduse Posted at: 2019-02-24T20:05:24.183Z Reads: 17

```
I can't confirm 100%, but that could be a good root cause for the smoking PPM
```

---
## \#33 Posted by: J_Dizzle Posted at: 2019-02-24T20:15:23.259Z Reads: 15

```
Well I cut one positive wire, and there is no more smoke, but I think the vesc is fried.
```

---
## \#34 Posted by: JohnnyMeduse Posted at: 2019-02-24T20:16:07.131Z Reads: 17

```
does the blue light still powerup?
```

---
## \#35 Posted by: J_Dizzle Posted at: 2019-02-24T20:17:02.201Z Reads: 17

```
No, no signs of life at all
```

---
## \#36 Posted by: JohnnyMeduse Posted at: 2019-02-24T20:24:34.799Z Reads: 16

```
HUMMM... Yeah I'M guessing that the TVS diode as been shorted. Maybe if you have a multi-meter you could check if D5 is shorted
```

---
## \#37 Posted by: J_Dizzle Posted at: 2019-02-24T20:28:32.087Z Reads: 16

```
ok, where is that located?
```

---
## \#38 Posted by: JohnnyMeduse Posted at: 2019-02-24T20:31:32.508Z Reads: 16

```
![IMG_20170818_105854|374x499](upload://1nUzLfn390UkgBX45bEeFO23u3P.jpg)
```

---
