# My first build (100% DIY)

### Replies: 11 Views: 712

## \#1 Posted by: kntzn Posted at: 2019-05-29T21:50:28.303Z Reads: 293

```
Hi. This is my first post here but I’m really into e-skating for more than 2 years. 
Well, everything has started when I was riding my penny-style shortboard on the street without any lights. So that was the moment when i realized that I need some kind of lights on my board. But my knowledge of electronics was lower than the Ohm’s law. So I’ve made my lights after few months of youtube tutorials. 

But then I thought about the motor on the board and I have dived into the e-skating.

I should mention that I am living in Russia, where there is no e-skates on the streets even today. I saw them 3 times maybe, not more. So it is really hard to get good esk8 hardware. So I’ve decided to DIY the board. Including the Deck, RX and TX units as well as Anti-spark. “For what reason?” - you may ask. I will answer: “Cheaper(that really matters for me) and they are much more customizable”.

So I’ve created my first deck and enclousure:
![image|375x500](upload://i1l3Lzi6fP18FtOysZzMQipKuEf.jpeg) ![image|375x500](upload://wHDU8fUqYWPC5meNSrBT6QxsaUS.jpeg) ![image|669x500](upload://7kQ0stkdm7PEL2yzq9k2iDAYOir.jpeg) ![image|690x388](upload://vZ7NFN7tqrjiQRx3bEHz2CTVvAd.jpeg) 

And ordered batteries, motor, motor mount and so on from AliExpress (because it is cheaper, and if you would add shipping cost from US, it is MUCH cheaper) 
When everything has arrived, I’ve started the building process.
But electronics inside the enclusure was really messy:
![image|666x500](upload://FMhf0MqPtP8ZMMwc7VeCZhk01r.jpeg) 

And this is were everything has started because right after that 3 cheap esc’s were thrown away one after another
After that I’ve stopped for a few months.

The 3rd generation started here: I’ve bought a VESC. Tried again. But this time my anti-spark switch based around BTS555 fired itself and I got tired from this messy electronics once again:
![image|666x500](upload://5uh2EuNc38kBueYorP4GlCkNOLI.jpeg) 
So i decided to create the longer board that would be capable to fit bigger enclosure. 
However, this prototype was able to move me around for maybe half a mile or so.


And the 4th generation has started. New deck and enclousure:
![image|375x500](upload://9CTDR3ndPE2irgzkZhwnQ3h5TuH.jpeg) ![image|690x318](upload://foIBr9RMtSoQdo15OxTsUX7pDOc.jpeg) 
Much better cable-management and components mount:![image|666x500](upload://9sDvlzpNLTN2LNpXCqrdhOR4xON.jpeg) 
So this board is complete. It’s specs:
Betteries: 4x HRB LiPo (5Ah, 3S, 25C) (10Ah; 6s in total)
Motor: Chinese 5065 (270kv, 2.4 gear ratio, 1800w)
ESC: VESC (Maytech)
RX/TX: custom
Anti-spark: custom
BMS: no (but RX monitors the battery and balancers are installed) 

But it still have another problem: RX-TX pair connection is really poor so I’m going to upgrade their radios. 

That’s it. Over more than a year I have solved problems with my DIY Anti-spark, Deck and Custom RX-TX is also going to be overhauled right after I will pass my exams. 

P.S: I hope that my grammar is satisfactory for you to read this text. I’m really sorry for my language.
```

---
## \#2 Posted by: venom121212 Posted at: 2019-05-29T22:17:43.997Z Reads: 241

```
Welcome! Your grammar came through great. Nice build, I really like the shape and color scheme of the second one. @Andy87 is in Russia as well and very knowledgeable and friendly. I'm sure he knows the struggle to get parts and maybe some good sources.
```

---
## \#3 Posted by: barajabali Posted at: 2019-05-29T22:51:49.495Z Reads: 228

```
Sweet build! I like the unconventional build style
```

---
## \#4 Posted by: Andy87 Posted at: 2019-05-30T03:47:31.717Z Reads: 182

```
Hi! Great build and heads up for all the parts you made by your own. You right in Russia esk8ing is not really common but there still a lot just all over the country. If you didn’t know already there is this group as well https://vk.com/electricboard

You can find a lot of information and parts there as well.
```

---
## \#5 Posted by: kntzn Posted at: 2019-06-06T11:59:46.796Z Reads: 128

```
An upgrade of components mount:
![image|666x500](upload://tCbX2QFThcf6b8UirM65pLKoERy.jpeg) ![image|666x500](upload://gZHtbXlvenNtnFPChjHrkoQmn2E.jpeg) 

Now I use velcro instead of brackets, bolts and nuts. It is much easier to service the board
```

---
## \#6 Posted by: Sergiu Posted at: 2019-06-07T13:18:05.418Z Reads: 94

```
Very nice build. And pretty too.:+1:
```

---
## \#7 Posted by: Alex753 Posted at: 2019-06-07T17:36:09.892Z Reads: 91

```
Great !
Are you using a BMS to charge your 4 batteries at once ?
```

---
## \#8 Posted by: kntzn Posted at: 2019-06-07T18:02:20.770Z Reads: 86

```
Hi. My batteries connection is 2S2P, so i use 2 balancers for each 2P group to prevent overvoltage when charging.
```

---
## \#9 Posted by: Jcbernie Posted at: 2019-06-07T18:12:43.934Z Reads: 84

```
So I’m new to the forum, Great site.  I recently purchased a evolve carbon gt, and have to say I’m very dissatisfied with the board and the company.  Make long story short, my board malfunctioned after the first 5 rides due to condensation and moisture leaking into the deck.  The company refused to guarantee repair or replace the board.  After a long winded debate with evolve support and Affirm (finance) company, it was determined i was responsible for the damage which is #%*%.  Push comes to shove, I’m getting the board back.  My question to everyone out there: Is there an DIY “kit” or recommended schematic that I could use to build and and upgrade the original carbon deck, trucks and wheels from the old board? I believe all the internal electronics and controllers have to be replaced. Motors are still functioning but i welcome recommended upgrades and improvements on the stock board. Thank you in advance.
```

---
## \#10 Posted by: kntzn Posted at: 2019-06-07T18:43:18.169Z Reads: 74

```
Hello.
Well, IMO if your board could not be guaranty repaired any more and you whant to reuse it’s components, you should find out what could be used from your wrecked board. I assume that battery and motors (as well as their mounts) are ok, so what you gonna need is RX+TX and two or dual motor VESC. There is a lot of guides here in the forum how to connect VESCs, how to setup them and so on. 


But also you can find a new electronics for evolve board (maybe someone sell them? Idk, sorry) and just replace the broken one.
```

---
## \#11 Posted by: kntzn Posted at: 2019-08-24T23:51:39.479Z Reads: 48

```
Update 2: 
After month of testing all arround the Moscow I can clearly state the fact that my new RX-TX are really strong units, as well as connection between them. Moreover, connection quality is even beter than on the pre-built Yuneec Ego-2 board of my friend. So here they are:![image|666x500](upload://9dgweDgCUEQFzSv8RQjliTwKaB7.jpeg)

My TX does not currently feature the custom 3d-printed enclousure, but lack of it is defentetely temporary.

So, my RX has plenty of features:
1. Single-PPM output
2. Connector for external current shunt & voltage probe
3. Communication based around HC-12 module
4. 2 PWM outputs for external lights
5. Hall sensor input
6. External buzzer output, external indication lights, external battery voltage 7-seg display. 
7. Thermistor input.
8. SD card logging.

So, currently i’ve coded p.1 - p.3. But others are coming too.

TX is being up-to-date with the RX features, currently displaying voltage of the board and current riding mode.
```

---
