# Different motors &amp; Dual VESC w canbus

### Replies: 4 Views: 495

## \#1 Posted by: Money Posted at: 2018-03-19T19:39:40.483Z Reads: 96

```
I'm just kind of curious if anyone has tried a dual motor setup using different motors, each connected to a vesc with canbus connected.

In the drone world, this is a big no no. But since each vesc is configured for each motor, I wonder if this is possible. Any body have any success with this?

Sorry if this has already been discussed. I searched for a related topic and didn't find anything.
Thanks
```

---
## \#2 Posted by: Colson003 Posted at: 2018-03-19T20:54:14.833Z Reads: 80

```
I ran a 5065 270kv (which I believe was closer to 230kv) with an SK3 6364 245kv. Worked just fine for me. 
Also the 5065 was in sensored FOC while the 6364 was sensorless FOC. This was all over can on TB VESC, only 6s though.

Edit: also to add to this very strange setup; the 5065 was geared 16/36 while the 6364 was geared 15/36. 

Why was I running this setup? Well I had 2 5065 motors, but then one broke, replacements weren’t available so I picked up the 6364

2nd edit: this was on 3.34fw and traction control was off.
```

---
## \#3 Posted by: Money Posted at: 2018-03-20T00:42:49.149Z Reads: 63

```
Wow. ok. thanks. That's encouraging.
```

---
## \#4 Posted by: NickTheDude Posted at: 2018-03-20T03:46:56.733Z Reads: 44

```
http://www.electric-skateboard.builders/t/uneven-dual-rear-drive/113
```

---
