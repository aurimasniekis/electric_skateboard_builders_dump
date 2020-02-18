# Weird issue with focboxes

### Replies: 11 Views: 322

## \#1 Posted by: DAddYE Posted at: 2018-11-20T22:55:05.736Z Reads: 129

```
Hi all,

while I'm riding sometimes happens that my motors stop working, like they get only 1 amp, it seems to me that the Focboxes lose the settings. In fact, usually just reflashing the mode from metr.at solves the issue.

The thing, however, is, that if I keep closed the metr.at app I don't see this issue.

Can be that metr try to do something without ... consent lol? @rpasichnyk thoughts?

Here my logs:

https://drive.google.com/open?id=1btN7Vn6kSOtdfXcr1Jh-LjC-fT_OLkqS

Thanks guys.
```

---
## \#2 Posted by: rpasichnyk Posted at: 2018-11-21T07:03:58.770Z Reads: 107

```
Do you have other UART devices? Like UART remote? Or display?
```

---
## \#3 Posted by: DAddYE Posted at: 2018-11-21T20:07:33.377Z Reads: 86

```
Yes, the Photon remote
```

---
## \#4 Posted by: rpasichnyk Posted at: 2018-11-21T20:25:35.609Z Reads: 81

```
Alright, this is actually something I noticed a few times. Basically when the commands are coming to VESC from different sources (CAN and UART) at the same time, weird stuff can happen. No issues with PPM though.

@Pimousse @Deodand @janpom @Wajdi @Ackmaniac @twan @emmaanuel  

I think this is a very nasty problem and it would be awesome if we can figure out why it's happening.
```

---
## \#5 Posted by: janpom Posted at: 2018-11-21T21:00:03.651Z Reads: 71

```
Just a wild guess. I noticed that when requests to VESC are too frequent, I get rubbish in the response. It's not that just some requests don't get the proper response. Literary all requests get rubbish responses unless enough time is allowed between them.

So maybe in case one request comes in over CAN and another over UART at the same time, it's the same kind of situation. Then potentially the remote could get a rubbish response and get confused and things go wrong from there.
```

---
## \#6 Posted by: Pimousse Posted at: 2018-11-21T23:07:06.917Z Reads: 55

```
This point is critical for me.
Currently, there is no priority given to a specific protocol over another one.
Say you set the VESC up this way : PPM + UART and "Send status over CAN" and you can drive the motor through 3 differents protocols (PPM, UART and CAN) without any hierarchy.
IIRC, this point has been mentioned, but can't tell BV's answer.

EDIT : Vedder promised a new FW with a lot of features (apparently) in the next days/weeks.
This may have been managed hopefully.
```

---
## \#7 Posted by: DAddYE Posted at: 2018-11-21T23:35:51.770Z Reads: 56

```
Mmm, but happens even when I use the ppm remote and turn off the photon. Do you think the receiver is still sending something even when the remote is off?
```

---
## \#8 Posted by: Wajdi Posted at: 2018-11-22T01:16:44.254Z Reads: 56

```
There is just as much a Vesc can handle at a time before things go wrong. As @janpom mentioned, once a command is sent, a wait time is needed before getting a correct response. If requests are sent faster than what the Vesc can process, then corrupted data will be an issue.

I thing the vesc needs a better protocol management, especially when communicating through different protocol channels. 

However I personally didn't experience the issue @DAddYE is describing, I'm running the Photon receiver on UART and dual setup on CAN bus with no issues.
```

---
## \#9 Posted by: DAddYE Posted at: 2018-11-22T15:47:24.841Z Reads: 35

```
Mmm, this is interesting 

https://www.electric-skateboard.builders/t/universal-advanced-vesc-remote-control-photon-custom-design/24654/1016?u=daddye

@rpasichnyk thoughts on my issue?
```

---
## \#10 Posted by: rpasichnyk Posted at: 2018-11-22T16:30:16.711Z Reads: 29

```
You already tested with Metr App off. Can you unplug Photon receiver and test with another PPM remote? This way we can make sure that it is neither an issue with Metr Pro nor the issue with Photon remote, but the problem when you have them both.
```

---
## \#11 Posted by: DAddYE Posted at: 2018-11-23T06:43:42.404Z Reads: 20

```
Sure, will test ASAP
```

---
