# Building an extra battery pack for a Raptor 2

### Replies: 37 Views: 2272

## \#1 Posted by: Eboosted Posted at: 2018-01-16T00:07:40.797Z Reads: 285

```
So, after more than a year waiting, at last I got my Raptor 2.

I removed the battery before shipping it to Lima Peru, so I could have one battery ready for my trips in USA and wouldn't have the need to make an expensive international battery shipment every time I travel with my batteryless board.

[img]https://i.imgur.com/Laki2Re.jpg[/img]

I'm going to build a new battery pack:
[img]https://i.imgur.com/yUcfRWx.jpg[/img]
[img]https://i.imgur.com/f1EYhJR.jpg[/img]

However in order to wire the BMS into the battery correctly I need the Enertion BMS pin out order.

Is there a way to detect whats pin goes to what positive side pack? An incorrectly wired BMS could burn the BMS.

[img]https://i.imgur.com/xtmierK.jpg[/img]
[img]https://i.imgur.com/CsxZq7l.jpg[/img]

There are eleven pins on the BMS, can someone send me a picture of their Space Cell battery just to see which one is pin #1?
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2018-01-16T00:13:19.448Z Reads: 271

```
@blasto could probably help you with the pinout of the bms
```

---
## \#3 Posted by: ATLesk8 Posted at: 2018-01-16T00:55:18.696Z Reads: 265

```
The bms is not part of the battery pack in this setup correct? Thats an interesting design decision. I think it's nice and efficient as you only need one bms for as many battery packs as you desire.
```

---
## \#4 Posted by: Skitzor Posted at: 2018-01-16T00:56:33.648Z Reads: 260

```
Yeah, but that LCD looks likes someone spilled loctite all over the place
```

---
## \#5 Posted by: Surfer Posted at: 2018-01-16T19:39:30.542Z Reads: 240

```
Oohhhh!!! congratulations for your new toy!!! i love the R2!
@Blasto what do you think about to run this hubs with 12S?
```

---
## \#6 Posted by: Battosaii Posted at: 2018-01-16T20:04:39.817Z Reads: 224

```
Someone will do it soon enough, it should be pretty insane at 12s I'm still waiting for mine to show up to try it out.
```

---
## \#7 Posted by: DavidBanner Posted at: 2018-01-16T20:04:42.961Z Reads: 219

```
use a multimeter on the bms plug on the battery pack...

ahh hang on, do you have access to the battery pack?
```

---
## \#8 Posted by: Eboosted Posted at: 2018-01-16T23:02:40.642Z Reads: 213

```
I'm building a new battery pack tonight, as soon as I finish it and plug it on the board, I'll measure the voltages from the BMS pins
```

---
## \#9 Posted by: Blasto Posted at: 2018-01-16T23:24:01.288Z Reads: 214

```
I’ll probe my battery when i get home in a few hours.

Yes 12S should be pretty insane
```

---
## \#10 Posted by: pat.speed Posted at: 2018-01-16T23:28:54.784Z Reads: 211

```
Isn't it a 10s bms, if so how will he wire it for 12s?
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2018-01-16T23:33:31.481Z Reads: 208

```
He need to change the bms, but with a 12s3p configuration, he should be able to fit a second bms for the 12s
```

---
## \#12 Posted by: pat.speed Posted at: 2018-01-16T23:34:08.649Z Reads: 206

```
Ahhh ok

10 chars
```

---
## \#13 Posted by: Blasto Posted at: 2018-01-16T23:35:09.516Z Reads: 201

```
Yeah it’s a 10S bms. Can’t use it and would need to put a zeors resistor on the switch to not use a bms at all (r6 i believe, says by-pass on the silkscreen)
```

---
## \#14 Posted by: pat.speed Posted at: 2018-01-16T23:35:46.840Z Reads: 196

```
So why does he need the pin out then?
```

---
## \#15 Posted by: JohnnyMeduse Posted at: 2018-01-16T23:38:23.543Z Reads: 196

```
Because he want to make a replacement battery for the Raptor, not a completely different battery

[quote="Eboosted, post:1, topic:43818"]
I removed the battery before shipping it to Lima Peru, so I could have one battery ready for my trips in USA and wouldn’t have the need to make an expensive international battery shipment every time I travel with my batteryless board.
[/quote]
```

---
## \#16 Posted by: pat.speed Posted at: 2018-01-16T23:40:27.603Z Reads: 190

```
I understand that but if wants to make a new battery that is 12s he won't be able to use the existing bms? So why does he need the pin out, I think I'm kinda lost here
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2018-01-16T23:43:25.449Z Reads: 189

```
He never mentioned wanting to do a 12s Battery this only as been a suggestion from other people 😉
```

---
## \#18 Posted by: pat.speed Posted at: 2018-01-16T23:45:46.971Z Reads: 190

```
Oh I understand now. I read a post up a bit and thought he was meaning this board was going to run 12s. Thanks mate
```

---
## \#19 Posted by: darkkevind Posted at: 2018-01-16T23:57:37.239Z Reads: 197

```
Is it not labelled B+ & B- at each end of the 11 pins?
```

---
## \#20 Posted by: Blasto Posted at: 2018-01-17T01:55:02.311Z Reads: 194

```
![image|375x500](upload://1r3w1R2tWpi5zAzDChssyybm7ls.jpeg)![image|375x500](upload://9eSYbVubaxIEX04zzOkzugz1ydQ.jpeg)

Jst xh 11 pin
```

---
## \#21 Posted by: Eboosted Posted at: 2018-01-17T04:00:23.278Z Reads: 187

```
So I understand the black wire goes to the negative of battery pack, the remaining to each positive of each pack in order respectively?

@blasto thanks man!
```

---
## \#22 Posted by: Eboosted Posted at: 2018-01-19T03:18:44.578Z Reads: 182

```
I finished the battery today, but before connecting the balancing wires I went ahead and connected the battery, however the board doesn't not turn on.

I wonder if there is some kind of safety device that prebent the board from turning on if the balancing wires are not connected.

I checked the fuse and it was ok.

Any input will be appreciated.

thanks!
```

---
## \#23 Posted by: Blasto Posted at: 2018-01-19T03:22:37.998Z Reads: 180

```
[quote="Eboosted, post:22, topic:43818"]
I wonder if there is some kind of safety device that prebent the board from turning on if the balancing wires are not connected.
[/quote]

yes the BMS controls the main switch, the balance wires must be plugged. You also might need to plug the charger once to kick out the BMS of it’s low voltage state
```

---
## \#24 Posted by: Eboosted Posted at: 2018-01-19T03:31:26.606Z Reads: 181

```
[quote="Blasto, post:23, topic:43818"]
the balance wires must be plugged. You also might need to plug the charger once to kick out the BMS of it’s low voltage state
[/quote]

I'm going to use a 11 pin JST connector but I'm still unsure on the correct wiring.

Would you please help me out letting me know in this picture what is the positive of first pack? does the first wire goes to negative of the battery?

https://i.imgur.com/CsxZq7l.jpg
```

---
## \#25 Posted by: Blasto Posted at: 2018-01-19T03:35:12.755Z Reads: 181

```
![image|542x500](upload://fOaP7EFLyLntGkvC7JP0oSZ6zaH.jpg)

![image|690x389](upload://djjBhxE1Hwx7SVArPTIoRUldoma.jpg)
```

---
## \#26 Posted by: Lobap Posted at: 2018-02-25T23:11:59.685Z Reads: 161

```
Do you have by chance the wiring diagram of the Raptor 2??? 

I have the Space Cell 4 (whithout bms + switch + plug) but going through some trouble to connect it to my dual FOCBOX diy build! Thanks.
```

---
## \#27 Posted by: Eboosted Posted at: 2018-02-26T00:45:31.276Z Reads: 157

```
Well today it's the first test.

I'm travelling to Orlando with my Raptor with no battery

[img]https://i.imgur.com/1oxV7d3.jpg[/img]

I wonder if they could refuse the boarding by not believing that the eboard has no battery, I'm taking an allen wrench to take off the enclosure in case they want to verify it.
```

---
## \#28 Posted by: mikenyc Posted at: 2018-02-26T00:58:06.235Z Reads: 152

```
Can you make a R2 enclosure for the evo with battery meter/power button window? Thx!
```

---
## \#29 Posted by: JohnnyMeduse Posted at: 2018-02-26T01:14:30.482Z Reads: 149

```
You can just switch the Regular enclosure of the Raptor2 to a new deck.
```

---
## \#30 Posted by: Eboosted Posted at: 2018-02-26T01:29:48.164Z Reads: 145

```
[quote="mikenyc, post:28, topic:43818, full:true"]
Can you make a R2 enclosure for the evo with battery meter/power button window? Thx!
[/quote]

I don't get it, you want the R2 design? or a copy of the enclosure?
```

---
## \#31 Posted by: mikenyc Posted at: 2018-02-26T01:44:18.406Z Reads: 140

```
The same enclosure you made for the Evo, but with the window cut out, I guess. Trying to keep it as “factory feeling” as possible. 

Otherwise, I’m swapping over to the blood slayer
```

---
## \#32 Posted by: JohnnyMeduse Posted at: 2018-02-26T02:02:22.988Z Reads: 137

```
Are you in a hurry to swap it to the bloodslayer ?
```

---
## \#33 Posted by: mikenyc Posted at: 2018-02-26T02:03:35.584Z Reads: 136

```
No, I’m waiting for this enclosure riser pad that’s supposed to come out
```

---
## \#34 Posted by: JohnnyMeduse Posted at: 2018-02-26T02:06:53.254Z Reads: 136

```
Because they are still working on there design, but Zenit https://www.zenitboards.com/fr/ are working on something similar to the bloodslayer, but lighter... [spoiler]and who knows maybe a version with an enclosure integrated[/spoiler]
```

---
## \#35 Posted by: mikenyc Posted at: 2018-02-26T02:54:05.994Z Reads: 133

```
Wow integrated enclosure would be dope. I checked out zenit after trying your deck when you were in nyc. I really liked it. 

I already got the blood slayer though, but no reason I can’t use it for a different build.
```

---
## \#36 Posted by: willpark16 Posted at: 2018-05-28T22:12:14.734Z Reads: 114

```
Did it work?
```

---
## \#37 Posted by: Eboosted Posted at: 2018-05-29T05:23:59.043Z Reads: 97

```
It did work at the moment, I was able to cross customs and airport security with no issues at all, however when I went to pick up the spare battery to my friend house I found out he had flown out of the city for work.

So I had to take my board back without even riding it.
```

---
