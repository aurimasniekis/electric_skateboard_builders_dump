# Any good portable chargers?

### Replies: 27 Views: 910

## \#1 Posted by: Kingdom421 Posted at: 2019-01-31T03:40:35.530Z Reads: 182

```
Um yeah does anyone know of a good portable charger for on the go
```

---
## \#2 Posted by: Andy87 Posted at: 2019-01-31T03:48:21.234Z Reads: 182

```
What exactly are you looking for?
We even don’t know for which voltage...
```

---
## \#3 Posted by: MysticalDork Posted at: 2019-01-31T03:53:31.463Z Reads: 180

```
@Kingdom421 Give us more info. BMS or balance charger? Voltage? Current? Battery chemistry?
```

---
## \#4 Posted by: Kingdom421 Posted at: 2019-01-31T04:05:50.430Z Reads: 176

```
Let me check real quick its not for a diy it's a prekit
```

---
## \#5 Posted by: Kingdom421 Posted at: 2019-01-31T04:26:05.113Z Reads: 170

```
I had to leave real quick so all I know it's a Lithium 3200mAh
```

---
## \#6 Posted by: Andy87 Posted at: 2019-01-31T07:46:43.949Z Reads: 155

```
The voltage, your desired charge current and the adapter plug type we need to know as min.
```

---
## \#7 Posted by: Surfer Posted at: 2019-01-31T07:55:17.754Z Reads: 146

```
You can use this one for 10s to 12s up to 7,5 amps charge
Meanwell hlg-320h-48b
Is cc-cv, the best thing is no noisy fan.
Also not the cheapest.
```

---
## \#8 Posted by: MysticalDork Posted at: 2019-01-31T08:57:09.102Z Reads: 138

```
@Surfer Yeah, no. That's a LED driver, not a battery charger. It's not designed to charge batteries, and it has no current ramp-down or charge termination. It'll charge your battery all the way to 4.2v/cell at maximum current and continue to trickle charge it indefinitely once it's there. That's a **PERFECT** recipe for a battery fire. Do NOT use that thing to charge your batteries.
```

---
## \#9 Posted by: pat.speed Posted at: 2019-01-31T09:52:55.052Z Reads: 124

```
You can make your own with a boost converter, spare Lipo and watt meter
```

---
## \#10 Posted by: Surfer Posted at: 2019-01-31T10:22:18.808Z Reads: 115

```
Oh yeah I see that you don't have any clue about what you are talking about :)
```

---
## \#11 Posted by: Kingdom421 Posted at: 2019-01-31T15:53:06.065Z Reads: 102

```
![1548949967820|690x212](upload://rQoMQjZGRtVE97GXe5T2HaY48mb.jpeg)
```

---
## \#12 Posted by: Kingdom421 Posted at: 2019-01-31T15:55:39.689Z Reads: 98

```
![1548950065195|690x172](upload://5NiNgiCWMrKegQxl05UWB4DgAAU.jpeg)
```

---
## \#13 Posted by: Andy87 Posted at: 2019-01-31T15:56:11.756Z Reads: 98

```
Which charge plug you have?
How much amps the charger should have?
```

---
## \#14 Posted by: Kingdom421 Posted at: 2019-01-31T16:02:04.610Z Reads: 97

```
12amps USA Wall plug
```

---
## \#15 Posted by: Andy87 Posted at: 2019-01-31T16:05:19.817Z Reads: 96

```
Have a look at this one
https://s.click.aliexpress.com/e/bNlA6rea

Is it the same charge plug than you have?
```

---
## \#16 Posted by: Andy87 Posted at: 2019-01-31T16:05:53.169Z Reads: 88

```
Your charger is 2.5A 😉
```

---
## \#17 Posted by: Kingdom421 Posted at: 2019-01-31T17:00:53.931Z Reads: 82

```
I have that already I'm looking for something portable I can plug it into so o don't have to find an outlet. I guess it's call a power bank.
```

---
## \#18 Posted by: Kingdom421 Posted at: 2019-01-31T17:07:51.148Z Reads: 82

```
This is what I'm thinking about trying. https://www.rockpals.com/products/rockpals-280wh-portable-generator-rechargeable-lithium-battery-pack-solar-generator-power-station-with-110v-ac-outlet-dc-output-usb-output-for-cpap-backup-emergency-hurricane-storm-and-outage-camping?variant=13342825349189&gclid=Cj0KCQiA1sriBRD-ARIsABYdwwHr_I_UonNpspYcsmFJXG5W0a4z5lFyhws7Aexyo0vyaPWxK-LpvkwaAueeEALw_wcB
```

---
## \#19 Posted by: Andy87 Posted at: 2019-01-31T17:12:14.875Z Reads: 79

```
You need to say what you searching...
We can’t read your mind....
```

---
## \#20 Posted by: Kingdom421 Posted at: 2019-01-31T17:18:39.497Z Reads: 74

```
Haha oops bro my bad I'm just waking up i meant to attach this https://www.rockpals.com/products/rockpals-280wh-portable-generator-rechargeable-lithium-battery-pack-solar-generator-power-station-with-110v-ac-outlet-dc-output-usb-output-for-cpap-backup-emergency-hurricane-storm-and-outage-camping?variant=13342825349189&gclid=Cj0KCQiA1sriBRD-ARIsABYdwwHr_I_UonNpspYcsmFJXG5W0a4z5lFyhws7Aexyo0vyaPWxK-LpvkwaAueeEALw_wcB
```

---
## \#21 Posted by: mishrasubhransu Posted at: 2019-01-31T17:23:24.149Z Reads: 67

```
WINGONEER 600W DC 10-60V To 12-80V Step-up Module Boost Power Suppy DC Converter https://www.amazon.com/dp/B01MG4211N/ref=cm_sw_r_cp_apa_i_V7YuCbT9CSVF5

Just plug it in to some low DC voltage source.
```

---
## \#22 Posted by: MysticalDork Posted at: 2019-01-31T17:24:23.209Z Reads: 66

```
Please enlighten me, then. How am I wrong? Got a graph of voltage and current over time? I'd love to see one.
```

---
## \#23 Posted by: Hummie Posted at: 2019-01-31T17:33:03.768Z Reads: 69

```
@MysticalDork  Cc and cv regime is over-rated.  As long as it’s a regulated current and under the max charge rate it’s good (although the charge rate is also likely conservative n you could probably put more than rated at low soc) 

 These supplies do a constant voltage and the current follows ohms law and the pack voltage. If u graph it it’ll be a constant voltage and the current will be at likely the peak output and then decrease as getting closer to charged. It doesn’t trickle charge 

The led drivers are supposedly more robust but I like the golden knob 

https://www.amazon.com/Adjustable-Converter-110V-220V-Switching-Transformer/dp/B0777MH681/ref=mp_s_a_1_2?ie=UTF8&qid=1548956283&sr=8-2&pi=AC_SX236_SY340_QL65&keywords=adjustable+48+volt+power&dpPl=1&dpID=51jlylEpA7L&ref=plSrch
https://www.amazon.com/gp/aw/s/ref=nb_sb_ss_i_1_13?k=led+driver+48v+output&sprefix=led+driver+48&crid=X1QY78HCE40X
```

---
## \#24 Posted by: MysticalDork Posted at: 2019-01-31T17:43:53.370Z Reads: 56

```
Alright, I concede that point. What about charge termination?
```

---
## \#25 Posted by: Hummie Posted at: 2019-01-31T17:51:20.208Z Reads: 55

```
With charge termination happening at maybe 4.2 and then recharging happening if the cell were to sink to maybe 4.1, and that being a continuous cycle, cell charge termination doesn’t do anything except keep the cell from sitting on a constant 4.2v, where it will suffer most deterioration.  If u were to set a bulk charger to 4.1 and leave it there for years maybe it would fare better as it never has to get to 4.2.  If u did set the bulk supply to 4.2 the cell will sit there constantly and not go over, but not nice to the cell to sit so high
```

---
## \#26 Posted by: Surfer Posted at: 2019-01-31T18:03:55.860Z Reads: 53

```
You can choose the voltage termination, it has 2 pot to adjust current and voltage.
Anyway your point was good because not all led drivers are the same, with meanwell the appropriate for our use is HLG series.

Thanks @hummie, I couldn't explain as good as you :)
```

---
## \#27 Posted by: Kram720 Posted at: 2019-07-17T11:32:56.184Z Reads: 25

```
This will do the job myself and a couple other guys use them
https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com.au%2Fulk%2Fitm%2F183692739972
```

---
