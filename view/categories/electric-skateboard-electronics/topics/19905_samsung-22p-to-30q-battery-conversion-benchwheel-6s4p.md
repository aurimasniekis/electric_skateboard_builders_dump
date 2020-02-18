# Samsung 22p to 30q Battery Conversion (Benchwheel 6s4p)

### Replies: 24 Views: 2489

## \#1 Posted by: cradster Posted at: 2017-03-29T11:04:33.874Z Reads: 249

```
Hi, I recently bought a Benchwheel Dual to see if electric skateboarding was for me.  Turns out it very much is my thing and I've pre-ordered a Raptor 2.  In the meantime I'm looking to upgrade the Benchwheel because it's range has really dropped off and I'm thinking it's the battery.

The board currently has Samsung 22p cells in a 6s4p configuration.  Does anyone know of any reason why I couldn't replace the cells with Samsung 30q cells?  I am assuming that the existing charger and hardware will continue to work as expected but would really like to get some feedback before shelling out on 24 * 30q cells.
```

---
## \#2 Posted by: t0m_r1dd1e Posted at: 2017-03-29T21:30:27.827Z Reads: 229

```
You absolutely could, if you're prepared to solder them all up. You'd get a nice bump in total capacity as well.
```

---
## \#3 Posted by: mmaner Posted at: 2017-03-30T00:04:08.246Z Reads: 213

```
I'm no expert on batteries, but from a engineering perspective I don't see any reason why not. The voltage will remain the same, I doubt the BMS cares about the amps, the motors might wear out pretty quick with the extra amps though.
```

---
## \#4 Posted by: cradster Posted at: 2017-03-30T10:38:42.911Z Reads: 203

```
Thanks for getting back to me guys.  I'm waiting to here back from a [company](http://floreat-energies.co.uk) that specializes in custom battery packs. I believe the heat from soldering can be damaging so I'm looking to get them spot welded.

Right, I'm off to buy some cells, hopefully I'll have an update soon for anyone else considering doing the same.
```

---
## \#5 Posted by: t0m_r1dd1e Posted at: 2017-03-30T15:04:16.478Z Reads: 180

```
The BMS DOES care about amp draw (as it's probably fused), but the ESC will only pull as many amps through it as it was originally designed to. It's not that the upgraded battery will push more amps just because it can. The board should feel exactly the same except with more range and possibly less voltage sag.
```

---
## \#6 Posted by: mmaner Posted at: 2017-03-30T16:41:51.565Z Reads: 161

```
[quote="t0m_r1dd1e, post:5, topic:19905"]
The BMS DOES care about amp draw (as it's probably fused
[/quote]

I repeat, the BMS does not care about amps.  Specifically because it is NOT fused.  I know this because I bought one for my kid and I work on it all the frikkin time.
```

---
## \#7 Posted by: t0m_r1dd1e Posted at: 2017-03-30T16:55:05.119Z Reads: 149

```
Fair enough. My mistake. But regardless, the ESC isn't going to pull more current than it originally did.
```

---
## \#8 Posted by: cradster Posted at: 2017-04-20T08:37:56.459Z Reads: 141

```
Quick update for anyone interested. I assembled a new battery pack using new Samsung 30Q cells and can confirm that everything is working great.  I've used it for a couple of weeks and it performs better than when it was new.  

As expected every area of performance is improved, hill climbing, acceleration, range, top speed.

I haven't had to change any other components and the charger still works, although it takes a little longer to charge from flat which is to be expected.
```

---
## \#9 Posted by: Technotron Posted at: 2017-05-20T16:49:12.650Z Reads: 133

```
Very cool! I have the same board and am also looking for an intermediate solution to get a bit more consistency of the 1800w dual. Their shop told me my board would have the 25r Samsung batteries but it's still using the 22 ones... kinda pissed about that!

How much did you end up paying for the custom battery pack? Did you provide the cells to them? Lastly, would it be OK to ask for your order no. from these guys? Would make it a lot easier to explain to them what I am looking for :slight_smile:

Cheers man!
```

---
## \#10 Posted by: bisoe Posted at: 2017-05-21T01:10:30.174Z Reads: 130

```
Great!! I got the same e board with same probelem..I dont know alot about the technical stuff..
but is it possible to connect a E-bike battery 36v 8.8ah ICR18650-22P in chain with my current battry on my benchwheel?

(link) https://kmdbattery.en.alibaba.com/product/60527001791-803450512/E_bike_battery_36v_8_8ah_Samsung_ICR18650_22P_ebike_battery_for_36v_250W_motor.html
```

---
## \#11 Posted by: cradster Posted at: 2017-05-23T00:43:28.584Z Reads: 130

```
I ended up buying the cells, a spot welder and then built the pack myself.  I'd made a few enquiries and it was going to cost around 250GBP to get a pack made by a company so it worked out cheaper DIY.

Batteries:
https://www.fogstar.co.uk/products/samsung-30q-3000mah?variant=33334816199

Spot Welder:
http://www.ebay.co.uk/itm/UK-Shipping-18650-Battery-Charger-800-A-0-1-0-2-mm-36V-60A-788H-Spot-Welder-/152395706530?hash=item237b7df0a2:g:IXgAAOSwopRYecNg

Pure Nickel Strip:
http://www.ebay.co.uk/itm/1m-Pure-Nickel-Plated-Strip-Tape-Belt-for-18650-Battery-Welding-0-15-x-27mm-/252950497384?hash=item3ae5064868:g:THgAAOSwCGVX-RJi

Insulators:
http://www.ebay.co.uk/itm/20pcs-cardboard-18650-battery-Electrical-Insulators-Insulating-Adhesive-Paper-/132122770215?hash=item1ec3217b27:g:YPIAAOSwTM5Yw9Mk

There are plenty of YouTube videos showing you how to put a battery pack together.  The benefit of DIY is I've now got the option of selling the Spot Welder on ebay and getting 100 pound back :o)
```

---
## \#12 Posted by: cradster Posted at: 2017-05-23T00:47:49.621Z Reads: 118

```
bisoe I honestly don't know.  The OEM battery is 6s4p which outputs around 24v, 36v might be to much.
```

---
## \#13 Posted by: Technotron Posted at: 2017-05-26T19:59:50.976Z Reads: 112

```
Thanks, much appreciated. I went DIY as well!
```

---
## \#14 Posted by: darkkevind Posted at: 2017-06-20T14:57:46.277Z Reads: 89

```
Ouch! You paid a lot for those batteries! :confused:

https://eu.nkon.nl/samsung-inr-18650-30q-3000mah.html
```

---
## \#15 Posted by: SpeedSloth Posted at: 2017-06-20T15:37:40.006Z Reads: 87

```
How often are they out of stock? This is the best price I've seen :slight_smile:
```

---
## \#16 Posted by: darkkevind Posted at: 2017-06-20T15:38:44.135Z Reads: 86

```
True, but they're back in stock NOW!! lol

Oh I've just re-read your message. Yeah, quite often out of stock. They came back in stock today :slight_smile:
```

---
## \#17 Posted by: sl33py Posted at: 2017-06-20T15:55:21.834Z Reads: 86

```
@cradster - kudos man for diving in and DIY the battery!

For the next person who finds this and wants to duplicate, i'd recommend one of the arduino spot welders over the ebay one linked.  Simple and less $.  You have to use a car battery and a bit of fiddling for settings, but likely similar to the 788 welder - until you find setting that gives you a good weld through your thickness of nickel strip chosen.  You can build your own and recommend upgrading the FETs and adding TVS and Shottky diodes for longer life.  Search the forum here for arduino spot welder and you'll find several threads.

Nkon is great for prices, but super slow shipping sometimes...

HTH - GL all!
```

---
## \#18 Posted by: darkkevind Posted at: 2017-06-20T20:16:09.323Z Reads: 78

```
I'm going down this route for a cheap spot welder for my pack. No need for these expensive pre-built ones if you're careful.

https://youtu.be/Gk3vrKc4Y1w

Hacky, but it works, I've tried it.
```

---
## \#19 Posted by: sl33py Posted at: 2017-06-20T21:20:51.609Z Reads: 72

```
@darkkevind - hell no.  When i buy a few hundred dollars in new 18650 cells i'm not melting contacts "carefully" with a car battery.

You can do you, but i'd prefer not to pierce the battery and have bad things happen because i wasn't careful enough.

The nicer store-bought welders like the 788 listed, and arduino spot welder use timed pulses so you can consistently control the weld.
```

---
## \#20 Posted by: darkkevind Posted at: 2017-06-20T21:23:12.013Z Reads: 68

```
Haha! Chicken! :stuck_out_tongue: 

I'll be modifying my setup to include a solenoid relay switch to control the pulses... no risk :wink:
```

---
## \#21 Posted by: sl33py Posted at: 2017-06-20T21:28:34.154Z Reads: 71

```
HA!  true.  I tend to treat high amp and high voltage systems with some caution.  

When you weld together a pack of 12s in 3/4p and have 60-100Amps current - i'll stick with the arduino spot welder i built from pcb and BOM.  It was a fun project and i can control the timing in milliseconds.  Not prius/tesla car volts/amps - but more than i want to lick my fingers and touch contacts!
```

---
## \#22 Posted by: darkkevind Posted at: 2017-06-20T21:31:41.086Z Reads: 72

```
It's ok because if you do it right, the amps just go straight from one copper electrode, through the nickel and the battery metal and back out the other electrode, not harming anything inside the battery.
```

---
## \#23 Posted by: cradster Posted at: 2017-06-20T21:51:40.512Z Reads: 73

```
hehe i sure did but I wanted them quick ;o)
```

---
## \#24 Posted by: darkkevind Posted at: 2017-06-28T19:26:58.145Z Reads: 68

```
So... I just made this....

https://youtu.be/tlm-C_fiGS8
```

---
