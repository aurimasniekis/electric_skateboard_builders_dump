# Cell voltage dropping lower than other cells toward end of discharge?

### Replies: 22 Views: 277

## \#1 Posted by: mynamesmatt Posted at: 2019-05-25T07:25:05.384Z Reads: 78

```
Hey guys,
So to set the scene, i run 4 5s 4500mah nano techs in a 10s2p config. 

Usually with hard riding, I'll get about 19-20km out of it with dual 6374's. 

On Thursday, i rode 19km no problem, with cells all relatively close to each other voltage wise (within 0.15 of a volt of each other). Yesterday, i rode 16.5km, and my bms shut down as one of my cells dropped to 3.3v when the others were just hitting 3.55. 

Now what I'm thinking is, due to differing internal resistances, some cells discharge faster than others. This really shouldn't be the case.... right? 

So I've swapped 2 lipo packs so one pack from the 5s2p is now with the other (swapped pairs). This should help shouldn't it? it would help keep the voltage somewhat similar i believe? 


Seriously calling all electro experts here (@b264  & @namasaki you guys especially) as i know i dont have dead cells, i just feel like the internal resistance differences have an effect on a linear discharge. 

here is the metr data
https://metr.at/r/nJZoL

Thanks yall
```

---
## \#2 Posted by: anders Posted at: 2019-05-25T07:51:58.689Z Reads: 69

```
Hi,

I have a 12s 4.6Ah 90c Graphene pack running 80 battery amps, 44V (3.66v/cell) soft cutoff and 42.6V (3.55v/cell) hard cutoff in my esc.  I have monitored my cell deviation at lower cell voltages and as long as I stay at these voltages or above my deviation stays within 12mv or  0.012V if I discharge deeper with high amperage the deviation increase quick. My voltage sag at high amp is around 1v according to HUD.
```

---
## \#3 Posted by: Okami Posted at: 2019-05-25T08:30:27.914Z Reads: 63

```
Yes, stay above 3.55v. 

Below 3.5v cell drift becomes quite visible but they recover rather fast after u plug the charger and start charging them up
```

---
## \#4 Posted by: mynamesmatt Posted at: 2019-05-25T08:56:43.664Z Reads: 61

```
Yeah its just weird how temperamental it is. like one day i ride 19km with room to spare, next day i ride very similarly, and only get 16 and it dies. one of the cells were still at 3.65v and the other at 3.25v. Im discharging through a bms so shouldn't it really help with discharging more evenly? or is the balance current not enough to keep up with the drain?
```

---
## \#5 Posted by: dareno Posted at: 2019-05-25T09:10:41.206Z Reads: 59

```
How was the day?   Hot as all fuck or same as the rest of the times?
```

---
## \#6 Posted by: anders Posted at: 2019-05-25T09:19:59.287Z Reads: 55

```
I try not to go below 3.7v/cell and I always balance charge with icharger so I can monitor deviations and internal resistance. Have you set a low voltage cutoff in your esc? most bms's cutoff are very low for lipo. My internal resistance range from 2-2.3 mΩ /cell.
```

---
## \#7 Posted by: mynamesmatt Posted at: 2019-05-25T09:22:45.090Z Reads: 50

```
was perfect weather. got the board in germany atm and it was like 22 degrees so defs not warmth related. on top of that, my enclosure has no heat dissipation so after 5-10min my enclosure sits at about 35 degrees anyways
```

---
## \#8 Posted by: mynamesmatt Posted at: 2019-05-25T09:24:17.829Z Reads: 48

```
yeah low voltage cutoff is at 3.5v start and 3.3v end as that last bit of juice is often what gets me home. My esc still said it was at 36v, but as one cell was so much lower the bms cut out. the bestech HCX-D223V1 i have is for lipo so it's hard cutoff is 3 2v
```

---
## \#9 Posted by: anders Posted at: 2019-05-25T09:32:23.202Z Reads: 45

```
seems a bit low for lipo especially when concidering high amp draw, have you checked how much sag you get with full battery vs low battery?
```

---
## \#10 Posted by: mynamesmatt Posted at: 2019-05-25T09:40:19.854Z Reads: 39

```
yeah i mean i know when i get to that point so I back off, but yes probs a bit low. full battery when i pull 70a (35a batt max each) i get about 0.8v sag. when near empty it goes to about 1-1.5v. I've made an "eco mode" on my metr so it's limited to 50a total. that'll probs help a bit
```

---
## \#11 Posted by: anders Posted at: 2019-05-25T09:43:26.036Z Reads: 37

```
I read this post https://www.electric-skateboard.builders/t/low-battery-riding/32768/11?u=anders and took @Deckoz advice.
```

---
## \#12 Posted by: Okami Posted at: 2019-05-25T21:00:10.224Z Reads: 28

```
@anders some good info there, kudos to @Deckoz for sharing it.

I agree about the point that lipos low end voltage gets tossed around quite a bit..

From general experience Ive had with lipo on friction drive ebike, it does get bad below 3.55v per cell. 

At 3.6-3.7v it is 'manageable' but below these 3.55v the voltages 'get tossed' around quite a bit and it gets quite visible that battery is close to its last remaining capacity.

--

Some good tips from Deckoz about internal resistance and how to look after when battery starts to get bad. Truly an insider info not everyone gets to witness themselves when starting out with lipos/batteries in general.
```

---
## \#13 Posted by: Namasaki Posted at: 2019-05-26T06:51:19.064Z Reads: 22

```
[quote="mynamesmatt, post:7, topic:94915"]
was perfect weather. got the board in germany atm and it was like 22 degrees so defs not warmth
[/quote]

Cold weather can have an adverse affect on battery performance and 22deg is cold enough to freeze.

BTW, what is the C rating on your Nano Tech's?

If you have an IR meter, you can check the internal resistance of your packs

Internal resistance increases as batteries age.

One of your packs or even just 1 or 2 cells in a pack could have increased internal resistance.
```

---
## \#14 Posted by: Sebike Posted at: 2019-05-26T08:04:58.709Z Reads: 22

```
22 degrees Celsius (Germany? ) equals 72 deg Fahrenheit. 

I know people that would freeze at that temperature, but my batteries think that's pretty ok weather 😉
```

---
## \#15 Posted by: mynamesmatt Posted at: 2019-05-26T09:47:42.907Z Reads: 19

```
[quote="Namasaki, post:13, topic:94915"]
BTW, what is the C rating on your Nano Tech’s?
[/quote]

they're 35c constant, 70c peak. and 2 in parallel so double. They should be just fine current output wise
```

---
## \#16 Posted by: Namasaki Posted at: 2019-05-26T14:42:21.132Z Reads: 15

```
[quote="Sebike, post:14, topic:94915"]
22 degrees Celsius (Germany? ) equals 72 deg Fahrenheit.
[/quote]

He didn’t specify C or F
I’m in the US so I default to Fahrenheit.
```

---
## \#17 Posted by: Namasaki Posted at: 2019-05-26T14:50:36.772Z Reads: 15

```
[quote="mynamesmatt, post:15, topic:94915"]
they’re 35c constant, 70c peak. and 2 in parallel so double. They should be just fine current output wise
[/quote]

Parallel doubles capacity.   
I don’t think it doubles the C rating.   
I believe what  you have is 9000mah 35C. 

An IR meter would tell you straight up the condition of each cell.
![image|414x414](upload://ufJXj232MhIyQJu82A0sEzn6C4K.jpeg)
```

---
## \#18 Posted by: mynamesmatt Posted at: 2019-05-26T14:57:43.080Z Reads: 12

```
[quote="Namasaki, post:17, topic:94915"]
Parallel doubles capacity.
I don’t think it doubles the C rating
[/quote]

yeah it doesn't double the c rating but it doubles the current output capability. Can you measure internal resistance with a multimeter?
```

---
## \#19 Posted by: Namasaki Posted at: 2019-05-26T14:59:01.982Z Reads: 13

```
No, you need a special meter like the one above
```

---
## \#20 Posted by: Namasaki Posted at: 2019-05-26T15:05:43.476Z Reads: 12

```
The Turnigy IR meter seems to be discontinued. 

There is another brand available. 

https://www.hobbytown.com/revolectrix-lipo-battery-internal-resistance-ir-meter-lipo-only-revdcir/p700121
```

---
## \#21 Posted by: Okami Posted at: 2019-05-26T18:22:47.457Z Reads: 11

```
I also vote on checking cell IR... 

Cant boldly claim you have started the damage.. but if you manage to pull high amps when on low side of battery capacity, it might as well start some funny things..

Otherwise I would just check your range more consistently.. were the conditions really the same etc..
```

---
## \#22 Posted by: Hummie Posted at: 2019-05-26T18:40:01.685Z Reads: 11

```
won’t the internal resistance parallel the capacity so can be revealed by how quickly it depletes and fills.  What use is the cell ir good for that watching the voltages doesn’t show
```

---
