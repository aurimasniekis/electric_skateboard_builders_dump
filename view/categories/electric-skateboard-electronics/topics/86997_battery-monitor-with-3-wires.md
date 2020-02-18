# Battery monitor with 3 wires

### Replies: 5 Views: 185

## \#1 Posted by: reiko Posted at: 2019-03-12T23:36:57.259Z Reads: 88

```
I want to hook up a 3 wired battery monitor to only show voltage while the board is on.

As far as I understand, battery monitors with 3 wires don't plug straight into the battery, but instead use an external power source to measure the battery voltage. This gave me a supersketchy idea.

I am using the dual ESC substitute from eBay without an anti-spark switch. The only switch I have on the board is the switch on the ESC. I found a spot on the ESC which only starts giving off voltage when the ESC is on.

Is it possible to use this spot as a power source to power the battery monitor? The spot gives off around 8-10 volts and considering the voltmeter doesn't pull over a few milliamps, then it should be fine, no? 

Alternatively, since the switch and the included battery monitor on the ESC both light up once the board is turned on, would it be okay to tap power from one of their sources? I think there is even a 5v marker on the ESC...
```

---
## \#2 Posted by: rojitor Posted at: 2019-03-13T12:55:34.720Z Reads: 59

```
Just join red with yellow
```

---
## \#3 Posted by: reiko Posted at: 2019-03-13T14:40:38.161Z Reads: 45

```
I only found battery monitors that take in 2.5-30 volts and can measure up to 100. If I join the yellow and the red wire, I can only measure 30 volts, but my pack is to be 10s
```

---
## \#4 Posted by: xilw3r Posted at: 2019-03-14T08:21:16.727Z Reads: 32

```
Hard to answer since I know nothing about the ESC, but on VESC 6 the PPM input supplies 5V with up to 1A current, I run the arduino receiver off of this and also I tap into this to feed the voltmeter. I assume that your ESC also has PPM input somewhere? Perhaps dig into the specs, see if its mentioned. I would not want to leech power from random spots with weird voltages such as 8 to 10 (??big range for one spot)
```

---
## \#5 Posted by: MysticalDork Posted at: 2019-03-14T08:46:33.603Z Reads: 21

```
You could always add a small dc-dc converter for like $5. Use it to run lights etc as well.
```

---
