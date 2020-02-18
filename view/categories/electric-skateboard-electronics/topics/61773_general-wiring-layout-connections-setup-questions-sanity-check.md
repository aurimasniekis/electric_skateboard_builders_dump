# General wiring/layout/connections/setup questions/sanity check

### Replies: 7 Views: 240

## \#1 Posted by: birdus Posted at: 2018-07-13T15:38:26.796Z Reads: 61

```
I think I've got the basic layout of my setup, but I have a question or two and just want an extra set of eyes double-checking what I'm thinking.

Let me make one thing clear before beginning, so as to remove some confusion/complexity from the conversation. I know there are two schools of thought regarding a BMS (Battery Murdering System?). I'm using brand new, high quality batteries. I'm never going to charge up to 4.2 volts nor drain past about 3.6 volts. I'm not going to use a BMS. I'm aware of the various possible issues, but that's my choice.

(Second picture down is a little closer up shot.) 

So, battery on the right outputs into an on/off switch. Where I solder the connector to the on/off switch input (loose in photo), I'll also add a small set of wires going to the XLR connector for charging the battery pack.

Output from the on/off switch (loose connector shown in photo) will feed into a splitter which will distribute the power to 2 VESCs. I'll wire the white wire from my voltage indicator into that hot battery wire (red) when I add the connector so that when I turn on the power switch, I'll get a voltage indicated. The red for the voltage indicator will get 3.3V or 5V from a VESC and I guess its black can go to the other battery wire or to a GND on the VESC (I'd like feedback/confirmation on that).

The 2 VESCs will plug into the splitter for power and the motors will plug into the VESCs.  told me that any of the three wires from the motors (black/blue/yellow) can plug into any of the three black bullet connectors coming out of the VESC. That seems odd to me. Any feedback?
![20180713_070246|690x270](upload://Ae07wA8mB9yxCYbiO0u0CDt8kcO.jpg)

I ended up with several male-to-mail connectors (for some reason). I think I'll use one of them to connect the red (and maybe black) to a 3.3V or 5V and a GND from a VESC to power the voltage indicator.
![20180713_070122|690x388](upload://p9xeciOkAi5zqwEbOyz1wDpwg6W.jpg)

The CAN bus connector will plug into both VESCs so they can coordinate. I believe it plugs into the white connector in the center at the top. They both have 4 pins.

For some reason, I have 2 VESC sensor wires. I don't think I need them. The motors have sensor wires coming out of them. I think they will plug in to the white connector in the upper left, underneath the large, red wire.

I believe the two white connectors at the bottom of the VESC (6 pins each) are unused. They have available 3.3V, 5V, and GND. That's where I thought I might plug in the male-to-mail connector for the voltage indicator.
![20180713_063442|690x388](upload://glohjt6pfKktMklAdYMr3Fxp20C.jpg)

How does the receiver hook into a VESC? I think I'm missing the wire for that.
![20180713_070317|690x421](upload://uwDPkdTVmVySMmWEEug5VQx9fbS.jpg)

Although I have a few gaps to fill in (with assistance from you all!), I think I've covered all the components and connections.

Thanks!
Jay
```

---
## \#2 Posted by: wafflejock Posted at: 2018-07-13T17:33:54.091Z Reads: 45

```
The VESC male to male 3 pin JST is meant to hook between the receiver and the VESC (3 pin connector at the edge of the VESC (bottom left in the close up picture above) you'll need to snip out the heatshrink a bit around the 3 pins (exacto knife works well).  The bind port at the bottom (of the receiver) is usually used when initially binding the transmitter to the receiver, typically you will have a loop on a 3 pin connector that connects the far left pin to the far right pin (GND to signal).  The middle pin on servo connectors is the 5V so it's hard to mess them up basically if you flip it around 180 you end up with swapping signal and gnd but you can't easily reverse polarity (send 5V into gnd).  You'll need to follow the instructions for your transmitter/controller to get it into binding mode (usually some button you hold down while powering it up).

Believe in most cases channel 1 is the throttle channel and channel 2 is the steering channel, but no harm in trying each really so long as you don't short the power coming from the VESC to the receiver or reverse polarity (hard to do as explained above) you should be fine.

The three pins are 5V GND and Signal, power comes from the VESC to supply the receiver with power to turn on and the signal wire is used for sending data/signal back to the VESC.

---

Side note it looks like a 12S1P battery this might be fine if you are light and not climbing hills you might not stress out the cells too much but would be curious how that works out for you for the most part people go with 3P or more when using 18650 cells since typically they have max discharge around 20A a piece.  You can see the realtime data while connected over USB but would suggest grabbing a metr module or a regular bluetooth module and using ackmaniac firmware to get telemetry data.
```

---
## \#3 Posted by: b264 Posted at: 2018-07-13T17:46:34.737Z Reads: 45

```
[quote="birdus, post:1, topic:61773"]
several male-to-mail connectors
[/quote]

[quote="birdus, post:1, topic:61773"]
male-to-mail connector
[/quote]

I fail to understand where mail fits-in here.
```

---
## \#4 Posted by: birdus Posted at: 2018-07-13T17:50:48.733Z Reads: 47

```
Damn muscle memory.
```

---
## \#5 Posted by: birdus Posted at: 2018-07-13T18:03:10.926Z Reads: 42

```
Okay. I see the loop. So, I'll plug that in to channel 4 for pairing, then after that, use a male-to-male connector from channel 4 of the receiver to the three long pins on the VESC for normal communication. I just took a look at the instructions that came with the receiver. It says something about switching on the receiver for pairing. I'm guessing applying power to the VESC will provide electricity to the receiver, so I'll pretty much need to have everything hooked up to do the pairing. However, if I have the loop installed instead of the male-to-male connector, how will the receiver be getting power for pairing?

There is a bind button on the transmitter.

(I bought these from , if that helps.)

I'm actually making 6 battery packs like that one which I will be connecting in parallel. :slight_smile: I've read of a number of people over on endless-sphere.com who aren't using a BMS and are getting very good results (i.e., packs are staying in balance). That's the route I'm going, but I'm getting some criticism on my build thread [here](https://www.electric-skateboard.builders/t/no-clever-name-build-dual-6374s-12s6p-homemade-deck-superflys-218mm-trucks-custom-machined-parts-carbon-fiber), so I'm going to revisit my pack design. Right now, however, I'm in a bit of a rush to get the board done for a trip in a week, which will last a week. I'll revisit that issue when I get back.

Thanks for the tips on acquiring metrics.

Jay
```

---
## \#6 Posted by: wafflejock Posted at: 2018-07-13T18:56:28.512Z Reads: 27

```
Yah think you mis-typed/spoke there but will want the bind loop on the 4th slot marked B on the receiver and will want the male to male in slot 1 on the receiver.  You're correct though you'll need to power the VESC to get power to the receiver, alternatively you can use any other 5V DC source for getting power into the receiver (bench power supply, buck converter, 3 (or 4) AA 1.5V batteries in series would probably work) but easiest is probably just to power the VESC since you'll need to do that soon enough anyhow.
```

---
## \#7 Posted by: birdus Posted at: 2018-07-13T19:25:10.269Z Reads: 26

```
Thanks for giving me the benefit of the doubt. It actually just didn't click. Now it does. Male-to-male on slot 1 over to the VESC. Add the loop on 4 for initializing, then ditch it (so to speak).

Thanks!
Jay
```

---
