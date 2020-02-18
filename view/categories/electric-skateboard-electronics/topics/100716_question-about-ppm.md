# Question About PPM

### Replies: 2 Views: 126

## \#1 Posted by: ODBounty Posted at: 2019-08-22T19:32:50.277Z Reads: 31

```
Hey all, quick question about PPM mapping and setting up. So for a week I was using this receiver connection for my flipsky remote for my vesc 4.![nonesc|690x408](upload://aVcEoigZbRLjAQ45pXFQi5lil7o.png) 

I was able to do PPM mapping on it and everything was fine until i realized I didn't have a reverse function anymore. So i switched to this reciever connection ![vesc|690x375](upload://z4Iq2Ec4YUuWVwdS72yQwESlLb3.png) 

The board functions but now pulselength stays at 0 and i cant do PPM mapping for whatever reason. ![ppm|690x388](upload://jWGGLj3y4vXXsqp2dmyZXwWqUKO.png) 

Anything I'm missing that could help me solve this issue?
```

---
## \#2 Posted by: Anubis Posted at: 2019-08-22T19:35:47.781Z Reads: 29

```
UART replaces PPM. You do not do any mapping at all, it should just work as soon as you plug it in with no changes in your vesc settings.
```

---
