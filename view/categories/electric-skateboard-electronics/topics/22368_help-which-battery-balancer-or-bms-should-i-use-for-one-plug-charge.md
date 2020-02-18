# Help. Which battery, balancer or bms should i use for one plug charge

### Replies: 5 Views: 396

## \#1 Posted by: pau Posted at: 2017-05-04T11:28:51.327Z Reads: 64

```
Hey guys, 
This is my first electric skateboard build. 
I dont know what kind of battery system i should use. 
But i know what this system should do. I want a system,   where is only one plug to charge my battery.
For example. When you want to charge your laptop you only have one wire with a plug. And you just put it in your Laptop and it is charging. 

What kind of solution are existing? 
Thank for help. 


Cheers pau
```

---
## \#2 Posted by: aigenic Posted at: 2017-05-04T12:03:04.977Z Reads: 59

```
Depends on your battery, if you have 6s I would charge just with balance charger and use plug like this one: 
https://miamielectricboards.com/shop-1/ez
If you have higher voltage or li-ion cells, I would charge with BMS...If you want just one plug, the easist way would be intergrated BMS (in serie with ESC or bypassed)
```

---
## \#3 Posted by: pau Posted at: 2017-05-04T12:42:52.252Z Reads: 57

```
I think i will go for 6s. But i relized that 6s has a big size. There are to fat/height.  So i think it is better to have 2 3s and connect them in series. 
Is this still possible with that simple chargin port wire? 

If i want to do it with a bms. Is it much more expansive? And what do i need for that? If i want to use 2 3s lipo batteries?
```

---
## \#4 Posted by: aigenic Posted at: 2017-05-04T18:43:55.572Z Reads: 51

```
If you want to use 2 3s baterries you will have to modify the balance plugs (from 8 cabels to 7...it should be quite simple, i have an idea how, but i dont want to post it here, because i am not sure if it is correct :D ) 

As I said, tehre are three ways...you can buy charging port like the one I posted (or make a pair yourself)  and then you could charge with normal balance charger ( IMax B6ac is quite good and not too expensive). But you would have to use bigger plug with at least 9 connections) 

Or you can buy BMS, which supports discharge current bigger than you max motor Amps, you would connect it to baterry and to balance leads, then to ESC...This is probably the most expensive way

If you dont want to buy expensive BMS, you can buy cheaper and bypass it (just search forum), the disadvantage is, that you would loose some protections, which BMS can offer, like low/ high voltage protection (just during ride, if you charge it, it will protect the baterries from being overcharged)

If you decide to go with BMS you would also need a power source (similar to what you use to power your laptop) rated for the same voltage as the max voltage of your batteries...

The cleanest and simpliest way is to buy bigger MS and use it even during discharging...using smaller bypassed BMS is also a nice and clean way, but  you would need some other mecahnism to protect your batteries from low voltage (VESC, voltage meter)

BTW. sorry for my English...
```

---
## \#5 Posted by: aigenic Posted at: 2017-05-04T18:45:27.590Z Reads: 44

```
To be sure what is the cheapest, just search the internet...and find prices for 25.2V power supply, 6s lipo BMS, IMax balance charger...
```

---
