# Is it possible to make different speed modes with VESC?

### Replies: 11 Views: 2350

## \#1 Posted by: nikoli280 Posted at: 2017-06-19T18:18:19.595Z Reads: 265

```
Hi. I was wondering if it is possible to make different speed modes with a VESC?

Just like the ones boosted board has. Like Sport mode and so on. So i can controll how fast it accelerates and so on.
```

---
## \#2 Posted by: Jinra Posted at: 2017-06-19T18:21:13.436Z Reads: 273

```
This is much easier done through the remote you get. If you get the Benchwheel or Nano v2 remotes they have "speed" selector options. If you're using a VESC, you're most likely using "current" control which doesn't really control speed so much as acceleration. These two remotes will let you adjust how much acceleration you get with the throttle.

The benchwheel has a 50% throttle mode and the Nano v2 has a 70% throttle mode.
```

---
## \#3 Posted by: mmaner Posted at: 2017-06-19T18:29:28.814Z Reads: 263

```
Look at the @Ackmaniac firmware, you can make modes with it.  I have multiple modes setup for most of my boards.  I have a "SLOW" mode for all of them that I use when I let someone who has never skated before use a board.  I usually set the MAX Motor to 20 and the BAT Min to -10 for slow acceleration and soft breaks.

http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
```

---
## \#4 Posted by: nikoli280 Posted at: 2017-06-19T18:35:07.045Z Reads: 235

```
How do you switch between modes. I have a GT2B modifies controller as remote.
```

---
## \#5 Posted by: mmaner Posted at: 2017-06-19T18:40:39.390Z Reads: 230

```
You use his android app to connect to a BT receiver installed on the master VESC and create/select modes.
```

---
## \#6 Posted by: Stef Posted at: 2017-06-19T20:21:35.537Z Reads: 203

```
I use the benchwheel remote and I highly recommend it. I have dual 6355 on 10S which is way too much for commuting on flat roads, so I usually set the remote to 50%. However, when Im out riding for fun or take on some hills I set it to 100%.
Im suprised to see so few benchwheel remotes, for me the reliability, ergonomics, size, weight, rechargeable battery and speed modes have all been perfect.
```

---
## \#7 Posted by: Jinra Posted at: 2017-06-19T20:31:32.533Z Reads: 198

```
I absolutely love the remote myself, it's pretty much perfect. The only weird thing is that on my dual 6355 carbon board, the receiver disconnects for no reason at times (seems to be during high motor current). No idea what causes this, but I have to restart the receiver/board in order to reconnect as restarting the remote does nothing. I tried it with two different receiver/remote combos and they both fail. It's interesting since it never happens on my wood deck board with dual 5065's.
```

---
## \#8 Posted by: yaca Posted at: 2017-06-19T21:02:14.175Z Reads: 185

```
The slow mode of the benchwheel remote isn't 50%. At least mine is just 40%. The green bar at BLDC Tool goes from 50% neutral to 70% full throttle and for brake it  goes down to 10% instead of 0% in that mode. For me 40% is too weak (maybe because of watt-mode) so I prefer to use ackmaniacs app, it's fantastic and so easy to change speed and acceleration via android.
```

---
## \#9 Posted by: EdTech Posted at: 2018-10-11T19:05:44.834Z Reads: 109

```
So based on the settings set the controller automatically makes the other switches lower the speed based on the throttle mode it comes with? I'm new to this so sorry if my questions dumb.
```

---
## \#10 Posted by: SecrIT Posted at: 2018-12-14T10:53:26.444Z Reads: 94

```
@Stef

with your benchweel remote how did you calibrate it?

Did you calibrate it in HI mode? and then automatically LO mode is 50% ? 

If i calibrate mine in LO mode then when i switch to HI the motor just dies, i think because it goes beyond 100%.

If i calibrate mine in HI mode then LO mode is horribly slow.

Is there a true solution?

thx
```

---
## \#11 Posted by: Stef Posted at: 2019-02-08T13:04:47.979Z Reads: 64

```
@SecrIT  Sorry for late reply, first time im on here in a while.

I calibrated in Hi mode, Lo mode is then automatically roughly 50%, not sure about the exact percentage.

When you calibrated in low mode and then set to hi mode then its normal for the VESC to reboot as the signal will go far beyond the limits that you set, probably triggering a safety.

On my dual 6355 hi mode is rediculously powerful to the point that its scary and I rarely ride in hi mode. On low mode it is much much slower but still plenty for day to day riding. I can imagine that if Hi is just a little bit too much then Lo can be a little bit too low. Would have been better to have 3 modes, lo med and high, but for me it works fine.

If Hi is too much power and LO too little, you could choose to lower your max motor amps so that HI becomes  more manageable.
```

---
