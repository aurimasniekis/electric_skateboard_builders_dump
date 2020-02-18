# Charging a 10s2p setup with a balance charger

### Replies: 4 Views: 666

## \#1 Posted by: wheinrichs Posted at: 2017-12-19T12:26:43.072Z Reads: 98

```
Hi again,

I bought a bunch of my set up last night and now I'm getting into the wiring trying to figure out what my plan is. I've been reading around and have decided that (for now) I'm going to stick with a balance charger as opposed to a BMS. But that leads me to a few questions I was hoping someone could help me out with:

1. I have 4 of these [batteries](https://hobbyking.com/en_us/turnigy-battery-5000mah-5s-20c-lipo-pack-xt-90.html) and am wondering what the best way to charge them is. I've read that a lot of people recommend the IMAX B6 charger but from what I understand (which may be incorrect) that only supports a 5s battery. So to me that means I would have to charge all  batteries separately (which sounds like a nightmare). So how should I got about charging these correctly and easily?

2. Are there any safety features that are typically built into the electronics on the board? After I get this balance charger figured out I'll throw together a preliminary wiring schematic.

Thanks for all the help!
```

---
## \#2 Posted by: Der6FingerJo Posted at: 2017-12-19T12:49:21.984Z Reads: 92

```
Hi there!
 You can charge the batteries in parallel if you are careful. That means you have to check if the individual cells of all batteries are within ~0.02V to each other. But that would still take awfully long as the imax b6 only has 50W of output (correct me if i'm wrong) and would need 10 hours to charge the whole 20Ah. 

My recommendation would be an ISDT charger. They come with higher wattage for reasonable prices and i've been using the 500W one for a while now. Only thing is that you would need a power supply for them, which can be cheaply diy'd using an old server supply from Dell or HP and modding it to always put out 12V.

 That gives you around 300 Watts usable with the ISDT Chargers, if you would want the full 500W output, you would need 2 of those supplies in series for 24V output.
```

---
## \#3 Posted by: rojitor Posted at: 2017-12-19T14:33:43.104Z Reads: 72

```
The best way is a harness. You can connect series and parallel in the blink of an eye.
[https://youtu.be/tYaquShV2r4](https://youtu.be/tYaquShV2r4)

The imax will do......but it is really slow for 4 lipos at the same time.
Look for more amps. 200w charger at least.

If you are in usa this guy can help you. 
[http://lipoconnectionsolutions.com/main.sc](http://lipoconnectionsolutions.com/main.sc)

He has some chargers and makes custom harnesses.
```

---
## \#4 Posted by: bimmer Posted at: 2017-12-19T18:42:14.077Z Reads: 54

```
Honestly you could have gotten a 10S2P battery with charger for 150$ made of Samsung 25R cells. 

As for safety features I use a properly rated bms or for cheapet setups I use these.
<img src="/uploads/db1493/original/3X/a/7/a78076a0f702ef85090e949a74bcc066a0fe9fe1.jpg" width="281" height="500">
<img src="/uploads/db1493/original/3X/4/1/41fb38f089db43bb97b9f97219b053bdf1e54ca4.jpg" width="281" height="500">
```

---
