# VESC Connection

### Replies: 22 Views: 2972

## \#1 Posted by: arpitdave Posted at: 2016-04-01T02:45:33.840Z Reads: 183

```
I bought enertion motor, space cell, VESC. I have a FS-GT2 remote controller. when I turn the battery on, the VESC green and blue light both turn on. I was able to connect the controller to its receiver. Currently the servo cable is connected to the VCC channel of the receiver. When i plug the VESC into my computer I dont see it on BDLC. All I see is from the picture below. What is happening? How do i fix this?

Also, when i press accelerate on my controller the motor isn't rotating. Is there something I am missing?
```

---
## \#2 Posted by: arpitdave Posted at: 2016-04-01T02:46:19.635Z Reads: 188

```
<img src="/uploads/db1493/original/2X/4/443b0c9105c22dee04d2af1915840a76028972d4.png" width="690" height="350">
```

---
## \#3 Posted by: onloop Posted at: 2016-04-01T03:27:04.059Z Reads: 188

```
[quote="arpitdave, post:1, topic:2095"]
When i plug the VESC into my computer I dont see it on BDLC
[/quote]

what port is the VESC connected to? Are you using bluetooth?
```

---
## \#4 Posted by: arpitdave Posted at: 2016-04-01T03:27:49.980Z Reads: 188

```
It is plugged into through a USB on a macbook pro
```

---
## \#5 Posted by: onloop Posted at: 2016-04-01T04:16:29.096Z Reads: 189

```
http://www.electric-skateboard.builders/t/vesc-faq-in-depth-video-how-to-program-your-vesc/2088
```

---
## \#6 Posted by: arpitdave Posted at: 2016-04-01T04:31:57.722Z Reads: 182

```
Clarification: I changed the servo to channel 2. Now  when i press the acceleration the motor slightly moves and then stops. Any ideas?
```

---
## \#7 Posted by: onloop Posted at: 2016-04-01T04:35:05.031Z Reads: 168

```
did you do a motor detection?
```

---
## \#8 Posted by: arpitdave Posted at: 2016-04-01T04:36:29.723Z Reads: 163

```
what does that mean?
```

---
## \#9 Posted by: onloop Posted at: 2016-04-01T04:40:07.313Z Reads: 151

```
Owning/using a vesc requires some prior knowledge, read this stuff.

http://www.electric-skateboard.builders/search?q=vesc%20faq
```

---
## \#10 Posted by: arpitdave Posted at: 2016-04-01T04:40:38.455Z Reads: 146

```
I cant run a motor detection until the port is recognized by the BDLC right?
```

---
## \#11 Posted by: trbt555 Posted at: 2016-04-01T05:06:05.354Z Reads: 143

```
Select the correct port in the upper right drop-down under "serial connection" and click connect. (tip: it ain't bluetooth)
You'll see the connection status in the lower right portion of the window taskbar. Green is good, red is bad.
If your vesc has a firmware version that is incompatible with the BLDC version you're using, it will tell you so. You then have the choice to either upgrade the firmware (the binaries came with BLDC) or dowload a BLDC version that is compatible with the firmware on your vesc.
Please read-up on the vesc faq's and user threads before attempting any changes or you'll risk damaging your vesc.
```

---
## \#12 Posted by: arpitdave Posted at: 2016-04-01T05:15:03.316Z Reads: 132

```
So in the serial connection both the options in the drop down menu are bluetooth, one is bluetooth-Incoming-Port and the other is bluetooth-modem
```

---
## \#13 Posted by: arpitdave Posted at: 2016-04-01T05:30:20.866Z Reads: 134

```
Going through the FAQ, it seems that a problem could be the firmware. How do i know the correct firmware to upload. I couldnt find the instructions in any of the FAQ's
```

---
## \#14 Posted by: constantinos156 Posted at: 2016-04-01T08:05:03.408Z Reads: 129

```
Jacobbloy released a great in depth video in the FAQ section explaining a lot about the VESC, go through it and I assume all your questions will be answered
```

---
## \#15 Posted by: trbt555 Posted at: 2016-04-01T12:03:05.563Z Reads: 123

```
What's the hw version of your vesc, what is the version of bldc you're using ?


You can't flash the firmware with BLDC if you can't connect to the VESC by usb.
If your vesc doesn't have a bootloader you're in for some fun Linux command line stuff and you might be better off sendig it to someone who has already done this procedure.
```

---
## \#16 Posted by: Sharkface Posted at: 2016-04-01T14:52:35.078Z Reads: 118

```
@EnertionSupport usually puts firmware on the VESCs sold at Enertion, I thought I had to update my firmware but it turned out the usb cable itself was just upsetting the VESC. If the drop down is only showing bluetooth you might want to try a different usb cord and port. I know I had troubles connecting when I was connecting through a USB hub.

As mentioned before there is a youtube video that is fairlly long and in depth put out by one of our other members:

http://www.electric-skateboard.builders/t/vesc-faq-in-depth-video-how-to-program-your-vesc/2088


EDIT: missed the bit about your connections only showing bluetooth.
```

---
## \#17 Posted by: chaka Posted at: 2016-04-01T14:56:08.573Z Reads: 114

```
If you click the refresh button next to the "connect' button it should find the correct port, at least this is how it functions in the linux version.
```

---
## \#18 Posted by: arpitdave Posted at: 2016-04-01T15:08:14.861Z Reads: 105

```
The hardware is 4.10...
```

---
## \#19 Posted by: arpitdave Posted at: 2016-04-01T15:09:31.686Z Reads: 100

```
I did press refresh and nothing new appeared. I have all battery connected and on as well. The video that goes in depth doesnt resolve my problem. I can recognize the VESC so i cant make any of the setting changes that the video talks about.
```

---
## \#20 Posted by: chaka Posted at: 2016-04-01T15:11:05.788Z Reads: 97

```
Do you see 3 red flashes from the led's when you power up your vesc? If not then it does not have firmware loaded and will need to be flashed.
```

---
## \#21 Posted by: arpitdave Posted at: 2016-04-01T15:14:42.422Z Reads: 91

```
I only see the red ligth turn on as soon as I turn the battery on. Once it is on the red light goes away
```

---
## \#22 Posted by: Pow Posted at: 2016-06-24T16:22:53.040Z Reads: 72

```
Hi guys, can anyone provide me with a working download link for the 2.17 BLDC tool for mac? Ive tried many times to download from http://vesc.net.au but i can't get a download link! Thank you
```

---
