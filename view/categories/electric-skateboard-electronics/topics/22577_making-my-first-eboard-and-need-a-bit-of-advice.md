# Making my first eboard and need a bit of advice

### Replies: 15 Views: 478

## \#1 Posted by: pat.speed Posted at: 2017-05-07T07:54:26.579Z Reads: 79

```
Hey guys, I'm new to this community and looking to get some help with my first eboard. I currently have 2 3s lipos being shipped as well as a 190kv Keda motor. I also have 83mm wheels from enertion. I was just wondering what the best speed controller would be as I'm likely to upgrade to 12s in the future. Oh and I have a 3:1 gear ratio. Any help would be appreciated. Mostly to do with the Keda motor has anyone ever tried one?
```

---
## \#2 Posted by: Jinra Posted at: 2017-05-07T07:56:48.871Z Reads: 77

```
Pretty much everyone will tell you get a VESC. It's the best fit for esk8.
```

---
## \#3 Posted by: pat.speed Posted at: 2017-05-07T07:59:00.228Z Reads: 73

```
Yeah. That's the way I'm leaning but I just read a few things about the vesc not being good for 12s. What's your opinion?
```

---
## \#4 Posted by: Jinra Posted at: 2017-05-07T07:59:56.734Z Reads: 69

```
There's plenty of 12s builds for it, you just need to be careful as it's reaching the upper limits of the VESC, especially with a higher kv motor. Just stay within voltage and erpm limits and you should be fine.
```

---
## \#5 Posted by: pat.speed Posted at: 2017-05-07T08:01:41.337Z Reads: 67

```
Is there a way to limit erpm on the vesc. And is 190kv too high?
```

---
## \#6 Posted by: Jinra Posted at: 2017-05-07T08:03:33.408Z Reads: 63

```
You can turn on the soft eRPM limit in the app config panel on BLDC tool. 190kv would bring you to a theoretically max of 63,680 erpm which is over the 60k soft limit. You should be fine if you account for voltage sag, but to be safe I'd turn on the soft limiter.
```

---
## \#7 Posted by: pat.speed Posted at: 2017-05-07T08:07:08.735Z Reads: 62

```
Just clarifying, so if I turn on the soft limit it will keep the erpm under or at 60k?
```

---
## \#8 Posted by: Jinra Posted at: 2017-05-07T08:08:50.471Z Reads: 61

```
It will start braking to keep the eRPM under the limit
```

---
## \#9 Posted by: pat.speed Posted at: 2017-05-07T08:11:37.298Z Reads: 61

```
Ok thanks. And I don't really mind if that happens because I won't be going full speed all the time. Will it brake hard of just softly?
```

---
## \#10 Posted by: Jinra Posted at: 2017-05-07T08:12:49.351Z Reads: 59

```
There's a "start" and "end" setting for the limit. When it hits "start" it'll throttle back the speed with increasing strength until it hits the "end" limit.
```

---
## \#11 Posted by: pat.speed Posted at: 2017-05-07T08:15:09.090Z Reads: 55

```
Ok thanks for your help! I'm definitely going for a vesc then. You wouldn't happen to have a spare one you could sell me on the cheap would you? Enertions a bit pricey for me as I'm only 15
```

---
## \#12 Posted by: Jinra Posted at: 2017-05-07T08:16:22.330Z Reads: 53

```
I actually have one I'm selling for $80 right now, but there's someone already interested, if they don't pay by tomorrow I'll PM you if you're interested.
```

---
## \#13 Posted by: pat.speed Posted at: 2017-05-07T08:17:01.380Z Reads: 54

```
Yes thanks mate! Is 80 usd?
```

---
## \#14 Posted by: Jinra Posted at: 2017-05-07T08:17:21.981Z Reads: 53

```
Yep, based in Cali
```

---
## \#15 Posted by: pat.speed Posted at: 2017-05-07T08:19:22.303Z Reads: 53

```
Oh that's a bit of a bummer as I'm in Aus. Would I still be able to get it if I paid extra for the shipping?
```

---
