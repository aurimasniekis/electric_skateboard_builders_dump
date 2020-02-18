# Charging 12s? Need Help!

### Replies: 16 Views: 1859

## \#1 Posted by: Johnosu1 Posted at: 2016-06-21T20:58:49.828Z Reads: 160

```
I would love some help on my newbie delema lol. I am running 4 3s 30c 5000 mah in series and was wondering once i wire them all together how to charge them. I would like to put a charging port on the outside of my electronic's box. I would like something like plugging in a laptop so that i dont have to carry around a bulky charger. Is this possible?? i just dont want to ruin the new battery's i just bought but i am clueless in the subject.:) Thanks guys
```

---
## \#2 Posted by: Jack Posted at: 2016-06-21T21:05:40.541Z Reads: 155

```
@Johnosu1 Hey for the laptop style charger you talk about you will need a BMS which balance charges your cells for you, if you don't have a 12s charger this might be the best way to go. There are methods of charging your packs in parallel with a 6s charger but I would recommend a BMS as it's much easier. Just requires fitting another PCB under your board. If you've got space go for it! Get a 12s BMS thats rated for at least 60a.

Jack
```

---
## \#3 Posted by: Johnosu1 Posted at: 2016-06-21T21:23:53.130Z Reads: 145

```
Do you recommend any good place to get a bms??
```

---
## \#4 Posted by: Johnosu1 Posted at: 2016-06-21T21:26:31.976Z Reads: 139

```
also I am running a single 149kv sk3 if that matters.
```

---
## \#5 Posted by: Jack Posted at: 2016-06-21T21:27:51.112Z Reads: 126

```
http://www.batterysupports.com/44v-48v-504v-12s-60a-12x-36v-lithium-ion-lipolymer-battery-bms-p-270.html

This should be good, I am using the 10s version. :slight_smile:
```

---
## \#6 Posted by: Johnosu1 Posted at: 2016-06-21T22:24:02.631Z Reads: 120

```
so what do you use to plug into the wall with??
```

---
## \#7 Posted by: mason Posted at: 2016-06-21T22:44:11.357Z Reads: 119

```
60a? I thought we need 100+, although I could be wrong. I'm not very familiar with this type of stuff but would love to learn.
```

---
## \#8 Posted by: Johnosu1 Posted at: 2016-06-21T22:52:50.121Z Reads: 118

```
Ya me too @link5505. Im just a big kid that wants fast toys lol But i am not sure what the max amp out put of the motor i have??
```

---
## \#9 Posted by: Johnosu1 Posted at: 2016-06-22T00:40:13.225Z Reads: 108

```
what about something like this 
http://www.batterysupports.com/432v-44v-504v-4a-lithium-ion-lipo-battery-charger-12s-12x-36v-p-167.html
```

---
## \#10 Posted by: lox897 Posted at: 2016-06-22T00:53:40.697Z Reads: 104

```
Looks good. Your batteries can be charged at 5ah so that charger will work.
```

---
## \#11 Posted by: Johnosu1 Posted at: 2016-06-22T01:08:25.728Z Reads: 98

```
so that can be wired right in to the power leads between the vesc and the batterys?? what do i do with the balance charging wires??
```

---
## \#12 Posted by: lox897 Posted at: 2016-06-22T01:15:19.331Z Reads: 98

```
Plug it into the BMS. Just realised this from another thread, the BMS accepts a 9S connector and your ground wire goes straight to the BMS. You will need to buy something like this and solder the leads on: http://www.ebay.com/itm/9S-JST-XH-2-5MM-XH2-5-Connector-balance-wire-50CM-Cable-CellLog-18650-battery-/151933130079?hash=item235feb955f:g:v4EAAOSwHPlWgd4d
```

---
## \#13 Posted by: Johnosu1 Posted at: 2016-06-22T01:15:52.562Z Reads: 98

```
ok so even with that charger i would need a bms
```

---
## \#14 Posted by: Johnosu1 Posted at: 2016-06-26T21:23:17.369Z Reads: 79

```
After looking into it further and with the advice of @Pablo_702 i am going to get a dual 6s charger and make a harness to make it a 12s pack when using the board but charge the packs as 2 6s packs. thanks guys!!
```

---
## \#15 Posted by: Pablo_702 Posted at: 2016-06-27T05:56:39.397Z Reads: 75

```
Or you could get any single 6s charger and charge 1 pair (2 x 3s= 1 6s) out of time
```

---
## \#16 Posted by: TomasSyster2.0 Posted at: 2016-11-27T09:06:02.140Z Reads: 45

```
I have the same setup witch charger did you get?
[quote="Johnosu1, post:14, topic:4963"]
dual 6s charger
[/quote]
```

---
