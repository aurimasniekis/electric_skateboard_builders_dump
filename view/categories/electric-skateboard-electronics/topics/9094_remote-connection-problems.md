# Remote connection problems

### Replies: 25 Views: 3294

## \#1 Posted by: Strawbs Posted at: 2016-09-06T22:52:38.662Z Reads: 186

```
Hi All,

I have the Winning remote provided by Enertion with my dual motor kit.  It works fine 90% of the time but seems to have a small connection issue.  There occasionally will be a delay between when I throttle and the motors spinning.  Occasionally a delay when braking, and the worst is when I release the throttle, and the board continues to drive for a second or two... 

It seems like other people are having issues with this remote as well.  Is there a way to increase the signal to the receiver?  Is there a better remote out there that is more reliable?  Any thoughts would be much appreciated.

Thanks,
```

---
## \#2 Posted by: Jinra Posted at: 2016-09-06T23:14:29.582Z Reads: 175

```
Exact same issues a bunch of people here are experiencing with this remote, including myself. I've tried soldering an extra antenna on the receiver and remote but it doesn't help.

Pretty sure it's not a weak signal issue, but a design flaw with the actual remote itself.
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2016-09-06T23:43:39.615Z Reads: 164

```
Has anyone tried a different type of reciver?
```

---
## \#4 Posted by: Jinra Posted at: 2016-09-06T23:44:22.064Z Reads: 151

```
@Lizardking0069 has, same issue
```

---
## \#5 Posted by: Mikenopolis Posted at: 2016-09-07T00:29:33.654Z Reads: 151

```
I had the same issue riding in my home area. But this past weekend I rode about 8 miles (4 mile round trip) in another city and had ZERO drop outs. Really weird. But it is like someone said. Winning is a Russian roulette remote.

@Jinra I just received another receiver from Hobby King. Swapping that isn't really going to fix anything since it's lightly the remote that has issues right?

I really wish @onloop would tell us if his Nano-X, which visually looks like a reshelled Winning remote, has sorted out the issues we've had.
```

---
## \#6 Posted by: Jinra Posted at: 2016-09-07T00:31:08.125Z Reads: 141

```
yea, like i said, lizardking tried this and still had issues, i got a gt2b receiver myself but didn't bother trying.
```

---
## \#7 Posted by: michaeld33 Posted at: 2016-09-07T00:34:30.335Z Reads: 137

```
I just received a winning remote direct from Winning Corp. (yes that is their actual name)
Honestly, it's BAD. Really BAD, I kid you not. I was trying to go forward (pushing it forward), and it went backward. I don't even know how or why, but it was going BACKWARD!
```

---
## \#8 Posted by: michaeld33 Posted at: 2016-09-07T00:39:46.317Z Reads: 135

```
It's a shame too because the winning remote is REALLY nice, good size, good functionality, just horrible signal
```

---
## \#9 Posted by: Jinra Posted at: 2016-09-07T00:45:47.654Z Reads: 138

```
I bet the throttle was installed backwards
```

---
## \#10 Posted by: Lizardking0069 Posted at: 2016-09-07T00:50:49.358Z Reads: 137

```
The reciever that came with the winning remote died on me, thats why I tried the g3b reciever. I didnt really get to challenge the original's range. With the g3b the range should be much better as it has an actual coax antenna, not a pcb element. The things I like about the controller are the formfactor and the thumb stick. However, the travel distance and the smoothness of the thumb stick are not very good. I don't get good pushback like on the nunchuck. I may open up the winning remote to see how that can be improved. I was getting acceleration problems where I would push whole out throttle then released and the board kept going for half a second which was scary. I have the same problem with the nunchuck so it may be a vesc configuration issue. However, the lag effect is not that noticeable on the nunchuck; I really have to push up to a certain speed and let go to get the .5s lag.
```

---
## \#11 Posted by: Lizardking0069 Posted at: 2016-09-07T00:53:46.900Z Reads: 129

```
Swap two of the motor wires.
```

---
## \#12 Posted by: michaeld33 Posted at: 2016-09-07T00:54:38.962Z Reads: 123

```
But sometimes it went forwards, other times, backwards??
```

---
## \#13 Posted by: michaeld33 Posted at: 2016-09-07T00:55:03.137Z Reads: 124

```
Nope, my 2.4ghz mini remote works, just the winning. It's weird.
```

---
## \#14 Posted by: Namasaki Posted at: 2016-09-07T03:12:36.803Z Reads: 118

```
I had issues with the winning remote as well.
I am using the 2.4 mini again and it is absolutely flawless teamed up with the Vesc.
Once you get used to the trigger, it's really very good for control.
I have found that I get a lot more hand fatigue using a thumb control than a trigger control.
```

---
## \#15 Posted by: boards Posted at: 2016-09-07T03:17:51.015Z Reads: 114

```
I had this problem with my own nrf24 based remote. (I think winning is also based on this chip).

Solder a 22nf cap between + and - on the nrf module on the receiver and controller and it's much better.
```

---
## \#16 Posted by: caustin Posted at: 2016-09-07T03:30:57.175Z Reads: 114

```
Can you show a picture of how you solved it, easier to replicate!  Thanks if easy.
```

---
## \#17 Posted by: Dunmer Posted at: 2016-09-07T07:59:34.071Z Reads: 107

```
Is it maybe possible that the signal gets interupted by other 2.4ghz devices? (Wifi for example) Maybe these cheap controllers don't have freqeuncy hopping capabilities and stick to one band in the 2.4ghz and there for get bad disturped signals?
My Graupner does switch between 12 bands in 2.4ghz so you don't interuped other flyers but you also pay the price for it offcourse.
```

---
## \#18 Posted by: Tomkav Posted at: 2016-09-07T09:19:06.730Z Reads: 104

```
It doesn't have a very strong signal. When it happens try to release full grip of the controller. Works for me but I'm going to change it to the bench wheel style remote suggested by @Jinra.
```

---
## \#19 Posted by: Luke Posted at: 2016-09-07T09:47:19.684Z Reads: 101

```
I had to adjust the minimum and maximum pulsewidth everytime i use it on a new vesc, but apart from that mine is bombproof, should i be worried and look at getting a more reliable.. or should it be if its been ok so far
```

---
## \#20 Posted by: Kaly Posted at: 2016-09-07T11:53:49.943Z Reads: 99

```
My personal use one I have not problems at all when properly charge. The one my wife uses have had some issues, but can't determine properly because she never seems to have it properly charge. 

I think the transmitter in the remote does not produce a strong enough signal, it depends on the voltage level of the battery :-( , following on @Tomkav not having a full grip on the remote helps with signal issues. 

One more thing this remotes are working better when paired with the VESC. ;-)
```

---
## \#21 Posted by: sandrewvdv Posted at: 2016-09-07T11:56:27.450Z Reads: 91

```
Mine had the same issue. However, I was using a aluminium enclosure and my receiver was placed in this. 
Placing the receiver outside the box fixed this issue for me.

My thread on this: http://www.electric-skateboard.builders/t/constantly-cutt-off-when-riding-while-using-wining-remote/6914
```

---
## \#22 Posted by: Strawbs Posted at: 2016-09-07T22:43:59.025Z Reads: 86

```
Ok thanks for the feedback.  It sounds like this remote is shaky at best.  Does anyone have a good alternative I could switch to?  I'm looking for function over form.  I need it to be tried and tested to work 100% of the time.

Thanks,
```

---
## \#23 Posted by: Michaelinvegas Posted at: 2016-09-07T22:59:52.737Z Reads: 86

```
Every one seems happy using the mini remote... Starting the 3rd group buy if interested 

http://www.electric-skateboard.builders/t/mini-remote-group-buy-part-3-10-remotes-36-for-one-or-two-for-70-shipped-usa/9136?u=michaelinvegas
```

---
## \#24 Posted by: Alexander Posted at: 2016-09-17T14:05:58.317Z Reads: 76

```
I'm having THIS EXACT same issue with my new Raptor @Strawbs which uses that "Winning" remote. Yesterday the connection cut out on me momentarily on my very first ride and reengaged at full-throttle putting me swiftly on my ass - essentially as I was on an incline and had my back foot on the kick-tail so my centre of gravity was not ideal for the sudden jolt, but worst of all I damaged the carbon fiber when it went flying, tried braking but no joy :'( had to superglue it.. Serious bummer. I see on the Enertion website they're getting the new remotes in stock soon so will try one of them and see if it solves this. With a board this powerful, and yes it's power is shocking (in a great way) we NEED a really dependable remote system. <img src="/uploads/db1493/original/3X/d/6/d64482bf6628a5c73cf0d6bb6aa2f9cc7ab38532.jpg" width="640" height="360"><img src="/uploads/db1493/original/3X/d/e/def000c7e22d5b1871d05cbd951d2e789e7080b5.jpg" width="640" height="360">
```

---
## \#25 Posted by: Lsalt Posted at: 2016-09-17T19:52:14.196Z Reads: 65

```
That's  what I did as well. Had to mount the receiver outside the enclosure. Other components may cause interference but it is definitely a signal issue. Hold your remote by your board and crouch.....problem solved...equals signal. This told me it wasn't the vesc causing interruption.
```

---
