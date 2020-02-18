# Turn lights on and off with GT2B

### Replies: 7 Views: 1437

## \#1 Posted by: Kaden56 Posted at: 2016-11-04T18:43:43.174Z Reads: 139

```
I searched with every key word I could to try to find where people have discussed this before but I only found things referring to the nunchuck remotes and board lighting in general. If all the info I need is already somewhere else then please direct me there. 

I am doing a GT2B mod with a basic 3D printed enclosure but before I print the final one I want to know if it is possible to use the 3rd channel (little red button) on the GT2B remote to do things like turn headlights on and off. If so I will design a space in the remote enclosure to accommodate that little button. After seeing a recent thread of someone making a bldc tool that makes cruise control possible using channel 1 I may also try to keep the second trigger thing in the new remote as well but I haven't decided.
```

---
## \#2 Posted by: BexBle Posted at: 2016-11-04T19:00:19.735Z Reads: 135

```
I believe so here is a link i don't know if it will help but it might.    https://www.youtube.com/watch?v=KlrBF9IyL6o.
its for an RC but the idea may stay the same.


REUBEN
```

---
## \#3 Posted by: Pimousse Posted at: 2016-11-04T20:32:54.819Z Reads: 118

```
I use the 3rd channel to remotely toggle on/off headlights on my board.
For that, I use a sliding switch and a UBEC plugged in the 3rd channel of the receiver and powering my LEDs.
https://hobbyking.com/en_us/dr-mad-thrust-series-3a-bec-with-inbuilt-aux-controlled-on-off-switch-for-accessories.html

That's a very easy way to go !
```

---
## \#4 Posted by: Kaden56 Posted at: 2016-11-04T20:42:55.644Z Reads: 111

```
O cool I'm glad to hear this is easily possible! I'm running 10s would something like this work? http://www.valuehobby.com/hobbywing-5a-ubec-high-voltage.html

Also how exactly is this hooked up to the battery pack and the receiver?
```

---
## \#5 Posted by: Pimousse Posted at: 2016-11-04T20:49:20.962Z Reads: 102

```
I'm also running 10S and use exactly this one :
https://hobbyking.com/en_us/dr-mad-thrust-series-5a-hv-bec-with-inbuilt-aux-controlled-on-off-switch-for-accs.html
But with his model it's better to use a momentary switch on the 3rd channel of the remote because UBEC toggle each time 3rd channel is closed (one push = on, another push = off).

I built a Y connector to supply the VESC and UBEC from the battery (XT30 on UBEC).
I think the most annoying part is to wire LED to the UBEC :smile:
```

---
## \#6 Posted by: jmasta Posted at: 2016-11-04T20:56:31.722Z Reads: 94

```
Not seeing a 12S (50V) -> 12V version.  Anyone know how to do this with BEC that doesn't already have the aux switch?  I've seen it done before, so I know it's possible
```

---
## \#7 Posted by: sk8ace Posted at: 2016-11-04T22:13:31.589Z Reads: 85

```
I am using this: https://www.amazon.com/gp/product/B012W6RJ5I/ to power this headlight: https://www.amazon.com/gp/product/B00NPQUYM0/ 

Worked great on the GT2B 3rd channel button. I run 12s (2 6s lipos) but only had the headlight hooked up to one battery (not sure if it could take 50v lol). 

I am using the Mini remote now: https://electric-skateboard.market/product/2-4ghz-mini-remote-receiver/ and can still use this same setup. I use the turning wheel on the Mini remote to activate the headlight.
Early morning ride to work picture:
https://pbs.twimg.com/media/CuFAcbCXYAArMqy.jpg
```

---
