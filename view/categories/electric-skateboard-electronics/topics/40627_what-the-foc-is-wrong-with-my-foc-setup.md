# What the FOC is wrong with my FOC setup?!

### Replies: 3 Views: 530

## \#1 Posted by: Tomer Posted at: 2017-12-10T21:28:14.738Z Reads: 156

```
I just updated a VESC firmware and applied FOC settings to it. 
I don't mind if something will blow up with this VESC as the seller gave me a guarante
that if anything will fail I have full warranty.

So I followed the VESC-Tool step-by-step tutorial on how to enable FOC mode.
Now the VESC is acting in very odd way. It might be a normal behivoar as well, 
I'm new to FOC so I'm not sure what to expect. I assume it's fixable. 

Anyways, here is a video to describe it better:

https://www.youtube.com/watch?v=c_p819XcaUw

When I try to launch it from a standing still (or even if I push the board a bit), it starts to cog like crazy.
If I release the throttle and then push it again it starts to push normal. It also happen without any load on it.

By the way, it's configured for sensorless.

Any suggestions what could cause the problem?
```

---
## \#2 Posted by: DavidBanner Posted at: 2017-12-10T21:51:23.815Z Reads: 143

```
did you do the motor detection again after switching to FOC?

looks kind of similar to this: http://www.electric-skateboard.builders/t/intermittent-weirdness-focbox-or-motor-issue-anyone-seen-this-before/39551/7 ?

which is normal FOC behavior for a non sensored motor
```

---
## \#3 Posted by: telnoi Posted at: 2017-12-11T06:57:09.609Z Reads: 89

```
sensorless foc loaded startup has been smooth here without cogging...so I'd not consider it to be normal.
```

---
