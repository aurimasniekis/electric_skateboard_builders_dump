# Need Help for my DiY

### Replies: 7 Views: 1224

## \#1 Posted by: ElskerShadow Posted at: 2016-10-31T12:33:33.793Z Reads: 135

```
Hey there,
One year ago i had my first electric board. Was great but poor quality chinese board. After long tought I now know I won't ever buy again a pre build board. Because it will always be less reliable than a DIY board, and also this is not who I am.I like when i build things and that I know how to repair and maintain in a good shape.
So I live in Paris,France so the town is not very steep hilled, just a few 11/15% hills. There.s only montmartre with more hill. However my need is for a single motor since I wan't range more than incredible torque and power. I just need to go at least 30 km /h cruising with peaks at 40 km/h to avoid cars and different traffic problems. I had this problem with my first board, not enought speed to ensure security in the traffic. And i wan't a board that does not exeed 6 or 7 KG since I will need to lift it quite often. ( the board I had was incredebly low weight 5 kg and that was purely amazing)
So my plan is : Since i.m not an experienced builder I wan't to buy the carbon deck of enertion http://www.enertionboards.com/electric-skateboard-parts/carbon-fiber-electric-skateboard-deck/ I like the fact that all the component are in the deck, more convinient and even tho the carbon deck will be stiff it's not a problem for me since I wan.t a light board, and I don't mind the stiff deck.
The battery I will also go for enertion space cell because it's convinient, well reviewed and has a very large capacity with a single drive I can go at least 25 km ! ( real world range from an enertion raptor user with dual so I can except even more. http://www.enertionboards.com/electric-skateboard-parts/spare-raptor-battery/
I was told that the VESC of enertion are great ( even the best for some peoples ) so I bought this one. .
http://www.enertionboards.com/electric-skateboard-parts/vesc-standard/

I also choosed the enertion Mono Drive kit with R Spec motor but I will change the wheels to abec flywheels 

And my main concern is the remote, can I use with no concern about safety any 2,4 Controller with the vesc of enertion ? I Ordered this one 
http://esk8.de/  
It's the micro remote

So I already recieved the VESC but I don't know very much. How will I plug the reciever of the micro remote to the VESC ?  And how will i plug in the motor since there's no golden female wires like on the video of the build ( https://www.youtube.com/watch?v=O1kqiC0hzVc ) ? 
 <img src="/uploads/db1493/original/3X/b/7/b71266d0cdf3937bfbbc3be6b77c2664a2217052.jpg" width="666" height="500">
And i'll also need to know what I should expect, I mean will I have to program the VESC ? Actualy I'd like to to set up the acceleration since I wan't a smooth one and a smooth braking. And is ther's some little stuff that I will need, some extra wires etc... ? please tell me all you know !
Thank you very much for reading, and I hope you will help me to build  my board :)
Ps excuse my bad english i learned by myself so grammar & stufff...
```

---
## \#2 Posted by: DeathCookies Posted at: 2016-10-31T13:04:12.235Z Reads: 121

```
[quote="ElskerShadow, post:1, topic:12191"]
And my main concern is the remote, can I use with no concern about safety any 2,4 Controller with the vesc of enertion ?
[/quote]

You can use any rc transmitter with a PWM signal. Your choosen controller will work.[quote="ElskerShadow, post:1, topic:12191"]
How will I plug the reciever of the micro remote to the VESC ?
[/quote]

You need a female to female servo cable:
http://www.hangarone.co.nz/images/1313-500x500.jpg
Plug it in like this:
http://www.electric-skateboard.builders/uploads/db1493/optimized/2X/d/d2f73575e4cebb449055709cd9f93063e04c1e9a_1_375x500.jpg[quote="ElskerShadow, post:1, topic:12191"]
nd how will i plug in the motor since there's no golden female wires
[/quote]

You need to buy 5,5mm female bullet connectors. (The enertion r-spec motor uses 5,5mm male plugs). When you have the bullet connectors you need to solder them to the motor cables.[quote="ElskerShadow, post:1, topic:12191"]
And i'll also need to know what I should expect, I mean will I have to program the VESC ?
[/quote]

Yes you have to set it up properly. If you make mistakes you will destroy your VESC. so be careful and search in this foum for additional information!
```

---
## \#3 Posted by: ElskerShadow Posted at: 2016-10-31T15:06:10.116Z Reads: 88

```
Thank you so much ! You help a lot :) 
[quote="DeathCookies, post:2, topic:12191"]
You need to buy 5,5mm female bullet connectors. (The enertion r-spec motor uses 5,5mm male plugs). When you have the bullet connectors you need to solder them to the motor cables.

Is this good ? https://www.amazon.fr/ZIMO-Connecteur-Femelle-Connecteurs-Electriques/dp/B01LBDUFHW/ref=sr_1_5?s=electronics&ie=UTF8&qid=1477926068&sr=1-5&keywords=connecteur+prise+fiche+banane+male+femelle+4mm

Thank you for all your help, I will look on the forum for the VESC set up, I must do it when I'll have the motor and the battery or it can be done before ?
```

---
## \#4 Posted by: DeathCookies Posted at: 2016-10-31T15:14:20.441Z Reads: 84

```
[quote="ElskerShadow, post:3, topic:12191"]
Is this good ? https://www.amazon.fr/ZIMO-Connecteur-Femelle-Connecteurs-Electriques/dp/B01LBDUFHW/ref=sr_1_5?s=electronics&ie=UTF8&qid=1477926068&sr=1-5&keywords=connecteur+prise+fiche+banane+male+femelle+4mm
[/quote]

No, you have found **4mm** connectors but you need **5,5mm** connectors. [Here are the correct ones.](https://www.amazon.fr/Helicopter-Battery-Bullet-Female-Connector/dp/B00NZ18KE4/ref=sr_1_1?ie=UTF8&qid=1477926671&sr=8-1&keywords=5%2C5+female+bullet+connector)

You can setup the VESC partially when you have any power source. But i would recommend that you will set up it with your normal battery you are going to use.
```

---
## \#5 Posted by: rpn314 Posted at: 2016-11-01T06:54:43.453Z Reads: 64

```
On doing initial VESC setup (especially motor detection), wasn't the recommendation to use a low current and low voltage bench supply? I vaguely remember using a supply limited to 12v @ maybe 3 amps....
```

---
## \#6 Posted by: flatsp0t Posted at: 2016-11-01T11:24:56.692Z Reads: 58

```
That was only on first boot/firmware flash i think.
```

---
## \#7 Posted by: maker7 Posted at: 2016-11-01T18:38:27.113Z Reads: 46

```
I just got my Enertion VESC sorted out yesterday,  I made sure my batteries were charged (running 6s) and when I hooked everything up, the VESC had the latest 2.18 firmware - but would not detect my motor.  So i reflashed and made sure my battery settings were correct and everything started working.
```

---
