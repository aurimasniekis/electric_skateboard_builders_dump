# 6S4P 18650 Samsung Setup - Need Help

### Replies: 10 Views: 869

## \#1 Posted by: FrozenFury Posted at: 2016-08-12T05:00:54.165Z Reads: 158

```
I'm doing a 6S4P setup of 18650 Samsung batteries and I need some help. These are probably dumb questions, so sorry in advance. I'm a beginner who wants to learn more.

- Should I individually heat shrink tube each cell with [this](https://www.amazon.com/29-5MM-%C2%A6%C2%B518-5MM-Shrink-Tubing-Battery/dp/B00OPXLEXK/ref=sr_1_1?ie=UTF8&qid=1470977039&sr=8-1-spons&keywords=18650+heat+shrink&psc=1)?

- Should I heat shrink wrap the entire 6S4P setup? If so, what millimeter size wrap would I need to cover it?

- With [this motor](http://www.hobbyking.com/hobbyking/store/__18127__Turnigy_Aerodrive_SK3_6354_260kv_Brushless_Outrunner_Motor.html), will a 6S4P setup be fine? Or will it not work together?

- What type pure nickel roll should I use to spot weld the batteries?

- Will [this BMS](http://www.ebay.com/itm/221844012026?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT) work with my setup and what connector do I use to attach it to the ESC? Also do I connect the BMS to the batteries by soldering it?

- Will [this charger](http://www.ebay.com/itm/321751878865?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT) work and to connect it to the batteries, do I use a Anderson SB50 connector and an XT 90 anti spark connector?  

- If I solder the BMS to the batteries, would I use 10 AWG, 12 AWG, or 14 AWG? Or do I use those wires somewhere else?

- How do I connect an on/off switch and battery voltage meter to the setup? What would I use? 

- To attach the BMS safely to the batteries, should I use heat resistant adhesive tape? 

- Is there a diagram or specific way to spot weld/solder my batteries together? Since it's a 6S4P setup, I have 24 batteries, and to make it as thin as possible I want to do two rows with 12 batteries each. Is that possible? If so, how would I do it?

- I don't know how to spot weld so I'm going to go into a shop and have someone do it for me. Would an auto body shop be able to do it for me, and how much do you think such a service would cost?

Thanks!!
```

---
## \#2 Posted by: lox897 Posted at: 2016-08-12T06:03:03.148Z Reads: 149

```
Please stop creating multiple threads. Keep your questions in one thread.

Now onto your questions:

1. Don't heat shrink each cell
2. I would do two packs of 3s 4p and heat shrink each one so they don't short. Like @longhairedboy does.
3. That motor will work. Apparently 245kv is the best for 6s.
4. .15mm 10mm wide pure nickel
5. Get an 80amp bms because you have 4p and each cell is 20amp.
6. That charger will work, it should come with the connectors.
7. 10 AWG
8. Wire it like this: Battery > BMS > On/off switch > volt meter > esc
9. Use heat resistant tape like kapton
10. Look at @link5505 and @whitepony diagrams.
11. Get someone like @barajabali to spot weld your packs. He might as well make the whole pack.
```

---
## \#3 Posted by: ofekp Posted at: 2017-02-13T21:53:48.342Z Reads: 88

```
OMG, but I have a 190kv motor! Based on what do you say that 245kv is best for 6S?
Also, if I have a 6S LiFePo4 can I still use the same charger @FrozenFury suggested?

Thanks!
```

---
## \#4 Posted by: lox897 Posted at: 2017-02-14T00:51:57.498Z Reads: 82

```
245kv would be better yes. You will need a different BMS & Charger for your lifepo4 chemistry, they have a different charged voltage than lithium ion
```

---
## \#5 Posted by: ofekp Posted at: 2017-02-15T21:58:00.241Z Reads: 70

```
Ho no... I was counting on the rule of "the lower KV the better"... I guess I have another delivery to wait for now :(
Would you say it is important to go with a sensored motor? The motor suggested by @FrozenFury is not sensored.
Do you think anything will change if I use 9S1P? Cuz I have another 3S battery I can use. What motor will fit this setup best?

Thanks again!
```

---
## \#6 Posted by: lox897 Posted at: 2017-02-16T02:22:30.927Z Reads: 70

```
9s1p with 190kv will work great
And sensored motors don't matter, just push off and go
```

---
## \#7 Posted by: ofekp Posted at: 2017-02-16T14:56:45.556Z Reads: 67

```
You're awesome! Thank you so much!
```

---
## \#8 Posted by: Northlake Posted at: 2017-04-06T01:53:11.090Z Reads: 51

```
@ofekp keep the 190kv motor and just change your belt!!! if you use a 265mm (18T/36T) belt it corrects your motor so that it's as if you're running 9s1p at 190kv! but you're actually running 245kv at 6s! PROFIT $$$
```

---
## \#9 Posted by: ofekp Posted at: 2017-04-07T19:28:19.099Z Reads: 46

```
I am currently running 15/40 gear ratio, I can switch to 20/40 which will give me this ratio,
or I can get bigger wheels too right?

Thanks man :)
```

---
## \#10 Posted by: Northlake Posted at: 2017-04-08T15:28:11.459Z Reads: 41

```
Yea, my scenario was for 83mm wheels :P GLHF and no problem! we're all here to help.
```

---
