# How to add Capacitors to Compensate for Long Power Wires

### Replies: 15 Views: 1213

## \#1 Posted by: andchiang Posted at: 2018-04-02T22:33:56.983Z Reads: 216

```
Hello all,

I wanted to know what disadvantages to having long power wires from the battery to the vescs, and why?

And also, is there a way of adding capacitors to the vescs side of the wires to compensate for the long power wires?

What capacitors should I add in what configuration?

Thank you in advance!
```

---
## \#2 Posted by: Sebike Posted at: 2018-04-02T22:47:59.606Z Reads: 215

```
https://www.electric-skateboard.builders/t/add-vesc-capacitors-for-battery-cables-longer-than-12inch-30cm/12506?u=sebike
```

---
## \#3 Posted by: Cobber Posted at: 2018-04-03T01:13:00.612Z Reads: 199

```
https://emperformanceproducts.com/product/ripple-voltage-filter-energy-booster-cap-pack-23500-uf-12s-max-volt-8awg-wire/

or from yge

http://www.yge.de/en/accessories/

many more ready made and diy options out there...

How long are your wires? some of the rc esc manufacturers recommend 1 x additional cap (390uf) per 10cm/4 inches of wire.

Essentially you can't have too much, there is no downside to more except a spark when you connect/disconnect live leads so use a anti spark connector.
```

---
## \#4 Posted by: andchiang Posted at: 2018-04-03T13:07:52.588Z Reads: 167

```
![IMAG1519|281x500](upload://ruBGCZMmOH4sr0uzCFnTXEUmrIF.jpg)
My power wires are the red and black wires running along the board, they're about 2 feet long each. I should've thought about this more before inlaying everything into the board...
```

---
## \#5 Posted by: pat.speed Posted at: 2018-04-03T13:31:40.186Z Reads: 159

```
It’s super easy to make a capacitor bank. I pulled some capacitors out of a car amp. They are rated at 63v 3300uf and I connected 6 in parallel. That should smooth out most voltage spikes for sure
```

---
## \#6 Posted by: BoostedBuilder Posted at: 2018-04-03T13:34:11.620Z Reads: 155

```
Thats beautiful!
```

---
## \#7 Posted by: b264 Posted at: 2018-04-03T20:06:29.937Z Reads: 145

```
[quote="pat.speed, post:5, topic:51015, full:true"]
It’s super easy to make a capacitor bank. I pulled some capacitors out of a car amp. They are rated at 63v 3300uf and I connected 6 in parallel. That should smooth out most voltage spikes for sure
[/quote]

It will definitely do that.  It will make everything better except one thing.  Your antispark will need to be TOUGH and/or have a longer ramp-up time.  I wonder if @Kug3lis might be able to extend the ramp time in his upcoming king kong antispark so we can use more caps?
```

---
## \#8 Posted by: pat.speed Posted at: 2018-04-03T23:25:30.532Z Reads: 132

```
Yeah I’m kinda worried about the little resistor inside the antispark plugs, hopefully as150 bullets will be up to the task
```

---
## \#9 Posted by: andchiang Posted at: 2018-04-04T14:15:37.084Z Reads: 116

```
I've decided to add 3 more 63V 680uf capacitors to each FOCBOX, hopefully this will still be okay for my antispark XT90 and enough to make up for my long power wires.
```

---
## \#10 Posted by: Skunk Posted at: 2018-07-31T01:40:40.676Z Reads: 86

```
Does it make a difference if you run your caps closer to your FOCbox or your battery?
I'm gonna have my boxs in the cnc heatsink up top over my tucks. Probably a foot of cable will be needed.
```

---
## \#11 Posted by: PatRocks Posted at: 2018-07-31T01:48:20.178Z Reads: 82

```
For optimum effectiveness, the capacitor pack should be as close to the esc as possible. The problem with these voltage spikes is the effect they have on the capacitors inside of the ESC. It is those capacitors that additional cap packs are intended to protect.
```

---
## \#12 Posted by: Skunk Posted at: 2018-07-31T01:57:36.372Z Reads: 76

```
So my case probably won't have room inside.
There will be a gap between bottom of case and top of DECK. Would it be safe to mount a pack there?
```

---
## \#13 Posted by: PatRocks Posted at: 2018-07-31T02:00:54.016Z Reads: 79

```
Not sure what you mean, pictures?
```

---
## \#14 Posted by: Skunk Posted at: 2018-07-31T02:32:04.788Z Reads: 74

```
![faab3dd57863ddc809f19cc432cca561bdf7021f_1_313x500|313x500](upload://sg6cX1IQr6YJQpDY3PpDDi2k9VF.jpg)
If I made mounting bolts taller. Could I stuff a cap pack under there?
I guess the real question is how far from focbox is to far. @PatRocks
```

---
## \#15 Posted by: PatRocks Posted at: 2018-07-31T02:50:14.672Z Reads: 70

```
A couple inches is no big deal, i wouldn't worry too much about it. Wherever you put it, it will help at least a little... but again, the closer the better
```

---
