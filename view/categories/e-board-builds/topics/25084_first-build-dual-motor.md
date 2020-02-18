# First Build! &#124; Dual Motor &#124;

### Replies: 13 Views: 1212

## \#1 Posted by: DreJ Posted at: 2017-06-11T05:08:46.682Z Reads: 196

```
Hi guys this will be my first build so some heavy critiquing would be appreciated. 

[2x Motor](diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/)
[Dual Motor Mechanical Kit](diy-electric-skateboard-kits-parts/torqueboards-dual-motor-mechanical-kit/)
[2x Vesc](diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/)
[2x 5000mAh 5S 25C LiPos](https://hobbyking.com/en_us/turnigy-5000mah-5s-25c-lipo-pack.html)
[Remote Controller and receiver](diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-nano-remote-controller/)
Charger (No idea, help appreciated)
[Potential Deck?](http://www.newtons-shred.co.uk/bustin-maestro-pusher-longboard-london.html)

And I believe the only other things I'll need are these connectors. [1](https://hobbyking.com/en_us/xt90-battery-harness-10awg-for-2-packs-in-series.html) - [2](https://hobbyking.com/en_us/xt90-battery-harness-10awg-for-2-packs-in-series.html). **Will I need any other connectors if I'm not planning on soldering?**

I'm connecting the two batteries in series so that's what I use [these](https://hobbyking.com/en_us/xt90-battery-harness-10awg-for-2-packs-in-series.html) connectors for. **Do I only need one?**

Using [this calculator](http://calc.esk8.it/) I get a speed of 30MPH. I can't get this [range calculator](http://calc.esk8.it/) to work if I leave number of parallel cells at 0 though.

I was told by a user on this forum that 25C batteries definitely wouldn't be powerful enough and would lead to overheating and I would need at least 40C. Dexter from DIYelectricskateboards.com said 25C works fine. Any help?

I'm assuming there is space for two inputs from each VESC on the receiver? I don't need any adapters or connectors for that do I?

**CHARGING SOLUTION:** I have no idea how I'm planning on charging the batteries. What would work best to charge them both at the same time? **Preferably** without having to remove them. (Even though I still have to check on the liPos). Any help would be appreciated.

Also please list your preferred mounting solution of the electronics. So far all I have is the Tupperware method. Is this the preferred method for everyone?
 
Also is this a reasonable price to pay for the deck? And will it work well in terms of space for my electronics? Should I look for a cheaper/different deck? 

One thing I'm not sure about is in the dual mechanical motor kit which I listed, are the plates for mounting the trucks correct? Will these trucks and plates work with the deck?

Also I was told that the older version of this controller and receiver had connectivity issues. Has anyone tried the updating one that I linked?

Also will I need an on/off switch, they are quite expensive off DIY. How do you install them? Where do you plug it.

Will I need a voltage indicator?

**Most Important**: Will I need to buy literally ANYTHING else which I have not linked here?


Finally, what do you think of the build? Good? Bad? Advice? 


Thanks for the help guys <3
```

---
## \#2 Posted by: IsTalo Posted at: 2017-06-11T10:33:09.313Z Reads: 159

```
First, of course the range calculator is not working, Mah*0=0, put one if you have put 5000mah.

Man, I don't know how much does that motors consumes, but the current will be divided between them, so, 25C*5A= 125A, is that enough to your build?

Reading your post is clearly that you dobro studied how to make a esk8, but I will continue helping you!

The Anti-Spark switch is necessary, unless you want to solder an make a Loop key.

Tell me, how would you know your battery voltage without something to tell you? You need a Lipo 48v porcentage display.

Charging, go with a BMS, seriously

And man, there is a super low chance to you don't solder anything, somethings came without any connector, so go at the local HobbyStore and you're done
```

---
## \#3 Posted by: DreJ Posted at: 2017-06-11T11:03:57.356Z Reads: 144

```
Hi. Thanks for the reply.

How can I tell if 125A is enough for my build?

Here's the information for each motor:

* Max Power: 2500 Watts
* Max Amps: 80 Amps
* Max Volts: 12S

Does this tell you anything? What calculation do you use. Will you be able to tell me how many amps I need for my build?

Yeah man I've got all the connectors I need I think:

* Vesc can busk connector
* XT90 Parallel Connector
* XT90 Series Battery Harness 

Is that all I need?

If I go with [this on/off switch](diy-electric-skateboard-kits-parts/electric-skateboard-on-off-power-switch/), where do I plug it in? Do you have a diagram or tutorial?

As for charging, how do I know which BMS charger will go with my batteries?
```

---
## \#4 Posted by: IsTalo Posted at: 2017-06-11T11:29:48.408Z Reads: 124

```
Lets Begin, your specs are 80A per motor, but the current will be divided, so let's say that in a super hill that motors will consume 80A both, so 125A is enough. 

I do not think you need a parallel connector, you need a series connector and some Xt-90

I used to have the diagram, but I deleted it from the phone, but it is easy, between the Bms and the Vesc

You need a 10s Bms, can be anyone that can charge at least 5A, so you can charge your batteries in one hour. Search for Vlad Pomaev (I think is Pomaev) Bms tutorial on youtube, or something about Bms in the forum
```

---
## \#5 Posted by: DreJ Posted at: 2017-06-11T11:51:26.966Z Reads: 121

```
So at the moment all of the components are good the way they are? Nothing needs changes correct?

Don't I need a [Dual Vesc XT90 Parallel Connector](diy-electric-skateboard-kits-parts/dual-vesc-xt90-parallel-connector/) so that I can connect both vescs into the [XT90 Battery Series Harness](https://hobbyking.com/en_us/xt90-battery-harness-10awg-for-2-packs-in-series.html)?

Like this [schematic](https://gyazo.com/676575c8fd0787214f3467a3622ea23f) I made? So are those three the correct connectors. _(I made a mistake in the schematic. I put a wire from each vesc to the receiver but there should only be one.)_ 


Any idea where I can find the diagram you are talking about? Also the battery series harness that I linked says it can handle over 90A. Will that be fine?

Is [this](https://www.youtube.com/watch?v=jxHQjlHv1y4) the tutorial from Vlad you were talking about? This looks so complicated. Is there any simpler methods I can do?


Is there a youtube tutorial including a percentage display and an on/off switch? All of the tutorials I can find on youtube don't use an on/off switch or a percentage display.
Thanks for the help.
```

---
## \#6 Posted by: Blucas Posted at: 2017-06-11T12:18:09.074Z Reads: 103

```
I'm new to all this so what I say may not be correct, but from what I've gathered, an on/off switch is just an anti-spark switch (maybe :stuck_out_tongue:)
```

---
## \#7 Posted by: DreJ Posted at: 2017-06-11T12:27:28.360Z Reads: 110

```
So at the moment all of the components are good the way they are? Nothing needs changes correct?

Don't I need a [Dual Vesc XT90 Parallel Connector](diy-electric-skateboard-kits-parts/dual-vesc-xt90-parallel-connector/) so that I can connect both vescs into the [XT90 Battery Series Harness](https://hobbyking.com/en_us/xt90-battery-harness-10awg-for-2-packs-in-series.html)?

Like this [schematic](https://gyazo.com/676575c8fd0787214f3467a3622ea23f) I made? So are those three the correct connectors. _(I made a mistake in the schematic. I put a wire from each vesc to the receiver but there should only be one.)_ 


Any idea where I can find the diagram you are talking about? Also the battery series harness that I linked says it can handle over 90A. Will that be fine?

Also can I just use [this IMAX B6?](https://hobbyking.com/en_us/imax-b6-50w-5a-charger-discharger-1-6-cells-genuine.html)

**One more thing. My battery's discharge wires are bullet connectors as you can see [here](https://hobbyking.com/en_us/turnigy-5000mah-5s-25c-lipo-pack.html). Will these bullet connectors fit into this [XT90 harness?](https://hobbyking.com/en_us/xt90-battery-harness-10awg-for-2-packs-in-series.html)**


Thanks a lot for the help man.
```

---
## \#8 Posted by: IsTalo Posted at: 2017-06-11T12:36:05.153Z Reads: 105

```
Yeah it's correct, one servo cable to the reciever, and you can use the imax b6 but charge the batteries in parallel, no in series, Im going to travel now, so Maybe I answer late
```

---
## \#9 Posted by: Davey Posted at: 2017-06-11T12:43:14.244Z Reads: 106

```
No the bullet connectors won't fit properly into XT90 I guess
```

---
## \#10 Posted by: DreJ Posted at: 2017-06-11T13:02:25.664Z Reads: 100

```
It will with [these](https://hobbyking.com/en_us/hxt-4mm-bullet-to-xt90-battery-adapter-2pcs.html) right?
```

---
## \#11 Posted by: Davey Posted at: 2017-06-11T13:27:48.116Z Reads: 98

```
Yeah. Both have 4mm bullet connectors, so should work. If you want to connect them permanently you could simply solder the wires.
```

---
## \#12 Posted by: abenny Posted at: 2017-06-11T14:31:53.731Z Reads: 91

```
youll also need a male to male servo cable to connect your controller to the vesc
```

---
## \#13 Posted by: DreJ Posted at: 2017-06-12T06:32:12.735Z Reads: 74

```
Instead I can just go with [this](diy-electric-skateboard-kits-parts/) 4mm-hxt-series-connector/ 4mm HXT series harness right? That way it would plug straight into the batteries, then my on/off switch end would be 4mm HXT as well and the other end would be XT90 so it can connect to my parallel XT90 dual vesc connector. Sound alright?
```

---
