# Please help with my esc substitute

### Replies: 30 Views: 706

## \#1 Posted by: Carret Posted at: 2018-10-13T19:03:49.280Z Reads: 128

```
I bought these motors from dickyho https://www.google.com/search?q=diy+dual+1500+watt+longbaord+motor&oq=diy+dual+1500+watt+longbaord+motor&aqs=chrome..69i57j33l3.20834j1j7&client=ms-android-hct&sourceid=chrome-mobile&ie=UTF-8 
And I bought this esc substitute https://www.ebay.com/i/323326552273?chn=ps&var=512391639581&ul_ref=https%253A%252F%252Frover.ebay.com%252Frover%252F1%252F711-117182-37290-0%252F2%253Fmpre%253Dhttps%25253A%25252F%25252Fwww.ebay.com%25252Fi%25252F323326552273%25253Fchn%25253Dps%252526var%25253D512391639581%2526itemid%253D512391639581_323326552273%2526targetid%253D477790085665%2526device%253Dm%2526adtype%253Dpla%2526googleloc%253D9020169%2526poi%253D%2526campaignid%253D1591255861%2526adgroupid%253D62826452551%2526rlsatarget%253Dpla-477790085665%2526abcId%253D1139306%2526merchantid%253D114773922%2526pt%253D%2526gclid%253DCj0KCQjwr4beBRDNARIsAGZaZ5fkARSSLFZwJ1M76EYXI2CEWvtPFEwJArHUvRLnbk9kMMt3OR1_9Q0aAoVAEALw_wcB%2526srcrot%253D711-117182-37290-0%2526rvr_id%253D1702372185937%2526rvr_ts%253D6ec8ee0c1660ada1cbc3ffe1fffb4303
And I already had 2 10s 2p batteries that I wired in parallel. It worked for about a month and it could go 27mph, but then it started beaping and turning off when I would accelerate up to 27mph. I checked the voltage of the battery before, and it read 42v and then I checked the voltage after it shut off and it read 9v. When I unplugged the battery it jumped up to 42v again. Now I can't go even 20mph before it's shuts off. Please help me figure out why.
```

---
## \#2 Posted by: yuweng Posted at: 2018-10-13T20:02:04.809Z Reads: 119

```
it is either your 18650 or BMS couldn't supply the current thats why it shut off. The easiest & quickest way to check 18650 is to hook up a 0.1 ohm 5 watt resistor parallel to your multimeter & measure each cell, the voltage shouldn't sag to below 3 volt, the one that does is the faulty cell. You must do this quick or the resistor will get real hot or you can also dunk it into a glass of water to keep it cool. If its the BMS then you can bypass it, further info then use the search function, there are plenty of discussion here.
```

---
## \#3 Posted by: Carret Posted at: 2018-10-14T00:32:03.131Z Reads: 104

```
I have an extra 10s 40a bms,  can I wire that to one of my batteries and have 2 bms's on one battery?
```

---
## \#4 Posted by: yuweng Posted at: 2018-10-14T03:26:46.964Z Reads: 94

```
Yes you can but that will be a lot of work. You'll need to split your existing 2P battery into 1P & install each a BMS to it but doing so won't identify the fault. Since you can access to the battery, when it shut off, measure each cell & you'll know which one is the culprit.
```

---
## \#5 Posted by: Carret Posted at: 2018-10-15T03:45:24.870Z Reads: 79

```
Can you test individual cells even of they have been spot-welded together? I just put my longboard together and I took for a test ride and I couldn't even go 15mph, I think it's been getting progressively worse over time. And thank you so much for your help, this is my first time trying to build an electric longboard, Much appreciated.
```

---
## \#6 Posted by: M.Hboards Posted at: 2018-10-15T04:09:32.762Z Reads: 72

```
sounds more like a battery problem then a esc problem to me. also do you have a heatsink on it because  these esc's beep and shut off when they overheat.
```

---
## \#7 Posted by: Carret Posted at: 2018-10-15T04:35:29.240Z Reads: 72

```
No, but I was going to use some little fans to cool it though-It just stopped working after a couple of weeks, so I never got around to it.
```

---
## \#8 Posted by: yuweng Posted at: 2018-10-15T11:55:16.811Z Reads: 63

```
![10S2P|690x359](upload://vsROlbmAC4UMbYqJ9BIm6foYRdh.jpeg) 
in your case it means two cell, refer to the above pic, after it shut off, measure cell 1 to 10, one of them should be way less than 3 volts, thats the one. Normally its just one cell faulty. Split them up to identify it.

You can also measure directly at the BMS at each of the connector. Do not remove the BMS connector while doing this, it will just restore back to the normal voltage as you have experience it.

Pic taken from [JLabs](https://www.electric-skateboard.builders/t/custom-18650-battery-pre-build/2014)
```

---
## \#9 Posted by: Carret Posted at: 2018-10-15T12:03:57.812Z Reads: 54

```
Thank you so much, that makes total sense
```

---
## \#10 Posted by: Carret Posted at: 2018-10-15T21:19:06.039Z Reads: 46

```
I think it's my BMS, I measured the voltage before the BMS and it read 36v, and after the BMS it read 9, so should I replace the BMS?
```

---
## \#11 Posted by: M.Hboards Posted at: 2018-10-15T22:55:16.236Z Reads: 46

```
could be a few things 

one: your bms is bad (you can bypass it for charge only to fix this or replaced it )

two: you have a bad connection (a spot weld disconnected)

three: your cells are out of balance( measure each parallel pack with a multi meter to find out which one it is)
```

---
## \#12 Posted by: Carret Posted at: 2018-10-15T23:11:53.188Z Reads: 41

```
How off do the packs have to be, one says 36.4v and the other days 36.5v
```

---
## \#13 Posted by: Carret Posted at: 2018-10-15T23:25:46.569Z Reads: 41

```
If one of your batteries is discnected, wouldn't it still make a circuit?
```

---
## \#14 Posted by: M.Hboards Posted at: 2018-10-16T00:41:46.563Z Reads: 39

```
it would still make a circuit but it the parallel pack with the loose will lose its voltage must faster then the others so the bms would pick realize that and cut off power.
```

---
## \#15 Posted by: M.Hboards Posted at: 2018-10-16T00:43:56.027Z Reads: 38

```
not talking about the entire packs voltage im talking about the individual parallel packs voltage like @yuweng said
 .
```

---
## \#16 Posted by: Carret Posted at: 2018-10-16T01:12:37.255Z Reads: 34

```
Every battery cells voltage was very close to being the same
```

---
## \#17 Posted by: Carret Posted at: 2018-10-16T01:30:59.853Z Reads: 36

```
Is it dangerous to bypass the BMS for discharge?
```

---
## \#18 Posted by: M.Hboards Posted at: 2018-10-16T03:10:58.769Z Reads: 37

```
[quote="Carret, post:17, topic:71107, full:true"]
Is it dangerous to bypass the BMS for discharge?
[/quote]

most people say its fine there is tons of info on bypassing just use the search button.  I personally use my bms for discharge only. what cells is your battery using?
```

---
## \#19 Posted by: Carret Posted at: 2018-10-16T03:31:04.910Z Reads: 34

```
I'm not sure, I stole both my batteries off of prieviouse longboards, the cells are BFN ICR 18650 170320. I looked them up online and I couldn't find anything though.
```

---
## \#20 Posted by: Carret Posted at: 2018-10-16T03:32:18.430Z Reads: 34

```
Should I replace my BMS, or should I just keep the ones I have and assume i was just drawing to much?
```

---
## \#21 Posted by: yuweng Posted at: 2018-10-16T14:34:12.547Z Reads: 29

```
Since you said you have one spare BMS then just replace it.
```

---
## \#22 Posted by: Carret Posted at: 2018-10-17T03:34:24.338Z Reads: 27

```
I just finished my wiring and it's awesome, I'll do a speed test tommorow because it's pitch black out right now, but it seemed really fast. Though I never got To top speed
```

---
## \#23 Posted by: Carret Posted at: 2018-10-17T19:10:41.520Z Reads: 26

```
It goes 27mph. Thank you so much for your help, I really appreciate it, now I can finnaly ride my longboard
```

---
## \#24 Posted by: Carret Posted at: 2018-10-17T22:21:51.211Z Reads: 25

```
When I am going 27mph my batteries voltage starts to drop pretty fast and then the longboard esc starts to beep, when I stop the voltage climbs really fast back up. Is this because my batteries aren't strong enough?
```

---
## \#25 Posted by: M.Hboards Posted at: 2018-10-17T23:19:51.799Z Reads: 26

```
[quote="Carret, post:24, topic:71107"]
Is this because my batteries aren’t strong enough?
[/quote]

probably I would recommend using Samsung 30q'S
```

---
## \#26 Posted by: M.Hboards Posted at: 2018-10-17T23:24:36.807Z Reads: 26

```
where are you located? maybe I could weld you a new pack.
```

---
## \#27 Posted by: yuweng Posted at: 2018-10-18T02:21:55.833Z Reads: 25

```
you are most welcome, my friend. Quick view on your profile/ previous post seems like you're a speed devil :cowboy_hat_face: These Chinese ESC can go up to 20S with just a few tweaks & more suited for 4WD i guess. For you i think a 13S or 16S might be suitable, if you are interested then attach a high res photo of your controller here & i'll guide you. :sunglasses:

![10Sclogo|690x363](upload://ic3lU2ATINNVln5wmqXSLXJ0Lgq.jpeg) 

In the mean time, may be you wanna bypass the BMS. Just disconnect the wires from P- and connect it to B- and that will bypass the BMS.
```

---
## \#28 Posted by: Carret Posted at: 2018-10-18T03:20:18.857Z Reads: 23

```
I already bypassed it
```

---
## \#29 Posted by: Carret Posted at: 2018-10-18T03:20:41.554Z Reads: 23

```
Thats the only reason why I could hit 27 again
```

---
## \#30 Posted by: Carret Posted at: 2018-10-18T14:20:58.236Z Reads: 19

```
A person right by me is selling a battery pack made up of 30x LG M26 cells, are they any good and would that solve the problem of my batteries losing voltage really fast?
```

---
