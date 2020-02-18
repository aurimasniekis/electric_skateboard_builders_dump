# Do I have a blown ESC?

### Replies: 9 Views: 950

## \#1 Posted by: brandon Posted at: 2016-10-12T22:30:32.568Z Reads: 102

```
I have a 150A xcar esc from hobbyking. I finally thought I had everything I needed to go for a test ride, but when I turn it on, I get a red + blue led, which the manual indicates as the esc sensing a sensored motor, which i do not have. It should just be a blue light.

I don't have the receiver yet, would that have anything to do with it, or do I need to get ready to send this back to HK?
```

---
## \#2 Posted by: mccloed Posted at: 2016-10-12T23:32:30.571Z Reads: 91

```
I would say wait till you get a Transmitter and Receiver. This could just be the ESC saying there is no connection.
```

---
## \#3 Posted by: brandon Posted at: 2016-10-12T23:47:03.373Z Reads: 90

```
There are a couple videos online with seemingly the same issue. The manual also states that the ESC should detect the motor type and display the appropriate LED color on startup. I've also tried feeding it a signal via arduino but no dice.
```

---
## \#4 Posted by: Maxid Posted at: 2016-10-13T00:23:22.879Z Reads: 73

```
I have the same ESC - as far as I remember the motor detection and voltage beeps only happen after connecting the receiver AND turning on the remote.
Also how were you planning on doing a test ride when you don't have the receiver (and remote)? Also you need to "initialize" the ESC with your throttle setup.
```

---
## \#5 Posted by: brandon Posted at: 2016-10-13T04:19:16.278Z Reads: 53

```
Would you mind unplugging your receiver and seeing what it does?

I thought the controller was waiting for me, but it wasn't, but I was going to write up an arduino sketch to control it via bluetooth for the time being.
```

---
## \#6 Posted by: Maxid Posted at: 2016-10-13T07:16:37.013Z Reads: 49

```
ok tried it and have to tell you that when I unplug my receiver I get both LEDs to light up but they don't blink.

Edit: just realized that you did not say anything about blinking or not. So all good!
```

---
## \#7 Posted by: TarzanHBK Posted at: 2016-10-13T07:27:43.843Z Reads: 48

```
i have an x-car beast 150a which light up blue and red. After connecting the receiver and setting it up, it should go to blue.
just wait for your receiver to arrive :slight_smile:
```

---
## \#8 Posted by: lowGuido Posted at: 2016-10-13T09:10:02.112Z Reads: 33

```
You also need to do calibration first. As per the manual.
```

---
## \#9 Posted by: brandon Posted at: 2016-10-13T13:11:51.871Z Reads: 22

```
I don't suppose any of you happen to have an oscilloscope to take a look at the pulse widths? I did manage to get the led to stay off for about 4 seconds before turning red/blue, I must just have some values or timing wrong in my program, never any beeps though
```

---
