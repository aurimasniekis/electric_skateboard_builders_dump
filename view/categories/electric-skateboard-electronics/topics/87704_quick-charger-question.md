# Quick charger question

### Replies: 28 Views: 378

## \#1 Posted by: TreeFactory Posted at: 2019-03-20T04:00:52.877Z Reads: 119

```
I'm running a 12s1p 6000mah 65c bat with the 80 bestech bms that has a max charge rate of 4a. My understanding is that 1c for my batteries would be a charge rate of 6a. Is a 4a 50.4v charger ok?
```

---
## \#2 Posted by: nuttyjeff Posted at: 2019-03-20T04:08:56.948Z Reads: 119

```
Yes. Although im interested to know how small your BMS is with a max charge rate of 4A
```

---
## \#3 Posted by: TreeFactory Posted at: 2019-03-20T04:11:19.541Z Reads: 115

```
https://buildkitboards.com/collections/batteries/products/bestech-bms?variant=7201537785886
```

---
## \#4 Posted by: nuttyjeff Posted at: 2019-03-20T04:16:21.067Z Reads: 104

```
Damn, didnt know the charging current was so little on the Bestech. Good to know, thanks for the link (:
```

---
## \#5 Posted by: TreeFactory Posted at: 2019-03-20T04:19:58.122Z Reads: 102

```
I think some of the others have a higher charge rate. And for what it's worth the bestech can do quick charge though i'm a bit hazy on what that really means.
```

---
## \#6 Posted by: MysticalDork Posted at: 2019-03-20T04:20:00.227Z Reads: 97

```
Charging at anything less than the maximum rated is absolutely fine. Just don't go over either the BMS or battery rating. And make sure you have a fuse in series with your charge port.
```

---
## \#7 Posted by: TreeFactory Posted at: 2019-03-20T04:20:32.279Z Reads: 90

```
doesn't the bestech have a built in fuse?
```

---
## \#8 Posted by: MysticalDork Posted at: 2019-03-20T04:21:33.707Z Reads: 93

```
I don't know, and I wouldn't rely on just that. For one, it's a much bigger pain to replace a fuse on a PCB than to replace one in a fuse holder.
```

---
## \#9 Posted by: TreeFactory Posted at: 2019-03-20T04:23:42.320Z Reads: 82

```
Do you have a recommendation for fuse size? I'm guessing an 80a fuse
```

---
## \#10 Posted by: TreeFactory Posted at: 2019-03-20T04:24:13.707Z Reads: 83

```
I also have bot focboxes set at a max for 40a each
```

---
## \#11 Posted by: MysticalDork Posted at: 2019-03-20T04:24:46.354Z Reads: 81

```
No no no no. On the charge port. It's only going to see a four-amp charger, right? So put like an eight or ten-amp fuse on it.
```

---
## \#12 Posted by: TreeFactory Posted at: 2019-03-20T04:26:28.983Z Reads: 77

```
ooooo i see i see. thats jsut for if the charger fails or something? cause the charger im picking up tops out at 4a
```

---
## \#13 Posted by: MysticalDork Posted at: 2019-03-20T04:29:31.992Z Reads: 77

```
Not so much that, but as a general safety thing against shorts. What if some idjit decides to mess with your board while you aren't looking and shorts the pins in the charge port? Depending on the BMS and wiring, you could end up with a fried BMS or cooked wires, or even a fire. With a fuse, you'd get a small pop, a small spark and you can't charge until you replace the fuse.
```

---
## \#14 Posted by: TreeFactory Posted at: 2019-03-20T04:30:43.878Z Reads: 73

```
also I'm not sure if it means anything but at first I soldered the the - and + backwards and blew a charging brick but I dont see any damage on the bms and the board still turns on fine so im guessing everything is ok
```

---
## \#15 Posted by: L3chef Posted at: 2019-03-20T10:00:59.986Z Reads: 62

```
Wow 4a max charge. Doesn't this mean you will have very weak brakes?
```

---
## \#16 Posted by: Andy87 Posted at: 2019-03-20T10:11:24.751Z Reads: 57

```
Doesn’t that mean you have very fast no breaks? 🤔
I know that the values in the data sheet are for constant charging, so I assume no issues when breaking for a short period with 8-10a.
But if you for example drive down a longer hill and break for 30sec or longer, wouldn’t the bms cut off which would lead to a total loss of the brakes?
```

---
## \#17 Posted by: L3chef Posted at: 2019-03-20T10:27:30.091Z Reads: 55

```
Yup you should test the brakes with that bms. I think it will cut off under hard braking
```

---
## \#18 Posted by: Andy87 Posted at: 2019-03-20T10:33:36.470Z Reads: 52

```
But than I don’t understand why an esk8 shop sell this configuration 🤔
I mean it even doesn’t make a sense to wire it up for charge only. Ok it makes sense but is too big and too expensive to compair to a d140 for example.
```

---
## \#19 Posted by: L3chef Posted at: 2019-03-20T11:01:56.263Z Reads: 51

```
Could it be a typo? Can't understand it either why a eskate shop would sell it... I have a HCX-D223V1 aswell but with 20a max charge.
```

---
## \#20 Posted by: rich Posted at: 2019-03-20T11:50:50.166Z Reads: 48

```
I'm sure it's a typo because when looking at Bestech site it states 20A max. cont. charge and it's not an adjustable value so don't worry. Or is this a special version @JLabs? 

![HCX-D223v1|475x500](upload://oTfAjLJCjVuP8tLjTGhiRA97IC2.png) 


http://www.bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html

[quote="Andy87, post:16, topic:87704"]
I know that the values in the data sheet are for constant charging, so I assume no issues when breaking for a short period with 8-10a.
[/quote]

The regenerative breaking with BMS is one thing which confuses me from day 1. If the BMS has different ports (P- for discharge, C- for charge) I think the max charging current doesn't matter for regenerative breaking because the current flow goes back to P- and not C- anyway.

On a BMS with discharge and charge on same port the value for discharge and charge are the same. There are just more FETs on the C- trace (same amount as on P-) and discharge plus charge are connected to C-. There are also BMS available where all is connected to P-. Very confusing for beginner.

I have 5 BMS and all with same port because of my paranoia about a cut off due to breaking. But I've heard and read from experienced members that their BMS with different ports never shut off due to hard breaking so I guess it makes no difference. Would be interesting to hear the opinion from an electrical engineer about this case.
```

---
## \#21 Posted by: taz Posted at: 2019-03-20T12:26:54.336Z Reads: 40

```
[quote="rich, post:20, topic:87704"]
The regenerative breaking with BMS is one thing which confuses me from day 1. If the BMS has different ports (P- for discharge, C- for charge) I think the max charging current doesn’t matter for regenerative breaking because the current flow goes back to P- and not C- anyway.
[/quote]

This.

I want to increase my regen current settings on my Evo that has that particular BMS and I have not done it yet because I do not know what will happen.
```

---
## \#22 Posted by: rich Posted at: 2019-03-20T12:36:48.692Z Reads: 39

```
[quote="taz, post:21, topic:87704"]
I want to increase my regen current settings on my Evo that has that particular BMS
[/quote]

What's your actual batt regen settings?

For example I set -15A each vesc so -30A in total. In real life the total batt regen current flow never exceeds about -15A (monitored by app), the highest ever was -17A but usually it's less even with hard breaking.

Edit: But I have to say that i mainly break at low or mid speed or downhill and usually not at higher speed. When I ride fast then I don't break, why should I :laughing:?
```

---
## \#23 Posted by: Sn4pz Posted at: 2019-03-20T12:51:34.739Z Reads: 35

```
[quote="rich, post:22, topic:87704"]
why should I :laughing:?
[/quote]


Plenty of good reasons... XP 

I worry about this too, and although the regen current might be beneficial for a smaller battery, have you guys ever thought of using the Rbreak that maytech makes? Ive been thinking about it, and more and more im ok with the idea of losing regen current, but trading it for always usable breaks
```

---
## \#24 Posted by: taz Posted at: 2019-03-20T12:57:04.284Z Reads: 33

```
On that particular board I have it set at -10A per Vesc.

So 2 x 10A= 20A which is the BMS's maximum charge current.

There are lots of times where my total regen current is right at the limit.

Here is an example

https://metr.at/r/KiU1r?zoom_start=446&zoom_end=511
```

---
## \#25 Posted by: rich Posted at: 2019-03-20T13:05:10.780Z Reads: 32

```
[quote="Sn4pz, post:23, topic:87704"]
Rbreak that maytech makes?
[/quote]
What's that and which esc?

[quote="Sn4pz, post:23, topic:87704"]
im ok with the idea of losing regen current, but trading it for always usable breaks
[/quote]

I personally never lost brakes only balance.

[quote="taz, post:24, topic:87704"]
There are lots of times where my total regen current is right at the limit.
[/quote]

Interesting. Seems I'm not breaking hard enough
```

---
## \#26 Posted by: taz Posted at: 2019-03-20T13:07:09.820Z Reads: 33

```
I would be very interested to see what my currents are with my Trampa (regen set at -40A per vesc :joy:) but I don't have a metr pro module installed in that one.
```

---
## \#27 Posted by: Sn4pz Posted at: 2019-03-20T13:33:38.370Z Reads: 32

```
[quote="hyperIon1, post:1, topic:80239"]
RHEOSTATIC BRAKE module
SAMPLE PRICE $30

![Rheostatic Brake.jpg](https://www.electric-skateboard.builders/uploads/db1493/original/3X/5/d/5d9a0100a07741e21f3d61aee52f276ecf6940c7.jpeg)

Battery: &lt;=12s
Operation voltage: 57V
Startup time: 200ms
Max current: 5A
Function: when brake reverse voltage is higher than operation voltage, Rheostatic Brake starts working and reduces the reverse voltage to protect ESCs.
[/quote]

Meaning it should help prevent errors like over voltage, and I would guess some of the amperage as well, I think it was brought up that Regen was lessened.

This is guesswork on my part, but it seems like a product that would be pretty applicable
```

---
## \#28 Posted by: TreeFactory Posted at: 2019-03-26T20:22:42.014Z Reads: 20

```
I've double checked with Build Kit Boards and have been assured that it's a typo on the sheet and that BMS is indeed a 20a charge max
```

---
