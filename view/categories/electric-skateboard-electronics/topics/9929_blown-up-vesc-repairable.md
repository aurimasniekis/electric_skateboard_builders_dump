# Blown UP VESC repairable?

### Replies: 4 Views: 708

## \#1 Posted by: Flo Posted at: 2016-09-21T08:32:05.537Z Reads: 117

```
<img src="/uploads/db1493/original/3X/2/3/23c28aa0d2430ffca49350f69b0ca0e299f93390.JPG" width="690" height="460">
I attached huge Heatsinks to my VESC in my electric bike. I was so silly not to use self-securing nuts. Due to Vibrations the Heatsinks got loose and shorted the MOSFETS as seen in the picture. When powering up the VESC, the LED doesn't even light up any more and you can see that the DRV8302 is burned. At other parts there is at least no visible damage...
Does anybody know the VESC so good that you can tell me if there is a huge possibility that the VESC will work again after changing the DRV8302 (and the STM32F) or is it completely broken and I shouldn't try to repair it..?
Thanks for any help :)
```

---
## \#2 Posted by: DeathCookies Posted at: 2016-09-21T08:51:30.113Z Reads: 108

```
People can only decide whether your VESC is repairable or not (**only** changing stm and drf) when you are providing pictures of the top and back side of your vesc to see all components. ;)

@chaka is your man.

chaka, it is annoying to be the man of the men, isnt it?
```

---
## \#3 Posted by: Flo Posted at: 2016-09-21T10:36:17.656Z Reads: 92

```
Here are the pictures. The only visible damage is the hole in the DRV8302. But I can't draw any conclusions if a faulty DRV8302 would cause the LED to stay dark or if that is a sign that the stm is faulty , too or if that's a sign that there are multiple things broken and rapairing isn't really reasonable...<img src="/uploads/db1493/original/3X/e/d/ed9128d0951f134fc9b23e09a96248f6c1c96036.JPG" width="690" height="460"><img src="/uploads/db1493/original/3X/7/2/723c2334717ffa7343e802be22bf5acf850f6fe9.JPG" width="690" height="460">
```

---
## \#4 Posted by: chaka Posted at: 2016-09-21T13:39:54.854Z Reads: 80

```
Yeah it's toast. Not an easy repair either since a failure like this usually fuses leg 29 V_SUPPLY to the pcb. It will need to be carefully clipped before using hot air to remove the chip.

Once you have a fresh DRV chip you will find out if you need a new stm chip. You could also use some jumpers to supply the 5v rail to check the stm chip first. You would need some sort of 5v supply to do this.
```

---
