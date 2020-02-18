# \[HELP\] ESC controlled via arduino

### Replies: 5 Views: 160

## \#1 Posted by: itsmark Posted at: 2019-04-02T21:30:30.853Z Reads: 46

```
This is for a mechatronics project. I want to control an electric skateboard ESC with a ppm output signal from an arduino. As this is the first electric skateboard I will be building, I just ordered on of the first things I found with a quick google search. I got [this](http://www.diyeboard.com/dual-hub-motor-9052mm-1000w75kv-power-truck-front-truck-kit-p-558.html) dual hub motor truck. For the ESC, I went with [this](http://www.diyeboard.com/upgraded-v21-dual-hub-motor-sine-wave-foc-esc-speed-controller-p-610.html) due to the wiring diagrams showing it was compatible with my motor setup. 
I only noticed after I ordered it that the ESC has a built in receiver for the included remote so I don't know how I would interface the arduino to the ESC.
Can I control this ESC with an arduino? Is there a better ESC for the job? I am definitely a beginner when it comes to building things like this so any help is appreciated.
```

---
## \#2 Posted by: Mich21050 Posted at: 2019-04-02T21:47:17.093Z Reads: 43

```
Ok, so first off all diyeboard is a shitty seller. Big mistake buying from him. \
Regarding your second question. You won't be able to controll your esc with anything other that the "standard" remote. \
The best esc for your setup would be a vesc. You can interface with it using uart or a pwm signal. :slight_smile:
```

---
## \#3 Posted by: linsus Posted at: 2019-04-02T22:03:56.887Z Reads: 35

```
Pro tip, do re-search before going into a spending spree. Atleast when I went to school I had to motivate my choices of hardware :grimacing: "first thing I found" could be pretty much..useless
```

---
## \#4 Posted by: itsmark Posted at: 2019-04-02T23:09:55.312Z Reads: 26

```
Thanks for the help guys. So VESC is the way to go. Is there a good value you would recommend? What about the Torque ESC?
```

---
## \#5 Posted by: KaramQ Posted at: 2019-04-03T00:55:42.676Z Reads: 23

```
The focbox unity, flipsky dual 4.20, Ollin vesc
```

---
