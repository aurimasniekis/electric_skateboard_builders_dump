# Motor spin and VESC tool issue

### Replies: 8 Views: 303

## \#1 Posted by: SeVeSeventyOne Posted at: 2019-06-13T18:09:45.485Z Reads: 65

```
Hi,
Few questions, setup 12s, FSESC6.6, SW3.57, HW60,
I went through VESC tutorial how to set basic parameters, FOC detect with wizard etc. I did not manage to spin the motor properly after detection was succesfull. During the detect motor was running smooth, but after detection I used arrow keys to perform testing, it chops constantly.
What is the difference during detection and "normal" run ? and why it ran smooth on detect phase only?
What does the arrow keys do, which speed it tries to drive the motor ? can i adjust it ?

If I run FOC detection, what does the motor selection make a difference?, I selected ~2kg outrunner and I got an error: -11 ???? .VESC terminal code: "FAULT" said no fault messages.. ?
Then in wizard I chose ~6kg hub motor and motor spun okay.

https://www.youtube.com/watch?v=5qXtW_bkiIo

 Now what is the difference, did I get the correct parameters or are they just rough estimations or even incorrect, should i try to tweak them somehow, which direction ? Does FOC require pole count?, where can I see that or set it? Shouldnt detection know that already and show it on that info box after detection is done?  I remember playing around with Texas Instruments FOC demo board, and pole count was essential parameter to drive the motor.
Anyway by using arrowkeys motor does this after FOC detection completed:
https://www.youtube.com/watch?v=ZlLF0NHaJDw

Is there any good tutorial for troubleshooting issues? For me it is a bit ackward to start randomly try everything, I should know where to start and are my settings completely useless. I can start posting my current settings if that has any help to anyone.



Thanks
```

---
## \#2 Posted by: trampa Posted at: 2019-06-13T18:46:24.220Z Reads: 52

```
Choice of motor size determines amps used for detection. Startup with keyboard might not send enough amps to get a proper startup. You can define a higher Amp usage for keyboard controlls in the tool.
```

---
## \#3 Posted by: SeVeSeventyOne Posted at: 2019-06-13T19:06:26.254Z Reads: 49

```

Do you mean this setting window ?
I raised the current up to 14Amps and nothing, problem just got worse.
During motor detection I hardly saw not more than an 1amp and still smooth running.
I'm running on 12S and 14 amps is quite a bit of wattage to just start the free spinning motor...

![VESCtool_pic1|642x499](upload://z2DvEpZ3XVPCpn33OqjU7xkI2kG.jpeg)
```

---
## \#4 Posted by: trampa Posted at: 2019-06-14T10:02:20.357Z Reads: 36

```
Hub motors can be a bit trickey. It also depends on the ESC. Don't know how well the Flipsky stuff works. 
The original Trampa VESC SIX Plus should spin this motor up with out any issues.
```

---
## \#5 Posted by: trampa Posted at: 2019-06-14T12:23:02.070Z Reads: 29

```
What about Hall sensors? Do you use them?
```

---
## \#6 Posted by: SeVeSeventyOne Posted at: 2019-06-14T12:35:01.730Z Reads: 28

```
I did not try sensors, I thought since it ran smooth in FOC detection mode, I dont need them. But I guess detection ran on open loop.
```

---
## \#7 Posted by: trampa Posted at: 2019-06-14T12:52:30.141Z Reads: 27

```
That is FOC open loop, correct.
```

---
## \#8 Posted by: SeVeSeventyOne Posted at: 2019-06-14T19:13:52.454Z Reads: 20

```
Hall sensors are now connected. I have tried few things but if I spin the wheel by hand motor turns but shuts down after 0.5 seconds like its going out of sync or something and shuts down itself.

Where I can see pole count of the motor? I can set there a pole count manually, and when using wizard detection, nothing happens. I can input crazy pole count numbers and no change by wizard. Are those numbers even used to anything, don't know.
```

---
