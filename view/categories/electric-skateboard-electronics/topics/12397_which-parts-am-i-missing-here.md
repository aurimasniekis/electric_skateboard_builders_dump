# Which parts am I missing here?

### Replies: 14 Views: 729

## \#1 Posted by: dedinski Posted at: 2016-11-03T16:11:40.503Z Reads: 107

```
Hey guys,

Thanks for taking your time to check this post out. Well I ordered the stuff from the photo, expecting it would all come ready for assembly and the hard part would be to set up the VESC. 

Turns out Im missing parts for connecting the motor and battery directly to the Enertion <img src="/uploads/db1493/original/3X/0/3/03f94640fa6683d4d1747d9fe8a05135120394c6.jpg" width="375" height="499">VESC. I am definitely not an electrician, so I also dont know how to parralel my batteries. 

If you can help, please do!
```

---
## \#2 Posted by: NickTheDude Posted at: 2016-11-03T16:32:04.073Z Reads: 100

```
Thats a male XT90 connector on your VESC, and male 4mm bullets on your motors. You are going to have to solder female 4mm bullets on to your VESC.

Since you have 3S batteries, I'm assuming you want to combine them to make a single 6S battery. To do this you need to connect them in series. You can either make your own series harness, or buy a connector from hobbyking.

https://hobbyking.com/en_us/xt90-series-adapter-1pc.html

Then you are going to have to cut the connectors off your batteries, and solder on male XT90s.

Plug the adapter into the VESC, then plug the batteries into the adapter, then plug the 4mm bullets into each other and your circuit should be good to go. 

However, this has nothing to stop the spark from occuring when you connect the circuit. You may want to buy some sort of antispark switch or make a loop key.
```

---
## \#3 Posted by: rpn314 Posted at: 2016-11-03T16:32:22.923Z Reads: 92

```
At the very least you're missing bullet connectors and it looks like you'll need xt90 or xt60 (can't tell from the picture) to connect the batteries to the VESC.. I think the turnigy sk3 motors have 4.5mm bullet connectors.

To hook in parallel red connected to red, black connected to black, and then red connected to black on the VESC. Though if you only have those two batteries, were you planning on connecting them in parallel or series? From the picture it looks like that's the 4s Zippy 5000's and connecting them in parallel I don't think will work for you. Series however would give you an 8s pack which would work. To do that, The black on one pack connects to the red on the other, and then the remaining black and red go to the vesc.

Edit: I'm apparently a slow typer. @NickTheDude beat me to it and looks like he knows better :slight_smile:
```

---
## \#4 Posted by: mattdig Posted at: 2016-11-03T16:44:01.219Z Reads: 85

```
I'm pretty sure the VESC has an XT-60 on it (mine does).
```

---
## \#5 Posted by: NickTheDude Posted at: 2016-11-03T16:44:53.349Z Reads: 78

```
My bad, it could be XT60 instead, it should say on the plug itself.
```

---
## \#6 Posted by: dedinski Posted at: 2016-11-03T17:12:52.151Z Reads: 72

```
Great save in the last second! I was already about to buy the XT90. Thanks for your replies. 

If I was to buy 2 more batteries (for 12S)... 

I would need: 

1. change all the battery wires to XT60 male (so 4x)
2. 2x series adapter
3. 1x paralel adapter

...and I asume i would connect the circuit in that order from the battery to vesc?
Can you advise me which antisparkswitch to get, where to insert it in the circuit and also where do i put the battery life meter. 

Im really lost on the bullet connectors, I ve never soldered some before...Any suggestions on that?

Again, thanks for all your trouble!
```

---
## \#7 Posted by: TarzanHBK Posted at: 2016-11-04T11:11:57.634Z Reads: 46

```
there is the 245kv motor in your picture, so you´re not able to run it at 12s with the vesc.
245kv and 9s max
```

---
## \#8 Posted by: dedinski Posted at: 2016-11-04T12:10:43.745Z Reads: 46

```
And for this setup, do I need an antispark switch and which one should I get?
```

---
## \#9 Posted by: dedinski Posted at: 2016-11-04T12:20:18.266Z Reads: 47

```
I would really like a suggestion on which antispark I would need. I found this, but seems a bit expensive?

diy-electric-skateboard-kits-parts/electric-skateboard-on-off-power-switch/
```

---
## \#10 Posted by: mountainboardlover69 Posted at: 2016-11-04T12:30:05.855Z Reads: 42

```
no just a antie spark xt90 anti spark key
```

---
## \#11 Posted by: TarzanHBK Posted at: 2016-11-04T12:53:04.798Z Reads: 40

```
you can choose between a simple xt90s loop key or an vedder antispark swich like the one you linked (diy´s is not exactly an vedder, but it works the same way ;))
```

---
## \#12 Posted by: treenutter Posted at: 2016-11-04T15:06:16.217Z Reads: 33

```
[quote="NickTheDude, post:2, topic:12397"]
Then you are going to have to cut the connectors off your batteries, and solder on male XT90s.
[/quote]


@dedinski it is critical to keep the stripped battery wires from touching each other. Watch youtube videos about soldering connectors to your battery. It's not that difficult, but you need to know the essentials.
```

---
## \#13 Posted by: NickTheDude Posted at: 2016-11-04T15:13:38.056Z Reads: 36

```
THIS A MILLION TIMES. I was complete soldering noob a few months ago (still pretty much am). I made that mistake and welded my scissors to the batter pack...
```

---
## \#14 Posted by: mountainboardlover69 Posted at: 2016-11-07T09:39:23.028Z Reads: 28

```
but how i mean like
```

---
