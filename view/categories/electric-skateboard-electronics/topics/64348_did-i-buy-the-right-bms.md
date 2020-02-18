# Did I buy the right bms?

### Replies: 26 Views: 856

## \#1 Posted by: TiMMaTTie Posted at: 2018-08-09T14:40:25.518Z Reads: 166

```
Hi,

I got tired of opening my enclosure to charge lipos and ordered a bms I intend to use for charging only. I started looking at some wiring diagrams and got kind of confused. I bought the following cheap BMS without much information: https://www.ebay.com/itm/222272460111.

The only pads I am seeing are B+, B- and P-. I see most other BMS diagrams feature a C or CH port. Is this bms good for discharging only or should I connect the battery ground to p-?

Thanks!
```

---
## \#2 Posted by: b264 Posted at: 2018-08-09T14:49:33.816Z Reads: 160

```
The battery negative always connects to B-

If there is no C- port then the charge jack negative connects to P-
```

---
## \#3 Posted by: TiMMaTTie Posted at: 2018-08-09T15:27:51.155Z Reads: 153

```
Thanks, I understand. I'm only charging with 2A, so shouldnt matter if I use the last balance lead of the second lipo (2*4s) or the large/main ground wire right?
```

---
## \#4 Posted by: b264 Posted at: 2018-08-09T15:30:49.904Z Reads: 145

```
If you're charging at 2A there shouldn't be a problem using only the balance leads.  As long as you're only using the BMS for charging and not for discharging.  That specific BMS isn't even one that could be used for discharging, so you're okay.  You should put a 5A automotive fuse on the charge jack though, if you can.
```

---
## \#5 Posted by: Superflim Posted at: 2018-08-09T15:47:16.553Z Reads: 130

```
why would you only use a bms for charging?
```

---
## \#6 Posted by: b264 Posted at: 2018-08-09T15:50:45.936Z Reads: 128

```
So your brakes can never cut-out.  Or because your BMS is rated for 5A and you are drawing 80A peak.  Or because you want to remove a possible failure point in your drivetrain.

I'd rather slightly overcharge my battery and reduce its lifespan SLIGHTLY than have my brakes cut out because I hit the brakes on a big hill with a fully-charged battery and when the battery got full, the BMS cuts off charging.

And then of course the #1 reason: cost
```

---
## \#7 Posted by: pedro Posted at: 2018-08-09T16:54:21.949Z Reads: 114

```
I buy this bms, the description say is a normal bms, safe for charging and discharge. but i'm suspicious with circuit, because i don't have -P port

![bms|448x500](upload://bBDUe6E38r337h9a7hLq5c67eKR.JPG)

https://www.banggood.com/pt/37V-42V-10S-45A-Li-ion-Battery-Protection-Board-BMS-PCB-System-p-1177351.html?gmcCountry=PT&currency=EUR&createTmp=1&utm_source=googleshopping&utm_medium=cpc_elc&utm_content=2zou&utm_campaign=pla-all2-pt-pc&gclid=EAIaIQobChMIrNbyxbfg3AIVBoXVCh1kFwVhEAQYASABEgKW4_D_BwE&cur_warehouse=CN
```

---
## \#8 Posted by: b264 Posted at: 2018-08-09T17:03:19.811Z Reads: 105

```
It would appear C- is the P- port on this specific one.

Beware that running the ESC from C- will POSSIBLY cut-out the brakes on full battery conditions.  It really depends a lot on the internal design of the BMS.

Edit: this one does cut off brakes if the battery hits 42.8 ± 0.5 V
```

---
## \#9 Posted by: TiMMaTTie Posted at: 2018-08-09T19:03:12.464Z Reads: 94

```
Using a magsafe instead of jack actually, but I'll keep it in mind, thanks!
```

---
## \#10 Posted by: rey8801 Posted at: 2018-08-09T19:06:36.855Z Reads: 93

```
As @b264 said. It will cut off your brakes even if you charge the battery to 41V instead of 42. In the first kilometers if you brake hard it will cut your brakes. I learnt it in the wrong way :tired_face: Use it charging only!
```

---
## \#11 Posted by: b264 Posted at: 2018-08-09T19:14:15.167Z Reads: 89

```
[quote="rey8801, post:10, topic:64348"]
It will cut off your brakes even if you charge the battery to 41V instead of 42.
[/quote]

Maybe.  It depends on a lot of things.  It most certainly CAN though.  Envision the scenario where the total pack voltage is 41V but a few cells got unbalanced because the pack is old -- and once one single cell hits 4.2V the BMS can cut off charging to the whole pack, effectively killing your brakes.  Not that I want to damage my battery, but if the alternative is cutting the brakes at high speed, I'll take slight battery damage in that rare scenario.
```

---
## \#12 Posted by: rey8801 Posted at: 2018-08-09T19:16:06.974Z Reads: 81

```
The overvoltage to the battery is gonna be for few sec so not a big deal to me. On the other hand don't have brakes will 100% damage you in few sec :laughing:
```

---
## \#13 Posted by: pedro Posted at: 2018-08-09T22:13:24.810Z Reads: 74

```
so, im fuck....prefer be safe, what BMS you guys have?
```

---
## \#14 Posted by: b264 Posted at: 2018-08-09T22:24:22.550Z Reads: 72

```
The Bestech D190 is a good one.  You will be fine, I just would not route the ESC negative wire through the BMS.
```

---
## \#15 Posted by: pedro Posted at: 2018-08-09T22:27:44.070Z Reads: 70

```
just to make clear!
this BMS can balance the cells on charging!
and (can/cant) balance the cells on discharging?
for brake i can´t trust!
And how works the break sistem, i thought if you not accelerate, the longboard automatically braake because the motor work like a resistance.
if I, move back with the remote controle, will probrably brake?
```

---
## \#16 Posted by: pedro Posted at: 2018-08-09T22:48:46.465Z Reads: 67

```
10A!!
if the battery are 36 volts, you just have 10A*36V=360Watts, what is the power of your motor? and the speed you can get
```

---
## \#17 Posted by: b264 Posted at: 2018-08-09T22:49:49.320Z Reads: 68

```
If you aren't discharging through the BMS (and also charging the regenerative power through the BMS) then the 10A only applies to charging with the charger and not discharging
```

---
## \#18 Posted by: pedro Posted at: 2018-08-09T23:06:14.878Z Reads: 64

```
true, so you have a bypass. i dont know if i go to this way, because the battery, probably will be unbalanced
```

---
## \#19 Posted by: b264 Posted at: 2018-08-10T02:29:27.963Z Reads: 62

```
It won't be unbalanced if you charge through the BMS but don't discharge through the BMS.
```

---
## \#20 Posted by: pedro Posted at: 2018-08-10T08:29:03.163Z Reads: 56

```
i don't remember which topic was, but i remember to read, the bms stop charging after the first cell reach 3.6 V, so the others will be lower, is this right?
```

---
## \#21 Posted by: TiMMaTTie Posted at: 2018-08-10T21:43:19.918Z Reads: 50

```
Okay so I connected the BMS and started charging. The charger LED was red, meaning it was charging. After a while I disconnected and checked voltages, both lipos on 16.9V which is normal since the charger stops at 4.25V per cell.

However, when I reconnected everything (without the charger), the BMS got quite hot. I noticed that this happened when I connected the balance cables. So I am assuming I wired something wrong but have no idea what... The esc wires are not connected which should not matter right?

I have wired it like this:![s-l1600|615x500](upload://urmd9fVtuRkOfaaEfg4YMecHdsX.jpg)
```

---
## \#22 Posted by: Brdchris Posted at: 2018-08-11T01:51:26.448Z Reads: 42

```
Don’t forget, charge only bms’s are normally much smaller also. And having a seperare e switch means being able to charge with your speed controllers off.
```

---
## \#23 Posted by: TiMMaTTie Posted at: 2018-08-11T11:12:05.785Z Reads: 39

```
Does anyone know how I could check if the BMS is fried?
```

---
## \#24 Posted by: TiMMaTTie Posted at: 2018-08-11T12:26:46.432Z Reads: 44

```
I just realized that I connected balance cables to the BMS before I connected B-, could this be the problem?
```

---
## \#25 Posted by: pedro Posted at: 2018-08-15T10:41:38.254Z Reads: 43

```
And this BMS or PCB, do you thin is safe? and can have brakes in my eletric longboard

You can change the pictures, for easy view

https://bmsbattery.com/bmspcm/330-smart-bms-513-cells-in-series-bms-pcm.html#idTab5
```

---
## \#26 Posted by: pedro Posted at: 2018-09-03T11:29:26.182Z Reads: 35

```
Hello, i found this bms, have -p port, do you thing is safe for use, my brake  sisteam will not fail?

http://www.batterysupports.com/36v-37v-42v-10s-45a-10x-36v-lithium-ion-lipolymer-battery-bms-p-266.html
```

---
