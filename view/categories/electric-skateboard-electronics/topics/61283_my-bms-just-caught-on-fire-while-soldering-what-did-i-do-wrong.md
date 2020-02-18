# My BMS just caught on fire while soldering. What did I do wrong?

### Replies: 31 Views: 611

## \#1 Posted by: Taliesin Posted at: 2018-07-08T20:51:19.624Z Reads: 171

```
My battery is fine thank god.

I think I may have soldered the balance leads in the wrong order. I went 1, 2, 12, ground. Started noticing smoke and flames right when I soldered ground (b13).

Only one resistor on the BMS is completely fried.

Anyways at this point I’m not sure whether to drop another $80 on the same BMS or just to skip BMS and charge and discharge manually.  Kind of at a loss right now.
```

---
## \#2 Posted by: pat.speed Posted at: 2018-07-08T20:55:00.446Z Reads: 163

```
I’m not quite sure what could have happened but I wouldn’t recommend manual charging. Maybe just get a charge only bms for cheap on ebay
```

---
## \#3 Posted by: Wilsonliang777 Posted at: 2018-07-08T21:00:09.976Z Reads: 159

```
I remember when I hooked up my first bms I mistakenly soldered the balance leads backward.  Me and I soldered 10th cell to the 1 cell slot on the bms.  It almost caused fire.

Third option is to buy a charge only bms.
```

---
## \#4 Posted by: Sebike Posted at: 2018-07-08T21:49:03.969Z Reads: 141

```
Was batt +and - connected to the bms before connecting balance leads?
```

---
## \#5 Posted by: Taliesin Posted at: 2018-07-08T22:03:38.204Z Reads: 129

```
No they were not
```

---
## \#6 Posted by: Sebike Posted at: 2018-07-08T22:21:06.123Z Reads: 124

```
They probably should have been. At least on the SuPower bms, it specifically sais that if you connect balance leads without batt + and - already connected, you'll fry the bms.
```

---
## \#7 Posted by: Taliesin Posted at: 2018-07-08T22:25:50.787Z Reads: 117

```
Thanks @Sebike
I just ordered another BMS.

I’ll connect battery + and - first. 

Then b1-12.

Then b13 to ground? Or should this one be connected before b1?

Man I watched a few videos on YouTube too and no one stated the importance of the order of soldering the balance wires.
```

---
## \#8 Posted by: Namasaki Posted at: 2018-07-08T22:26:00.561Z Reads: 113

```
A charge only BMS will fry if the balance leads are connected incorrectly.
I would get another $80 bms and start over but this time, take your time, don't get in a hurry.
Make sure you got it right before connecting anything.
```

---
## \#9 Posted by: Namasaki Posted at: 2018-07-08T22:27:25.636Z Reads: 105

```
Can you post a pic of the bms you are using?
```

---
## \#11 Posted by: Sebike Posted at: 2018-07-08T22:30:32.032Z Reads: 106

```
You have to double, triple check the wires before connecting to the bms, making sure voltages are correct on the balance leads, 3,7; 7,4; 11,1 aso. If you get this wrong, you'll also fry the bms. 

Make sure you check everything before connecting the bms next time!
```

---
## \#12 Posted by: Taliesin Posted at: 2018-07-08T22:31:40.798Z Reads: 104

```
![image|375x500](upload://j4lUu38UtJqFwFWVezZJgaB689e.jpeg)![image|374x500](upload://6LdizcvzaI3c0cdMGc8H2ASKz5y.jpeg)
```

---
## \#13 Posted by: Namasaki Posted at: 2018-07-08T22:38:14.935Z Reads: 106

```
Did you get a wiring diagram with that bms?
That is Bestech's newer version.
```

---
## \#14 Posted by: Sebike Posted at: 2018-07-08T22:52:34.851Z Reads: 100

```
If this is the same type of bms (apart from your being 12s and not 10s), you'll find a wiring diagram and some info on how to connect the bms.

https://www.electric-skateboard.builders/t/bestech-hcx-d596-the-new-80a-bms-wiring/41047/14

Where did you buy it? 

The seller should be able to provide you with the correct wiring, or else I would try getting it from Bestech.
```

---
## \#15 Posted by: Sebike Posted at: 2018-07-08T22:54:01.797Z Reads: 89

```
Hey @Namasaki, your profile picture resembles mine a bit. Wanna be friends?
```

---
## \#16 Posted by: Namasaki Posted at: 2018-07-08T23:00:51.839Z Reads: 84

```
Absolutely
```

---
## \#17 Posted by: Moros Posted at: 2018-07-08T23:04:15.019Z Reads: 88

```
[quote="Sebike, post:15, topic:61283, full:true"]
Hey @Namasaki, your profile picture resembles mine a bit. Wanna be friends?
[/quote]

[quote="Namasaki, post:16, topic:61283, full:true"]
Absolutely
[/quote]

awww cute.
```

---
## \#18 Posted by: Sebike Posted at: 2018-07-08T23:05:34.008Z Reads: 87

```
My first friend ❤️
```

---
## \#19 Posted by: Moros Posted at: 2018-07-08T23:07:46.860Z Reads: 88

```
So, ahh . . . could I join too?
```

---
## \#20 Posted by: Namasaki Posted at: 2018-07-08T23:23:18.980Z Reads: 86

```
Absolutely!
```

---
## \#21 Posted by: Namasaki Posted at: 2018-07-08T23:42:45.188Z Reads: 81

```
I wonder if you replaced that resistor, if the board would work ok.
It's worth a try. As long as nothing else got fried.
![31%20PM|264x191](upload://3GkkUOwD9uRtxQISvZC47yzyx7f.png)
```

---
## \#22 Posted by: Taliesin Posted at: 2018-07-08T23:45:32.981Z Reads: 77

```
How would I find out what resistor that is?
```

---
## \#23 Posted by: Namasaki Posted at: 2018-07-08T23:47:01.620Z Reads: 73

```
Get the color code rings off one of the good ones
```

---
## \#24 Posted by: pixelsilva Posted at: 2018-07-08T23:51:05.765Z Reads: 76

```
$80 dollars for a BMS ?? ....what? ...are they dipped in gold? Geeeeezzz!! Now the poor @Taliesin just invested the same amount (2 units) as a full fledged Vesc!! 

https://media.giphy.com/media/uQIpl0uCNhgis/giphy.gif
```

---
## \#25 Posted by: Namasaki Posted at: 2018-07-08T23:53:03.465Z Reads: 74

```
It's an 80a bms
$80 probably includes shipping and customs
The bms it's self should only be about $50 or $60
```

---
## \#26 Posted by: pixelsilva Posted at: 2018-07-08T23:55:14.565Z Reads: 71

```
Still, the dang thing is nowadays the prime suspect for most Vesc related gremlins. :grimacing:
```

---
## \#27 Posted by: Namasaki Posted at: 2018-07-08T23:55:48.421Z Reads: 71

```
Been running mine for couple years now with not problems.
I have the older style Bestech BMS
```

---
## \#28 Posted by: Moros Posted at: 2018-07-08T23:56:22.676Z Reads: 71

```
and also includes a power switch, replacing the need to have an anti spark switch.
Then there is the DieBieMS that samau18 is selling that cost $120.
```

---
## \#29 Posted by: Namasaki Posted at: 2018-07-08T23:57:38.913Z Reads: 74

```
[quote="Taliesin, post:22, topic:61283, full:true"]
How would I find out what resistor that is?
[/quote]

![02%20PM|690x348](upload://2227JH3LvxHyCF40VNvzQtwE0jc.png)
```

---
## \#30 Posted by: pixelsilva Posted at: 2018-07-09T00:05:20.999Z Reads: 70

```
Gossip on the streets is that most Vesc-torch related issues point to these nasty temperamental fellows. :roll_eyes:
```

---
## \#31 Posted by: Namasaki Posted at: 2018-07-09T00:08:22.601Z Reads: 70

```
Guess I've been lucky cuz I haven't torched a Vesc yet.
Still running my old Ollin Vescs that I bought 2 or 3 years ago
Note: I run BLDC mode unsensored with split PPM, 170-175kv on 10s.
So I run as low risk as possible.
```

---
## \#32 Posted by: Taliesin Posted at: 2018-07-09T00:56:49.202Z Reads: 56

```
It was $50 before shipping.

I ordered another one and I’ll just be more careful next time. Thanks for the help guys.
```

---
