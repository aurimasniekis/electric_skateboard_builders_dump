# Drone Connecting Receiver to Flight Controller

### Replies: 6 Views: 4779

## \#1 Posted by: wmj259 Posted at: 2017-09-23T22:54:22.965Z Reads: 46

```
Hello,

I was deciding on building a drone, and went with it. 
I currently am stuck on how to connect the receiver to a Flight Controller. The receiver and transmitter are a 6channel version. I am confused with how to wire them up together. I made a makeshift connector, using the servo wires from the ESC to jump from the FC to the receiver. Other than that, I am confused with how to continue. 
If it helps, this is the flight controller I have:
https://www.pitchrollyaw.net/cl-racing-f4-flight-controller
Looking at the diagrams they have:
<img src="/uploads/db1493/original/3X/8/f/8f3a85ffa1c0b3dbc755555898372506e627d2ce.png" width="187" height="500">
<img src="/uploads/db1493/original/3X/8/f/8f3a85ffa1c0b3dbc755555898372506e627d2ce.png" width="187" height="500">

I got the GND and the 5V connected to the Receiver. Was able to bind to the controller.
<img src="/uploads/db1493/original/3X/8/1/81c4937fb0d6ed318f91527db278853ec9090f9e.jpg" width="281" height="500">
<img src="/uploads/db1493/original/3X/a/0/a02e389079a851b6f2c638527290d6436eb47332.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/0/d/0dd39e589385d1c44aeb6cf62fd6f5b8ba025219.jpg" width="690" height="388">
```

---
## \#2 Posted by: SilentException Posted at: 2017-09-23T23:36:07.072Z Reads: 33

```
With this receiver you can use either PPM or iBUS, Select the one you choose in Betaflight configurator. I would go with iBUS but some of the older receivers default to PPM mode on startup and there is a bit of trickery involved to get them to start with iBUS enabled. Don't know what's the case with this particular one, sorry. Diagram PPM/iBUS.

<img src="/uploads/db1493/original/3X/1/8/189c5826536b2fcc12fbc0e8b0eac0fb7ecd1f64.png" width="666" height="500">
```

---
## \#4 Posted by: wmj259 Posted at: 2017-09-23T23:54:23.777Z Reads: 27

```
Is PPM mode not good?
Also will the whole drone be controlled through one channel? I know that Helis have servos so that's why each servo is on its own channel, but this has me confused.
```

---
## \#5 Posted by: SilentException Posted at: 2017-09-24T00:01:32.325Z Reads: 27

```
PPM is fine but it tends to be bit more unstable than iBUS. You can see that as oscillating channel values in Betaflight for example. PPM is Pulse Position Modulation which means you do have all the channels on the same PIN but signals are offset from one another. iBUS is a serial based signal and protocol which by itself means it is more stable and less susceptible to noise/interference.
```

---
## \#6 Posted by: wmj259 Posted at: 2017-09-24T00:03:50.993Z Reads: 24

```
So in the picture you made, the only wires i would need connected for iBus would need to be the top three horizontal servo? Is the 5V and voltage also tied into those pins? VCC i suppose is the votlage.
```

---
## \#7 Posted by: SilentException Posted at: 2017-09-24T00:07:21.415Z Reads: 23

```
For both PPM and iBUS you need three wires. GND, VCC and signal. 

You choose which connection you want to make to your FC. Top right three horizontal servo are GND, VCC, signal, yes. PPM is bottom left, vertical GND, VCC, signal.

In reality, it doesn't really matter where you connect GND and VCC, all GND and VCC pins are internally connected in the receiver but easy to check with multimeter.
```

---
