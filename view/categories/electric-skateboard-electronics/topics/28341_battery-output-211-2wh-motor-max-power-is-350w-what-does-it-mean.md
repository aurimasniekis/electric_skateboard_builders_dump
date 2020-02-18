# Battery output 211.2wh, motor max power is 350w, what does it mean?

### Replies: 5 Views: 765

## \#1 Posted by: ray1202 Posted at: 2017-07-23T03:13:06.951Z Reads: 56

```
Hi, 

Stupid questions, I am looking into building something else but I don't know where to post the question to, so I hope someone here can help me. If I have a battery out putting 211.2wh (8.8ah X 24v), and the motor has max power of 350W, does that mean the motor will only run at 211.2watt max unless I get a better battery?
```

---
## \#2 Posted by: Boardnamics Posted at: 2017-07-23T05:53:27.369Z Reads: 51

```
No, Wh refers to the total energy stored inside the battery. It is basically the electrical engineering equivalent of Joules. One watt hour is equivilent to the energy released in a 1W load for 1 hour. 1J x 60m x 60s = 3600J per 1Wh. The total discharge in watts from a battery can be found by finding its C rating. This tells you how many amps can be drawn by the battery without some sort of failure. Higher C rating is always better, as it almost always denotates that the cells are of lower IR.
Okay I am getting off hand here. 350W for an 8.8ah battery should be fine unless it is extremely low quality or something.
350w/24v = 14.6A. An 8.8ah battery, or 8800mah means that the C rating would have to be less than 2C, not likely.

You will be fine using that battery :slight_smile:
```

---
## \#3 Posted by: willpark16 Posted at: 2017-07-23T05:55:03.820Z Reads: 50

```
Those two don't have to do with one another except that they will work
```

---
## \#4 Posted by: ray1202 Posted at: 2017-07-24T00:18:59.783Z Reads: 32

```
Thanks, i really need to learn about these.
```

---
## \#5 Posted by: Okami Posted at: 2017-07-24T22:05:12.945Z Reads: 23

```
If u can, search around @ray1202 , from *Wh* rating you can tell how many miles /kms u should be able to ride,

As about other stuff:

To get some data for.how many amps your battery might put out (or watts for.beter reference)

U have to know:

**Battery capacity**
**Battery voltage**
**Battery power output** (either in amps per cell or C rating)

Then you get max amps / watss it might produce.

With lipo unless u go below 5ah and 6s, u shouldnt have any problems (theoretically) if C rating is at least 20c or so

(15C - safer measure.to take)

15C x 22.2v (nominal battery volts) x 5ah =
75 x 22.2v = 1665 W of power
```

---
