# Will this battery kit work with my vesc?

### Replies: 14 Views: 260

## \#1 Posted by: Shiven Posted at: 2018-12-17T02:48:52.908Z Reads: 82

```
I've been looking for a new battery solution for my board (I currently have a 10s2p battery).

I looked around for some pre-soldered batteries and found this place and this kit
(http://www.diyeboard.com/10s5p-360wh-18650-battery-power-kit-with-bmscharger-enclosure-p-572.html)

The kit includes a 10s5p battery, a charger, power button, and a battery indicator.

My question is- is there any way to plug the power button into my maytech vesc? Here is a link to the vesc I have
(https://www.ebay.com/itm/Maytech-Benjamin-Vedder-Electronic-Speed-controller-VESC-for-electric-longboard-/322900537630)
```

---
## \#2 Posted by: ElectricCoast Posted at: 2018-12-17T03:24:12.784Z Reads: 77

```
I'd strongly suggest not to purchase from DIYeboard.  They're products are not the greatest and their customer service is exceptionally poor.  Just my 2 cents worth
```

---
## \#3 Posted by: AlanZhou Posted at: 2018-12-17T03:29:19.897Z Reads: 75

```
Their shipping is read fast though, DHL Express but anyways I agree diyeboard does not use the best of cells
```

---
## \#4 Posted by: J_Dizzle_2.0 Posted at: 2018-12-17T04:35:24.617Z Reads: 67

```
Yes, this pack will work with the vesc. You won't be plugging the power switch into the esc, it is already installed in the enclosure. Most people wouldn't recommend this pack, including me, as although it will work you will experience extreme voltage sag during normal cruising.
```

---
## \#5 Posted by: Shiven Posted at: 2018-12-17T04:52:33.211Z Reads: 54

```
Doesn't the power button need to plug into the vesc?
```

---
## \#6 Posted by: J_Dizzle_2.0 Posted at: 2018-12-17T04:53:54.105Z Reads: 51

```
Yes, sorry, I wasn't thinking straight. Yes solder an xt-90 onto the switch, plug into vesc xt-90. easy
```

---
## \#7 Posted by: sanderfu Posted at: 2018-12-17T18:37:30.274Z Reads: 36

```
Just wanted to mention that the voltage sag is not *that* bad on the 10s5p, its much worse on the 10s2p, the sheer amount of cells somewhat make up for their poor performance. I have the 10s5p pack myself and only experience sag when down to approx 30% which I find okay. Many other better options out there though for lighter and better packs ;) 

And regarding your question, yes it will work but be aware that the vesc may be able to pull more juice than the battery/bms can handle, so use conservative settings and ask others on the forum (I am in the process of upgrading to vescs for this pack myself).

And btw you will need an extra kill switch (or loop key), the button that comes with the diyeboard pack is for their built-in killswitch in their esc.
```

---
## \#8 Posted by: Shiven Posted at: 2018-12-17T22:10:42.638Z Reads: 34

```
Thanks for the reply! Exactly what I was asking!
```

---
## \#9 Posted by: bartroosen12 Posted at: 2018-12-17T22:43:06.010Z Reads: 29

```
Does anyone know which cells this 10S5P pack uses?
Looks like 360Wh/36V = 10Ah so 2Ah/cell
(Samsung INR18650-20R I guess)

Because if that's true, you're better of with a 10S2P with 30Q cells from meepo/wowgo/ownboard
```

---
## \#10 Posted by: dareno Posted at: 2018-12-18T00:06:49.832Z Reads: 27

```
[quote="J_Dizzle_2.0, post:6, topic:78215"]
Yes solder an xt-90 onto the switch, plug into vesc xt-90. easy
[/quote]

The switch on the kit is for the esc that they also sell.    You plug that switch directly into the vesc/ battery and it will go boom boom.  No point in buying that complete kit because the battery meter won't work either.  Get a decent antispark and meter or just use a loopkey.
Those cells and the ownboard and meepo etc are the same lg units.  The factory that produces the diye stuff is the same factory that supplies all those generic chinese brands and the 5p is the best of a bad bunch saying that it will be a marked improvement on the 2p version. 
Better off spending the money on a custom 30q pack.  Don't cheap out on the battery its the heart of the board.
```

---
## \#11 Posted by: Shiven Posted at: 2018-12-18T00:09:30.075Z Reads: 26

```
Awesome! Thanks for letting me know!
```

---
## \#12 Posted by: brenternet Posted at: 2018-12-18T00:16:01.938Z Reads: 26

```
The dickwad who owns that site shared private information of a forum member here recently in a childish outburst. Full name, address, credit card information, email, phone number.. the works.

Untrustworthy to the absolute maximum.
```

---
## \#13 Posted by: b264 Posted at: 2018-12-18T00:42:56.431Z Reads: 24

```
[quote="ElectricCoast, post:2, topic:78215, full:true"]
I’d strongly suggest not to purchase from DIYeboard. They’re products are not the greatest and their customer service is exceptionally poor. Just my 2 cents worth
[/quote]

search this place and reddit for information about diyeboard scams
```

---
## \#14 Posted by: Shiven Posted at: 2018-12-18T00:54:21.613Z Reads: 20

```
Holy crap, I had no idea
```

---
