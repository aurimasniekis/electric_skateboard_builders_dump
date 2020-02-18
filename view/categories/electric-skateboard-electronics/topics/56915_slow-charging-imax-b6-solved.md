# Slow charging imax b6 - Solved -

### Replies: 18 Views: 1980

## \#1 Posted by: danyCRO Posted at: 2018-05-27T10:55:50.835Z Reads: 96

```
Hi.
After many problems of charging and fake charger, I buyed Imax b6 genuine from Hobby King.
But it is stil the same.
I can charge only <1.7A, if i want set 1.8, it show Input voltage error.I have this:

Batters: 2 lipo batterys (2x5000mah, 3S)
Charger: Imax B6 Genuine
Adapter: Model: LX1205, Output: 12v, 5A.

On that charger I need arond 6 hours to charge 2 batterys, so that is like all day!
I only see that my adapter is too hot.. Is problem with adapter or what? How you can charge on 3a and be done for 45min? I need 6 hours.
```

---
## \#2 Posted by: Slak Posted at: 2018-05-27T11:24:21.490Z Reads: 91

```
First, 5000mAh won't be charged in 45min at 3A. It will take more like 2h10min, with normal charge program.

Second, I have an IMax B6 AC (almost same model) and I can charge my 3S Lipo at 6A (because 80/12.6=6.34 so 6A is good) ! Have you tried another charger to see if yours isn't damaged ?
```

---
## \#3 Posted by: danyCRO Posted at: 2018-05-27T11:56:14.095Z Reads: 93

```
Imax Charger or adapter? I tried 2 chargers for now lol

This guy tell that he charging 1 baterry 5.0 for 45min-60min. But think he charging at 5A.
https://youtu.be/_G0e4_WeKzw
```

---
## \#4 Posted by: jourm Posted at: 2018-05-27T12:16:39.737Z Reads: 77

```
If you supply your charger with 12v 5a, that's 60w, the you charge the batteries at 25.4v 1.7a about 50w, that makes sense. You are not gonna get 150w out of a charger you are only supplying with 60. so to charge you battery at 5a you would need about a 12v 12a Powersupply
```

---
## \#5 Posted by: pat.speed Posted at: 2018-05-27T12:19:01.028Z Reads: 72

```
And at 150w say bye bye to the charger. Imax B6 can only charge at 2,3a max anyway on 6s. It limits its self to that voltage as not to over heat to much, it an only do 5a on lower voltage batteries
```

---
## \#6 Posted by: danyCRO Posted at: 2018-05-27T12:32:53.355Z Reads: 66

```
I saw in one video recomendation that better not charge lipo more than 2.5-3.0 amps..
So I will be happy if my charger aviable charge at 3A.
Which adapter need for that?

Which adapters you have guys?
```

---
## \#7 Posted by: Slak Posted at: 2018-05-27T12:52:31.265Z Reads: 65

```
I meant charger, to see if you could charge your lipo at 6A with another charger. I misread the adapter part in your OP and jourm well explained the problem :)

My IMax B6 AC doesn't need an adapter and is 80W, that's also why I din't get you were limited to 60W ,sorry.
For the "more than 2.5-3.0A charge" thing, I saw "you can" and also "you can't" around Internet but I trust more the "you can" source so my lipos charged at 6.0A and it's ok for me (they are 8Ah so it's 0.75C).
```

---
## \#8 Posted by: jourm Posted at: 2018-05-27T12:55:42.795Z Reads: 57

```
Well, the Imax B6 is only rated for 50w if I looked at the right one, so that would mean that you need to upgrade both charger and power supply. I use a 200 w charger from hobbyking and an old computer powersupply. Most lipos are recomended to be charged under 1C, so for a 5aH battery that is 5a. 
https://hobbyking.com/en_us/turnigy-reaktor-250w-10a-1-6s-balance-charger.html?___store=en_us and https://hobbyking.com/en_us/hobbyking-350w-25a-power-supply-100v-120v.html?___store=en_us  
would get you there but might be a little overkill.
```

---
## \#9 Posted by: danyCRO Posted at: 2018-05-27T13:35:08.858Z Reads: 56

```
I bayed this week second charger, so I will not buy third one, for now. 
 
Can I buy 12V 12A adapter? Do I burn imax (which can charging only to 50W).
```

---
## \#10 Posted by: jourm Posted at: 2018-05-27T13:55:26.448Z Reads: 54

```
With your 50w Imax you can only charge 6s  25.2v/50w ≈ 1.9a. So buying a powersupply and no charger wont help you much. Before you buy something, you have to do the math
The power P in watts (W) is equal to the current I in amps (A), times the voltage V in volts (V):

P(W) = I(A) × V(V)

so if you want to charge a 6s (25.2v) battery with 5a you charger has to be able to handle 25.2 x 5 = 126w and then you need to supply that charger with 126w for 12 volt that would mean that you need 126/12 ≈ 10.5a and that is without ideally, in reality you would probably need like 150w charger and 13a powersupply.
```

---
## \#11 Posted by: Okami Posted at: 2018-05-27T19:15:05.650Z Reads: 45

```
I would recommend getting 100 - 150W capable charger. I also fell for this at first that I got a slow charger..

Uve got to think in watts / watthours to get it right.

So if u got 5ah 22.2v battery (nominal, not max volts) then u need almost 100 W charger to charge in 1 hour, if battery is quite empty

Though something seems off if u say 6hours.. u should be able to charge in 2-3h.

My final note would be to look for Turnigy Reaktor chargers, these can charge even at ~12A @ 6s, if your power supply allows.

They come at around 55usd now but is worth it. Lots of modes and u can adjust charge current while charging. 

---
PC psu can be used as power supply, if u needs lots of power. Just needs to bridge 2 terminals together.
```

---
## \#12 Posted by: danyCRO Posted at: 2018-05-27T20:32:37.921Z Reads: 36

```
Thank you for detailed answers.
I have 3s (12.6v) battery x2.
And when charging parallel I set settings for 3S (not 6s).

But how guy from video above charging 5mah battery for 1 hour with imax charger like mine?
```

---
## \#13 Posted by: pat.speed Posted at: 2018-05-27T21:17:34.842Z Reads: 29

```
He probably didn’t discharge his battery fully. Apart from that it is not actually possible to do this.
```

---
## \#14 Posted by: danyCRO Posted at: 2018-05-27T21:55:32.219Z Reads: 27

```
Thats makes sense.👍
```

---
## \#15 Posted by: danyCRO Posted at: 2018-05-30T18:06:59.153Z Reads: 24

```
Maybe my this test can show something:
I test my charging 1 battery 3S.

Start from about 9.20v. 
Set to 2.0A and charging to 11.16v (~25min), then show input voltage error.
Set to 1.9A, charging to 1.42v (~55min)
Set to 1.8A, charging to 12.05v (~2h20min)
Set to 1.7A, charging to the end (~2h50min).

So charging can start with 2, but finish with 1.7a.
```

---
## \#16 Posted by: Okami Posted at: 2018-05-31T07:21:10.958Z Reads: 20

```
Well u could always buy Accucel 80w charger.. I assume u didnt know it is on hobbyking, it is about same price as genuine B6.. not sure for how much u can sell yours now but for 80w charger u would also need at least 100w supply or so.

Ive got 72w PSU for it and can max charge at 2.5A, with proper supply 3A should be possible.. though it has super loud and annoying fan.

If I were u I might even try charging with "brick" battery charger and add some indicators, to know at what level the cells are
```

---
## \#17 Posted by: pat.speed Posted at: 2018-05-31T07:26:36.591Z Reads: 22

```
The error is caused by the power supply. I used to charge my 6s lipo at 2.3 amps the whole time. The amps will automatically decrease as the battery charges.
```

---
## \#18 Posted by: danyCRO Posted at: 2018-06-04T22:00:57.884Z Reads: 16

```
I solved problem.
The problem was in input voltage.
I bought charger 16v 4.5A 75w.

Now charger can charge at 4.2-4.3a.
No more input voltage error.
That is enough to me.
1 3S battery charged for 70min.

Thanks everyone for help :)
```

---
