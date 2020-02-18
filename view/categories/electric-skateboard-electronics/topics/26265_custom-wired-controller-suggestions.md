# Custom Wired Controller Suggestions

### Replies: 7 Views: 737

## \#1 Posted by: jango955 Posted at: 2017-06-27T13:50:06.772Z Reads: 108

```
So i'm working on my first build, but despite a few issues minor issues, I'm currently sitting on a dual drive board with specs shown below:

2 320 KV Motors
2 hobbyking 120a ESC'S
custom built 22.2v 3300Mah Batteries
Custom cut Saltrock longboard deck
Paris Trucks

However, I HATE wireless controllers. So, i've been working through some alternatives.
So far i've been using a servo tester, modded with a log slide potentiometer. Unfortunately, each time i use the board i have to play with the servo tester settings until i find the correct one to control the board, and in doing so, the motors usually suffer some erratic commands ( like full power forwards then immediate full power reverse )
As this is.... rather unhealthy, and the controls are a little crude, i want a stronger alternative.

Currently looking into wired wii nunchuck + arduino circuit board
Modding a scalextric controller to Arduino

If anyone knows of anything easier, cheaper or generally more effective, i'd really like to hear it! as i said previously, looking for a wired alternative that's more effective than a servo tester.
```

---
## \#2 Posted by: smurf Posted at: 2017-06-27T17:17:58.660Z Reads: 94

```
I saw a video on YouTube last year where this one guy made a wired controller for his board. Unfortunately that was before I started saving all useful links.
```

---
## \#3 Posted by: wafflejock Posted at: 2017-06-27T20:12:56.102Z Reads: 80

```
I made a wireless remote of my own based on the nrf wireless modules and arduino pro mini boards.  If you wanted to you could do something similar but just have a wire that runs down the JST/servo throttle plug on the ESC.  In the arduino I hard coded the top and bottom limits for the incoming potentiometer values and over a year riding with it and the values have never had to be changed from the original programming.  The arduino nano or pro mini boards would work but the 3.3V/8MHz variant is probably what you'd want so you can use the 5V off the BEC on the ESC and have it going in the RAW or VIN pin and getting regulated down to the correct voltage for the board (I've used both 5V and 3.3V boards powered off 1S LiPo and they work but it's a bit out of spec).

The servo library in arduino makes it easy to make a call to writeMicroseconds(1500) or the like on a "servo" instance to generate a pwm signal (believe at 50hz by default).

https://github.com/shusain/eskatecontroller

Since you're wanting to forgo the wireless the PCB isn't really necessary I just made those to make sure the wireless module pins all stayed connected and to get rid of the wire clutter from those modules.  All you need is two signal wires for the potentiometer and the ESC, and the power/ground into the arduino and power/ground into the potentiometer.
```

---
## \#4 Posted by: wafflejock Posted at: 2017-06-27T22:32:20.791Z Reads: 70

```
Also, I just ordered some of my boards from pcbway.   It was the same price to get 10 as to get 5 and couldn't just order the 2 (or 1) I actually need/want so I have a few spares if you want one PM me and can probably ship you one in an envelope when I get them here (just hit shipping in China, coming to IL)  You could use the same board in your wired setup just skip putting the nrf module on the board but hook up the ESC wires and potentiometer wires and solder the arduino pro mini on there (programming is a bit difficult once it's assembled but can put 90 degree male headers on the pro mini to make hooking it up to a FTDI break out board easier).  You'd have to mash up the code from the transmitter and receiver (and pull out the transceiver parts) but shouldn't be too difficult.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-06-27T22:40:55.565Z Reads: 66

```
why do you hate wireless controllers?
The one I use works so good that I couldn't imagine any wired controller that would be better.

<img src="/uploads/db1493/original/3X/3/c/3c5eae8e683ede16b8de22b22f5f5b1eb00577d6.jpeg" width="375" height="500">
```

---
## \#6 Posted by: _AI Posted at: 2017-06-28T02:42:38.566Z Reads: 54

```
I agree with you
```

---
## \#7 Posted by: psychotiller Posted at: 2017-06-28T02:46:39.134Z Reads: 49

```
I have a wiimote that you could plug your wired nunchuck straight into and it would be the best controller ever! No dropouts, cruise control, and flawless acceleration and braking.

$20 + shipping
```

---
