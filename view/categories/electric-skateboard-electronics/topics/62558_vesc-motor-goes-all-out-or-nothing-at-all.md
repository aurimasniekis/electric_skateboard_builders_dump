# Vesc Motor goes all out or nothing at all

### Replies: 2 Views: 138

## \#1 Posted by: MaxMaker Posted at: 2018-07-22T20:14:30.378Z Reads: 47

```
I could really use some help with my VESC. Why can’t this be plug and play?😒 

My motor either spins all the way or not at all. With keyboard control it only makes noises. Yesterday it worked better, but sometimes it spun clockwise and sometimes counterclockwise. Today I re-did the entire setup with FW 3.9 and now It behaves like in the video.

* 12S
* Alienware 100kv Motor
* PPM from Arduino, Arduino to Arduino comunication with NRF24  (Mapping is very responsive)
* 8AWG cables throughout. 30cm battery cable. 

https://youtu.be/z1iPQ_k1jL0
```

---
## \#2 Posted by: AutoItKing Posted at: 2018-07-22T22:02:59.526Z Reads: 29

```
Current control will do that as the motor needs very little current to spin up to full speed with no load. Normal operation.
Spinning the wrong way is an issue though. I always kick to start so it knows which way to go.
```

---
