# VESC and nyko kama, what is going on?!

### Replies: 34 Views: 3249

## \#1 Posted by: massy Posted at: 2016-04-16T13:20:18.417Z Reads: 187

```
Hello!

So I went out to try my board outside for the first time today and it has already tried to kill me at least three times. 

I have the Nyko Kama connected to the vesc. Soldered -> JST. It works flawlessly inside my home and did periodically outside as well. However it cuts out insanely often and it's sometimes even hard to get the signal back, this has NEVER happened in my apartment (currently 3 meters from board and it's constantly connected and everything works). 

I have noticed my VESC blinking red 3 times on boot and once when disconnected. I cannot get any fault codes out of BLDC by typing faults. "No faults registered since startup". 

I redid the soldering on the reciever and it seemed to work for a bit, but then the board tried to kill me and it was back to being as horrible as before. 

Suggestions? Do I live in signal mekka or what the hell is going on?

Edit: Also tried to wiggle the shit out of all cables to see if theres a loose connection on either nyko or power source, cannot get the remote to disconnect and cannot get the VESC to reboot by doing so... :(

NEVERMIND THIS (woks fine when I disconnected the Nyko Kama): Noticed it just makes a click noise when trying to control through BLDC with keyboard which seems like DRV fail but works fine with remote and so does motor detection.
```

---
## \#2 Posted by: trbt555 Posted at: 2016-04-16T14:19:28.246Z Reads: 175

```
Doesn't sound like a nunchuck problem, could be vesc is cutting out due to other reasons.
Please post screenshots of your bldc tool screens.
What voltage are you running ?
```

---
## \#3 Posted by: massy Posted at: 2016-04-16T14:25:22.685Z Reads: 173

```
Yeah I'm really confused about this since it seems to work so well indoors. Initial thought was definitely bad connection somewhere but having trouble finding one. Running 10S. Still having vibrations as main suspect though as the only time it worked really well outdoors was on some kind of flat stones. However sometimes it didn't want to connect at all so...

It might be the VESC rebooting but I have also experienced it running away from me so that must have been a remote cut out, not VESC.

Edit: Can legitemately control the board on the floor while being 4 meters + and through a wall while indoors, outdoors is a disaster if it even decides to work at all.. 

<img src="/uploads/db1493/original/2X/1/14f00ecc5561babffc92cf38d74b12668c7941c0.png" width="690" height="431">
<img src="/uploads/db1493/original/2X/d/d6515811d7db1d3a04a745e7f22d7e8cd5555328.png" width="690" height="431">
<img src="/uploads/db1493/original/2X/8/8cbb91eb29dcf805750f4090cbd295228673eafa.png" width="690" height="431">
```

---
## \#4 Posted by: trbt555 Posted at: 2016-04-16T15:53:36.507Z Reads: 142

```
How do you tell that it doesn't want to connect ?
```

---
## \#5 Posted by: massy Posted at: 2016-04-16T15:55:10.047Z Reads: 143

```
The LED on the remote just keeps blinking, then suddenly after a delay of half a second to 10 it connects again. This could be either because VESC turned off or the remote has horrible signal I guess. 

 At one point I got mad, left the street because as soon as I stood on the board it would disconnect (not even accelerating with it). While carrying the darn thing home 150 meters it was connected the whole way, don't even know where to start looking for faults.

Also, it shouldn't blink red 3 times on boot right? If not it's strange I can not get a fault code out of it.
```

---
## \#6 Posted by: trbt555 Posted at: 2016-04-16T16:19:23.017Z Reads: 143

```
That does't sound right.
In my experience the nunchuck will not reconnect by itself, you need to push the s button to make it connect.
At least mine works that way.
3 red blinks on boot is normal.
```

---
## \#7 Posted by: massy Posted at: 2016-04-16T16:22:42.504Z Reads: 142

```
Oh nice (that sounds almost too happy :stuck_out_tongue: ), couldn't remember the three lights from before so got worried the VESC was screwed up. Maybe it's just the Nyko Kama remote or reciever that is screwing my life up, really hope it's nothing worse.

I think my remote starts the "blinking process" automatically when disconnected, it just starts looking again (I THINK), can double check when it has stopped raining.
```

---
## \#8 Posted by: massy Posted at: 2016-04-16T18:50:46.107Z Reads: 133

```
You are correct, it does not reconnect without pressing the button. However it seems to have bad signal or something. Using cruise control can be a bit choppy for example (probably dropping and gaining signal before dropout or something, just as if there was a drop and reconnection). Or just giving a little quick throttle and releasing -> board just keeps that speed until timeout.

If the problem even has with the remote to do. Don't know how to progress really and now the weather is crap so..
```

---
## \#9 Posted by: lox897 Posted at: 2016-04-16T22:01:18.268Z Reads: 124

```
If you post a picture of your soldering @lowguido should be able to see if it's a good connection. He barely ever gets drop outs and he soldered. Most likely could be something else though.
```

---
## \#10 Posted by: massy Posted at: 2016-04-16T22:10:28.741Z Reads: 123

```
Yeah pretty sure the soldering is fine. Went out again to try, worked sporadically, maximum 20 seconds each time before a minor drop. I will post a video in 10 minutes showing the behaivior (which after my latest test round also appears when at home). Only change was new batteries in the Kama (measured to be better than old).

Should not be the VESC cutting out, brakes are applied until the board comes to a stop.
```

---
## \#11 Posted by: lowGuido Posted at: 2016-04-16T22:14:22.909Z Reads: 119

```
sounds more like a VESC issue than a Kama issue to me, but yeah show me what you got anyway.
```

---
## \#12 Posted by: massy Posted at: 2016-04-16T22:25:29.798Z Reads: 121

```
I have no clue to be honest. Here's the video anyhow. This did not happen on benchtests earlier, it started happening after I went out for a test ride/swapped Nyko Kama batteries for BETTER ones. 

As you can see the remote connection LED blinks whenever the *bleep* it wants :'(

Originally the problem only happened when outdoors, no matter if I'm on it or not. Earlier when at home I could control it all across my small apartment through the walls, outside it said "nono, you are 50 cm away, I won't work".

Edit: Just now the board is stuck on a constant blue led and the remote won't connect at all because the reciever doesn't realize the remote is not connected....

https://www.youtube.com/watch?v=2Nmg9nPxI2k

@lowGuido Not very visible due to hot glue but as mentioned, even resoldered today because of the problems. They stayed the same. 

<img src="/uploads/db1493/original/2X/3/39e676f0e2b395e7c7fabcc9f6ca3cb68aae3d87.JPG" width="690" height="388">
```

---
## \#13 Posted by: lox897 Posted at: 2016-04-16T22:33:01.190Z Reads: 113

```
Can't see the video. It's on private.
```

---
## \#14 Posted by: massy Posted at: 2016-04-16T22:34:29.476Z Reads: 110

```
Oops, forgot to press publish, fixed. Also, note the blink and the cutoffs when using the cruise control button.
```

---
## \#15 Posted by: lox897 Posted at: 2016-04-16T22:51:09.492Z Reads: 111

```
Please categorise this topic. It fits in eboard electronics.
```

---
## \#16 Posted by: massy Posted at: 2016-04-17T00:29:18.207Z Reads: 113

```
I think I have noticed that the closer I go the motor cables with the reciever, the more drop outs. Holding the reciever above motor cables and giving some throttle causes it to cut out instantly and continously. Most other people doesn't seem to have longer cables and better placement though?
```

---
## \#17 Posted by: lowGuido Posted at: 2016-04-17T00:35:55.401Z Reads: 112

```
this thread needs more pictures.
Y'all know I can't reed!
```

---
## \#18 Posted by: massy Posted at: 2016-04-17T00:37:50.028Z Reads: 112

```
Yeah, gonna have to go sleep now and hope it works better with the reciever away from the motor cables. Will take pictures tomorrow with and actual camera and not my cell phone.
```

---
## \#19 Posted by: trbt555 Posted at: 2016-04-17T06:01:44.066Z Reads: 111

```
That IS weird.
Put a multimeter across VCC and GND while doing this exact test and verify the vesc 5v supply isn't doing weird stuff before you start doubting the soldering.
```

---
## \#20 Posted by: massy Posted at: 2016-04-17T12:39:57.925Z Reads: 115

```
So while the motor wires seemed to cause interference it didn't help in actual riding conditions. Will try measuring the voltage later. I suspect you mean 3.3 V @trbt555, right?  

@lowguido and then there were pictures.

Problem can be reproduced by tapping the circled antenna area with my finger. Starting to think the antenna has bad connection.
<img src="/uploads/db1493/original/2X/c/c02dffcd60caedf20d633b511470cfa968fddad0.jpg" width="690" height="460">

Small flexing gap, should it be there? I'm really starting to suspect the receiver is screwed for some reason.
<img src="/uploads/db1493/original/2X/6/6f4cde9909b114ae5577bb4e5d092dce431c1896.jpg" width="690" height="460">

The ceramic component is very slightly burnt from a soldering iron, in my mind that shouldn't be the problem but might get one quickly later and swap it out just to be safe. 
<img src="/uploads/db1493/original/2X/2/29b4d0f93c125b139d97d7ba54473b329f8cd86f.jpg" width="690" height="460">

<img src="/uploads/db1493/original/2X/b/be0c41126ffaee4d2229c5f05fb35bfae682a792.jpg" width="690" height="460">
```

---
## \#21 Posted by: lowGuido Posted at: 2016-04-17T12:46:24.005Z Reads: 105

```
that reciever is actually 2 boards joined together only by the solder joints on the edge. perhaps one of the joins is loose. I hot glue the boards together now after I accidentally tore them apart once
```

---
## \#22 Posted by: massy Posted at: 2016-04-17T12:47:42.199Z Reads: 103

```
Funny you say that, I just put some superglue in the gap so that's gone. Cannot see any problems with the soldering between the boards but might try heat it up and let the solder flow a bit and see if that helps.
```

---
## \#23 Posted by: trbt555 Posted at: 2016-04-17T13:03:18.459Z Reads: 103

```
Yeah, I meant 3.3V but if you can reproduce the problem by tapping the antenna, you don't need to look any further.
Probably a bad connection between both pcb's. 
You'll never be able to trust it,  I'd chuck it and get a new one.
```

---
## \#24 Posted by: massy Posted at: 2016-04-17T13:09:50.156Z Reads: 102

```
Yeah, I'm really starting to narrow it down to that too.

Don't even know where to get a new one anymore though, most sellers won't ship to Sweden and would rather not wait a million weeks :'(
```

---
## \#25 Posted by: lowGuido Posted at: 2016-04-17T13:16:23.284Z Reads: 105

```
dont be like that.. a bit of solder and shes good as new.
```

---
## \#26 Posted by: massy Posted at: 2016-04-17T13:17:35.301Z Reads: 106

```
Maybe, just tried with no good result, might take a trip and lend some tools a bit later (my soldering iron SUCKS).
```

---
## \#27 Posted by: massy Posted at: 2016-04-21T10:09:53.770Z Reads: 100

```
@trbt555, @lowGuido  So I just got a new reciever and nunchuck, seems to show at least some of the same symptoms even with the new one. Have not had time to go outside to test it though but not feeling too positive, guess there might be something wrong with the VESC? :'(
```

---
## \#28 Posted by: lowGuido Posted at: 2016-04-21T10:17:32.431Z Reads: 100

```
What firmware you using on VESC ? Have you tried flashing it with a different version?
```

---
## \#29 Posted by: massy Posted at: 2016-04-21T10:21:36.777Z Reads: 105

```
2.16 on hardware 4.10. Flashed the default firmware as the BLDC tool prompted that it needed to be updated to work with my version of bldc tool.

edit: no, not tried any other

edit2: I've used the same JST connector both times though but it doesn't drop out more when jiggling it around so doubt that's it but the only thing I can think of. Gonna have to go outside later and test some.

@trbt555 measured the 3.3 pin and it gives a stable 3.343 volts.
```

---
## \#30 Posted by: massy Posted at: 2016-04-22T07:26:31.360Z Reads: 110

```
Worked much better last night, could actually ride without problems. Might have narrowed it down to a bad JST connector (although haven't tried the old receiver with new JST). Had some surprises with cruise control and braking though so might have to change some settings in BLDC because I guess I might hit some limit when braking (or cruising downhill).
```

---
## \#31 Posted by: lowGuido Posted at: 2016-04-22T10:11:52.618Z Reads: 102

```
I have found the cruise control on fw 2.16 surges too much. I have rolled back to fw 1.14 for smooth cruise. 
I think that the lose jst might be the issue with your droppouts .
```

---
## \#32 Posted by: massy Posted at: 2016-04-23T12:53:35.168Z Reads: 101

```
Yeah I saw you wrote that in another thread. Have been skipping cruise control in the meanwhile, might try other firmware later on. 

However it seems my VESC reboots when braking(mainly downhill) or accelerating up a hill. I guess I might hit some limit? Judging from the settings in my second post in this thread, is something looking wrong or should I try change some values? Not really sure what to try. 

Voltage cut off? Battery was at 39 V when i finished riding so not all that close to 33 V but maybe that is it anyway?
```

---
## \#33 Posted by: lowGuido Posted at: 2016-05-07T04:08:58.347Z Reads: 64

```
4 posts were merged into an existing topic: [VESC + Nyko Nunchuck, unstable cruise !?](/t/vesc-nyko-nunchuck-unstable-cruise/1809)
```

---
## \#34 Posted by: Eboosted Posted at: 2016-12-22T23:26:52.353Z Reads: 41

```
Did you ever fix these problems? what was the culprit?
```

---
