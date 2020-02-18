# \[SOLVED\]Winning Remote not controlling motor

### Replies: 9 Views: 1045

## \#1 Posted by: Pyrax Posted at: 2016-09-07T15:56:01.992Z Reads: 144

```
Before I had assembled my e-board my Winning remote worked fine and I was able to control the motor using it, however after assembling the board I was no longer able to control the motor using the remote. At this time when I went into the bldc tool there was no activity in the Pulswidth (ms) section of the PPM tab. After reading around the forum I found a thread saying I should buy http://www.hobbyking.com/hobbyking/store/__10625__HobbyKing_GT_2_2_4Ghz_Receiver_3Ch.html from hobbyking. After plugging it in an setting it up I am now able to see the Pulsewidth(ms) section changing however the motor will still not spin. There are no detected faults within the VESC. If anyone knows how to fix the problem any help would be very appreciated. Thanks
Edit: I am also able to spin the motor using the BLDC software when running motor detection.
```

---
## \#2 Posted by: Blasto Posted at: 2016-09-07T16:03:53.944Z Reads: 140

```
make sure your receiver in binded, check your connections. at the very least, if your receiver is working you should see a display of about 1.5ms on the bldc tool. I suspect your connections from the vesc to the receiver is in question here.
```

---
## \#3 Posted by: Pyrax Posted at: 2016-09-07T16:06:57.528Z Reads: 129

```
Im pretty sure the receiver is binded since when I turn the remote on an of the LED responds. There is a Pulswidth of around 1.55ms. Im pretty sure the connections from the receiver to the vesc are correct. Ground on the outside pin, then positive and then signal.
```

---
## \#4 Posted by: Blasto Posted at: 2016-09-07T16:24:33.128Z Reads: 115

```
Ah ok that's good, make sure you are in the right channel
```

---
## \#5 Posted by: Pyrax Posted at: 2016-09-07T16:27:15.833Z Reads: 113

```
Ah ok, I see what I did wrong. Since channel 3 is used for bind I assumed that it was not supposed to be used. After changing the receiver to channel 3 it now works fine. Thanks for the help.
```

---
## \#6 Posted by: DeathCookies Posted at: 2016-09-07T17:45:21.532Z Reads: 103

```
Normaly you use chanel 2 for throttle.
```

---
## \#7 Posted by: mccloed Posted at: 2016-09-07T21:38:46.321Z Reads: 91

```
True. When you switch from the stock receiver with these remotes it only works on channel 3 with the Hobbyking receiver. Weird, Huh?
```

---
## \#8 Posted by: ralphy Posted at: 2017-03-28T17:24:21.371Z Reads: 49

```
So you bind on ch 3 and then plug in the vesc into channel 3?
```

---
## \#9 Posted by: holomouse Posted at: 2017-07-07T21:47:26.816Z Reads: 35

```
Just for the record - the Winning remote also binds successfully with Turnigy 9x rx: https://hobbyking.com/en_us/turnigy-9x-2-4ghz-8ch-receiver-v2.html and the throttle is on ch3.
```

---
