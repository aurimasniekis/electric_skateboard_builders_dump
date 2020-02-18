# 13S A Realistic Possibility?

### Replies: 16 Views: 1394

## \#1 Posted by: pshaw Posted at: 2017-11-17T02:40:13.501Z Reads: 272

```
How many of you have had a decent amount of time running 13S. Apparently our current available hardware can handle it... it's just a little odd to fit in most setups. Any 13S out there?
```

---
## \#2 Posted by: b264 Posted at: 2017-11-17T02:44:38.448Z Reads: 270

```
Technically, it can handle 14S, according to the numbers I'm reading, but it's WAY, WAY, WAY better to not push electronic components to their full rated capacities....  (@4.285V / cell maximum)

I'd stick to 10S normal and 12S max personally...  Maybe 14S for a one-run dragster record-breaker but not a daily rider board

Also keep in mind motors are a reactive load... that can feed back-pressure into the circuit, easily pushing the numbers past their ratings...

Maybe I shouldn't have put this here because now lhb is going to make a 14S LoLz

No, seriously, if you faceplant tarmac from a 13S or 14S burning up your controller, you can't say you weren't warned
```

---
## \#3 Posted by: mmaner Posted at: 2017-11-17T02:50:55.216Z Reads: 259

```
That's why I run 10s, I can bury the throttle and brake and not have to worry about blowing a vesc. I would worry all the time at 12s.
```

---
## \#4 Posted by: b264 Posted at: 2017-11-17T02:54:49.474Z Reads: 247

```
Everyone keep in mind the standard rule of thumb when engineering electronics is 50%  
  
So a EE designing a product to be UL-certified and mass produced and sold --- will take one look at the VESC they'd run it max 7S by default.  So 10S and especially 12S are already at 72% and 86% capacity already -- plus the pressure from the inductor flyback in the motors ...

TL;DR: play with fire, get burned
```

---
## \#5 Posted by: scepterr Posted at: 2017-11-17T03:14:27.792Z Reads: 232

```
I ran a 14s5p mj1(@4.05v/cell) 30A limited ebike pack I made on my board just for shits and giggles, around the block with brakes turned off. Thank God I have bindings 😂
That's another 14s5p completed sitting behind, combine to make triangle 😉 
<img src="/uploads/db1493/original/3X/8/b/8be092481a917ebb9e8ada3f11f44a315a03bea5.jpg" width="375" height="500">
```

---
## \#6 Posted by: b264 Posted at: 2017-11-17T03:38:04.280Z Reads: 213

```
[quote="scepterr, post:5, topic:38581"]
I ran a 14s5p mj1(@4.05v/cell) 30A limited ebike pack I made on my board just for shits and giggles, around the block with brakes turned off.
[/quote]

Charging only to 4.05V / cell might have saved your ass from tarmac-burn  -- that's the difference between 99.9% max and 94.5% max
```

---
## \#7 Posted by: E1Allen Posted at: 2017-11-17T06:14:23.443Z Reads: 190

```
C'mon guys. Pushing the limits only drives creativity to create better equipment. 24S please.
```

---
## \#8 Posted by: Ackmaniac Posted at: 2017-11-17T12:56:33.186Z Reads: 168

```
My Mountainboard is currently a 13S (Li-Ion) but i did not charge the battery 100% so far. That will need some modifications where i am currently waiting on parts. And firmware changes to protect the system from over-voltage are also in beta status. Will let you know when i know more.
```

---
## \#9 Posted by: pshaw Posted at: 2017-11-17T18:15:26.982Z Reads: 145

```
[quote="Ackmaniac, post:8, topic:38581, full:true"]
My Mountainboard is currently a 13S (Li-Ion) but i did not charge the battery 100% so far. That will need some modifications where i am currently waiting on parts. And firmware changes to protect the system from over-voltage are also in beta status. Will let you know when i know more.
[/quote]

What modifications are you speaking of to run with 100% charge? I’m assuming you mean hardware as you mention software in the works....
```

---
## \#10 Posted by: b264 Posted at: 2017-11-17T22:58:35.265Z Reads: 141

```
[quote="E1Allen, post:7, topic:38581, full:true"]
C'mon guys. Pushing the limits only drives creativity to create better equipment. 24S please.
[/quote]

I can't agree more.  Get to work on this new open-source ESC that can handle 200 volts at 100 amps
```

---
## \#11 Posted by: pshaw Posted at: 2017-11-18T00:32:17.241Z Reads: 136

```
Hah. It’s actually mind-boggling that our “best esc” available is actually just a slightly less shitty version of the vesc (vesc6). Still has DRV... still only is capable of 95% duty cycle... etc etc. 

And this polished turd I speak of is damn near 300 bucks to get to the states. 

Someone needs to pick up where Rafael Chang left off and finish the infinity esc. Everything is out there and publicly available ... just need someone to finish the coding. 

End rant lol
```

---
## \#12 Posted by: pixelsilva Posted at: 2017-11-18T00:53:03.394Z Reads: 132

```
[http://i.imgur.com/iNsvEnJ.gif](http://i.imgur.com/iNsvEnJ.gif)
```

---
## \#13 Posted by: Deckoz Posted at: 2017-11-18T02:06:11.822Z Reads: 129

```
My next board is 13s.  Yep I'm not skeered.
```

---
## \#14 Posted by: b264 Posted at: 2017-11-18T02:14:30.791Z Reads: 130

```
[quote="pshaw, post:11, topic:38581"]
Hah. It’s actually mind-boggling that our “best esc” available is actually just a slightly less shitty version of the vesc (vesc6). Still has DRV... still only is capable of 95% duty cycle... etc etc.
[/quote]

I know two people that could design a better one.  There are two problems.  1) it'd take a shitload of time 2) it'd cost more  
Nobody I know is willing to give away a thousand hours in free labor to make it a reality.  If a few different skate companies all came together behind it, it could be a reality very easy.  Unfortunately, skate companies don't work together very well.  Then you have companies like tramppa who think they can just take over an open-source project, which discourages anyone else from touching it.  Should I go on?
```

---
## \#15 Posted by: pixelsilva Posted at: 2017-11-18T04:06:39.782Z Reads: 125

```
Naaa-aaahh, we just imagine the sink hole you are talking about. Thats why foxes and other cuties are coming up lately.
```

---
## \#16 Posted by: Pambalos Posted at: 2019-11-03T19:55:31.897Z Reads: 39

```
Can you post a link to the infinity project? I'd like to take a look at it
```

---
