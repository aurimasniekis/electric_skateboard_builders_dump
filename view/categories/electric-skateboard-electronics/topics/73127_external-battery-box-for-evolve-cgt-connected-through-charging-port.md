# External battery box for Evolve CGT (connected through charging port)

### Replies: 3 Views: 398

## \#1 Posted by: bohacjan Posted at: 2018-11-02T13:35:54.499Z Reads: 74

```
I would like to DIY an external battery pack for my Evolve CGT (currently 10s5p SonyVT6), that I should be able to **connect through the regular charging port**.

The point is to increase the range for longer rides (just put box on board between legs, strap it and connect to charge port). It will be only used on long trips.

I am pretty novice to electronics, so I am looking for any helpful advices from you guys. My idea is to use 6S Lipo battery as power source, then a step-up converter to put 42V and 3/4Amps on output.

Sofar I have bought [this converter](https://www.aliexpress.com/item/900W-DC-to-DC-Power-Converter-High-Precise-Control-Boost-Converter-Voltage-Step-Up-Converter-Module/32870031438.html) and a few 5.5x2.1 / 5.5x2.5 connectors (dont know which one is correct for my Evolve). Connectors are on the way and the converter was delivered just today.

Still need to find some suitable case for the converter and battery (still not sure about the size of the battery, will get probably the cheapest per/Wh 6S battery from hobbyking).

So guys what are your thoughts about this?

FYI i am not able to put bigger battery inside the board and don´t want to cut or drill in that awesome carbon deck.
```

---
## \#2 Posted by: Skunk Posted at: 2018-11-02T13:41:53.418Z Reads: 64

```
https://www.electric-skateboard.builders/t/range-extender-plugged-into-charge-port/64327?u=skunk

Here ya go
```

---
## \#3 Posted by: marsrover001 Posted at: 2018-11-02T16:49:28.795Z Reads: 50

```
The closer your input voltage is to your target voltage, the more amps you can draw.

For example when I tried 6s > 15s (onewheel) I could only charge at 1a. To make voltage you draw more amps, and the inverse is also true.

Now the easy solution would be get another 6s battery, make it 12s and off you go. Well the converter you have is a boost converter, it can't step 12s down to 10s. (I've tried) You can put 2 6s batteries in parallel but you still run into the issue of the converter not being powerful enough to boost that high.

But I do see you are still shopping for a battery, so consider buying 2 5s batteries and putting them in series. The converter will be most happy converting 42v to 42v, and will just regulate amps. You could direct connect, but that will only work if you connect a fully charged booster pack with a fully charged board and let them discharge together. The inrush current will be too high if you plug in a booster pack to a low or dead board.

Now the evolve BMS does limit current, but it's also known to be a cheap POS and is IMPOSSIBLE to get anywhere. So don't risk it and keep a controller on there to limit current.
```

---
