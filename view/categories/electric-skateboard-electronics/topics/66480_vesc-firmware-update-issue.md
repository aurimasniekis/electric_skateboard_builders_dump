# VESC Firmware Update Issue

### Replies: 12 Views: 889

## \#1 Posted by: ElBandido Posted at: 2018-08-29T17:16:48.814Z Reads: 129

```
I powered up my vescs, and while updating the firmware, ran into an issue with one of them.


![uploadingfirmware|690x420](upload://cko3R1JY6ul80WAhKpPggsjO3rv.png)


I updated the first one by navigating to the firmware tab in VESC-tool, and selecting the hardware and the new firmware. It worked just fine.

With the second VESC, I followed the same process, but it seems to not be taking the new update. I get this error message when I try to connect after loading the update.


![oldfirmware|500x173](upload://1uWA2nYnURSLund2KCVwSSUjeJn.png


![couldnotconnect|502x135](upload://6jX9ja23dxFd9zq7Z24mIh9x38w.png))



After some looking around, I think that it might be that my VESC doesn’t have a bootloader, but I’m not positive.

What do y'all think it could be?
```

---
## \#2 Posted by: maller Posted at: 2018-09-16T14:34:19.438Z Reads: 99

```
Hi there,

I have the same problem with my (Flipsky) (ESC). As far as I can tell the bootloader (under the firmware tab) is succesfully uploaded to the ESC, but when trying to update the firmware the ESC restarts and only a blue led comes on and then I get the same error as you have.

When I unplug power and reconnect it, both a blue and a green led come on, and vesc-tool can succesfully connect to the controller again. However, after connecting vesc-tool gives me a message saying I need to update the firmware. I am hoping someone can help with this error.
```

---
## \#3 Posted by: rexpepper651 Posted at: 2018-09-16T14:49:01.238Z Reads: 95

```
what flipsky esc are you using? im just curious.
```

---
## \#4 Posted by: DougM Posted at: 2018-09-16T15:19:37.149Z Reads: 91

```
I have the same problem - I haven't tried to load the bootloader yet because I wanted to get the board on the road  (not risk bricking anything), and now it's raining so the whole thing is on hold.

Isn't @BarbaraZ a flipsky rep?
```

---
## \#5 Posted by: maller Posted at: 2018-09-16T18:39:12.679Z Reads: 90

```
On the box it says it's an HGLRC-Flipsky 50A ESC. It looks like this one: https://flipsky.net/collections/electronic-products/products/torque-esc-vesc-%C2%AE-bldc-electronic-speed-controller.
```

---
## \#6 Posted by: maller Posted at: 2018-09-16T18:40:06.826Z Reads: 85

```
I do not know @BarbaraZ, but if she/he is indeed a flipsky rep it would be awesome to get a reply from her/him :).
```

---
## \#7 Posted by: DougM Posted at: 2018-09-16T22:33:09.405Z Reads: 79

```
Try this:

flipsky-service@outlook.com

Good Luck, let us know the outcome.
```

---
## \#8 Posted by: Jamesk8 Posted at: 2018-09-25T22:33:08.592Z Reads: 69

```
hi did anyone have any luck here? I'm having the exact same issue
```

---
## \#9 Posted by: ElBandido Posted at: 2018-09-25T23:12:28.318Z Reads: 70

```
Hey James, I did end up getting it to work.

I had to buy an ST-link v2 programmer, and reflash the problem speed controller.  Then I was able to load the firmware and get it to spin my motor
```

---
## \#10 Posted by: Jamesk8 Posted at: 2018-09-25T23:29:41.988Z Reads: 64

```
well that's a pain! thanks for your reply... fingers crossed i can get this thing working!
```

---
## \#11 Posted by: maller Posted at: 2018-10-03T09:38:04.453Z Reads: 58

```
I am still in contact with Flipsky service. They do provide great help, but no solution so far.
```

---
## \#12 Posted by: Miniproto Posted at: 2019-07-30T14:31:08.154Z Reads: 20

```
hi people the problems do still exist in 2019,any solutions ?
```

---
