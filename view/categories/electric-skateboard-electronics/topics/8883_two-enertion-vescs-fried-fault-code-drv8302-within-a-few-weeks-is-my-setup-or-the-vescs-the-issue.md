# Two Enertion VESCs fried (fault code DRV8302) within a few weeks. Is my setup or the VESCs the issue?

### Replies: 4 Views: 686

## \#1 Posted by: Nicolai Posted at: 2016-09-04T06:36:59.805Z Reads: 146

```
I'm pretty frustrated. I've been working on a DIY skateboard for months now but I've now gone through two VESCs from Enertion and I've probably ridden one mile on my board total. Both are fried because of DRV8302 fault codes. The first VESC blew when I tried to switch to FOC mode. The second one blew before I could even ride the board with the new VESC, when I adjusted the battery regen on BLDC tool (the exact same numbers that worked perfectly well in BLDC mode on the first VESC with my board setup). I'm definitely going to try to warrantee these faulty VESCs, but in the meantime I'm really unsure what I'm doing wrong. I've read so many feeds and watched so many esk8 support tutorial videos online and I can't seem to figure it out. Is it possible that I have a short in my board somewhere?

Parts:
- Enertion Space Cell Pro 4
- Enertion 6374 motor
- Enertion VESC
- Hobbyking GT2B tx/rx

Any help would be appreciated. Should I order a VESC from a different supplier maybe?
```

---
## \#2 Posted by: onloop Posted at: 2016-09-04T06:47:26.683Z Reads: 145

```
There is a bug in the firmware. Did you update the firmware? If not it probably killed the vesc. Latest batches have new firmware.

Changing back and forth from foc to BLDC can cause problems. Stay on BLDC unless you must have a silent operation.

If you have a platinum warranty we will send you two new ones. Email support@enertionboards.com
```

---
## \#3 Posted by: Nicolai Posted at: 2016-09-04T06:53:34.668Z Reads: 143

```
Thanks @onloop! I seriously appreciate the gesture, and I'll definitely be sending out that email. And no, I didn't update the firmware for the second VESC that I received because when I connected to it and read the configuration, the firmware tab said that the VESC firmware was up to date with the most recent version, so I didn't think I had to reinstall or reboot it.
And I certainly learned my lesson about changing from BLDC to FOC when I fried my first VESC that way... BLDC now and always for me haha
```

---
## \#4 Posted by: racidon Posted at: 2016-09-04T07:24:37.083Z Reads: 134

```
[quote="Nicolai, post:3, topic:8883, full:true"]
Thanks @onloop! I seriously appreciate the gesture, and I'll definitely be sending out that email. And no, I didn't update the firmware for the second VESC that I received because when I connected to it and read the configuration, the firmware tab said that the VESC firmware was up to date with the most recent version, so I didn't think I had to reinstall or reboot it.
And I certainly learned my lesson about changing from BLDC to FOC when I fried my first VESC that way... BLDC now and always for me haha
[/quote]

I never did anything in BLDC except for initial setup and this has and still happens to me 3 out 3 vescs I'm moving on to other products :)
```

---
