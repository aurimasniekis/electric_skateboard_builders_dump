# VESC won&rsquo;t connect

### Replies: 5 Views: 669

## \#1 Posted by: radium Posted at: 2017-02-16T18:54:28.901Z Reads: 79

```
I am attempting to program my TorqueBoards VESC. I have tried on OSX using the BLDC tool from enertion and on Linux Mint(Ubuntu based) using Vedder's instructions on his website.

I know people say you are supposed to use a low voltage low amperage power supply when programming the VESC, but I don't have one, so I am using a single 6S lipo.

The vesc is connected to the motor, but not to the RC receiver.

Upon delivering power to the VESC the red light blinks 3x, then a red and a blue light stay on until I remove power.

On MacOS(not OS X) BLDC-Tool only has one serial option and it is something about bluetooth. On Linux Mint it lists TTYS0-TTYS9 options. I have tried every port option on Linux to no avail. I have tried plugging in the VESC to various USB ports on both computers.

I'm currently installing Windows 10 onto the Linux box to attempt this on Windows. In the interim does anyone have any suggestions on why it might not be working?

On linux, I added myself to the dialout group as suggested by Vedder, but I still have to run sudo ./BLDC_Tool to get access to the serial ports. As far as I can tell neither computer is even acknowledging the connection. Perhaps my mini USB cable is bad?

I am going to go buy a 2nd Mini USB cable right now just in case since I have to run to the store anyway.

As a side note the USB cable between VESC and computer gets noticeably warm when plugged in.
```

---
## \#3 Posted by: radium Posted at: 2017-02-16T19:52:49.438Z Reads: 69

```
I can't tell if it's a red or a green light flashing 3x on power up. I'm color blind. I think it's red though, and I think it's actually a blue and a green LED that remain on indefinitely.
```

---
## \#4 Posted by: Luke Posted at: 2017-02-16T20:08:01.350Z Reads: 64

```
It's usually a red light that flashes three times. You can always ask for @torqueboards for a hand on his website. but first maybe try it with a new usb cable.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-02-16T22:07:15.839Z Reads: 54

```
what type of Mac are you using?
```

---
## \#6 Posted by: radium Posted at: 2017-02-16T22:52:13.312Z Reads: 49

```
I am using a 2013 MB Pro. I actually got it working... turned out my cheap USB cable had an internal short. How do I tag this post solved?
```

---
