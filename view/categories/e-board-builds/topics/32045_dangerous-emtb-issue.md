# Dangerous emtb issue!

### Replies: 11 Views: 674

## \#1 Posted by: hahne Posted at: 2017-09-01T21:14:55.184Z Reads: 127

```
Hey everyone! 

I recently made an electric mountainboard. Its awesome! But there is a critical issue that I am having with it. For some reason, while riding the wheels lock-up and I get thrown off. Luckily, this has only happened at relatively low speed, but was still enough to mess up my ankle. At my board's top speed of 50km/h though, this could be a life threatening issue. since it happens so fast, and only once in a while, I have not been able to pinpoint if it is one or both of the drive wheels that lock up. 

Anyone have any suggestions? 

The build uses: 
2x 55mm motors 
2x hobbywing max6 ESCs 
1x arduino/ Hc-05 bluetooth module
2x multistar 10amp batteries in parallel
and a chaindrive
```

---
## \#2 Posted by: Dornacht Posted at: 2017-09-01T21:18:14.049Z Reads: 121

```
If they are locking up and not turning, I would say it would be two of your motor leads are shorting out, either where they connect with the esc or internal
```

---
## \#3 Posted by: lunasicc Posted at: 2017-09-01T21:32:32.742Z Reads: 117

```
Too many variables, your remote could be cutting out and could be actuating 100% brake on failsafe. It would be rare that both motors would short out due to them being on there own speed controllers
```

---
## \#4 Posted by: hahne Posted at: 2017-09-01T21:35:33.994Z Reads: 110

```
Okay I have a spare motor, so maybe I'll try swapping one out. I noticed that one of them was making a weird scraping noise when I received it. if they were shorting, wouldn't they lock up on each rotation though? sometimes this problem presents itself 15 minutes into a ride. 

Thanks!
```

---
## \#5 Posted by: hahne Posted at: 2017-09-01T21:38:47.151Z Reads: 103

```
Yeah I think it might just be one motor that is seizing, but its hard to say for sure. I'm using my phone to control the arduino via bluetooth. It never failed before on my previous longboard build, but that was also a different ESC/Motor combo.
```

---
## \#6 Posted by: Dornacht Posted at: 2017-09-01T21:40:13.845Z Reads: 91

```
I couldn't tell ya without seeing it, they can do interesting things if it is a bad motor
```

---
## \#7 Posted by: hahne Posted at: 2017-09-01T21:47:05.033Z Reads: 84

```
Okay I'll try to get a recording of it sometime soon
```

---
## \#8 Posted by: lunasicc Posted at: 2017-09-01T21:56:13.165Z Reads: 74

```
Honestly I'd ditch that Bluetooth setup and just buy a gt2b in the mean time and run it. See if that resolves the issue. Not a bad test for only $26
```

---
## \#10 Posted by: hahne Posted at: 2017-09-01T22:38:21.716Z Reads: 66

```
I just tested the thing, and it looks like the problem is only on the left wheel. It suddenly stops, even when it is in the throttle up position. The right has not presented the issue YET. Although the right is giving me a strange vibration that i'll deal with later.

Also worth mentioning that the primary ESC on the left is the only one that powers the arduino setup. The secondary ESC only receives the signal wire. (not sure if that would cause any problems)
```

---
## \#11 Posted by: hahne Posted at: 2017-09-01T22:43:07.333Z Reads: 59

```
I'll probably look into that too. I just tested the thing, and it looks like the problem is only on the left wheel. It suddenly stops, even when it is in the throttle up position. The right has not presented the issue YET. Although the right is giving me a strange vibration that i'll deal with later.

Also worth mentioning that the primary ESC on the left is the only one that powers the arduino setup. The secondary ESC only receives the signal wire. (not sure if that would cause any problems)
```

---
## \#12 Posted by: hahne Posted at: 2017-09-15T01:27:58.152Z Reads: 32

```
SOLVED! 

Program of the arduino was sending a less than minimum speed signal to the ESC upon loss of bluetooth signal, causing wheel lockup. Code altered to fix this.

Throttle returning to neutral position was also sending a less than minimum speed signal, causing lockup due to improper calibration of the ESC throttle. Correct calibration fixed this issue
```

---
