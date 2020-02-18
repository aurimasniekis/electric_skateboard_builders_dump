# Battery Advice 10s5p 30Q

### Replies: 20 Views: 429

## \#1 Posted by: doakickflip Posted at: 2019-04-06T22:12:19.467Z Reads: 149

```
I'm going on vacation but won't be able to bring my board with me :disappointed_relieved: I'll be away for, give or take, 4 weeks. 

How should I leave my batteries? Should I fully charge it before I go? Should it be disconnected from the ESCs? Is there a certain way of keeping it in storage safely? It's a 10s5p 30q pack.
```

---
## \#2 Posted by: venom121212 Posted at: 2019-04-06T22:17:05.657Z Reads: 147

```
Id store it half full, off the charger, battery pack disconnected, and optimally the battery pack would be in a fireproof bag.

But then again we leave them connected to our boards regularly so I'd just do the first 3 suggestions if you don't have a fireproof bag :slight_smile:
```

---
## \#3 Posted by: Slydunan Posted at: 2019-04-06T22:20:28.956Z Reads: 137

```
Ideally batteries shouldnt be stored full. Storing at about half charge is better
```

---
## \#4 Posted by: pjotr47 Posted at: 2019-04-06T22:24:08.981Z Reads: 134

```
The best is stored the battery’s around 3,45v each cell in a cool and dry space. 

Disconnect the whole pack from everything. The ESC and antispark (if you use it) can drain the pack a bit.
```

---
## \#5 Posted by: mishrasubhransu Posted at: 2019-04-06T22:25:29.552Z Reads: 130

```
Store it at 3.5V disconnected from everything. If you have a good bms then you don't even have to do that.
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-04-06T22:26:52.254Z Reads: 123

```


[quote="mishrasubhransu, post:5, topic:89636"]
If you have a good bms then you don’t even have to do that.
[/quote]

thats not true, always disconnect from esc and anti spark because some anti sparks draw 0.5 watts even when turned off, for ex the fatboy antispark
```

---
## \#7 Posted by: AlanZhou Posted at: 2019-04-06T22:27:49.026Z Reads: 116

```
1 month is a pretty long time and your battery will probably drain to 0% if you store at around 3.5v, so id say store at 100%
```

---
## \#8 Posted by: pjotr47 Posted at: 2019-04-06T22:30:37.665Z Reads: 115

```
1month is okay for a battery. I have cells who are laying here for more then 3 months. They where 3,45v. I think they are now 3,35v. Let me check it tommorow.
```

---
## \#9 Posted by: AlanZhou Posted at: 2019-04-06T22:32:31.432Z Reads: 113

```
cells will always last longer then a pack with a bms in it, even the bms draws power which can cause the pack to go flat
```

---
## \#10 Posted by: pjotr47 Posted at: 2019-04-06T22:36:10.804Z Reads: 107

```
I know. But a bestechpower bms draws less then 50 micro ampere’s. So that is 0,00173watt

Edit: 3,45v is around 4wh. So a 10s5p would be 200wh. So 200wh/0,00173watt = 115 000 hours.
```

---
## \#11 Posted by: AlanZhou Posted at: 2019-04-06T22:37:15.087Z Reads: 104

```
yeah lol, all he needs to do is unplug from anti spark then because theirs a chance that will be the killer
```

---
## \#12 Posted by: pjotr47 Posted at: 2019-04-06T22:38:11.779Z Reads: 100

```
Yeps. Those antisparks and vesc can be a killer.
```

---
## \#13 Posted by: mishrasubhransu Posted at: 2019-04-06T23:05:14.547Z Reads: 96

```
@AlanZhou, I said a good BMS. So fatboy doesn't count because it's neither. Let's take a Bestech BMS as an example. It says it takes 50uA(~ for 10S battery) current draw to function.  Say you want to allocate 1Ah of your 10Ah battery to BMS, it's going to last you 1Ah/50uA = 1,000,000/50 hours = 20,000 hours = 833.33 days. If you want to have a factor of safety of say 2,5, or even 10, you are good for 3 months. A little bit of math, helps :) . Let me know if I have made calculation mistake somewhere.

http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D105.html
```

---
## \#14 Posted by: AlanZhou Posted at: 2019-04-06T23:06:10.490Z Reads: 93

```
it sounded like you said if you had a good bms you wont have to unplug from an antispark
```

---
## \#15 Posted by: mishrasubhransu Posted at: 2019-04-06T23:06:46.255Z Reads: 94

```
I meant one doesn't have to unplug the battery from the BMS.
```

---
## \#16 Posted by: venom121212 Posted at: 2019-04-06T23:28:51.562Z Reads: 90

```
Yeah I could see why that would make sense. All my packs have been shipped fully charged. I'm sure there's a time table where it makes sense. Thanks for the correction!
```

---
## \#17 Posted by: doakickflip Posted at: 2019-04-07T06:13:32.506Z Reads: 73

```
So general consensus is:

- Charge/Discharge the pack to 3.45V per cell (34.5V) / half full
- Disconnect from ESC and other devices that can discharge it
- Keep in a cool dry place, preferrably in a fire proof pouch/bag/container

Thanks to everyone for your input.
```

---
## \#18 Posted by: b264 Posted at: 2019-04-07T06:26:02.468Z Reads: 69

```
[quote="doakickflip, post:1, topic:89636"]
I’m going on vacation but won’t be able to bring my board with me :disappointed_relieved: I’ll be away for, give or take, 4 weeks.

How should I leave my batteries? Should I fully charge it before I go? Should it be disconnected from the ESCs? Is there a certain way of keeping it in storage safely? It’s a 10s5p 30q pack.
[/quote]

Have you been using it regularly?  Does it have a loopkey that disconnects everything?  If the answers are both "Yes" then just ride it once to get it between 25% and 70% charge, and leave it.  If they aren't both "yes", please elaborate.
```

---
## \#19 Posted by: doakickflip Posted at: 2019-04-07T10:23:40.398Z Reads: 59

```
Yes, on average 80km / week for the past year or so. 
Yes, my setup is battery (no bms)-> loopkey (no anti-spark) -> ESCs

So just disconnect loopkey and that should take care of it?
```

---
## \#20 Posted by: Jaydawg56 Posted at: 2019-04-07T13:41:51.206Z Reads: 54

```
I have a vtc6 10S5P pack and left it for about 5.5 weeks.  I left it plugged into my unity and worried about that parasitic drain. Contacted Jeff (@Deodand) said don’t sweat it; it is designed for it.  

6 weeks later I check my voltage and it didn’t drop at all... stayed steady at 36.7
```

---
