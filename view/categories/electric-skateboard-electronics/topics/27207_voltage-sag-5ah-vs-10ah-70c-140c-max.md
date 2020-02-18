# Voltage sag, 5ah vs 10ah, 70c/140c max

### Replies: 8 Views: 506

## \#1 Posted by: lunasicc Posted at: 2017-07-10T05:01:02.768Z Reads: 84

```
i currently have (4) 4S 5000mah 70c lipos. i will be running 8s on my emtb. i would like to run just 2 packs in series(5ah total) and carry the other 2 in my pack while riding, keep some weight off my board and it looks more tidy/less wiring. my only concern with this is voltage sag. theoretically, wouldnt i loose a slight amount of range compared to just running them all at once? and what about power delivery, when the battery is near 10-15% remaining? will i notice a difference in power?
thanks in advance for the input
```

---
## \#2 Posted by: Okami Posted at: 2017-07-10T06:18:30.040Z Reads: 74

```
70c looks like good figure to go with..

<img src="/uploads/db1493/original/3X/5/d/5d0a29e7c16c78e118e7657761f74ab7e8601ba6.png" width="681" height="494">

Use this tool:

http://calc.esk8.today

I would say 300Amps is plenty. People usually say to downrate the rating, so I chose 60c, not 70.

--

From range perspective with mountainboard.. 148wh is not a lot go to go with. With regular elongboard you might be able to go about 8 miles /13km but mountainboard takes more energy, so I would say maybe 5miles / 7 km with mountainboard.

Can you shed some details what mountainboars setup u have in firstplace?
```

---
## \#3 Posted by: lunasicc Posted at: 2017-07-10T07:36:09.884Z Reads: 50

```
trampa holy pro, e toxx direct drive5:1, max6 esc's, 8s, 240kv aps hev motors(maybe if i decide to wait long enough for them to ship) if not ill run 200kv. i know the 148wh isnt much. but i would always be riding with a small backpack anyway so i could just throw the other charged batterys in there. i would actually prefer that. i just didnt know if there would be any feelable voltage sag, im sure with a 25c battery it would be bad
```

---
## \#4 Posted by: Okami Posted at: 2017-07-10T07:38:00.236Z Reads: 45

```
Well I dont know yet how it might perform in bmx track.. but 8000w of max power delivered from batteries (8s 5ah 70c) sounds like way enough :slight_smile:
```

---
## \#5 Posted by: lunasicc Posted at: 2017-07-10T07:43:41.583Z Reads: 43

```
thats kind of what i figured to, just not sure as im new to this. thanks for the reply! i think your the most frequent poster on this forum:joy:
```

---
## \#6 Posted by: Okami Posted at: 2017-07-10T09:55:50.723Z Reads: 35

```
Lol.. i hope that is not a bad reputation, there are days when Ive got a bit more time and then I can chime in on such battery related / mountainboard questions a few times.. 

I just know it sometimes sucks when nobody replies you, so I kind of try not to put people in this situation by giving at least some info to feed on.

@lunasicc
```

---
## \#7 Posted by: NAT-Frank Posted at: 2017-07-10T16:49:33.215Z Reads: 26

```
For what its worth, I'm running 2 x 5S 5000mah 25C Nanotechs in series and I get no voltage sag at all with a single 6374 motor and I weigh 190lb. Hard acceleration and small hills have no effect at all.
```

---
## \#8 Posted by: Okami Posted at: 2017-07-10T17:44:56.892Z Reads: 23

```
10s = 37v X 5 ah x 25C
= 

4625 W of Power. 

_I wonder are there any specific levels which trigger higher voltage sag (like how close to maximum cell can deliver vs the voltage drop made)_

I would say you @NAT-Frank get plenty of 'reserve then', as you probably max consume only ~50A x 37v =  1850 W.. Which leaves about 50% of power deliverable (at least from what they claim)

---
Though, it looks like it might also be related with how the cell are made and what chemistry it is. 

I dont know how much different effect these Graphene cells has but I know they have been marketed and branded as high grade ones, even at lower C ratings I think.

I know this is true for different types of Li-ion cells. Different type of cells experience different levels of voltage sag, even sometimes when their ratings might be close to each other, one cell might be way better than the other one.. Or their curves might be very individual, with sometimes 'capacity pockets' and points at which their voltage starts to drop rapidly.
```

---
