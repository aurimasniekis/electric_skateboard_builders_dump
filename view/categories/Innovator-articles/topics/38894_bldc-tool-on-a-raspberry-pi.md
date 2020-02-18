# BLDC Tool on a Raspberry Pi

### Replies: 17 Views: 2070

## \#1 Posted by: orkunturkey Posted at: 2017-11-21T09:50:06.781Z Reads: 225

```
Before you ask why I want to run BLDC Tool on a Raspberry Pi, why not?
There would be so many things you can achieve if you had realtime access to your VESC. you could program things to work in a certain way. besides, you could do a lot more by adding motion, heat sensors etc.

I tried compiling the BLDC Tool on a raspberry pi 2 running on Raspbian Jesse, with no luck. I think thats because I was unable to make Qt work on the Pi.

Before I give more details regarding what went wrong when I tried compiling the BLDC Tool on the pi, I just wanted to see if anyone had any luck with this.

Orkun
```

---
## \#2 Posted by: scepterr Posted at: 2017-11-21T09:58:39.119Z Reads: 217

```
Tried these fixes?
http://vesc-project.com/node/138
```

---
## \#3 Posted by: orkunturkey Posted at: 2017-11-22T11:40:30.071Z Reads: 187

```
I owe you lunch! After eight hours of fiddling around trying to compile the qt app on the raspi, this was the only thing that made it work. Thanks, man! I will make a short how-to guide about this soon.
```

---
## \#4 Posted by: longhairedboy Posted at: 2017-11-22T13:04:14.874Z Reads: 176

```
oh hell yes. 

Would you be able to source some sort of screen to go with it.. like some kind of touch screen or maybe a clamshell device with a screen and keyboard?
```

---
## \#5 Posted by: orkunturkey Posted at: 2017-11-22T14:31:20.709Z Reads: 165

```
@longhairedboy I already tried doing that on a 3.5 inch GPIO touchscreen. But since qt apps dont scale like that, it was impossible to see the whole window without maybe panning around the screen. Instead I was thinking of creating an iphone hotspot and connecting to the  raspi via VNC. Nevertheless, this is what it looked like :slight_smile:

<img src="/uploads/db1493/original/3X/2/9/29d916921ed86598117183c57ca889cca4833c9c.jpg" width="281" height="500">

<img src="/uploads/db1493/original/3X/3/5/35f3cc80f1bd34989908fcdb60854bba1166b8ec.jpg" width="281" height="500">

I know its whacky as hell, but I just wanted to see how worthwhile it is to collect usage data and adjust settings on the go.
```

---
## \#6 Posted by: orkunturkey Posted at: 2017-11-22T14:35:18.369Z Reads: 146

```
Three problems remain with this setup:

* Feeding power to the pi through the VESC.

* Adding another vesc to make use of the dual hub motors.

* Editing the Ackmaniac BLDC Tool to work on smaller resolution screens WITHOUT panning. (cant show how it looks like on the screen since I had to delete the LCD Drivers for emptying space for all the qt packages)
```

---
## \#7 Posted by: longhairedboy Posted at: 2017-11-22T14:44:01.468Z Reads: 141

```
BLDC Tool needs a locally hosted service API so it can run headless. Compiling QT for a million screens is stupid when you could load it up as a service and just plop a JS app on top of it. Any JS app. For any situation, such as these dumb tiny screens.
```

---
## \#8 Posted by: orkunturkey Posted at: 2017-11-22T14:48:22.418Z Reads: 140

```
not very familiar with javascript. I will look what needs to be done tomorrow. it would be awesome if someone housed an LCD screen on their setup, for benchmarking with different VESC builds, motors, etc.
```

---
## \#9 Posted by: longhairedboy Posted at: 2017-11-22T14:57:38.104Z Reads: 138

```
You could effectively do that with a data logger and then build something to parse and display the data in a usable , friendly, and possibly exciting  fashion. Plenty of charts and graphs and the ability to compare them as overlays and whatever. There are apps for phones that do some of this but i would like to see a nice desktop app with big screen support for really showing all those datas and their bits. At some point i'm going to do this because that's actually something i can do. Ripping logs is a skillset i happen to have. Also replaying the log as recorded media through some kind of dashboard would be amazing.
```

---
## \#10 Posted by: scepterr Posted at: 2017-11-22T19:06:50.342Z Reads: 130

```
Power for rpi from any battery 
<img src="/uploads/db1493/original/3X/9/4/94236902f3569c0c91efe177f0e4c7a9466e68df.jpg" width="666" height="499">

@longhairedboy  fuck screens, portable projector, screen on the road in front of you 😎
```

---
## \#11 Posted by: longhairedboy Posted at: 2017-11-22T19:10:26.759Z Reads: 126

```
only if it can be done with high powered lasers to defeat the sun light. 

lasers that can also be used to target and vaporize flying insects headed for my face.
```

---
## \#12 Posted by: orkunturkey Posted at: 2017-11-23T02:43:05.831Z Reads: 114

```
you thought I haven't thought about this? :smiley: You wouldn't be able to see it during the day though!
```

---
## \#13 Posted by: scepterr Posted at: 2017-11-23T02:44:35.619Z Reads: 115

```
You wouldn't be able to see an rpi screen either 😋
```

---
## \#14 Posted by: rodread Posted at: 2018-02-01T14:14:25.188Z Reads: 101

```
Well done on porting to Pi, I'd love to try this too.
Any progress on writing the "How to?" 
I've got a need to change contorl parameters on the fly whilst running... and recording data would be great too.

I'm using a bike hub motor in regen (For a flying wind turbine.. Daisy windswept-and-interesting.co.uk)
Taking a Pi out in the field is going to be better than taking my pc out.. :frowning:
 
For my first test all I want to be able to do is
Monitor unloaded ERPM, then set an ERPM level and send it as a UART control equivalent of the VESCtool (in Windows) button for setting ERPM speeds. I'd also like to be able to send the equivalent stop command to avoid any regen.
I'm hoping to eventually use live wind data or line angle data to set rotor speeds.

Any bonus functionality like displaying voltage... rocks!
thanks
```

---
## \#15 Posted by: orkunturkey Posted at: 2018-02-02T07:52:57.134Z Reads: 93

```
I first started with the standard raspbian jesse OS. You need to update and upgrade your OS to make sure everything is working fine. So begin with entering these:

    sudo apt-get update
    sudo apt-get upgrade
Depending on your internet connection, this might take a while. After this, you are going to get the dependencies to compile bldc-tool on your raspberry pi:

    sudo apt-get install qt-sdk

Always good practice to restart after this.
make sure you have the correct bldc-tool for your specific firmware. I used the @Ackmaniac's bldc-tool for my setup, since it supports v2.54
After this, change your working directory on the terminal to the folder where bldc-tool files are. 

    cd /(PATH TO YOUR BLDC-TOOL FILES)
Now we have to add some parameters into the vesc_tool.pro file. Open that with nano:

    nano vesc_tool.pro
add this line to the end of the file. press ctrl+c and then type Y to save your changes:

    CONFIG += C++11   

afterwards, run these two lines to clear your working space:

    make clean
    qmake

You will have to wait for a while, it took me around 5-7 minutes to compile everything together. At the end you should have a new file called BLDC_Tool . Run this line in the BLDC_Tool directory to run the program:

    ./BLDC_Tool

I might be wrong about the file name but it should be a file with no extension. Let me know if you run into any problems. It would be a nice idea to create a mobile hotspot and make the raspberry connect to it, and then create a VLC Connection to the raspberry to control the operation of the BLDC Tool
```

---
## \#17 Posted by: Clonkex Posted at: 2018-02-02T10:29:20.015Z Reads: 86

```
You might have to
`sudo chmod +x BLDC_Tool`
first, then
`./BLDC_Tool`

because I 100% definitely know what I'm talking about, mmhmm, definitely, absolutely no copy-paste at all...

:P

EDIT: For future reference, b264 posted a those instructions but then deleted his post because he remembered he wasn't going to be helpful any more, so I copy-pasted them from the edit history ;)
```

---
## \#18 Posted by: roidimitris Posted at: 2018-12-14T22:35:14.232Z Reads: 34

```
Thanks for this awesome post!
It looks like it can't run the make line and compile.
It gets me here: make: *** No rule to make target 'clean'. Stop.
```

---
