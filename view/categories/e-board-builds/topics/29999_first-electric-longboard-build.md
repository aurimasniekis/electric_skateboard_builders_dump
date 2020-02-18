# First electric longboard build!

### Replies: 8 Views: 1201

## \#1 Posted by: VincentUK Posted at: 2017-08-07T22:29:14.995Z Reads: 95

```
I am building my first electric longboard and I have come to the point where I need some expert counseling. Below you can review my battery, bms, switch and charging schematics. I will be building this component in the next couple of days and will post more drawings and pictures of the other part of my setup as I go along. I would love to get some feedback of what you guys think and if you have any warnings or suggestions on improvements! <img src="/uploads/db1493/original/3X/a/b/abf5c0c91b70b742b0ea39613bb5b18cf32a51f7.png" width="690" height="387"> If you think the bms is connected in a weird way I completely agree with you :P for more info on why this is the case you can have a look at this thread: http://www.electric-skateboard.builders/t/8-pin-in-a-6s-bms/26003/58 It pretty much has all the good stuff in it. 

At this moment in time I only have 3 questions that I feel that I need answered before I get soldering.
1. What does it mean for my setup if my BMS is rated at 50A continues-discharge and my batteries can do 60C?
2. Is my series sensor wiring correctly drawn out in the diagram?
3. my charging plug is rated at 20V 4A but my charger will do 25V 5A. Will my plug melt and start burning if I use it? Or is it fine?

Okay so if you are still reading I might as well lay out my master plan. So I want to create an electric longboard that can work as my ride to uni this autum. It's only 3km to school and almost all flat so I'd thought I go small on the battery as it I only need maybe 5-6km per charge. I know that I am being a bit optimistic now and realistically I will most likely just charge the board between lectures but I think a 6s 5000mAh or (2x 3s 5000mAh wired in series) will suffice. Smaller battery also means that I do not need to carry around a tank when I'm in class. 

I wanted charging to be as simple as possible, so I went and bought a BMS (PCM-L16S50-985 by Smartech). To control my motor 6355 260Kv motor (diy-electric-skateboard-kits-parts/6355-260kv-epower-motor/)  I bought the famous VESC (diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/).

To control my board remotely I have designed a custom 3d printed Arduino powered remote (Iknow that was a mouthful xD). More images, models and code on that later! Anyways, I plan to use an Arduino nano and a HC05 bluetooth chip down on the board so that the board can receive instructions from the remote. The Arduino will then relay these commands to the VESC via its UART port.

Yeah, that's basically it, for now. I look forward to hearing what you guys have to say about the project!
```

---
## \#2 Posted by: darkkevind Posted at: 2017-08-07T22:36:56.090Z Reads: 84

```
Your charging brick is underpowered and will never fully charge your batteries. 2 x 3s is 25.2v so you'd need a charging brick to match.

Your series wiring looks fine although if I were you, I'd bypass the BMS for discharge and just use it to charge. That way you'd leave the discharge threshold to the VESC.
```

---
## \#3 Posted by: VincentUK Posted at: 2017-08-07T22:38:36.863Z Reads: 80

```
I just double checked and luckily it says its 25.2V 5A. Or maybe that is still underpowered?
http://alienpowersystem.com/shop/chargers-power-supply/charger-for-bms-d223-6s-25-2v/
```

---
## \#4 Posted by: darkkevind Posted at: 2017-08-07T22:39:03.623Z Reads: 75

```
No, that's fine then.
```

---
## \#5 Posted by: VincentUK Posted at: 2017-08-07T22:40:27.184Z Reads: 72

```
Is 50A continues to little?
```

---
## \#6 Posted by: darkkevind Posted at: 2017-08-07T22:44:30.795Z Reads: 70

```
Depends on your motor's or motors' max Amp rating... and also your  max motor setting in the VESC setup.
```

---
## \#7 Posted by: IsTalo Posted at: 2017-08-07T22:45:51.809Z Reads: 68

```
I do not have anything to add to help you, but I really want to know if it is going to work, because mine bms is on my closet waiting to find someone that wants it...
```

---
## \#8 Posted by: VincentUK Posted at: 2017-08-07T22:49:18.196Z Reads: 63

```
I will let you know as soon as I can start soldering! still waiting on some cables and connectors that I ordered. Should be here tomorrow or the day after tomorrow!
```

---
