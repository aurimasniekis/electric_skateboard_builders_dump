# Everything bought except batteries,charger and motors

### Replies: 10 Views: 807

## \#1 Posted by: lunasicc Posted at: 2017-07-02T01:40:44.546Z Reads: 114

```
build will be a trampa holypro
dual max6
etoxx direct drive 5:1


i will be running 8s. im wondering what the best setup would be for batteries. i was thinking 2 4s1p in series.
something like this

https://hobbyking.com/en_us/zippy-flightmax-8000mah-4s1p-30c.html?___store=en_us

based off calculations, i could get roughly 24km range from this setup? it seems to good to be true. i see people running massive battery setups that are double or triple the size.
and would i notice a huge difference in higher c rated batteries? would 30c be sufficient?

another question is charging, looking for suggestions on a good double bank charger where i could charge both 4s batteries at the same time.

for motors, i think im going to go with 240kv aps hev. i realize i will have slight cogging from a stop but id like to have the top speed. maybe a 200 or 220kv might be better
thanks for any input!
```

---
## \#2 Posted by: flywithgriff Posted at: 2017-07-02T01:43:14.291Z Reads: 100

```
I'm sure someone with more knowledge will chime in but I do know higher C rating is always better for minimizing voltage sag.
```

---
## \#3 Posted by: wafflejock Posted at: 2017-07-02T03:52:41.605Z Reads: 86

```
That's true but 30C with 8Ah means they're rated for 240A which is pretty high really, when you get large Ah batteries the C rating is usually going to be lower than you're used to seeing on say 3-4Ah packs where you'll see more of the 40-60C or whatever (it's sort of a dumb system from a consumers point of view).
```

---
## \#4 Posted by: Namasaki Posted at: 2017-07-02T05:52:23.531Z Reads: 75

```
@flywithgriff @wafflejock
Your both correct.
It is always better to have the highest C rating possible however 8ah at 30C should work fine however, I would not go any lower than 30C regardless of the capacity.
A good example is the multistar packs that are 10-15ah but only 10C and are known to be rather weak.

Therefore it is my belief that though  C rating x  capacity = Discharge rate, The C rating is the more important factor in the equation.
```

---
## \#5 Posted by: wafflejock Posted at: 2017-07-02T06:27:46.366Z Reads: 68

```
I imagine that could be due to the connections between the cells.  On average you usually have more surface area of layers wrapped in the pack so should get more amperage throughput but I think they always use the same tab sizes regardless of cell size (could be wrong but I've disassembled a few).  Might also have to do with heat build up in bigger packs building up the internal resistance, the chemistry is way beyond me though.
```

---
## \#6 Posted by: lunasicc Posted at: 2017-07-02T06:55:38.277Z Reads: 65

```
good to know. thanks guys. so realistically im not going to notice much of a performance increase compared to a 45-65c pack with a 8ah pack.

any advice on a charger? im currently looking at this one
https://www.amazon.com/gp/product/B00SZ1CBVC/ref=ox_sc_act_title_1?smid=A215PENFG8OL60&psc=1

just hook both packs together in series with xt90's and charge individualy. as a 8s charger is hard to find and expensive
```

---
## \#7 Posted by: Okami Posted at: 2017-07-02T14:32:52.627Z Reads: 56

```
Concerning range, it looks like u might be able to get about 230wh out of 8s lipo at 8ah.

I took 7.8ah as capacity you might get, as i think it is not always good to take everything out of battery, even if it can do it, so some "safe zone" should be accounted for.

As u should know, i think, pneumatic tires are hardly ever as energy efficient as the longboard urethane wheels.

At best, if u had maybe hard pumped 7inch tires, u could maybe expect 15wh/km of consuntion.

Though it looks like 18-20wh might be a better number to go with for pneumatic tire setup.

I dont really have any reference to speed, but i believe the estimates should be somewhat true, if you go faster than 15kph.

So,.in your case, i would expect about 11.5km at close to worst estimate and about 15km of range, if you do happen to have it very energy efficient.

(230wh / 20wh = 11.5km 
230wh / 15 wh = 15.33 km )

So about 13km could be quite good range for such setup.

Though this holds true if nothing has changed to how i make calculations and real world situation (like battery having more than 8ah, for example)

---

For reference, I had a pack with 192 wh of energy (calculated amount) and i was really happy if i could  do 10km, as the real world situation was that i did not charge till 4.2v per cell always, so i probably had less than that and max was about 8km with not fully charged pack.

If you can, i would advise to aim for 15km of range, unless u plan to have swappable packs.

In my experience 8km is not enough, so i now have a pack of 20-25km range
```

---
## \#8 Posted by: Namasaki Posted at: 2017-07-02T15:57:26.841Z Reads: 48

```
[quote="lunasicc, post:6, topic:26561"]
any advice on a charger? im currently looking at this one

  
    amazon.com
  
  
    

UP120AC Duo Dual 2 Port (2x 12Amps, 2x 120Watts, 240Watts Total): LiPo, LiHV, LiIon, LiFe, NiCd, NiMh, Pb AC/DC Balancing Battery Multi-Chemistry Multicharger with 300Watt Power Supply by Ultra Power



LiPo, LiHV, LiIon, LiFe Battery Balance Charge Charge Fast Charge Storage Mode Discharge NiMH, NiCD Battery Manual Charge Auto Charge Discharge Re-Peak Cycle Pb Charge Discharge Battery Memory Battery ...



$89.99
[/quote]


I've owned this charger for over a year now and I can say that it works very well.
```

---
## \#9 Posted by: lunasicc Posted at: 2017-07-02T17:27:40.501Z Reads: 45

```
@Okami thanks, that makes a little more sense. seems a little more realistic. and i actually do plan to have swappable packs, as i will probably be riding with a backpack all the time anyway. id rather have it on me rather than my board for un sprung weight.
@Namasaki, sounds good. i think i will order this. cheapest ive found for it. 


i have a question regarding wiring. i will be using max6 esc so technically i dont have to run a xt90 anti spark loop. but i think its best to anyways just incase i need to disconnect power quickly. i think my wiring will be very similar to the attached photo. with the power switch in the diagram replaced for a xt90 antispark. or should i just use a standard xt90 for the loop because my esc have a on switch? will it matter?<img src="/uploads/db1493/original/3X/0/8/0819780f9776658dee44bf976457eab82d386fb9.png" width="690" height="387">
```

---
## \#10 Posted by: Okami Posted at: 2017-07-02T18:37:37.892Z Reads: 43

```
I think wattmeter needs to go inline with the load (esc and motor)

It is good it comes after power switch, otherwise it would need it's own on/off switch to power it off.

As about the on/off switch on escs. You can leave it in On position and just 'control' power with the main antispark(xt90) switch.

I would say better go with antispark one, as you might get tired of getting sparks if you connect it for power instead of using the car esc's switch.

Though - I cannot really comment on whenever using car escs switch all the time is a good idea or not, maybe @ Nowind could answer this, as he seems to be using some max6 (or max8? ) in a few setups I think.

If you think switch will be sturdy enough not to fail (and it actually looks quite okay to me), then yeh, why not :slight_smile: 

Though I would wait till someone else replies about this as opinions might differ about this

--

As about the power demand and range calculation - I think someone tried to make a calculator for that but then I have to look.

I think NoWind even pushed one of his boards to consume about 40wh/km.. but that was a bit extreme and riding conditions were also a bit harsh :slight_smile:

So.. I think unless you go 40kph all the time, you should get at least these 10km or so, out from that 8s 8000 mah pack, or since you work with NoWind anyways, maybe ask him what he thinks is a good capacity for a pack depending on riding conditions you plan to do.

--

Calculator for battery / other stats here:

http://calc.esk8.today

the only con is, it is still needed to enter wh/km value as Wh/mi, so 29wh/mi is equal to 18wh/km.

Otherwise use google to convert other wh/mi values.
```

---
