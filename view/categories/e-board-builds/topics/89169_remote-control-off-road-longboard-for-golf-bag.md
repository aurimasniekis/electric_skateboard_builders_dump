# Remote control off road longboard for golf bag

### Replies: 7 Views: 445

## \#1 Posted by: Golfmechanic Posted at: 2019-04-03T00:47:43.560Z Reads: 97

```
New member here. I am wanting to take existing off road electric long board or make one that I can control remotely with Wii nunchuck.( or any cotroller for that matter) To operate it remotely and also have option to ride it.  I was looking into VESC but have no idea if it would be cable of controlling both motors at same time for forward, reverse and to achieve turning have wheels go different speed. I found this video from one of the members. This would be perfect if only it controlled both wheels and could code it for turning. https://youtu.be/PV64I1yTcsM
```

---
## \#2 Posted by: Skunk Posted at: 2019-04-03T00:59:19.951Z Reads: 95

```
I think in order to get a skateboard to turn via the motors you'll need 4wd. And some more advanced speed controls.
```

---
## \#3 Posted by: wafflejock Posted at: 2019-04-03T01:08:55.244Z Reads: 91

```
If you search for "VESC differential steering" that's generally what you're describing in more technical terms and comes back with some results.  You can do what you want with multiple VESCs (need one for each motor to independently control current flow through coils in each motor to drive them at different speeds).

You'd also need to have a custom receiver most likely to take the signal from the controller and send control signals to each VESC that corresponds to the input (typically the VESC just takes a throttle value, the result of that throttle input can be chosen in the VESC tool to be a particular target velocity or target current... current mode is used by most riders for natural feel of more trigger/throttle is more torque/push).

If actually using a skateboard as platform the differential steering probably won't work well since pushing from say the back wheels you'll be dragging the front wheels left and right, ideally you put differential steering in the center of the vehicle and/or use casters for the non-driven wheels so they can rotate to point the direction they're being pushed (plan on doing this for beer bot project at work using similar system for driving a cooler around work, unfortunately budget is held up since we moved offices and other more pressing things, but hopefully will happen soonish).

Anyway back to your project, transmitter would have to transmit both a throttle and direction value over to the receiver and the receiver would need to use those values to determine what throttle to send to each motor/VESC until it gets more input and changes those values.  I've made my own transmitter/receiver and there are at least 3 other custom ones I've seen on here so there's lots of previous work if you look up DIY controller (search in top right is magnifying lense).  If you have any programming experience and/or are willing to learn some then you could do it yourself, transmitter/receiver is based on an arduino connected to an nrf24l01 as well and the receiver simply outputs PPM signal to the VESC (you can now buy boards with both the main MCU chip from the arduino and the nrf and all necessary supporting components built into one like here: https://www.amazon.com/gp/product/B07N2P8FCD/  If you do some searching can find them cheaper.

---

Can find my really basic code for doing the transmitter/receiver here:
https://github.com/shusain/eskatecontroller

Along with plans to make the custom PCB I was using before the boards above existed (or I was aware of them).  My code isn't the greatest but it's probably the simplest so good for beginners.
```

---
## \#4 Posted by: Golfmechanic Posted at: 2019-04-03T01:33:46.103Z Reads: 73

```
Awesome information! Mechanically I know I can put something together that will work. And I think you guys gave me enough information to get the electric controller side done. This is what I currently own.   
https://photos.app.goo.gl/QJsZgb18bV5DBHLZ8
And morph that with
https://photos.app.goo.gl/c7gvPqZNQd7S4avk8
But use off road long board as foundation.
```

---
## \#5 Posted by: wafflejock Posted at: 2019-04-03T03:31:27.688Z Reads: 63

```
Yah looks doable, the main issue will be getting a pulley that you can fasten to the wheel and doesn't collide with anything.  Oh and a motor mount basically getting the whole two pulleys and belt part lined up and mounted to existing hardware can be a challenge (tried an ebike once too but still just a bike for now)

Also if you or anyone decides to try the boards I linked from Amazon the code is here:
https://github.com/keywish/keywish-nano-super-kit

specifically in lesson20 folder there are example emitter/receiver code that work and are simple
```

---
## \#6 Posted by: maxchilton Posted at: 2019-04-03T16:20:06.071Z Reads: 37

```
[quote="Golfmechanic, post:1, topic:89169"]
New member here. I am wanting to take existing off road electric long board or make one that I can control remotely with Wii nunchuck.( or any cotroller for that matter) To operate it remotely and also have option to ride it. I was looking into VESC but have no idea if it would be cable of controlling both motors at same time for forward, reverse and to achieve turning have wheels go different speed. I found this video from one of the members. This would be perfect if only it controlled both wheels and could code it for turning. [https://youtu.be/PV64I1yTcsM ](https://youtu.be/PV64I1yTcsM)
[/quote]

buy this, electrify it, put off road wheels on it, replace stroller/kid with golf bag

![860x0_q70_crop-scale|690x470](upload://5xlCWhcAxrsHGWUx8OL5X7pedYm.jpeg)
```

---
## \#7 Posted by: Golfmechanic Posted at: 2019-12-22T01:51:29.780Z Reads: 15

```
I have a item number 183513521688 from eBay.
(ROAD-Electric Skateboard-Dual 3300W-31mph-19mile Range) Then I bought( HGLTECH 2.4GHZ PPM YK01 REMOTE CONTROL FOR ALL ESC )
I am trying to either program HGLTECH to my
Longboard board with or without the receiver that came with the HGLTECH. Anyone have any idea?
I have no schematic for longboard and I don't see any where I can plug in receiver.
```

---
