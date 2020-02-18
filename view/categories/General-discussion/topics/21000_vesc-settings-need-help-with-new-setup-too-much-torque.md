# VESC settings need help with new setup! Too much torque

### Replies: 4 Views: 555

## \#1 Posted by: Mattmccrary8 Posted at: 2017-04-14T14:58:42.050Z Reads: 95

```
Ok so I'm almost completely done with my build, just putting on the enclosure. My setup is a TB 63 190kv motor ( the thing is huge lol ) and 2 5s 5000mah zippy lipos in series to make a 10s batt. What should my motor max settings be and batt max because the motor max is at 80, min -70 and batt max 50. The torque is way to high, what adjust that? And what settings adjust the remote to make it less touchy. I'm using a nano 2.4 from TB as well and his VESC bldc.
```

---
## \#2 Posted by: t0m_r1dd1e Posted at: 2017-04-14T15:41:13.128Z Reads: 93

```
Drop Batt Max to like 30 amps and see how that feels.
```

---
## \#3 Posted by: Hummie Posted at: 2017-04-14T15:58:52.264Z Reads: 89

```
leave the battery max and drop the motor max.  generally battery max is high speed power and motor max is low speed power
```

---
## \#4 Posted by: Stef Posted at: 2017-04-14T16:18:57.503Z Reads: 81

```
Oh oh, im building a dual TB 6355 with 10S on a 25" wheelbase deck xD Looks like I will have to do some taming too.

I second hummie, torque is generally proportional to current in the motor. Limiting your motor max current would be the best approach.

If you want to keep your max torque for hills, but still want to ' tame'  the board, you could limit the ' max ramping (dont remember the exact name)'  setting instead. This way the current is applied more slowly.
```

---
