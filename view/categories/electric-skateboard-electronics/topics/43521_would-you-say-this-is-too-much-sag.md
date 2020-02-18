# Would you say this is too much SAG?

### Replies: 9 Views: 663

## \#1 Posted by: Eboosted Posted at: 2018-01-12T05:58:56.326Z Reads: 146

```
I'm running Trampa board with 8" pneumatics on 12S4P with Samsung 30Qs, dual 6374S 170KV, 13/62T pulllies and ESCape with @ackmaniac firmware.

My settings are:
Motor Max 80A
Motor Min -60A
Battery Max 40A
Battery Min -20A

[img]https://i.imgur.com/uVbt2m6.jpg[/img]

Under full thottle voltage sags from 47.4V to 42.5V, is this a normal behaviour or I'm pushin my luck here? Even though, battery max has been restricted to 40A on ESC tool it draws 61.2A on each VESC.

Any input would be greatly appreciated.
```

---
## \#2 Posted by: thisguyhere Posted at: 2018-01-12T06:10:40.474Z Reads: 133

```
hey alan, this is nearly identical to the question i had as well:

http://www.electric-skateboard.builders/t/6v-sag-too-much/32002

if you're using a bms for both charge and discharge, yes, the sag can be a problem.

if the voltage sags below your bms cutoff, the bms will cut power.  usually, when you pack is at max sag will be when you're demanding the most from it, like hard acceleration.  my bms cutout during full throttle uphill and it threw me off the board:

http://www.electric-skateboard.builders/t/ate-shit-today-and-loop-keys/33613/30
```

---
## \#3 Posted by: jmasta Posted at: 2018-01-12T06:14:28.799Z Reads: 116

```


[quote="Eboosted, post:1, topic:43521"]
battery max has been restricted to 40A on ESC tool it draws 61.2A on each VESC
[/quote]

I sure hope that's not 60A per VESC, or you'd be pulling 30A per cell.  60A total is reasonable and safe for your 4p 30Q pack. 120A is not

That has to be total current in the chart, which would make way more sense since you limited each VESC to 40A battery max
```

---
## \#4 Posted by: thisguyhere Posted at: 2018-01-12T06:17:39.155Z Reads: 114

```
where you seeing 120a?

batt max is 40a, dual drive, so 80a batt max.  4p pack so 80a safe discharge.

looks ok to me.

edit

ok I see it in the chart.
```

---
## \#5 Posted by: Eboosted Posted at: 2018-01-12T06:24:58.551Z Reads: 113

```
I have always been confused by this, I'm not 100% sure if this is total current draw from the battery or current for each ESC, @ackmaniac would you please chime in?

[quote="thisguyhere, post:2, topic:43521"]
hey alan, this is nearly identical to the question i had as well:
[/quote]

I just read your post, thanks for the input, well I feel I'm not alone here :grin:
```

---
## \#6 Posted by: jmasta Posted at: 2018-01-12T06:37:47.905Z Reads: 108

```
The sag is normal, per discharge charts

47.4V total = 3.95V per cell
42.5V total = 3.54V per cell, under roughly 15A per cell


Look at the 0.75 Ah vertical line.  The 0.2A red curve (which is basically resting voltage) is roughly at 3.95V.  The 15A purple curve is at about 3.55V.  Your results correspond almost perfectly with the published data


http://lygte-info.dk/pic/Batteries2012/Samsung%20INR18650-30Q%203000mAh%20(Pink)/Samsung%20INR18650-30Q%203000mAh%20(Pink)-Capacity.png
```

---
## \#7 Posted by: willpark16 Posted at: 2018-01-12T07:47:52.860Z Reads: 87

```
What are your settings for each vesc?
```

---
## \#8 Posted by: Ackmaniac Posted at: 2018-01-12T07:50:30.943Z Reads: 83

```
Depends on the amount of Vescs you entered in the app. When it is set to 2 then motor amps, battery amps and the consumption values (Wh, Ah)  are doubled. At the point where you set the cursor in your image you are also not at the highest motor amps you have reached.
```

---
## \#9 Posted by: Eboosted Posted at: 2018-01-12T08:56:22.853Z Reads: 74

```
@jmasta your explanation is perfect, thanks for taking the time to explain in such a clear way.
```

---
