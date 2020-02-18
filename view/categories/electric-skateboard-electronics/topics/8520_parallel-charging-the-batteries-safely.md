# Parallel Charging the batteries safely?

### Replies: 14 Views: 790

## \#1 Posted by: Duarte Posted at: 2016-08-28T20:28:19.922Z Reads: 135

```
Hey guys
I'm building my first eboard and I came across a problem, I'm going to use 8 Multistar High Capacity 4S 5200mAh (http://www.hobbyking.com/hobbyking/store/__65268__Multistar_High_Capacity_4S_5200mAh_Multi_Rotor_Lipo_Pack_EU_Warehouse_.html) and I want to charge them in parallel.
My question is, since I'm charging them in parallel the batteries would have combined 615,680W and the charger that a want to use as a limit off 100W (http://www.hobbyking.com/hobbyking/store/uh_viewitem.asp?idproduct=80422), would it be save to charge the batteries in parallel with this charger? Or would I nedd to use another charger with a higher Watts capacity?
```

---
## \#2 Posted by: Hummie Posted at: 2016-08-28T21:06:39.931Z Reads: 123

```
The watt hours of the battery doesn't matter.  You could charge them in parallel.   You will just be charging slowly at 100 watts
```

---
## \#3 Posted by: Duarte Posted at: 2016-08-28T21:57:53.306Z Reads: 114

```
That's great :smile:
Thanks for the information!
```

---
## \#4 Posted by: torqueboards Posted at: 2016-08-28T21:58:14.008Z Reads: 112

```
Perfectly safe to charge in parallel. I prefer it. You need a higher quality charger. I'd recommend the iCharger 208B + 350W HK Power Supply. Otherwise, charging in parallel will take way too long.
```

---
## \#5 Posted by: Duarte Posted at: 2016-08-28T22:43:17.128Z Reads: 93

```
That's a good tip but it's a bit pricey for me in the moment since I'm already spending a lot of money in the batteries and other components, but will consider getting a better AC charger since they are cheaper and don't need a power supply, but in the future I will buy one of those with dual charging capability since I wan't to upgrade my board to an 10S and that way I can charge all the batteries at the same time
```

---
## \#6 Posted by: torqueboards Posted at: 2016-08-29T03:17:17.285Z Reads: 88

```
IMO Don't get dual charging it's pointless if your only trying to charge in parallel. Purchase the iCharger 208B $120 and a 350W HK Power Supply $40. We'll worth it.
```

---
## \#7 Posted by: Duarte Posted at: 2016-08-29T09:40:26.747Z Reads: 76

```
What if i got one with the capability to charge 4 at once and charge 4 4S batteries in two of then and 4 6S in the other, so I would be charging 16 batteries in total, would that be worth the money spend?
```

---
## \#8 Posted by: DeathCookies Posted at: 2016-08-29T09:56:25.976Z Reads: 70

```
If you want to charge about 16 batteries you will need a high amperage power supply + charger otherwise you will need days to charge!
```

---
## \#9 Posted by: Duarte Posted at: 2016-08-29T11:23:27.831Z Reads: 64

```
Will 1000 plus W be enough to charge it quickly?
```

---
## \#10 Posted by: DeathCookies Posted at: 2016-08-29T11:33:16.502Z Reads: 64

```
W = U * I
W / U = I

W = 1000
U = (6S batteries) 22,2V
I = X

1000 / 22,2 = 45A

If you are charging 10 6S batteries in parallel you get (45A / 10 = ) 4,5A per battery and will charge a 5Ah pack in about 1 hour.

So yes, charger with 1000W would be good for so many batteries. But i dont think you will find a good AD/DC charger with so much wattage. I think you have to buy a power supply and a dc charger.

Maybe i can offer you my [1080W power supply](http://www.hobbyking.com/hobbyking/store/__20611__Turnigy_1080W_100_120V_Power_Supply_13_8V_18V_60amp_.html) for a cheap price. My one is with **EU PLUG**!
```

---
## \#11 Posted by: torqueboards Posted at: 2016-08-29T16:51:25.150Z Reads: 51

```
Typically, a parallel charging board only allows for 6 batteries at a time.

To charge 16 batteries at a time, you'll need to make a custom connector.
```

---
## \#12 Posted by: DeathCookies Posted at: 2016-08-29T16:56:23.568Z Reads: 48

```
What is when You plug a parallel board in a parallel board? Should work?!
```

---
## \#13 Posted by: Duarte Posted at: 2016-08-29T18:36:48.680Z Reads: 45

```
I'may working on building my batteries in a modular case, so the conectores use to connect the batteries in parallel can be use to charge them also rigth?
```

---
## \#14 Posted by: DeathCookies Posted at: 2016-08-30T08:03:46.943Z Reads: 38

```
It sounds right but it would be better if you can draw a schematic or wiring. Then the people can approve or not approve your idea ;)
```

---
