# Weird VESC Problem

### Replies: 2 Views: 240

## \#1 Posted by: bharned Posted at: 2017-08-28T00:25:58.355Z Reads: 61

```
Hi guys, this is my first post in here. I've used this forum a lot to put the parts together for my first build. So far I'm happy with how things are coming together, but I have run into a problem when getting my VESC set up. 

I purchased the partially assembled VESC online, but then soldered on the MOSFETS, shunt resistors, microcontroller and DRV myself. I built two battery packs for the board (both 5s), and when getting the VESC set up I only connected it to one pack. After installing the firmware and everything per Vedder's Youtube tutorials, I hooked up the motor (Turnigy SK3 6463 245kv) and ran the 'detect motor' function. The motor ran very roughly for a while during the test, then I got the "detection failed" message. I didn't get any other error messages or fail codes. I looked through the forums, tried a bunch of solutions, and finally tried increasing voltage. I hooked up the other battery pack in series (so I now have it hooked up to 10s) and ran the detect motor function again. This time the motor did not spin up, and I got a DRV failure message. 

The weird thing is that I can go back to 5s, run motor detection, and the motor will spin up again with no DRV error message (still doesn't successfully detect the motor though). It only gives me the DRV fail code when I hook it up to 10S. I hate the thought of trying to replace the DRV with that ground pad soldered underneath it.  Any thoughts?
```

---
## \#2 Posted by: scepterr Posted at: 2017-08-28T00:31:11.935Z Reads: 58

```
Bad joint somewhere? When in doubt, reflow everything.
```

---
