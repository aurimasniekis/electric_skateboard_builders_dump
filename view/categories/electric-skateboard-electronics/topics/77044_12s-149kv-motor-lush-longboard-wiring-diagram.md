# 12s, 149kv motor Lush Longboard Wiring diagram

### Replies: 2 Views: 226

## \#1 Posted by: 532Hz Posted at: 2018-12-04T19:21:25.987Z Reads: 56

```
Hey folks,

I've decided to embark upon designing my own e-board and have done a fair bit of reading  on this forum as well as other sites.

Where i live in the UK is notorious for hills so it was very important for me to have as much torque as possible. I've skated on a cruiser style longboard for as long as i can remember so i wanted to stick with that style of board as well.

The specs are as follows:

2 x 6s batteries run in series as 12s
TB VESC v4.12 (Firmware v.3.40)
Turnigy SK3 149kv
TB Nano Remote
Lush Longboards 'The Machine'
TB 218mm Wide trucks
15T & 18T Motor Pulley
36T Kegel Pulley 15mm Wide
TB Motor Mount (also purchased HobbyKing Turnigy Motor mount)
80mm Orangutang Kegel
1/2" Risers
280mm Belt drive

This is how she is looking whilst i wait for the 10awg, XT90 connectors and 5.5mm female bullets to replace the 4mm connectors currently on the motor.

![41FE68CE-CEB7-42D5-98B5-521092BB9B6C|196x500](upload://mvcvYn0ojxLvG6m01sslKqDOyBp.jpeg) 

![62166572-0E5D-40A3-834D-162B2DDF4CDE|375x500](upload://hntTrtwoZ6R7e5gu4ozt5hqEhL2.jpeg) 

I never excelled in the electronics class at school (which by the way, was a long time ago) and am feeling a little apprehensive about the whole electronics side of the project.

The diagram below shows how i think that it should be configured...

_![The%20Machine%20E-Board%20Wiring|690x487](upload://qQtgYhPqDTw3kjZws1N4NQHkUe0.jpeg)_ 

I've not decided on whether to use a fuse in the circuit or not as have been unable to find fuses that seem appropriate. The Maxi-blades that goto 70amps seem alright although i can only find ones rated at 36V, which are not suitable for a 50v setup.

https://eskating.eu/product/anti-spark-power-switch/

This fuse with switch from skating.eu also will provide the right amount of amp protection but doesn't mention voltage ratings and says that anything above 40amp fuse is non-removable. Does that mean its a £30 disposable fuse holder?

Also i read that there are many of you out there riding with no fuse at all...


Does the circuit in the diagram look functional?

Would it hurt to incorporate the anti spark key loop within the Series adaptor (to minimise wiring and XT90 connectors)?

Should i or should i not use a fuse as well as anti-spark?

Any advice or criticism welcome ;)

Much Love!
```

---
## \#2 Posted by: Andy87 Posted at: 2018-12-04T20:04:05.189Z Reads: 28

```
The diagram looks good so far.
If you use a fuse, look for 58v fuse on amazon.
Like this 
https://www.amazon.com/Automotive-Fuses-BF1-150A-piece/dp/B00HKIC864/ref=mp_s_a_1_5?ie=UTF8&qid=1543953683&sr=8-5&pi=AC_SX236_SY340_QL65&keywords=58v+fuse&dpPl=1&dpID=31IUwfgTtbL&ref=plSrch
There also cheaper versions. Just didn’t found on the go...
If you use a xt90s antispark loop key, you don’t need any other switch in your circuit.
```

---
