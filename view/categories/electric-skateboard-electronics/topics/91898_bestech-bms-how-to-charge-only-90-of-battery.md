# Bestech BMS: How to charge only 90% of battery?

### Replies: 17 Views: 253

## \#1 Posted by: Aleks1 Posted at: 2019-04-27T02:23:01.612Z Reads: 92

```
Does anybody knows how to make BMS charge the battery until 90% and discharge until 20%?
![12s_LiPo_Datsheet-2|389x500](upload://AatYQVNxvv65e9yg7iSJiFbhqkM.jpeg) 
Thank you!
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-04-27T02:33:21.191Z Reads: 87

```
when it charges to 90% it means one of your p groups is outta balance and the bms cant correct it

^one of the only ways to make it charge to 90% :rofl:
```

---
## \#4 Posted by: Aleks1 Posted at: 2019-04-27T02:35:23.992Z Reads: 87

```
Mine works good, and charges up to 100%, but I want to limit it to make it safe
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-04-27T02:35:50.988Z Reads: 83

```
i thought that i thought the over charge relase voltage is only for when the cell goes over 4.25v

my bestech d124 even after charging stays at 41.9v
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-04-27T02:36:27.480Z Reads: 73

```
limit it via your charger if it can do it
```

---
## \#7 Posted by: Winfly Posted at: 2019-04-27T02:36:47.456Z Reads: 71

```
Nvm I read the question wrong. 


Edit: the topic title was misleading, so I changed it.
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-04-27T02:37:28.358Z Reads: 66

```
me too at first but then i turned it into a joke :wink:
```

---
## \#9 Posted by: Winfly Posted at: 2019-04-27T02:37:45.555Z Reads: 65

```
You can either get an adjustable charger, or step down your charger voltage to 90% charge voltage with a buck converter.
```

---
## \#10 Posted by: Aleks1 Posted at: 2019-04-27T02:39:28.282Z Reads: 63

```
thanks, sounds like a lot of work😂 Gonna wait until my cells are going to die, and only then I will build new setup)
```

---
## \#11 Posted by: AlanZhou Posted at: 2019-04-27T02:39:59.387Z Reads: 62

```
[quote="Winfly, post:9, topic:91898, full:true"]
You can either get an adjustable charger, or step down your charger voltage to 90% charge voltage with a buck converter.
[/quote]

so you can in theory get a little bit of charge from a 9s charger if you had 10s?

^in a emergency situation
```

---
## \#12 Posted by: Aleks1 Posted at: 2019-04-27T02:41:51.017Z Reads: 60

```
I have 12s Lipo and 50v 1 amp charger. And using 12s 80amp bms
```

---
## \#13 Posted by: Winfly Posted at: 2019-04-27T02:41:52.948Z Reads: 56

```
Yes but it will only charge up to 9S voltage. I borrowed a 10S 6A charger for my 12S during a groupride so I can have more and range.

Gotta make sure that your battery is already lower than the voltage of the charger you are plugging in, so you don't risk breaking your charger if you charger doesn't have reverse current protection.
```

---
## \#14 Posted by: AlanZhou Posted at: 2019-04-27T02:42:41.622Z Reads: 56

```
lol :rofl: welp you learn something evey day

what would happen if your battery voltage was higher than the charger

like.... nvm answered
```

---
## \#15 Posted by: AlanZhou Posted at: 2019-04-27T02:43:51.037Z Reads: 56

```
[quote="Winfly, post:13, topic:91898"]
Gotta make sure that your battery is already lower than the voltage of the charger you are plugging in, so you don’t risk breaking your charger if you charger doesn’t have reverse current protection.
[/quote]

i was just about to ask that :rofl:
```

---
## \#16 Posted by: JLabs Posted at: 2019-04-27T02:58:25.693Z Reads: 55

```
Does anyone know about using a lower voltage charger for a pack? I accidentally grabbed my 10s charger for my 12s pack one day, no hard done, but this would be a really good way to to 100% charge and get to storage voltage.

Realistically I dont think it should do anything, but im not an EE or a battery connoisseur.
```

---
## \#17 Posted by: taz Posted at: 2019-04-27T07:37:25.077Z Reads: 43

```
This is not the proper solution. If you just charge at a lower voltage, the BMS will never start balancing the cells. You either ask the factory if they can adjust the BMS or get a different BMS.
```

---
## \#18 Posted by: Winfly Posted at: 2019-04-27T21:56:32.981Z Reads: 34

```
You right. I think if you order directly from Bestech, you can specify what spec you want your BMS made.
```

---
