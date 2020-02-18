# I think I fried my new bms help

### Replies: 5 Views: 173

## \#1 Posted by: Uc21 Posted at: 2019-05-12T18:50:47.750Z Reads: 77

```
i was wiring my bms when the positive from wire from the volt meter touched the bms one of of the pins fried I soldered it back but I’m not sure if it’s safe to use what do you think at the moment it’s hooked up to the charger and everything seems fine. ![image|375x500](upload://vA9kY3uUFO4qX984iGI8veSPHc7.jpeg)
```

---
## \#2 Posted by: Dirt_Bag Posted at: 2019-05-12T23:02:22.511Z Reads: 62

```
If thats the pin to a mosfet, its might still work. Those mosfets are what let power out of the batteries and to the esc. 

Assuming that mosfet is dead, its not a total loss.

Take the rated amperage of the bms and divide it by the number of mosfets exactly. This will tell you how much each mosfet can handle safely. From now on, subtract the amperage of one mosfet and you now have your safe max amperage. 

When you use this bms for next few times, charge it to a little under maximum battery voltage and then measure each p group manually. It it appears to be balanced correctly every time for about a dozen cycles, the bms is probably ok.

Make sure you let it sit for i would say 2 hours after removing from charger. Just to make sure it has had time to complete a balance cycle.
```

---
## \#3 Posted by: Uc21 Posted at: 2019-05-13T00:01:59.406Z Reads: 47

```
I’ll give it a try thanks you.
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-05-13T03:23:07.959Z Reads: 38

```
[quote="Dirt_Bag, post:2, topic:93595"]
Assuming that mosfet is dead, its not a total loss.
[/quote]

Mosfet is probably gone and it might have taken a trace with it.

@Uc21 might want to Toss that BMS as if it fails it might be wayy more costly then to just replace the bms, not to mention the possible loss a power suddenly
```

---
## \#5 Posted by: Uc21 Posted at: 2019-05-14T00:19:39.709Z Reads: 15

```
Is it normal that the voltage coming through the bus is lower than directly from the pack and I probably will just get a new bms but do you think I can house it just to get the focbox and everything set up?
```

---
