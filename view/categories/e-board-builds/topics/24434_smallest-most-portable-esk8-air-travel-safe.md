# Smallest/Most Portable Esk8 - Air Travel Safe

### Replies: 13 Views: 1164

## \#1 Posted by: Charster10 Posted at: 2017-06-02T17:19:20.242Z Reads: 156

```
Hey guys -

This is my 3rd build and I need a bit of help on a few things. 
I know people have done air travel safe builds before but I just can't quite see what would work for me, nevertheless I've started building an air safe esk8 board, and so far I have most of the parts.

I'm building my own small custom deck and I have 20" X 8" of free space in the middle between the trucks and edges (kinda a penny board size but not penny board shape) 

What I'm mainly questioning is: I have 2x 3s 5000mah lipos which are like new and being used. I'm happy using 1 of them on the board as I don't need to travel very far, this board is only going to be used when I take it on holiday and I would just like to cruise a few miles along the coast or in cities. But back to the lipos...would I be able to use a single battery with a vesc and a sk3-5055-320kv motor? 

Thanks! 

_**P.s. I'll upload some photos of the deck and the finished setup if some of you want me too!**_
```

---
## \#2 Posted by: NickTheDude Posted at: 2017-06-02T18:58:10.846Z Reads: 139

```
With one of those lipos you would have about 5km of range and very, very little power if you use a VESC. Probably only 500W max.

If you wired the lipos in series you would have too many watt hours to take on a plane.

My reccomendation would be to get a couple 4000mAh 3S lipos and wire them in series to stay below the 99Wh limit. Then get a hobbyking x-car beast 150A ESC, not only is it cheaper than a VESC but it should be able to put more power down. Also try to get lipos with a C rating higher than 25 so you can output a decent amount of amps without damaging the lipos.
```

---
## \#3 Posted by: Challlsss Posted at: 2017-06-02T18:58:18.051Z Reads: 128

```
I just took my build across the country last weekend! You will be able to carry it straight through TSA depending on deck size. Otherwise you may have to check the board and carry on the batteries.  Just stick with the 6S system, otherwise you will have next to no torque.
```

---
## \#4 Posted by: Challlsss Posted at: 2017-06-02T19:01:07.381Z Reads: 126

```
@NickTheDude
This is not correct for (US) air travel. You are allowed up to 2 101-150 kWh batteries (carry on only) through TSA. 
5 Ah * 6 * 4.2 = 126
```

---
## \#5 Posted by: Charster10 Posted at: 2017-06-02T19:01:15.524Z Reads: 124

```
Ah I see. What would happen if I had my 2 lipos disconnected separately then connect them back up when I arrive in my destination? @Challlsss
```

---
## \#6 Posted by: Charster10 Posted at: 2017-06-02T19:01:55.994Z Reads: 116

```
I normally travel around Europe baring in mind, I'm not from the US :/
```

---
## \#9 Posted by: Challlsss Posted at: 2017-06-02T19:05:17.723Z Reads: 121

```
<img src="/uploads/db1493/original/3X/6/2/621f556e2cc882bdb038cece4591db2586b3c2bc.png" width="690" height="237">
I found this.
Looks like if the airline allows it you may be able to get away with it, but you will likely have to disconnect them.
```

---
## \#10 Posted by: Charster10 Posted at: 2017-06-02T19:08:09.064Z Reads: 117

```
Perfect! What I'll do is I might just try out a 3s setup on a flat...then if it's total shit I'll put the other battery on and keep it like that, thanks for your help !
```

---
## \#11 Posted by: Charster10 Posted at: 2017-06-02T19:09:10.421Z Reads: 115

```
Btw, I already have a vesc spare so there's not much point selling it and buying a car esc
```

---
## \#12 Posted by: Challlsss Posted at: 2017-06-02T19:09:33.715Z Reads: 113

```
you do you... I personally would never do a 3S build
```

---
## \#13 Posted by: Charster10 Posted at: 2017-06-02T19:10:10.902Z Reads: 110

```
I'll test it...for science ey
```

---
## \#14 Posted by: anorak234 Posted at: 2017-06-02T20:34:53.318Z Reads: 102

```
I built something very similar to what you're aiming for (should help a bit):
https://www.electric-skateboard.builders/t/mobious-semi-1-custom-deck-semi-enclosure-airplane-legal-travel-build/6861
Keep in mind, United Airlines and a few others have now completely banned electric skateboards, so be weary of which airline you choose.
```

---
## \#15 Posted by: Charster10 Posted at: 2017-06-02T21:00:14.704Z Reads: 87

```
Thanks! And yeah I noticed... I normally fly with virgin atlantic and emirates (I know for certain Virgin Atlantic allow these batteries) need to check emirates and few other airlines but your setup looks awesome! My deck is sort of a similar shape funny enough, I'll send a picture on here tomorrow once it's been jigsawed-out :) @anorak234
```

---
