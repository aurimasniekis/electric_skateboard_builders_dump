# DRV fried on another VESC

### Replies: 5 Views: 342

## \#1 Posted by: ryanguzman Posted at: 2018-04-27T16:21:05.544Z Reads: 81

```
**Parts**
VESC 4.12 (FW: 3.38)
[Motor](collections/electric-skateboard-motors/products/electric-skateboard-motor-6355-190kv)
[Batterys](https://hobbyking.com/en_us/multistar-high-capacity-6s-12000mah-multi-rotor-lipo-pack-1.html)

**Settings**
12s
BLDC
PPM & UART
https://imgur.com/SVKHfGN

I have have been using mu built eBoard for around 6 months now, and put probably close to 1000 miles on it. The board has been functioning perfectly fine the entire time. Recently I took a small ride, about 20 minutes then put the board down for 10. When I got back on it I accelerated hard and made it maybe 10 feet before it gave out under my feet. Took the board home and stripped it down, ran faults and kept getting a drv error. 

So my process so far has been simple, but I started by getting 3 new DRV's and I put a new one in without changing any settings. It fried as soon as I gave any load to the motor (without the pully attached!), instantly done. So I then replaced it again, and reupdated all my settings (No idea what settings I was using prior) so I would have a fresh start and know it wasn't due to me fucking up a setting prior.

My issue is that when I try to detect the motor, it doesn't turn. The motor flicks a little but and makes that high pitched noise R/C cars do, but nothing else. So here I am thinking I must have a failed motor but when I use my multimeter on the motor there is no shorts at all, and 0.3 Ohms phase to phase. When I put the motor in a drill and measure the AC voltage every phase makes about 1.6 volts.

So here I am, out of ideas and am looking to you guys for some guidance.
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2018-04-27T17:35:20.372Z Reads: 63

```
if there frying your not soldering them correctly u need pretty good equipment to do it properly
```

---
## \#3 Posted by: ryanguzman Posted at: 2018-04-27T17:59:33.013Z Reads: 56

```
The original fried too, I never soldered that one or changed the settings in 6 months of riding it. I'm not new to SMD soldering and have used all the proper equipment.
```

---
## \#4 Posted by: Exiledd_Top Posted at: 2018-04-27T18:18:08.504Z Reads: 52

```
then it's just a faulty pcb
```

---
## \#5 Posted by: ryanguzman Posted at: 2018-04-27T18:38:13.691Z Reads: 45

```
So I can connect it to the PC, flash firmware on it, upload new settings, it blinks and responds, the PPM is working, and its faulty? 

Also I have just found that T motor in realtime data is reading -70-80C.
```

---
