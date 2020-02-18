# Pointers in building custom controller for eboard?

### Replies: 7 Views: 916

## \#1 Posted by: cjoliver Posted at: 2016-06-19T20:54:05.502Z Reads: 126

```
Once all my mechanical and electrical stuff comes in, I plan on building a custom controller for the VESC. Im not talking about rebuilding an existing controller into a smaller form controller, but to start from scratch and take advantage of the UART controller implemented into the VESC.

So I was wondering if anyone else has tried this and what they've come across?

I've heard connection issues with the nrf24l01 but haven't seen any specific analysis of it

Also I want to make a screen on the controller with speed, battery level of both longboard and controller, and maybe distance traveled

Thoughts?
```

---
## \#2 Posted by: rpn314 Posted at: 2016-06-20T00:30:14.485Z Reads: 110

```
Look at the nunchuckRF project, which is really only a nunchuck in name. It's at least partially created by Vedder and its in a few topics on here and on endless-sphere. Also take a look at the topic on endless-sphere called [OpenSource Remote for VESC ArduBoardControl](https://endless-sphere.com/forums/viewtopic.php?f=35&t=73812). RollingGecko is using an arduino nano and UART over Bluetooth I believe.

Much like the nunchuckRF project, he's using an arduino shell, but I'm positive you could get it into just about any enclosure you'd prefer.
```

---
## \#3 Posted by: DougM Posted at: 2016-06-20T15:21:19.622Z Reads: 75

```
I did it - so far it has worked out great.

I use XBees to talk between the handheld and the controller board and have had very few communications issues (occasionally on one of the handhelds the XB goes offline but the controller correctly detects it and shuts down the driver.  Power the handheld off and back on and it all comes back.  This has not been a problem on the other 3 boards)

I use an Adafruit 9DOF in the handheld to determine the tilt of the controller.  horizontal is neutral, down is brake, up is go fast.  I have both a power switch and an "arm" button on the handheld.  My biggest mistake was putting these right next to each-other.  it confuses people.  Next time I'll make the power switch a slide switch and nowhere near the arm button.

I use Teensy 3.2's on both the controller and the handheld.  This works great but they are a bit power hungry.  I haven't played around with decreasing clock speed.  I did have one Teensy die from (best guess) static, so now I am in the process of covering all control boards with a metal shield.

I also have a display but it's mounted to the board since the act of looking at the display on the handheld would cause you to change the throttle position.  I get my displays from Buydisplay.com.

There's a lot of space for innovative controllers - good luck!

DougM
```

---
## \#4 Posted by: cjoliver Posted at: 2016-06-20T17:01:22.761Z Reads: 59

```
I thought about using Xbee, they're just a little expensive for what they do. They're probably like this because I've only seen them available in shield form. However I was thinking about using the nrf24l01 + PA (power amplifier), seeing one of these is about $10 and the receiving wouldn't need the PA but could be one of the cheap little ones.

Why use an IMU? Does the board not get confused when it goes up hills and changes the angle of your hand? 

I'm sure you already know about the arduino, but using these to program another atmega328 would allow you to mess around with the fuses and allow a more power efficient device

Thanks for the input! Doesn't seem like the eboard community focuses on controllers a whole lot
```

---
## \#5 Posted by: DougM Posted at: 2016-06-20T17:37:27.142Z Reads: 58

```
I don't know much about the NRF but I like XBee because it just works.  They are expensive and have a whole slew of features you really don't need, so for the same functionality you can probably find something cheaper.  I just didn't want to mess with it for the few I was building.  I did dial the transmit power down since I'm only going from handheld to board.  

I haven't focused much on power savings in the controller since I have yet to have the board outlast the controller and have yet to run a board completely down.

I use the tilt sensor because originally I designed it to be controlled with a phone before I decided that was a bad idea.  Out of that approach I liked the intuitiveness of a handheld you simply tilt to get what you want.  physical triggers seem old school.

The teensy as I'm sure you know lives in the arduino environment.  It just happens to be my go-to-platform.  You could just as easily do it on any Arduino, except for form factor.  There are lots of power saving features in the chipset - again I haven't taken the time.

DougM
```

---
## \#6 Posted by: cjoliver Posted at: 2016-06-20T21:15:59.192Z Reads: 41

```
I like the idea of the imu, but how do you deal with going up hills and confusing the it?
```

---
## \#7 Posted by: DougM Posted at: 2016-06-20T22:06:09.340Z Reads: 39

```
I use the IMU strictly as a tilt sensor on the handheld.  Because my body position changes when I climb hills it never knows the difference.

Is that the question you are asking?  Or am I confused?

DougM
```

---
