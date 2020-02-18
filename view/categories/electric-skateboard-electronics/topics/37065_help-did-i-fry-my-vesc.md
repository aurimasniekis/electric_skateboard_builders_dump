# Help? Did I fry my VESC?

### Replies: 5 Views: 664

## \#1 Posted by: linkedtim Posted at: 2017-11-01T15:23:38.926Z Reads: 86

```
I had previously successfully configured a Kama wireless controller with my VESC.
https://www.amazon.com/gp/product/B0047SFGDW/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1
The VESC I own is:
collections/esc-speed-controller/products/torque-esc-vesc-bldc-electronic-speed-controller
Unfortunately this is past tense because the connection was cutting out, which I attributed to not having soldered the connections. I put about 10 miles on the board before this started happening so went back to solder everything and suddenly I wasn't able to get the joystick or the C/Z button to react top the VESC. The receiver lights up and connects, but I'm not getting any wheels turning when using it. When connecting the VESC via BLDC, I have no issue using the keyboard to turn the wheels. This was happening with the I2C ports so I went back to square 1 with the wiimote I originally had working via: 
https://github.com/the-raspberry-pi-guy/skateboard
but now that setup isn't turning the wheels either using the servo connections. 
Could I have fried something on the board that would stop any signal reception on the bus responsible for VESC->wheel input?
```

---
## \#2 Posted by: Surfer Posted at: 2017-11-01T18:24:38.091Z Reads: 57

```
Did you check if it has errors? In bldc tool, terminal tab, type faults.
```

---
## \#3 Posted by: Yecrtz Posted at: 2017-11-01T18:49:26.028Z Reads: 50

```
As Surfer said, check for errors. If there is a red led blinking there is something wrong aswell.
```

---
## \#4 Posted by: linkedtim Posted at: 2017-11-01T19:51:29.410Z Reads: 50

```
Thanks for responding @Surfer. I had actually never used the terminal page on BLDC. I hooked it up, ran the command and it said "no faults encountered since boot". I turned the wheels via the keyboard and ran the faults command again, still no faults encountered. Connected the Kama nunchuck which connected to the receiver from the VESC, hit the throttle and still no communication from the Kama to the VESC to turn the wheels, re-ran the faults command and still **no faults**.
-Blue light is the VESC
-Solid red light is the Kama receiver. Kama nuncheck has a solid red light meaning it is connected.
 <img src="/uploads/db1493/original/3X/3/b/3b503d1946055e1334f80bc90d2f441c7663749d.jpg" width="375" height="500">
```

---
## \#5 Posted by: linkedtim Posted at: 2017-11-01T19:58:18.540Z Reads: 43

```
Thanks as well @Yecrtz. Only a solid red light on the Kama receiver once paired, otherwise I believe that is expected. I wasn't sure if, where the kama remote and wii remote both stopped working at the same time, there was a common port on the servo pin and I2C pin that I could have toasted accounting for pairing to be successful but wheel control to otherwise be unsuccessful through the vesc?
```

---
