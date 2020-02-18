# Crackling sound from motor that&rsquo;s not mechanical

### Replies: 6 Views: 309

## \#1 Posted by: Jakeii Posted at: 2018-05-11T16:45:45.650Z Reads: 92

```
So I just put in a new FOCBOX  and a new motor on my board and now I'm getting this strange sound from the motor. Although the sound still comes when I put the old one back in so I don't think it's that.

I can't test my old FOCBOX as it blew up, the only other thing it could be is that during an earlier test the receiver for my Benchwheel remote blew up :sweat:, so I had to switch to a crappy old winning remote, could that be the cause?
Video:
https://www.youtube.com/watch?v=MqMxmpyU_9M&feature=youtu.be
```

---
## \#2 Posted by: mmaner Posted at: 2018-05-11T16:47:54.001Z Reads: 88

```
Sounds to me like something is arcing or a bad bearing. Hard to tell.
```

---
## \#3 Posted by: Jakeii Posted at: 2018-05-11T16:49:53.767Z Reads: 88

```
On 2 separate motors? One is known good, the other is brand new, they both spin freely by hand :confused:
```

---
## \#4 Posted by: mmaner Posted at: 2018-05-11T16:50:47.667Z Reads: 84

```
It's just what it sounds like. Could be a bad wheel bearing, not a motor bearing.
```

---
## \#5 Posted by: Deckoz Posted at: 2018-05-11T17:06:35.432Z Reads: 74

```
Sounds like a bad detection

Rerun the detection with a higher duty cycle and amperage value.
```

---
## \#6 Posted by: Jakeii Posted at: 2018-05-16T14:34:49.334Z Reads: 29

```
Bingo! :+1: thanks, this was it, my battery was close to the cutoff voltage when doing the detection.
```

---
