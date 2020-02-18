# Battery, lipo or li ion?

### Replies: 12 Views: 3816

## \#1 Posted by: AlvinB Posted at: 2019-04-14T09:58:58.357Z Reads: 131

```
Hi, I have been trying  to choose a battery for my build, I have been leaning towards two of these batteries connected in series, but I think they need a higher c rating.

https://hobbyking.com/en_us/turnigy-graphene-professional-12000mah-6s-15c-lipo-pack-w-xt90.html

Another option would be a li ion battery like this one:
https://www.mboards.co/collections/all/products/12s4p-complete-battery-solution

But it's kinda pricey. 
Does anyone have a suggestion on a 6s lipo battery? Or should I make my own li ion battery?


Thanks.
```

---
## \#2 Posted by: mynamesmatt Posted at: 2019-04-14T10:09:49.664Z Reads: 122

```
firstly avoid mboards. i hear bad things about him, and he really only sells relabelled Chinese trash.

those graphene batterys can still produce 180a of current constant. and at 12s you'll never need that. also, those batteries have little to no sag towards the end of the batteries capacity.

If you want similar performance in liion, you'll need a very high p count to get the sag-less performance and current output.
```

---
## \#3 Posted by: AlvinB Posted at: 2019-04-14T10:58:02.247Z Reads: 110

```
So the c rating does not matter?
```

---
## \#4 Posted by: Bobby-gg Posted at: 2019-04-14T11:31:27.918Z Reads: 105

```
Yes, the c rating maters, but that's a 12000mAh battery so with a c rating of 12 it's a constant 144A output.

But how are you going to charge them? 

I use 2 hobbyking zippy 5s 5.8aH lipos in series at the moment and charge them individually using a lipo balance charger whereas if you get a battery with built in bms you can just plug it in to charge the whole battery in one go relatively safely
```

---
## \#5 Posted by: Gaza65 Posted at: 2019-04-14T11:39:36.965Z Reads: 101

```
Depends if want to mount your batteries on-top or underneath...me I prefer on-top for going over all terrain... MTB is my thing...good if you can try a board or 2 get a better understanding...
```

---
## \#6 Posted by: AlvinB Posted at: 2019-04-14T11:55:09.228Z Reads: 98

```
I will probably use a lipo BMS.

Probably this one:
https://alienpowersystem.com/shop/bms/battery-bms-with-switch-for-12s-lipo-battery/
```

---
## \#7 Posted by: Schulerbible Posted at: 2019-04-14T12:04:17.677Z Reads: 93

```
Lipos all the way. What we need are custom lipos with a more sleek form factor to fit inside a slim skateboard enclosure.
```

---
## \#8 Posted by: mynamesmatt Posted at: 2019-04-14T18:43:29.284Z Reads: 80

```
that bms will work great. it's the one i have as well. you just need to remember that you're limited to 80a total discharge from the battery to the vesc (which is usually enough). if you wanna run more current to your vescs then run a charge only bms
```

---
## \#9 Posted by: AlvinB Posted at: 2019-04-14T19:48:20.877Z Reads: 76

```
Any suggestions on a better, I have a high budget.
```

---
## \#10 Posted by: MysticalDork Posted at: 2019-04-14T21:12:22.244Z Reads: 65

```
One of the main design considerations between li-ion and li-po is the distinction between specific energy and specific power. Li-ion wins by a large margin in terms of specific energy (Watt-hours per volume), whereas li-po wins by a large margin in specific power (Watts per volume). Those lipos have about 0.33 Kwh per liter, where a 18650 pack has about 0.51 - A 55% increase. (And yes, that is taking into account the inefficient packing of round cells. It's even better if you ignore that.)

On the other hand, the li-ion cell can only produce 292 watts per liter, whereas the li-po can produce 1200 - A clear advantage for li-po.

Thus the choice between the two comes down to a question of range vs size vs power. For a given size, you will get more range but less power with li-ion, and the inverse with li-po. 

Above a certain size though, the power advantage stops mattering so much - You just aren't going to use more than X amount for a given vehicle design - You run into other limits like tire grip and the ability to stay on the board. Above that size, li-ion is the winner because you have all the power you need, and 55% more range. It's just a matter of figuring out where that point is for you.


TL;DR, li-ion is better for large packs, li-po is better for small light packs.
```

---
## \#11 Posted by: AlanZhou Posted at: 2019-04-15T15:33:00.045Z Reads: 41

```
[quote="MysticalDork, post:10, topic:90473"]
Above a certain size though, the power advantage stops mattering so much - You just aren’t going to use more than X amount for a given vehicle design - You run into other limits like tire grip and the ability to stay on the board.
[/quote]


Um sir but I'm building a 13s10p... Lots of the issues you discussed can be fixed easily, longer decks, vicious grip tape, 4wd..
```

---
## \#12 Posted by: epster Posted at: 2019-04-15T16:08:09.199Z Reads: 37

```
Yeah but you are kinda exceptional haha. For most normies/ cruisers a 12s4P is plenty. If you are upgrading from that you will have to need to pay attention to the things you just mentioned. But personally   I think that kind off power is quite overkill hahah.
```

---
