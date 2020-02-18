# WIIceiver dual ESC question

### Replies: 8 Views: 2428

## \#1 Posted by: joren Posted at: 2015-08-29T22:53:01.327Z Reads: 106

```
Hey, when connecting 2 ESCs to the Wiiceiver, do I need to cut one of the power wires?   I've heard from multi-copter guys that you don't want to send parallel BECs to a receiver.  Has this been a problem for the dual motor boards using a Wiiceiver..or the VESC?  I'm concerned with damaging the BECs as well as creating noise.
Thanks!
```

---
## \#2 Posted by: onloop Posted at: 2015-08-30T03:06:43.979Z Reads: 108

```
With Dual VESC it is not an issue as the RX is connected to only the master VESC. With a normal HOBBY RC ESC i think you would want to modify the servo cable so you only get power from one source.

http://www.electric-skateboard.builders/t/vesc-faq-connect-the-nyko-kama-wireless-wii-nunchuck/139/4
```

---
## \#3 Posted by: sl33py Posted at: 2015-08-30T03:33:51.650Z Reads: 106

```
It depends how you connect them.  With a simple "Y" servo connector - then yes i'd remove power from one so you aren't using the BEC from the second VESC to send power to your Rx.

You can hard-wire the VESC to your Nyko - check out onloops link and how-to.  You can also connect dual VESC utilizing the canbus connectors (enables traction control option as well).

HTH - GL!
```

---
## \#4 Posted by: torqueboards Posted at: 2015-08-30T05:35:15.864Z Reads: 97

```
The Wiiceiver is standalone meant for an RC Eboard type build. You can get the parts kit from Austin David and/or purchase the plug & play from me.

A similar wiiceiver is pre-built into VESC (custom code/programming by Ben but with similar features).

Wiiceiver (to run two motors/escs) you would connect to the dual 3 pin ports and/or using a Y connector if no built in BEC/UBEC.

The Nyko Kama & Receiver itself do have issues with connectivity and interference.

Some people as Jacob Bloy and Ben Vedder have worked on customized Nyko Kama & Receiver which use 2.4ghz with Nrf24L01 which makes it much more stable and uses a lot less power.
```

---
## \#5 Posted by: lowGuido Posted at: 2015-08-30T05:53:20.206Z Reads: 85

```
i just cut the middle pin off one of the ESC cables when running 2 ESC's off 1 wiiceiver.
I have connected them both at the same time without major issue, but I like to play it safe.
```

---
## \#6 Posted by: sl33py Posted at: 2015-08-30T05:57:30.168Z Reads: 79

```
Same here.  I had both connected including power from both VESC to my Rx before i remembered to cut one of the power.  The one or two days i rode it with both didn't seem to damage the VESC's or Rx.  Still good to only supply from one if using a simple Y servo cable.

My next dual VESC will be using only one connection from VESC to Rx and then the canbus connection w/ traction control to the second VESC.
```

---
## \#7 Posted by: joren Posted at: 2015-08-30T06:22:14.982Z Reads: 76

```
thank.  I have hobby ESCs, not VESCs.  It seems the consensus is to clip a red wire to be safe.  Safe is the way to go.  

If I may ask a follow up question:  Has anyone encountered problems with multiple Nyko Kama wireless units interfering with each other?  As in if two boards were ridden side-by-side, both controlled with wireless nyko kama wiiceivers? Hopefully they accounted for having 2 plugged into a Nintendo Wii.

Cheers.
```

---
## \#8 Posted by: lowGuido Posted at: 2015-08-30T06:50:13.359Z Reads: 72

```
I have had 4 nyko kama controllers ridden side by side without any issue.
as you said. they are designed to work with nintendo wii so thats 4 players in close proximity.

I have never had more than 4 at once, so that would be interesting..
```

---
