# Upgrade Questions

### Replies: 13 Views: 1366

## \#1 Posted by: mason Posted at: 2016-06-01T20:14:47.055Z Reads: 116

```
I burned out my [motor](http://www.electric-skateboard.builders/t/burned-out-motor/4010) the other day, so I am replacing my ESC and motor. What I have on order is a VESC and 200kv motor both from @chaka. I currently have 2x 3s 5000mah 20c LiPos from hobbyking. I am planning on adding batteries because 6s on 200kv isn't very fast. Should I buy another two of the batteries I have already for 12s, or get something else?

Thanks.
```

---
## \#2 Posted by: claudiofiore88 Posted at: 2016-06-01T20:19:30.255Z Reads: 113

```
If you refer to @chaka's thread here you'll see that 10s is actually the optimal battery for a 200kv motor.

http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#3 Posted by: mason Posted at: 2016-06-01T20:50:00.508Z Reads: 108

```
couldn't I just limit the voltage coming from the lipos? (12s but limit to 10s output)
```

---
## \#4 Posted by: chaka Posted at: 2016-06-01T21:08:44.783Z Reads: 100

```
The trouble with running 200kv at 12s is you will be running close to 10k rpm with a full charge and you will encounter errors if using a VESC. I think you would be happy at 9s and since you are already locked into 3 cell packs that would be your best bet.
```

---
## \#5 Posted by: NNGG Posted at: 2016-06-01T22:58:51.663Z Reads: 85

```
Is 12S preferable on a 190kv motor, a 170kv motor or a 150kv motor according to the VESC?
```

---
## \#6 Posted by: chaka Posted at: 2016-06-01T23:04:45.203Z Reads: 84

```
i wouldn't go any lower than 170kv at 12s and no higher than 190kv if I were building a speedboard. 

You can take it up to 200kv but it gets a little unreliable and causes problems with a full charge. You have to be sure you don't rev up the motor when it is unloaded or you can fry your drv chip.
```

---
## \#7 Posted by: NNGG Posted at: 2016-06-01T23:07:09.764Z Reads: 83

```
At 12S and 149kv it will climb hills proficiently is my guess at 16/36?
Correct me if Im wrong
```

---
## \#8 Posted by: g4tv4life Posted at: 2016-06-01T23:10:34.285Z Reads: 81

```
Yeah, Chaka's suggestion is the best budget wise. Just snag another 3s 5000 mah and go 9s.
```

---
## \#9 Posted by: chaka Posted at: 2016-06-01T23:46:56.196Z Reads: 76

```
In my experience it wont climb any better than a 192kv sk3 at 12s, a 149kv sk3 even at full charge will only hit around 7300 rpm. You end up losing 20% of the motors powerband. Not optimal but it does work well. 16/36 gearing is actually a little tall for a well rounded single drive. It will have good top speed but the climbing performance will suffer unless used in a dual configuration.
```

---
## \#10 Posted by: g4tv4life Posted at: 2016-06-02T05:16:53.873Z Reads: 65

```
On a unrelated topic Chaka, I have a 270kv 6364 that I'll be running at 6s single drive. I was thinking of using 16/36 gearing, the calc tells me a weighted top speed of 18mph. Do you think that gearing is safe for decent torque? 14/36 maxed out at like 15mph which seems a little to slow. What do you think?
```

---
## \#11 Posted by: chaka Posted at: 2016-06-02T13:49:00.801Z Reads: 63

```
It's a bit of a compromise since you will be maxing out at 6000 rpm.  If you could ad 2 cells and bring your voltage up to 8s you would have access to the full range of power from that motor.

Your calculations are a little off. At these speeds our boards run at almost 100% efficiency unless you have a really tight belt or an abnormally small motor.
```

---
## \#12 Posted by: g4tv4life Posted at: 2016-06-02T18:21:12.359Z Reads: 53

```
I'm account for some efficiency drop due to the fact I'm on the heavier side (230lbs or 104kg). I got a good deal on a 6s fvt esc so I'm limited to 6s at least for the time being, I'll probably go up to a VESC at some point and move into a 8 or 10s config. but for the time being, you think the 16/36 ratio is best?
```

---
## \#13 Posted by: Randyc1 Posted at: 2016-06-06T01:01:31.223Z Reads: 41

```
I have a single 245kv on 10s,... should i limit RPM to around 8800 ?
```

---
