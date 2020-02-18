# Replaced DRV, current spikes and intermittent DRV error

### Replies: 5 Views: 558

## \#1 Posted by: JohnA Posted at: 2017-07-21T00:25:15.369Z Reads: 82

```
My vesc 4.12 stopped working a month ago and today I tackled replacing it. It went well it seemed, but when I plugged it back in it still wasn't working. It would jolt the motor, and then show a DRV error when the sampling was activated. But a second later the error would go away. During the motor jolt, the plot shows a current jump anywhere from 7amps-57 amps. I'm hoping the new DRV isn't fried yet, but there is obviously an underlying problem. I reloaded the firmware (4.18) and it didn't change anything.  The vesc was bought from torqueboards 4 months ago, I've only used it in BLDC. Attached are pictures, before replacement, after and a picture of the graph. Let me know if you have any ideas! Thanks.<img src="/uploads/db1493/original/3X/4/2/420d386a91619c04df6daec7696b4a8ba3616bc7.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/2/a/2af1f0441a9c15c45e8baae576266ae00b78a7ba.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/5/0/506964b790ea4cb5f27e60ec0a0112f061224d81.jpg" width="281" height="499"><img src="/uploads/db1493/original/3X/5/c/5c11b4297d1bf792b5f0491131ea4e7824e8dd16.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/b/9/b90d76e04957f3be4f7d26f20ec30c2abc54b569.JPG" width="375" height="500">
```

---
## \#2 Posted by: JohnA Posted at: 2017-07-21T00:41:51.905Z Reads: 69

```
Also, I've tried more then one motor, so the motor isn't shorted and causing it. @JohnnyMeduse  any ideas? Or @chaka ?
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2017-07-22T13:16:16.027Z Reads: 44

```
Hi John, did you retouch any of  the soldering over the DRV with a soldering Iron, I do believe that you might have a cold solder joint on one of the pads.
```

---
## \#4 Posted by: JohnA Posted at: 2017-07-22T14:39:04.977Z Reads: 39

```
@JohnnyMeduse  I used a desoldering wick to get all the access off, then touched each pin with the iron like in Benjamin vedders YouTube video. I'll try putting more solder on them today and see if that helps
```

---
## \#5 Posted by: JohnA Posted at: 2017-07-22T18:00:24.725Z Reads: 27

```
@JohnnyMeduse well. Resoldered it and made sure each connection is good. Plugged it in and tried a motor connection. Blew the drv right up <img src="/uploads/db1493/original/3X/4/4/44c47a0882ca6c164845346a2cbae68a44ab5494.JPG" width="375" height="500">
```

---
