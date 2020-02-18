# Mountainboard please review my build

### Replies: 17 Views: 509

## \#1 Posted by: kanies Posted at: 2019-08-29T11:40:42.900Z Reads: 147

```
Hi,
Firstly I would like to start that I want to build my own mountainboard.
I have used calculator found on this forum and my top speed should be about 45km/h.
I think that I have thought through my design, but what do I really know? :slight_smile:

Basicly I am depending at you! Please give me a feedback and tell me what can go wrong.

1. Motors: 2x FATJAY 6368 190kV D-shaft sensored (14 poles), they are about 800W each and max current is 65A.
https://pl.aliexpress.com/item/32908081789.html?spm=a2g0s.8937460.0.0.15a42e0eMZA4LA

2. Power cells: 10s6p battery, made from 18650 cells. I want to build my battery like a schematic below:
https://pl.aliexpress.com/item/32887423130.html?spm=a2g0s.8937460.0.0.3b242e0esvciGF
![bms|690x446](upload://gYkFGdCl8d7vlbkiflugWcFG6vX.png) 

3. BMS: I want to go with 25A 36V and seperate port. I tried to read how to choose this component but it gave me the most headache. Here I think I need some help.
https://pl.aliexpress.com/item/32875971231.html?spm=a2g0s.8937460.0.0.25fb2e0eXpQ6C5

4. Anti-Spark:
https://pl.aliexpress.com/item/4000055170478.html?spm=a2g0o.productlist.0.0.5bcf70behqTNpV&algo_pvid=1383da22-f23d-4a4c-bca1-82b67adeac53&algo_expid=1383da22-f23d-4a4c-bca1-82b67adeac53-0&btsid=cea2d584-ce3f-49a1-b65b-bd56fb1a8d85&ws_ab_test=searchweb0_0,searchweb201602_5,searchweb201603_52

5. 2x VESC: HGLRC FLIPSKY FSESC 50A V4.12 - I do not know If I choose a good controller? I wanted it to be powerfull to manage those 190kV motors. From what I understand I can connect them together like in the photo below:
https://pl.aliexpress.com/item/32913068461.html?spm=a2g0s.8937460.0.0.291c2e0eo0M2VY
![Esk8%20Construction%20Diagram%20-%2012s5p%2C%20x2%20FocBox|690x292](upload://vDSURjLf12rDgHKnpagWbSQ1rVT.jpeg) 

What do you think? All the components are choosed wisely? Is there some part that prevents other from working in 95% of its capability?

Thank you for all hints!
```

---
## \#2 Posted by: kanies Posted at: 2019-08-30T06:19:30.801Z Reads: 132

```
The most concerns I have with BMS that it might have less power that I need? One motor have 864W and in peak it can go 2340W. So basicly 24A in normal mode and in peak about 60A.

Does it mean that I need 10s 60A BMS? Or 25A BMS can handle about 60A in peak?

:smile: anyone?
```

---
## \#3 Posted by: ZackoryCramer Posted at: 2019-08-30T06:43:48.113Z Reads: 126

```
I am guessing you have some way of cutting a keyway on that motor because set screws will *screw* you over.
```

---
## \#4 Posted by: Tinp123 Posted at: 2019-08-30T06:49:25.010Z Reads: 126

```
where to start... your battery choice is wrong. Those cells are rated on Mooch test as so-so 4.9A battery. In 6P configuration, your battery could output barely 30A. I don't even know how much will they sag, but probably very very much. Use samsung 30Q, which is some standard. 

which ever bms you get, you can wire it for charge only (you will use anti-spark). in this configuration, bms discharge rate doesn't matter. 

about anti-spark. I would probably buy one with good reputation on forum, instead of random one from aliexpress. you could use loop key too, cheaper and more secure option.

think twice about your battery configuration. 6P in one layer will be about 55cm long. you will have to use wires for series connections, because nickel will break quickly (because every board flexes and that will create forces on nickel in series connection)

flipsky 4.12 is good cheap vesc. for that money you can't go better.
```

---
## \#5 Posted by: kanies Posted at: 2019-08-30T07:22:29.642Z Reads: 113

```
[quote="Tinp123, post:4, topic:101042"]
hose cells are rated on Mooch test as so-so 4.9A battery. In 6P configuration, your battery could output barely 30A
[/quote]

So from what you wrote I understand that I need to change the cell. Where did you found the information about Mooch test of those batteries?

I've found those Samsung 30Q on aliexpress:
https://pl.aliexpress.com/item/32966561237.html?spm=a2g0o.productlist.0.0.70ce5d44ODasRN&algo_pvid=f4b4d14e-dbdd-48ab-94a3-881250a67426&algo_expid=f4b4d14e-dbdd-48ab-94a3-881250a67426-18&btsid=026e86e3-04ac-4a26-b51f-80f37b1c5cf9&ws_ab_test=searchweb0_0,searchweb201602_5,searchweb201603_52
**You were speaking about them?**

About the 6P being too long. I want to mount it on my frame in 3D printed case so that wont be a concern. It will be even longer about 65cm with a case:
![obraz|533x500](upload://o7e0oammtnkIulaTXSvJkzKWp4H.jpeg) 

So from what you told me about BMS I understand that if I choose 25A BMS It will carry those motors even in the peak load (65A each)? Can you explain why is that?
```

---
## \#6 Posted by: Tinp123 Posted at: 2019-08-30T07:38:36.906Z Reads: 104

```
here is test:

https://www.e-cigarette-forum.com/threads/panasonic-ncr18650b-4-9a-3200mah-18650-bench-test-results-a-so-so-4-9a-battery.773723/

I can tell you right now that those 30Q cells from aliexpress are fake. Even from photo I can see that positive (+) end has 4 legs, and original has 3.

buy cells from nkon (if you are from EU. if you are from USA, you will have to wait maybe even 2 months  for your order from nkon). I know battery might seem extremely expensive when you want to build you first board as cheap as possible, but it is only part that you should do right and not save your money on it. you could always use quality battery in your new build. 

if you gonna use printed case, then it is ok to use nickel everywhere. I see you are ready for one really long battery :smiley:

I am talking about bypassing bms - aka wiring it for discharge only. in one circuit you will have bms and battery - bms has only one purpose here - to balance charge battery. in another circuit you will have only wires from battery + and - to connector to vesc. 

or you can use bms for both charge and discharge, but then take at least 60A bms. your 6P 30Q battery will be capable of more than 100A discharge.
```

---
## \#7 Posted by: Andy87 Posted at: 2019-08-30T07:57:24.904Z Reads: 92

```
Grind a flat spot on the shaft and you golden.
Green loctite does a good job as well if you don’t want to do anything on the shaft
```

---
## \#8 Posted by: Andy87 Posted at: 2019-08-30T08:06:12.373Z Reads: 94

```
@Tinp123 did give some good recommendations already. Can just second that you should stay away from buying cells from AliExpress. It’s not worth the troubles. 30q are 2.49€ at nkon right now and you can be sure they are legit.
Which deck you are using?
Your batter rig is stiff, most mtb decks have a flex, that will not work.
Think about top mount battery. You might not like the look in the beginning, but it’s way more practical. 

Skip the antispark switch and go with loopkey.
I have seen too much anti spark switches blow up and a loopkey is super cheap.

If you really want performance I wouldn’t go with 4.xx hw vescs. They heat up quick if you set them up to more than 30A bat max.
```

---
## \#9 Posted by: Andy87 Posted at: 2019-08-30T08:16:19.687Z Reads: 84

```
We have some mtb experts over here
https://forum./
Might get more feedback if you ask there.
```

---
## \#10 Posted by: kanies Posted at: 2019-08-30T08:16:29.710Z Reads: 86

```
[quote="Andy87, post:8, topic:101042"]
30q are 2.69€ at nkon right now and you can be sure they are legit
[/quote]

Yeah, but my problem is that I don't have a spot welder and I am looking for preassembled batteries that have nikel strip mounted on. That will alow me to just weld cables with a typical solder. At nkon website I haven't found any :frowning: 

Buying a spot welder is right now a crazy idea just for making a one battery pack. :slight_smile:
```

---
## \#11 Posted by: Andy87 Posted at: 2019-08-30T08:21:00.107Z Reads: 91

```
You can select the nickel taps on if you check out
![image|328x500](upload://kNRsZrVIPCoWrSJo2G6IeMoO4lH.jpeg) 

In the green box in the down part.

You can also get pre welded packs.
Just ask in the place I linked. 
Some battery builder offer that service.
They basically just weld you the p group and you than can solder them up how you want
```

---
## \#12 Posted by: kanies Posted at: 2019-08-30T20:26:53.177Z Reads: 80

```
Okay, from your experience batteries with nickel taps are easy to solder? Does it mean that is safe to solder them together using those preassembled nickel strips?

Because in my mind there is an idea that I will be not doing soldering directly on battery but on that nickel tap and therefore it won't heat up the cell. 

Am I right?
```

---
## \#13 Posted by: Andy87 Posted at: 2019-08-31T07:41:21.585Z Reads: 70

```
I never bought cells with nickel strips. 
I have a spotwelder and do my packs with it.
Wires I solder on I try to solder before I weld the nickel to minimize the heat on the cell.
Nickel will also heat up.
If you have a strong solder iron and use flux you should be able to do a good solder join in a short time without to heat up the nickel and with it the cells too much.
```

---
## \#14 Posted by: kanies Posted at: 2019-09-03T10:06:34.871Z Reads: 63

```
Tank you for all of your response.

Using all of your feedback I draw a connection design of all the parts.
Can you help me with my questions?
1. I want to be able to use some 24V led strips. Will a L7824T Voltage Linear Regulator change the Voltage from 36V to 24V as required for those LEDs?
3. I want to use some switch. Can it be a random switch? Or it must to check some parameters?
Like, here I've got some 36V switch:
https://pl.aliexpress.com/item/32944328781.html?spm=a2g0o.productlist.0.0.69461509kkIjoZ&s=p&algo_pvid=923dc394-fd2d-4fe2-97c9-0641d832cbda&algo_expid=923dc394-fd2d-4fe2-97c9-0641d832cbda-3&btsid=193d2406-eda9-4233-bc92-f259d1ee9075&ws_ab_test=searchweb0_0,searchweb201602_5,searchweb201603_52

![obraz|413x500](upload://hZKhYQpSTiXGRz5ALXDrznoDGLE.jpeg)
```

---
## \#15 Posted by: joeofford333 Posted at: 2019-09-04T04:16:00.325Z Reads: 51

```
Higher voltage 60v focbox can handle it
```

---
## \#16 Posted by: kanies Posted at: 2019-09-04T07:37:53.219Z Reads: 48

```
I think that you understood me wrong. I am not seeking for a different solution for ESC or VESC, I believe that in that matter my design is well thought.

My troubles are within me wanting to connect 24V LED strip to 36V battery, so I want to downgrade the Voltage to 24V. Second issue is that I want to mount a simple switch (on/off) and I am asking if a regular switch will be ok? Or I need to look for some parameters?
```

---
## \#17 Posted by: Andy87 Posted at: 2019-09-05T12:56:44.860Z Reads: 37

```
to get your 24V just use a step down converter which output 24V and can handle the load of your lights. 
for the switch it is the same, it need to be able to handle the voltage and the current for your lights.
```

---
