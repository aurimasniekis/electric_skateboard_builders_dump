# Lipo power bank

### Replies: 7 Views: 1609

## \#1 Posted by: Sebastiaan Posted at: 2016-03-09T14:08:41.843Z Reads: 98

```
Anyone here ever made a portable lipo power bank by any chance?
I'm currently have a 2 x 5s 8000 mah in series setup at my board.

I was thinking about making a powerbank complete with enclosure and all the bells and whistles to charge my lipo's. I have a iCharger 1010b+ that has to be powered from the powerbank.
The input voltage of the charger is max rated at 18v.

So i was thinking about wiring up 2 x 4s 10000mah in parallel.
http://www.hobbyking.com/hobbyking/store/__56844__Multistar_High_Capacity_4S_10000mAh_Multi_Rotor_Lipo_Pack.html

Would this work?
```

---
## \#2 Posted by: trbt555 Posted at: 2016-03-09T15:32:45.228Z Reads: 95

```
Let me get this straight: you want to power your charger using lipo's, so you can charge other lipo's ?
Can't you just swap lipo's and save yourself a lot of hassle ?

Anyway:
Your destination pack needs 5S x 2 x 8 = 336Wh to fully charge.
Your source power bank has 4S x 10 x 2 = 336Wh available
Taking into account the lower voltage of the source pack and all sorts of inefficiencies and heat losses, you'd most likely not be able to charge your lipo's completely.
```

---
## \#3 Posted by: Sebastiaan Posted at: 2016-03-09T15:58:49.833Z Reads: 85

```
I could swap lipo's but that's a hassle, especially at my current board design. 
My enclosure is just screwed on, the balance cables are connected on a different second part of the enclosure and are also taped in there. Everything leads to external charging ports.

Weird, i only took the mAh in account, thinking with 20000 mAh i could fully charge my lipo's.
```

---
## \#4 Posted by: barajabali Posted at: 2016-03-09T17:30:19.857Z Reads: 78

```
Wouldn't that take a while tho ? What would the amp output be? For the charger. 

What about finding a small enough charger to build into the board and just having to plug it into a wall when you need to? A lot less to carry. More energy efficient. Just need to carry one plug around or find a way to stow it in the board

Is there a theory thread?? I gotta add my thought to it lol
```

---
## \#5 Posted by: claudiofiore88 Posted at: 2016-03-09T18:28:27.645Z Reads: 74

```
I have an Onyx 235 lipo charger.  It has the ability to be hooked up to my car battery with the included alligator  clips.  The only draw back is it only supports up to a 4s lipo. But that defeats the whole purpose of riding your board places.
```

---
## \#6 Posted by: laurnts Posted at: 2016-03-09T20:56:46.834Z Reads: 64

```
This is only a great idea if your power bank is using that Turnigy Graphene! So you could charge your power bank within minutes and theres always power in the backpack :D
```

---
## \#7 Posted by: onloop Posted at: 2016-03-10T07:37:40.596Z Reads: 50

```
i made one yesterday.

https://www.youtube.com/watch?v=Bn3eq3CEu9c
```

---
