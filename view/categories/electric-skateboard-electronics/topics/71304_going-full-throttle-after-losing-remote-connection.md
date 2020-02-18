# Going full throttle after losing remote connection

### Replies: 12 Views: 947

## \#1 Posted by: janpom Posted at: 2018-10-15T14:25:50.438Z Reads: 183

```
A very strange and scary incident happened to me yesterday. After switching off my remote, the board suddenly got going at full speed. Fortunately, nothing bad happened. It flipped over after going some 5 meters. I then switched the remote on again and the board immediately stopped.

I often switch off my remote before switching off the board. I must have done it like 100 times before and nothing bad has ever happened... until yesterday. I'm pretty scared to ride the board again until I investigate and ideally fix the problem. I don't like the idea that the same thing might happen while I'm riding. The board is an eMTB with 4.5 kW of power and it can easily go 50 kph.

Any ideas what might have happened? I haven't been able to reproduce the problem since the incident. I have two ESCapes and [this remote](https://hobbyking.com/en_us/hobbykingr-tmhk-gt2b-3ch-2-4ghz-transmitter-and-receiver-w-rechargable-li-ion-battery-1.html) from HobbyKing. It looks as though the receiver went crazy after losing the connection with the transmitter and instead of signalling neutral as it normally does in failsafe it signalled full throttle instead. Could that be right?
```

---
## \#2 Posted by: mmaner Posted at: 2018-10-15T14:28:37.948Z Reads: 174

```
https://www.electric-skateboard.builders/t/when-i-turn-off-my-remote-my-motor-goes-full-throttle-anyone-know-what-the-cause-it/40984/4?u=mmaner

https://www.electric-skateboard.builders/t/solved-board-accelerates-when-signal-is-lost/7588/5?u=mmaner

https://www.electric-skateboard.builders/t/different-fail-safe-strategies-for-remote-and-vesc/24083

https://www.electric-skateboard.builders/t/problems-that-have-occurred-and-how-to-prevent-them/1937/22

https://www.electric-skateboard.builders/t/help-motor-is-running-without-remote-being-on/29172/4

https://www.electric-skateboard.builders/t/solved-board-accelerates-when-signal-is-lost/7588/5
```

---
## \#3 Posted by: janpom Posted at: 2018-10-15T14:51:08.612Z Reads: 136

```
Thanks for the links. I have read through the threads, but unfortunately haven't found much help there. I do have the failsafe configured correctly and it has never failed me until yesterday. The failure only happened once and I haven't been able to reproduce it since then. That's the worst kind of problem to investigate. I was hoping that someone might have encountered the same thing.

[Here's](https://www.electric-skateboard.builders/t/help-motor-is-running-without-remote-being-on/29172/5?u=janpom) a mention of a bug in the GT2B remote. It's different from what I have encountered though.

I'm going to set a 30 kph speed limit in the ESCs as a precautionary measure. I rarely go faster than that anyway.
```

---
## \#4 Posted by: mmaner Posted at: 2018-10-15T14:59:46.177Z Reads: 129

```
sounds like interference.  You might relocate the RX to the center of the board, toe side so you have a more direct line of transmittal..
```

---
## \#5 Posted by: mtuan293 Posted at: 2018-10-15T22:16:41.564Z Reads: 103

```
I have a [mini remote](https://ebay.com/sch/sis.html?_nkw=2.4GHz+Remote+Transimitter+Receiver+Binding+Plug+for+Electric+Skateboard+OS917&_id=173406680080&&_trksid=p2057872.m2749.l2658) and noticed that when I turn the remote off, the receiver will automatically reset the pulse length to 1.600ms. So once I was playing with the knob and adjusted it down to 1.400ms or something and calibrated the min/max throttle around this value, so as soon as I turned the remote off, the value became 1.600ms which was around 20% throttle. 

So I think you should check in the VESC tool to make sure the pulse length value is the same whether the remote is on or off, in other words, **adjust so that the center value (0% throttle) must stay the same**.
```

---
## \#6 Posted by: janpom Posted at: 2018-10-16T06:12:21.218Z Reads: 86

```
Thanks for your input. I have read about this kind of problem elsewhere. I'm afraid it's not what's happening in my case though. It only happened to me once that the board started after switching off the remote. Other times it's all just fine.
```

---
## \#7 Posted by: janpom Posted at: 2018-10-22T19:58:41.463Z Reads: 70

```
It happened today again and this time I was able to consistently reproduce the problem several times. Here's how it behaved. After loosing the connection with the transmitter the receiver waited for 30s and then it started signalling ~90% of full throttle. It's back to neutral once it regains the connection. I tried it four times and it was the same each time.

However, once I turned the power off and on again, I was no longer able to reproduce the problem. So it looks like the receiver only gets into this weird state sometimes, possibly after being used for a while.

It sounds a bit like what @danielz describes [here](https://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888/496?u=janpom), except it can't be consistently reproduced and I believe my failsafe actually is pretty close to 1500ms. Still, the match in the 30s delay is suspicious.

At any rate, I'm getting a different remote.

Here's a recording of the weird behavior:
https://www.youtube.com/watch?v=-TsKB68wZvY
```

---
## \#8 Posted by: Sebike Posted at: 2018-10-22T20:09:48.163Z Reads: 64

```
yes.. I've been through this same exact behaviour as well.. 

It's the failsafe that acts weird. This happened after I tried to set the vesc to gradually slow down whenever connection was lost (ackmaniac implemented this feature as I recall it). 

Never got it to work properly due to this crazy behaviour, so I had to reset failsafe to its original neutral setting.

Edit- I had to play around with the calibration knobs a bit when re-setting the failsafe before it went back to normal.
```

---
## \#9 Posted by: itsmikeholland Posted at: 2018-10-22T20:24:11.511Z Reads: 61

```
This happened to me while I was vacationing with my board in Barcelona 😆 for me, it was because a connection was lose between my receiver and vesc. Originally the board would unpredictably go FLYING out from underneath me, I was able to change the settings so that it instead would brake, but Im not sure which setting. This same thing happened about a year later where the board would randomly slam on the breaks for a split second and it again was because of a connection problem between the receiver and the vesc. Make sure you have solid connections and consider superglueing the receiver and cable together. Dont glue to the vesc since its expensive to replace 😀
```

---
## \#10 Posted by: Sebike Posted at: 2018-10-22T20:25:28.172Z Reads: 58

```
what pulselength value does the vesc get when it's going full throttle after 30 secs?
```

---
## \#11 Posted by: janpom Posted at: 2018-10-22T20:27:14.019Z Reads: 55

```
Good question. I should have checked that. I'll do it next time the remote goes crazy again (if I don't replace it earlier).
```

---
## \#12 Posted by: danielz Posted at: 2018-10-22T22:16:03.485Z Reads: 49

```
Yep, the gt2b kind of has 2 failsafes, it ignores the one you set if it doesn't get paired when you first turn it on and reverts to the stock 1.5ms. Its a ridiculous design or flaw. The only way to get make it safe is to set the neutral point of your trigger to 1.5ms. Use the caibration knobs on the controller. Then manually reset the failsafeto this new 1.5ms, because thats the only safe value. If your custom set manual failsafe happens to be near 1.5ms you would never know there was a flaw. See my post here.

https://www.electric-skateboard.builders/t/failsafe-issue-never-seen-this-before/53057/12?u=danielz

https://www.youtube.com/watch?v=Sk8cuHxZtyc
```

---
