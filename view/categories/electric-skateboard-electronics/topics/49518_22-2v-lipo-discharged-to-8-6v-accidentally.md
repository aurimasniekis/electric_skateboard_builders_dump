# 22.2V LiPo discharged to 8.6V accidentally

### Replies: 11 Views: 483

## \#1 Posted by: Armitage Posted at: 2018-03-19T14:20:16.009Z Reads: 62

```
Hello, i accidentally left my board on and it discharged the 2x3s 22.2v battery to 8.6v. Is there any possible and safe way to charge them back up or is it better to just throw them away?
```

---
## \#2 Posted by: TarzanHBK Posted at: 2018-03-19T14:25:40.073Z Reads: 59

```
If they are not puffy, charge them reaaaaaally slow and keep an eye on them.
If they are swelling, throw them away.
Otherwise charge them up and run them down to 3,6V a few times and see if a cell is drifting.
If you´re lucky they are still working but lost capacity
```

---
## \#3 Posted by: SeanHacker Posted at: 2018-03-19T14:26:20.098Z Reads: 58

```
You could just go here and get some info. lol. ;) http://www.electric-skateboard.builders/t/lipo-22-2v-discharged-to-8v-help-on-discharge-cut-off/49402
```

---
## \#4 Posted by: DeathCookies Posted at: 2018-03-19T14:26:41.126Z Reads: 56

```
You can resurrect them but it is tricky.

first of all: Charge slowly!!!
second of all: you Need to watch the battery because now it can easily take fire!
third: get the Charge going with some tricks.... Most Balance charger will not let you Charge such a battery because of the unhealty under voltage. To still Charge it, just select analog power on your charger until it is in a chargable range
```

---
## \#5 Posted by: Armitage Posted at: 2018-03-19T14:30:12.807Z Reads: 50

```
It's actually also my post but about a different problem.
```

---
## \#6 Posted by: Armitage Posted at: 2018-03-19T14:31:34.791Z Reads: 52

```
Thank you all, but right now I only have the turnigy b6 charger that is automatic. I think I'll order new batteries and a bms.

Do u think that this one is okay or too sketchy? It also says for Li-ion but can I still charge LiPo's?
[6s 50A BMS](https://www.aliexpress.com/store/product/6S-50A-bms-2017-new-Li-ion-50A-large-high-current-BMS-PCM-with-SAME-port/1821822_32826354127.html?spm=2114.12010612.0.0.29a63632cXR9Ve)
```

---
## \#7 Posted by: DeathCookies Posted at: 2018-03-19T14:50:27.482Z Reads: 45

```
The difference between LiPo and a LiIon BMS are the cutoffs.
LiIon 2.5-4.2
LiPo 3.3-4.2

I think that 6S 50A is to less.... i do not prefer 6S at all but if you go that route aim about 80-100A and give the bms some breathing room (>120A)
```

---
## \#8 Posted by: Tuomalar Posted at: 2018-03-19T14:52:29.523Z Reads: 46

```
OR Just bypass it and use only for charging and use vesc's voltage cutoff.
```

---
## \#9 Posted by: Armitage Posted at: 2018-03-19T15:24:40.080Z Reads: 41

```
Yeah I think I'll choose that. But is there any device such as a LiPo alarm but as a switch that turns the power out when the cells are too low(because i have a 5v adapter also connected and that would still draw power when xt90 loop is connected)?

Is this one good, if I'm bypassing discharging? It says for Li-Ion and Lipoly: https://hobbyking.com/en_us/6s-li-ion-10a-pcm.html

or this: https://hobbyking.com/en_us/6s-li-ion-pcm-charge-4a-discharge-10a.html?wrh_pdp=7
```

---
## \#10 Posted by: Tuomalar Posted at: 2018-03-19T15:56:45.407Z Reads: 31

```
Nothing comes to mind. Just power of your board right away when you don't use it.
And first one looks fine.
```

---
## \#11 Posted by: Armitage Posted at: 2018-03-19T15:58:19.513Z Reads: 29

```
Thank you!! :slight_smile:
```

---
