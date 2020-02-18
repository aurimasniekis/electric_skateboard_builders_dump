# 6s ESC comparison

### Replies: 17 Views: 2315

## \#1 Posted by: jwu97 Posted at: 2016-07-08T14:04:25.916Z Reads: 231

```
Basically I'm looking for a reliable/bombproof/simple 6s (or 12s) ESC to go with a TB's 230kv 6374 for my new build.
From what I can find, theres:

-HobbyKing X-Car Beast 150A/120A (Cheapest at <$70) (switch)
-CC Mamba Monster 2 (waterproof, no enclosure needed) (Expensive AF $130+) (switch)
-Hobbywing ezrun max8 (waterproof, no enclosure needed) (Also expensive AF $120+) **(loud brakes???)** (switch)
-Hobbywing quicrun 08 (waterproof, no enclosure needed) (Decently priced $100) **(loud brakes???)** (switch)
-FVT/TB's 6s 120a (Cheap) (switch)
-APS 7s EV ESC (Cheap) (no switch)

-TB's 12s (upgradability) (no power switch) **(needs UBEC or is there a version with one built in?)** **(I find the brakes are kinda unpredictable/not analog)** (expensive @ $130+)
-Psychotiller's 12s **(Does this exist?) (power switch?) (internal UBEC?)**

Can people who have used the mentioned ESC describe their experience. My main concern is braking as I like to be able to slow down smoothly so I don't hit stuff LOL. (smoothness, loud sounds?)

I know many of you will recommend the VESC, but I really don't want to deal with the problems I see people having. Also, it seems like V6 will be out *soon* :joy:, so I'll just wait for that instead.

Thanks so much.
```

---
## \#2 Posted by: laurnts Posted at: 2016-07-09T08:39:28.413Z Reads: 202

```
Unfortunately, from all of my experience with various ESC, the VESC have the smoothest, noise free braking gradual braking with the highest braking force. I was skeptical too about it earlier, but now I have 3 ESC on my bench not doing shit, because VESC just out perform them in terms of acceleration, speed, heat management and braking. Trust me car esc wont satisfy you.

I got to say braking and starting is the devil of ESC problem and VESC just tackle this issue like baws!
```

---
## \#3 Posted by: flatsp0t Posted at: 2016-07-09T09:08:58.973Z Reads: 202

```
I think @Nowind has some experience with the Hobbywing ezrun max6.
He uses it for an MTB, but he seems to be happy with them.
```

---
## \#4 Posted by: Sean Posted at: 2016-07-09T09:28:58.084Z Reads: 192

```
I am using Hobbyking's Trackstar 150 Amp Car ESC 

http://www.hobbyking.com/hobbyking/store/__33984__TrackStar_150A_GenII_1_8th_Scale_Sensored_Brushless_Car_ESC_PC_Programmable_.html

It is pretty good, PC programming or programming via programming box. It has some brake noise, but isn't too loud. I am quite happy with it and it comes with a switch.
```

---
## \#5 Posted by: Nowind Posted at: 2016-07-09T11:00:38.671Z Reads: 187

```
Using the MAX6 on 8S and the Quicrun150A on 6S.
Both are water and IMO bulletproof.

But your demand of silence braking will not be satisfied.
```

---
## \#6 Posted by: flatsp0t Posted at: 2016-07-09T11:17:08.016Z Reads: 178

```
I think they are not that loud.

We are just spoiled by the VESC.
```

---
## \#7 Posted by: jwu97 Posted at: 2016-07-09T11:35:50.318Z Reads: 169

```
Did you have any problems with you're VESC ever? Also, what motor are you running? 
It really does seem like VESC's got the best features hmm. Just really concerned about reliability, seeing so many people frying their Vescs.
```

---
## \#8 Posted by: laurnts Posted at: 2016-07-09T16:46:55.591Z Reads: 162

```
Good quality vesc with proper implementation last long. I had two vesc version, 1 from enertion old batch and one from ollinboard. Fried mine completely from enertion (low quality batch), but the one from ollinboard havent let me down yet.

I had 3 from ollinboard, they are expensive, but you pay for the quality. As long as the configuration is right, not miss placing positive negative, not shorting, implement the right fuse... Youll be safe! Fuse really safed my vesc 2x when my connection are compromised.
```

---
## \#9 Posted by: mason Posted at: 2016-07-09T17:35:57.815Z Reads: 154

```
Stay as far away as possible from the quicrun. It resulted in my motor burning out due to no over ampage protection.
```

---
## \#10 Posted by: Nowind Posted at: 2016-07-09T19:08:29.303Z Reads: 146

```
You cant imagine how many MTB builds are running since 2 years with this Quicrun without one burned motor.
But maybe you was just unlucky.
```

---
## \#11 Posted by: Mark Posted at: 2016-07-09T20:05:09.036Z Reads: 146

```
I'm running the 12s torqueboards ESC. Very easy to program also pretty reliable. Only problem that i have found that the brakes are not reliable, 2 days ago i was just practicing, tried to break a very little to slow down and it went in reverse for 1 second. Ended up having huge wounds. Ordered protection immediatly.
```

---
## \#12 Posted by: mccloed Posted at: 2016-07-09T20:17:59.296Z Reads: 143

```
The @psychotiller ESC's were tested and the brakes were pretty unsafe. When hitting the brakes there would be a delay then full brake no matter how much brake was applied and you couldn't really adjust the brake strength. I'm sure he has some if you wanted to try one. Some of them have switches. Send him a PM.
```

---
## \#13 Posted by: electriclongboard Posted at: 2016-07-10T01:25:06.798Z Reads: 140

```
I would recommend the castle mamba monster 2 because it a good ESC, waterproof so you don't need to worry so much about it getting wet and dirty because this ESC is meant for a RC car and they get dirty AF. either than the price its a good ESC so I would spend the extra cash and get the mamba monster 2
```

---
## \#14 Posted by: torqueboards Posted at: 2016-07-10T01:26:19.833Z Reads: 140

```
@Mark - You sure you don't have reverse enabled?
```

---
## \#15 Posted by: Mark Posted at: 2016-07-10T08:13:00.134Z Reads: 139

```
No doubts, it's disabled
```

---
## \#16 Posted by: Maxid Posted at: 2016-07-10T09:23:39.893Z Reads: 135

```
X-car beast 150A: working flawlessly for maybe 2-300km now.
Had to reprogram the braking to 70% to be able to fully stop and set acceleration curve to very soft via my goolrc programming card (15€ from aliexpress).
I have removed the fan to make it silent and used the switch cables to include a bigger rocker switch outside of the enclosure as well as a battery capacity display.
```

---
## \#18 Posted by: Tijmen Posted at: 2017-06-07T11:03:50.193Z Reads: 55

```
I have the 120A X-Car Beast Series ESC and I'd like to make my board more waterproof. Currently I have a bunch of holes to supply air to the ESC, but from your experience, would the ESC be fine in an enclosed environment?
```

---
