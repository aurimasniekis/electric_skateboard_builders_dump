# Li-Po Series connection issues

### Replies: 31 Views: 423

## \#1 Posted by: Tachun Posted at: 2018-10-19T06:56:03.370Z Reads: 111

```
Hello,

I know theres probably someone who already had the same issue as me..

Im trying to connect 4 6s 4500mAh Lipos in series and paralell, and im having issues connecting them up.
The Lipos are balanced and charged to the same voltage but as soon as i connect them up my connectors burn out. I already redid the wiring for the balance leads and the xt60 connectors that im using, my setup works fine with just two Li-Po`s in series. Maybe someone has a idea what i could be doing wrong. 

My Setup:
170Kv Motor
40A Contactor with constant current source in paralell to precharge the Caps of my VESC and keep my contacts from dying
12S BMS
40A Fuse

Also sorry for any spelling errors i dont do english posts very often c:
```

---
## \#2 Posted by: Andy87 Posted at: 2018-10-19T07:03:30.259Z Reads: 107

```
upload some pictures and a diagram how you wired everyting up.
will help us to solve your problem.

and i didn´t understood what exactly burn out when you connect your packs in parallel. you wrote your connecots burn out.
you mean the xt60 connectors?
```

---
## \#3 Posted by: Tachun Posted at: 2018-10-19T07:22:12.632Z Reads: 102

```
Im not home atm, ill upload a picture when i can.

Im getting a spark when im connecting up my Lipos, i dont know why they are balanced and at the same voltage level, ive charred two connectors already and i have no ideay why.
```

---
## \#4 Posted by: mynamesmatt Posted at: 2018-10-19T08:18:51.726Z Reads: 93

```
you need an antispark first of all. wouldn't be using a precharger separate
```

---
## \#5 Posted by: TowerCrisis Posted at: 2018-10-19T08:23:02.368Z Reads: 89

```
If they're actually at the same voltages then you're definitely wiring something up wrong. You don't need an antispark between the backs, assuming that you'll be using a BMS.
```

---
## \#6 Posted by: Tachun Posted at: 2018-10-19T08:45:12.016Z Reads: 90

```
I had one but it died on me, i guess i had cheap knockoff fets on it..

Im currently building my own im just using the contactor while im doing that
```

---
## \#7 Posted by: Quezacotl Posted at: 2018-10-19T09:23:31.110Z Reads: 83

```
First thing coming to my mind, is that maybe you are connecting parallel cells plus to minus, the same way as series. Or two series and one parallel between them.
Just remember, parallel is plus to plus, series is plus to minus.
```

---
## \#8 Posted by: dareno Posted at: 2018-10-19T09:48:56.318Z Reads: 80

```
@J0ker3366 wheres the lipo king?  You're up.
```

---
## \#9 Posted by: Andy87 Posted at: 2018-10-19T09:56:59.855Z Reads: 82

```
let @Tachun upload his diagramms and pictures and than our lipo king can manage everything... at the moment it´s just guessing
```

---
## \#10 Posted by: lrdesigns Posted at: 2018-10-19T09:58:17.581Z Reads: 81

```
I don’t know what you got going on without pics. But my setup is 12s lipos but I charge 6s parallel x2. 

To charge I need to disconnect both plus and minus main power cables with two loop keys. Or that shit shorts out the balance wires. I have forgot a few times to un plug the two loop keys and it’s a bad seen. It vaporizers the pins in the balance plug. :scream:
```

---
## \#11 Posted by: dareno Posted at: 2018-10-19T09:58:42.888Z Reads: 79

```
Hes asleep anyway.
```

---
## \#12 Posted by: Andy87 Posted at: 2018-10-19T10:10:17.412Z Reads: 78

```
ok than let´s tag @J0ker3366 here once more that he will not pass it in the morning... :sweat_smile:
```

---
## \#13 Posted by: Tachun Posted at: 2018-10-19T11:38:17.884Z Reads: 75

```
![Bad%20wiring|500x500](upload://hk276LGjmMGGt22xGjw7jmRlejG.jpeg) 

I dont know if theres anything wrong with it...

also this looks like it was made with ms paint..
```

---
## \#14 Posted by: TowerCrisis Posted at: 2018-10-19T13:26:08.570Z Reads: 67

```
Is it sparking when you connect the parallel packs together, or when you connect the series ones?

Does it spark if you leave the balance wires completely disconnected from each other?
```

---
## \#15 Posted by: Tachun Posted at: 2018-10-19T13:28:10.113Z Reads: 67

```
it sparks when i connect the series packs, the balance wires are fine
```

---
## \#16 Posted by: Okami Posted at: 2018-10-19T13:30:35.042Z Reads: 66

```
I found about this hard way also..

 u cannot connect both series and parallel at the same time.. otherwise it shorts the battery / connectors as @lrdesigns pointed out..

U need to install manually operated switch, to switch between 6s charging and 12s discharge..

If 12s discharge is on loop key, then u can either add one more loop key for opposite polarity wire and charge when both keys are removed

Otherwise u need 4 port balance charger (or 4 chargers) and charge seperately through balance wires only
```

---
## \#17 Posted by: TowerCrisis Posted at: 2018-10-19T13:31:52.260Z Reads: 65

```
That's no bueno.. are the vesc's connected when you connect them? Is the BMS connected when you connect them?
```

---
## \#18 Posted by: TowerCrisis Posted at: 2018-10-19T13:33:30.837Z Reads: 64

```
He is using a BMS, he can charge all of them at once with a 12S charger
```

---
## \#19 Posted by: J0ker3366 Posted at: 2018-10-19T19:20:12.140Z Reads: 60

```
Yeah bruv, pictures of your current wirring set up would be great.
```

---
## \#20 Posted by: Namasaki Posted at: 2018-10-19T22:28:25.791Z Reads: 55

```
Surely this can't be right.
Why would there be a a pin after pin 12 that goes to the battery positive when pin 12 is already connected to the battery's main positive?  Assuming that this is in fact a 12s bms.
![15%20PM|289x138](upload://ar0xDp31TIu0e7z1IXrMgwa9HvM.png)
```

---
## \#21 Posted by: TowerCrisis Posted at: 2018-10-20T01:55:02.165Z Reads: 48

```
He's probably mistaken, I'd bet pin 1 goes to the pack negative.
```

---
## \#22 Posted by: Namasaki Posted at: 2018-10-20T02:51:16.627Z Reads: 49

```
Well, hopefully we can help him get it sorted out before the smoke comes.
```

---
## \#23 Posted by: Andy87 Posted at: 2018-10-20T06:01:48.674Z Reads: 43

```
@Tachun any update on it? You already figured it out by your own?
```

---
## \#24 Posted by: Tachun Posted at: 2018-10-21T20:21:03.991Z Reads: 41

```
Sorry for the late reply

![s-l400|400x223](upload://ltwdZPifyMVuMMqbQmbbtWpXEbX.jpeg)

Here's the picture the manufacturer has on their website
```

---
## \#25 Posted by: Tachun Posted at: 2018-10-21T20:31:36.005Z Reads: 40

```
Well I re-did all my wiring and connections to make sure nothing is wrong.. 

The long red cables are my balancing wires I connected all 4 of my 6s lipos up to make sure that the voltages are correct which they where.
I charged and balanced all my lipos to the exact same voltage and tried connecting them.

I don't understand why my connector is burnt they are already connected via the balance cables and it shouldn't matter if it's connected again in parallel via the higher gage discharge cables.

![IMG_20181021_222344|375x500](upload://mDPZbr2X4hmx8Er0ggzsuxsP3XP.jpeg) ![IMG_20181021_222458|375x500](upload://cn4ocGdzMPzXBaLbDclsMCfULZZ.jpeg) ![IMG_20181021_222512|375x500](upload://ff6ZaYdfp5OUV4ZoSIN2Q6msYCr.jpeg)
```

---
## \#26 Posted by: Namasaki Posted at: 2018-10-21T21:32:52.482Z Reads: 36

```
your drawing is showing an additional pin after pin 12 on the bms balance connector where you have the battery main connected.

The manufacturers drawing shows the 12th balance pin connected to the positive side of the 12th cell along with the main positive supply wire.
```

---
## \#27 Posted by: Tachun Posted at: 2018-10-21T22:26:00.139Z Reads: 34

```
Yeah I know that was wrong, my issue is not about the bms that works fine, the balancing charging and discharging works fine. I just cannot connect two 6s lipos parallel without creating a spark and killing the connector.

I don't know whats wrong, there shouldn't be any current when I plug my lipos in, they are at the same voltage and there is no load connected
```

---
## \#28 Posted by: Namasaki Posted at: 2018-10-22T01:36:08.234Z Reads: 33

```
does it spark when you plug the first pack into the pigtail?
or how many pack can you connect before it sparks?
```

---
## \#29 Posted by: TowerCrisis Posted at: 2018-10-22T01:48:43.332Z Reads: 30

```
Does it spark when you have the balance wires disconnected from eachother
```

---
## \#30 Posted by: Tachun Posted at: 2018-10-23T15:42:57.338Z Reads: 22

```
Yeah that too.. When I connected everything up everything was fine I could connect the balance wires and the first parallel pack but when I wanted to plug in the first series pack I had a spark while connecting
```

---
## \#31 Posted by: TowerCrisis Posted at: 2018-10-24T07:14:42.099Z Reads: 17

```
I mean EVERYTHING disconnected. Does it spark when absolutely no balance wires are connected between any series or parallel cells.
```

---
