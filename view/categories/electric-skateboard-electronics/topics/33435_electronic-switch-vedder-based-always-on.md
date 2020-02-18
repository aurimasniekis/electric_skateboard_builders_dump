# Electronic switch (vedder-based?) always on?

### Replies: 3 Views: 274

## \#1 Posted by: Caanon Posted at: 2017-09-18T19:00:46.641Z Reads: 57

```
Hey everyone!

Been lurking for a while now, reading up on how to build my own skateboard for commuting. Been going slowly since this is my first battery-powered project. I've made some decent progress so far:

- Big 'ol Turnigy 5065 236kv outrunner
- Got a VESC 4.12 up and running 
- Tweaked the v3.7 firmware to enable official Wii Nunchuck support (that was a pain... new controllers are apparently much more finicky with i2c timing)
- Machined a [custom bracket](https://photos.app.goo.gl/yjq9dCWUzPTndMCm2). Hat tip to @torqueboards [original design](diy-electric-skateboard-kits-parts/single-bolt-on-motor-mount-with-drive-wheel-kit/).
- Built an [8s2p pack](https://photos.app.goo.gl/oXSUAmHPCqwSLVep2) of A123 26650s
- Wired up [the harness](https://photos.app.goo.gl/foxt0BdzCzoAfYSc2)

So far so good, but now I'm running into a big of a baffling issue. I got the [electronic on/off switch from ](diy-electric-skateboard-kits-parts/electric-skateboard-on-off-power-switch/) - which I believe is based on Vedder's switch...? - since that would help with current inrush and give me pushbutton power to the board. Unfortunately I can't seem to get it to work correctly, since it seems like [it's always on](https://photos.app.goo.gl/0lvZbEuSrumU8q6d2). Sorry for the crappy video; my phone doesn't seem to want to focus anymore. The switch appears to always conduct current. There's no difference between when it's in series between the battery and the VESC and removing it entirely. Disconnecting the pushbutton from the switch's PCB entirely doesn't appear to change anything.

Has anyone seen this before? Any ideas on what might be going on? I've got an RMA number in case it's defective but I've got the sneaking suspicion I'm just doing something dumb :)
```

---
## \#2 Posted by: Veovis Posted at: 2017-09-18T19:11:02.874Z Reads: 52

```
I had the same issue with mine. From what others have said, when the mosfets are blown the switch will be stuck in the "always on" state, so I'm assuming that's what happened to yours.

Some people have reported switches from DIY that stop working after the first week, but mine never worked out of the box.
```

---
## \#3 Posted by: torqueboards Posted at: 2017-09-18T19:48:04.351Z Reads: 46

```
Yeah, currently the on/off switches have been failing more frequently. They should be perfectly fine but once you get to the point of it always being on it's usually dead.

We're doing final testing on our own custom on/off switch which we should hopefully be releasing soon. If any issues with our new switches we'll warranty them and work towards fixing any issues with them. We're aiming for creating much more reliable parts in the near future across the board. Anyone who currently has a broken DIY switch we'll offer a huge discount on a new switch with warranty. Just let our team know.
```

---
