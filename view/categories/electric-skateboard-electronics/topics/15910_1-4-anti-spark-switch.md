# 1.4 Anti spark switch

### Replies: 19 Views: 1395

## \#1 Posted by: Shogu12 Posted at: 2017-01-11T19:02:46.601Z Reads: 224

```
Today I received my antispark switch from @DeathCookies, works great. I soldered it up added a led switch and it works like a charm.  While his price was great and the parts labeled perfectly I'm  in need of 100 more and there is no room for someone else's margins. My questiom now if I make these, do I donate to vedder and how much do you think is appropriate?<img src="/uploads/db1493/original/3X/2/8/2811a935b286178a733f5f4494136b4b82cb2bb0.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/9/7/977ad2a4b5dcf8defe690a321535d8a6a3abbaf3.jpg" width="666" height="500">
```

---
## \#2 Posted by: ajaynagra Posted at: 2017-01-11T19:06:56.085Z Reads: 207

```
How much are deathcookies switches?
```

---
## \#3 Posted by: Shogu12 Posted at: 2017-01-11T19:20:04.554Z Reads: 201

```
If I remember  correctly 28€.
```

---
## \#4 Posted by: DeathCookies Posted at: 2017-01-11T19:35:00.991Z Reads: 195

```
If you are donating please Credit all people who have contributed:
- Jeremy Harris (original idea) 
- Fechter (redesigning The idea) 
- Vedder (redesigning The board) 

It is a pitty that everyone, Lets say The most,  thinks that the switch was invented by vedder on his own...
```

---
## \#5 Posted by: IDVert3X Posted at: 2017-01-11T22:19:07.869Z Reads: 184

```
Its a super simple circuit that was designed in 20th century. Basically it's mosfet as a switch. There is just an addition for the light and stupid car fuse. Why would anyone give credit / donation for something as generic as this? You can even find very similar circuits in some datasheets ( example applications section ) or you can design your own in 15-20 minutes.

I understand it for products like VESC, but for something like that? Really?
```

---
## \#6 Posted by: Pathaim Posted at: 2017-01-11T22:43:33.324Z Reads: 175

```
If you really need 100 go to a manufacturer like Vanda electronics or something, i guess it is a generic item but i think vedder would still appreciate a minimal donation
```

---
## \#7 Posted by: lox897 Posted at: 2017-01-11T22:56:36.054Z Reads: 170

```
[quote="Pathaim, post:6, topic:15910"]
go to a manufacturer like Vanda electronics
[/quote]

Vanda Electronics probably wouldn't be a good place to get these made. They specialise in VESCs. A good place would be MacroFab
```

---
## \#8 Posted by: Karen_Vanda Posted at: 2017-01-17T06:48:13.763Z Reads: 148

```
Hello lox897, 

This is Karen from Vanda Electronics. We offer more than just VESCs. We are making PCBA for electronic/automatic/medical/EV industries...etc for many years. Due to signing NDA with customers, we don't reveal detail info. We will be more than happy to assist you with your project.
```

---
## \#9 Posted by: lox897 Posted at: 2017-01-17T06:49:51.595Z Reads: 142

```
Hi Karen, I was unaware. Thanks for clearing that up!
```

---
## \#10 Posted by: Karen_Vanda Posted at: 2017-01-17T06:51:12.052Z Reads: 144

```
You're very welcome!
```

---
## \#11 Posted by: Eboosted Posted at: 2017-01-18T00:10:33.960Z Reads: 130

```
Karen what is the cost of a VESC? do you stock them?
```

---
## \#12 Posted by: Karen_Vanda Posted at: 2017-01-18T03:06:02.204Z Reads: 132

```
Hello Eboosted, 

USD98 for VESC.
USD110 for VESC with custom cables. 

Yes, we do stock VESC. Please visit our website for more detail info. Thank you. 
https://www.vandaelectronics.com/
```

---
## \#13 Posted by: Shogu12 Posted at: 2017-01-23T10:33:03.472Z Reads: 111

```
I'm  not interested in buying  these from anyone as I've  been trying to make as many parts as I can myself. Question: I've ordered 200pcb's of chaka improved sparkswitch pcb. And wouldnt you know the one I had failed open today :smile:. So my question now should I add heatsinks to the fets to increase cooling and hope that  helps or did I just  waste money?
```

---
## \#14 Posted by: Okami Posted at: 2017-01-28T23:54:33.803Z Reads: 93

```
@Shogu12 So does he have a proper pad for sinking the heat?

I wonder how much of ''conductive'' material there is on the pcb.. to cool down the mosfet..

Definately interested in making one of these, too.. Do you know about how much does it cost to order 5pcbs locally? I would just want to figure out the basic pricing of such service.. otherwise just as well order the pcb's from china.. I've hard ppl have done this before.
```

---
## \#15 Posted by: Shogu12 Posted at: 2017-01-29T00:15:17.545Z Reads: 85

```
6 cost 20$ on oshpark. I've added a heatsink to the back of the board and now it seems to work fine.
```

---
## \#16 Posted by: Okami Posted at: 2017-01-29T00:26:15.628Z Reads: 81

```
Ok cool, thanks for the info! 20 bucks does not sound bad at all.. so next thing is - where to find some fets under 20$.. :D I wonder is it possible to scavange some out of some power electronics.. like power supplies etc..
```

---
## \#17 Posted by: Shogu12 Posted at: 2017-01-29T00:42:27.041Z Reads: 77

```
Honestly just order them from mouser all in all it is like 10$ per switch... the headache of fixing one when it fails is worse than spending an extra 5$ on fets instead of using used/old/wrong ones.
```

---
## \#18 Posted by: Okami Posted at: 2017-01-29T00:47:18.356Z Reads: 82

```
mh, 10$ does sound great.. I dont want to spend 30-40$ just for a ''switch'' so I might as well order some pcb's and get the rest of components..

I've got a simple dc switch now.. but im not sure how long will it hold up.. and either does it add extra resistance or not.. Though, im using 6s li-ion, so voltage is only about 24v max
```

---
## \#19 Posted by: Shogu12 Posted at: 2017-01-29T01:19:26.878Z Reads: 84

```
Its not the 24V that will make your  switch fail but the A that will make it so hot it will solder together.  The sparkswitch with a proper heatsink can handle 80A...well mine does anyways. If someone asks for a quad setup I'll  probably add a 12v fan on the heatsink. I ride dual turningy 6364 260kv on 14s8p lifepo4 battery with 97mm wheels 32t wheel pulley and 15t motor pulley.
```

---
