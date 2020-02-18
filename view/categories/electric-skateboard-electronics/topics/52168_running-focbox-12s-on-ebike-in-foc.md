# Running Focbox 12S on ebike in foc

### Replies: 15 Views: 1081

## \#1 Posted by: district9prawn Posted at: 2018-04-13T16:10:07.879Z Reads: 212

```
Hi all, first post :grinning:

I've recently started using the focbox on my ebike with 12s battery. I read a lot of threads about how lots of people killed their vesc with 12s and foc. 

On my ebike though, erpm is lower than what most of you guys use. Four pole pairs and peak rpm around 9000. On the road I am usually at less than 7000 so less than 28k erpm. Also I don't use regen so I can't overspeed and fry anything while coasting down a hill. 

Do you reckon this usage will be ok for the esc long term?
```

---
## \#2 Posted by: FredrikHems Posted at: 2018-04-13T16:16:02.176Z Reads: 206

```
There is always a small risk with vesc’s as I see it, but you should be all good. :grinning: @Deckoz is running 13s foc, with fairly high E-RPM
```

---
## \#3 Posted by: Acido Posted at: 2018-04-13T16:18:09.813Z Reads: 202

```
I would some other ESC because the main thing to choose vesc over any other is smooth brakes(needed for eskate), others should have the same settings to edit, deliver more amps on a higher voltage.

Check out some other options
```

---
## \#4 Posted by: Battosaii Posted at: 2018-04-13T16:20:16.942Z Reads: 188

```
is @Deckoz  running FOC at 13s?  

btw from my understanding there is no ERPM limit in FOC thats only a BLDC thing.

ive been wanting to try FOC for a while now but im afraid of my 12s screwing up my focboxs
```

---
## \#5 Posted by: Deckoz Posted at: 2018-04-13T16:20:26.009Z Reads: 179

```
There are some running 14s FOC on ebikes... As on a bike you don't use Regen braking since you have disc or clamp brakes...
```

---
## \#6 Posted by: Deckoz Posted at: 2018-04-13T16:21:28.918Z Reads: 173

```
Yes. Mine and pahaw Evo are 13s sensored foc
```

---
## \#7 Posted by: district9prawn Posted at: 2018-04-13T16:26:22.059Z Reads: 165

```
Wow 14s is 58.8 at full charge. Even though I have no need for smooth regen braking I bought one to play with as I have heard lots of (mostly) good things about it over the past couple of years. I also need sensorless and on many ebike controllers the sensorless implementation is not that good.
```

---
## \#8 Posted by: Deckoz Posted at: 2018-04-13T16:29:39.196Z Reads: 153

```
Gotcha. Yea just don't use brakes at 14s the transients will be to high for the components (63v)o also only suggest it on L shaped vesc derivatives....
```

---
## \#9 Posted by: deucesdown Posted at: 2018-04-13T16:30:03.438Z Reads: 151

```
[quote="Battosaii, post:4, topic:52168"]
btw from my understanding there is no ERPM limit in FOC thats only a BLDC thing.
[/quote]

I thought the erpm limit was due to the speed of the voltmeters?
```

---
## \#10 Posted by: Deckoz Posted at: 2018-04-13T16:54:46.464Z Reads: 143

```
I've tested the focbox up to 110krpm.. and I believe blasto and Johnny have done the same. If not higher... 

My 13s calculated erpm is 73k. It's the noise on older hardware designs that leads to failures as line noise can cause improper readings, and over current at high duty cycles...noise and slower sample rates...which is why pretty much all new vesc designs use direct fets...

I'm actually gonna defer to @Blasto to answer @deucesdown as he will likely give a more thorough answer.
```

---
## \#11 Posted by: deucesdown Posted at: 2018-04-13T20:02:15.570Z Reads: 124

```
I'm starting to remember more, but IIRC it was something about the sampling rate of the DRV chip will only allow 1-2 samples per wave at higher ERPM, and a lot could happen between samples. Which makes me think it's not related to FOC vs BLDC at all. But I barely know what I'm talking about.

Sorry, I failed at googling up where I read that. I think on vedder.se forum somewhere.
```

---
## \#12 Posted by: Deckoz Posted at: 2018-04-13T20:52:46.442Z Reads: 113

```
Think your talking about FOC(modulation if phases) vs BLDC(timed sequence of phase firing)

FOC is always reading because the gate is always charged to some extent. Bldc switches phases and closes gates. 

With bldc the switching phase pairs is the erpm..(as far as I've always known)as it is closing and opening the gates. This makes power spikes which is why bldc is faster then FOC. 

FOC is continuous... No switching, or opening or closing the gate.. just modulating the gate voltage. So no erpm.
```

---
## \#13 Posted by: PatRocks Posted at: 2018-06-12T02:59:46.100Z Reads: 71

```
Hey @Deckoz , about 14s on FOCBOX, is the electronics-limitation specifically related to the on-board capacitors? And further, would an inline ripple filter (cap bank) mitigate the risk from regen? The bank I'm running is HUGE, 22 whole-farads (as opposed to uF). It's rated for 12s but the company that makes it (EM performance) have a 24s 6F bank too... just curious
```

---
## \#14 Posted by: onepunchboard Posted at: 2018-06-12T04:26:37.076Z Reads: 67

```
Holly Farad, 22? what do you do with vesc?
```

---
## \#15 Posted by: PatRocks Posted at: 2018-06-12T04:36:50.038Z Reads: 65

```
Keep them nice and happy/healthy!! I'm into overkill when it comes to hardware, and stumbled upon the pack while looking for "normal" sized cap banks. The others i found were similarly priced but with not even a fraction of the capacity, so I snagged it for $55 on eBay. It's probably instant death for most as switches tho, even my asm150 connector sparks a little when plugging in. The esc's stay on for about 30 seconds after unplugging them, lol
```

---
