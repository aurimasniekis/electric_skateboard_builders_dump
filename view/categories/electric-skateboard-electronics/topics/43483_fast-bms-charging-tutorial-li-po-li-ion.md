# Fast bms charging tutorial (Li-po, Li-ion)

### Replies: 18 Views: 6532

## \#1 Posted by: DjamboBuksne Posted at: 2018-01-11T18:37:18.751Z Reads: 403

```
A lot of people have to disconnect their batteries and than charge them one at the time... That takes alot of time so there is a solution; BMS

I used pictures from this video: https://www.youtube.com/watch?v=jxHQjlHv1y4

So first you have to choose the right bms for your battery.
I have 2x 3s 5Ah  Li-po batteries in series so I would need a 6s 5A BMS

Like this one; 
https://www.ebay.com/itm/Protection-Balance-Module-PCM-BMS-5A-for-6S-22-2V-Li-ion-Li-Po-battery-6S5W001/321790634514?epid=2218361580&hash=item4aec376a12:g:wlsAAOSwT6pVilFD


BMS has an over-current feature but we are going to bypass  that because our boards can draw much more and the cut-off voltage feature is integrated in the most of escs

When choosing for a bms, look that it has the balance charging.

This would be a diagram for a 6s battery

![s-l500|620x349](upload://oCT6N7qRhovG0JSO3kCrrJAVEwv.jpg)

![30054f0c-6239-4f9d-a8fe-eb799afc80a2|500x500](upload://a26zc1o5Zi7IGtNiGSoYZKf3YnC.jpg)

Output is directly from the battery and not from the drain of the bms because over-current feature.

In the description of the bms you can find all of the information...

![bms specs|664x499](upload://4IcSMjihzrmssHWdjNUFRAIlwra.png)

Now that you have that, you need a charger.

Now, look at the maximum charging current on your batteries.
On mine it is 2C so that's 10A, but slower charging is safer.
https://hobbyking.com/en_us/turnigy-5000mah-3s-20c-lipo-pack-xt-90.html

On the discription of the bms you have the charging voltage, on this one is 27-30V but it work's with 25.2V and that is the maximum 6s Li-po/Li-ion voltage

You can buy a charger like this one
https://www.ebay.com/itm/25-2V-2A-Smart-Charger-For-21-6V-22-2V-25-2V-Li-ion-Li-Po-Lithium-Battery-US-Plu/112630200819?hash=item1a394879f3:g:YN8AAOSwT2daB~kW&vxp=mtr

It even has the led that let's you know when the batteries are charger charged.. But charging with that would take alot of time so I built mine own charger.

First you need a power supply... I bought 24V 120W power supply from ebay. 

https://www.ebay.com/itm/AC-110V-220V-TO-DC-5V-12V-24V-Switch-Power-Supply-Driver-Adapter-LED-Strip-Light/152134115704?hash=item236be66178:m:mnohYz4NZlT_Dq5l5lWNUMg

It can go up to 5A but the standard voltage is 24V and we need 25.2V So we need to limit the current.

On 24V 5A 120W model you have to solder a 10K ohm potentiometer to R35 resistor

![MEDIUM|333x499](upload://m4sSh7k6vp0ofynKMWjdUjlLYzD.jpg)

![MEDIUM|620x413](upload://XCorIu51uGJGdZETj6tARFkgl8.jpg)

Now you can set it to 25.2V and about 4.7A in my case.

When charging like this, you can't tell when batteries are done charging so you would need to add an ammeter to it, when it's about 0, it's done charging.

![MEDIUM|620x349](upload://pfgNVhOYe4wgUFV9PFu6OpNqyUo.jpg)
```

---
## \#2 Posted by: Blitz Posted at: 2018-01-12T20:17:41.440Z Reads: 309

```
Could i use 10s Li-po BMS with 9s?

https://www.ebay.ie/itm/37V-42V-10S-45A-Lithium-ion-Li-ion-LiPo-Polymer-Battery-BMS-PCB-System-Ebike-36V/322451815873?hash=item4b13a03dc1:g:7xcAAOSwpuFaG3tY
```

---
## \#4 Posted by: Torcn Posted at: 2018-01-12T23:30:56.608Z Reads: 295

```
I would like to do the same. Do you think we can trust on those cheap bms from ebay? What charging port are you using?
```

---
## \#5 Posted by: DjamboBuksne Posted at: 2018-01-12T23:51:38.506Z Reads: 285

```
I'm not sure about 9s battery on the 10s bms, It would still balance all of the cells and the charging voltage than has to be  37.8V and not what the bms sheet says... I'm not sure...

This is my chg port 

https://www.ebay.com/itm/1-set-3pin-GX12-12mm-Aviation-Plug-Metal-Panel-Female-Male-Connector-Waterproof/332427828712?ssPageName=STRK%3AMEBIDX%3AIT&var=541460355716&_trksid=p2057872.m2749.l2649
```

---
## \#6 Posted by: Torcn Posted at: 2018-01-13T00:43:39.201Z Reads: 256

```
I'll do it with 6s setup like you
```

---
## \#7 Posted by: Blitz Posted at: 2018-01-13T00:50:27.857Z Reads: 248

```
You can charge both you're batteries in series using a balance charger, BMS is more useful on a 9s pack
```

---
## \#8 Posted by: DjamboBuksne Posted at: 2018-01-13T01:41:58.748Z Reads: 231

```
Could you do like 3x 3s bms in and charger leads in series
```

---
## \#9 Posted by: DjamboBuksne Posted at: 2018-01-13T01:42:12.729Z Reads: 220

```
I diddn't find a single 9s bms
```

---
## \#10 Posted by: Torcn Posted at: 2018-01-13T02:07:58.544Z Reads: 209

```
9s is not to common. Is more 8s and 10s
```

---
## \#11 Posted by: Torcn Posted at: 2018-01-13T02:11:37.450Z Reads: 207

```
I think is useful for any battery configuration so you can get easy method for charging. Charge with balance charger is a pain
```

---
## \#12 Posted by: Blitz Posted at: 2018-01-13T10:02:55.445Z Reads: 191

```
I know of 9s BMS but they cost a lot, I rather Just charge 2 3s bateries in series and the last 3s single, It Rains a lot in Ireland so i would not have an issue OF "Quick charge its day 2 i need to go to work" I would only be esk8ing for fun when the sun comes out.
```

---
## \#13 Posted by: Blitz Posted at: 2018-01-13T10:04:42.573Z Reads: 192

```
I don't mind Balance charging,

And as for 6s it couldn't be easier Just wire both batteries in series and cable route them so its easy to take them and plug in bling Bling Bling Balance charging has started.
```

---
## \#14 Posted by: pat.speed Posted at: 2018-01-13T10:16:50.943Z Reads: 184

```
Just letting you know but the overvoltage setting on your bms is set to 4.3 which could potentially harm your lipos
```

---
## \#15 Posted by: DjamboBuksne Posted at: 2018-01-14T13:17:26.054Z Reads: 178

```
[quote="pat.speed, post:14, topic:43483, full:true"]
Just letting you know but the overvoltage setting on your bms is set to 4.3 which could potentially harm your lipos
[/quote]

Yeah i know, that's why i charge it with 25.2V charger
```

---
## \#16 Posted by: Gandinator Posted at: 2018-07-31T22:19:28.087Z Reads: 129

```
Hi,

I am a noob so correct me if necessary.

I want to have 2 5S 5000mah lipos in series. If I get a bms for that requirement and the smart charger can't I just plug that into mains. Also where do you get the bit where you plug the charger in?

Thanks
```

---
## \#17 Posted by: Chrisjarram Posted at: 2019-01-11T08:42:38.785Z Reads: 81

```
Useful info thanks
```

---
## \#18 Posted by: Felixxx Posted at: 2019-04-06T13:11:17.339Z Reads: 59

```
I have 12s 1p lipo. Can I use 3 4s separate bms? For example 1 bms for 4 cells.
```

---
## \#19 Posted by: Chupacabra Posted at: 2019-06-23T04:29:34.555Z Reads: 33

```
This is an amazing tutorial bro. Thanks for this. 

I am using 2x 22000mah 6S. To avoid buying an expensive charger I am going to use these 

https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F283494884932

https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F223004221886
```

---
