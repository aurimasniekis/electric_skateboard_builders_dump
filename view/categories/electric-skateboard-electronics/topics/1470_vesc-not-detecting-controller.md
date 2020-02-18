# VESC not detecting controller

### Replies: 13 Views: 1344

## \#1 Posted by: evoheyax Posted at: 2016-02-20T04:10:47.276Z Reads: 87

```
Hey, I'm having an issue setting up the controller. I was able to get the motor detection working after messing with the settings long enough. However, I can't seem to get the controller working.

First of all, when I plug the receiver in, the red light on the receiver does NOT turn on. I flipped the cable around as it might have been the wrong way, but still, nothing.

I set the mode to ppm. Clicked save and then reboot. Then connect again.
Then under ppm, set the mode to current mode. I saved again and click the box next to display so I can see the throttle range.

But I get nothing. I followed the same steps vedder shows, and I'm using exactly the same controller he's using in his config video.

Checking the Realtime Data tab, and clicking activate sampling, I get the crazy graphs bouncing all over the place (which from my understanding, is what I should get). 

It also says fault codes: NONE. So it seems like everything hardware wise is working.

Just as an FYI, I also used this controller on my last board and after having issues with the vesc, tried it on my old setup and it does indeed work. So it seems to me like I'm doing something wrong with the setup.

Any help is much appreciated :)
```

---
## \#2 Posted by: treenutter Posted at: 2016-02-20T06:13:58.081Z Reads: 77

```
@evoheyax this might seem obvious, but are you certain you're using the right channel on the receiver?
```

---
## \#3 Posted by: evoheyax Posted at: 2016-02-20T06:22:54.056Z Reads: 73

```
I tried all possible combinations, and nothing. Using a brand new servo cable that looks good.
```

---
## \#4 Posted by: trbt555 Posted at: 2016-02-20T08:40:43.282Z Reads: 71

```
Have you measured the voltage between the GND and +5V pin on the ppm input of the VESC ?
```

---
## \#5 Posted by: Dedbny Posted at: 2016-02-20T08:56:05.583Z Reads: 69

```
Are you sure have match lined the right channel on the reciever as per the transmitters instructions.  Sometimes you have to turn the vesc first rather than the transmitter to get the channel set on the receiver.
On mine I know because the light goes steady from flashing when transmitter is on.
```

---
## \#6 Posted by: Sebastiaan Posted at: 2016-02-20T11:27:46.366Z Reads: 69

```
I put my bets on no voltage coming out of the ppm. Same as trbt555 says, measure the voltage on the wire going to the receiver. It should be 5v.
```

---
## \#7 Posted by: evoheyax Posted at: 2016-02-20T16:38:17.155Z Reads: 63

```
I just measured 2.9 volts, not 5 volts. But what does that even mean?

Could this be cause by me not giving enough volts to the vesc? I am giving it only 8.8 volts, seeing as both vedder and onloop warned to use as little power as possible to power the vesc during configuration.
```

---
## \#8 Posted by: evoheyax Posted at: 2016-02-20T16:50:54.652Z Reads: 60

```
I first tried using the same channel I used on this receiver on my old build, then tried all other channels, powering it on with it connected like you said. And no luck. I believe this 2.9v instead of 5v thing has something to do with it.

I just hope its a setting and not that the vesc is broken. Just yesterday was the first time I booted it up. Did a successful firmware update (I was extremely careful), now on firmware 2.15, vesc version 4.10. And after fiddling, got the motor detection to work.
```

---
## \#9 Posted by: Sebastiaan Posted at: 2016-02-20T16:52:58.095Z Reads: 59

```
It's probably because you are not supplying enough voltage, but wait for other users with experience to clear this up.
```

---
## \#10 Posted by: evoheyax Posted at: 2016-02-20T18:20:30.422Z Reads: 57

```
It's not the problem. I just soldered the connectors for my other vesc, and I get 5 volts. It also powers up the reciever. it blinks red, and when I turn my transmitter on, it stays a solid red, indicating a good connection. So now the question is, what is wrong with the first vesc I tried, which is giving 2.9v instead of 5v?
```

---
## \#11 Posted by: trbt555 Posted at: 2016-02-20T19:19:19.439Z Reads: 58

```
Check the voltage between pins 3 and 1 on P3, that's the 7-pin header along the side of the VESC.
Pin 1 is the pin furthest away from the mosfets.
You should read 5V. If not, you likely have a hardware problem.
```

---
## \#12 Posted by: evoheyax Posted at: 2016-02-20T19:27:09.073Z Reads: 57

```
I get the same 2.9v instead of 5v. Since it seems like a hardware issue, do you think this vesc would still work as a slave with my other vesc which seems to be 100% working as the master? Or is the problem fatal?

Thank you for helping :)
```

---
## \#13 Posted by: trbt555 Posted at: 2016-02-20T20:49:43.244Z Reads: 52

```
Try it. I think it might work.
I don't think you can do any harm either.
```

---
