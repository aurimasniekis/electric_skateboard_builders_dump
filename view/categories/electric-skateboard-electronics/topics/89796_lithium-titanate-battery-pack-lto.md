# Lithium Titanate Battery Pack(LTO)

### Replies: 18 Views: 795

## \#1 Posted by: bilkenter Posted at: 2019-04-08T13:02:53.767Z Reads: 160

```
Hello everyone,

I saw arguably new and interesting lithium battery which is Lithium Titanate Battery(LTO). It has high discharge and charge current characteristic. Also, it has lower degradation graph when comparing with lithium ion battery. For further information :
 https://en.wikipedia.org/wiki/Lithium-titanate_battery

I am planning to build 18s 1p battery pack. My battery cell features: 
2.3 volt nominal voltage. It varies between 1.5-2.8 volts.
Single cell can charge and discharge 400 amps continuous.

I assume that, I don't need BMS because there is no parallel cell or Am I missing something? What kind of protection do I need when I charge or discharge my battery pack?

I am looking forward to hear your technical suggestions.

Best 
Burak
```

---
## \#2 Posted by: Andy87 Posted at: 2019-04-08T13:06:31.078Z Reads: 151

```
you never balance the cells in a parallel pack, you balance the serial wired p-packs, so you need a bms as soon as you use more than 1s even if you have 1p only.
```

---
## \#4 Posted by: Andy87 Posted at: 2019-04-08T13:08:50.423Z Reads: 144

```
single cell is 2.3V, so 18s would be 41,4V
```

---
## \#5 Posted by: Sn4pz Posted at: 2019-04-08T13:09:19.186Z Reads: 143

```
Right. Duh... :rofl:
```

---
## \#6 Posted by: L3chef Posted at: 2019-04-08T13:11:13.012Z Reads: 144

```
Totally mind fucked to say "I've a 18s eboard"
```

---
## \#7 Posted by: Andy87 Posted at: 2019-04-08T13:16:19.613Z Reads: 137

```
after i have seen @b264 is riding a 12s board, nothing can shock me anymore :relieved: I always first check the nominal voltage :rofl:
```

---
## \#8 Posted by: L3chef Posted at: 2019-04-08T13:24:12.305Z Reads: 125

```
No way he's running 12s!! At least not with an vesc based esc :joy:
```

---
## \#9 Posted by: Andy87 Posted at: 2019-04-08T13:25:10.070Z Reads: 118

```
12s LiFePo4.... still below 10s LiIon ;)
```

---
## \#10 Posted by: L3chef Posted at: 2019-04-08T13:26:23.471Z Reads: 118

```
Ah i see :grin:
```

---
## \#11 Posted by: rusins Posted at: 2019-04-08T15:46:27.673Z Reads: 87

```
What cells are you thinking of using and from where? I'm certainly interested in seeing how this turns out, for science!
```

---
## \#12 Posted by: Davide Posted at: 2019-04-08T16:00:54.194Z Reads: 77

```
I’m really curious about this battery! Where are you getting the cells from?
```

---
## \#13 Posted by: ZachTetra Posted at: 2019-04-08T16:03:22.698Z Reads: 76

```
They are on AliExpress for $20 a cell...so $360 in cells but hella performance

It would be 15Ah and 90A/180A but also 5kg

Just under the weight of a 12s10p of 18650
```

---
## \#14 Posted by: Andy87 Posted at: 2019-04-08T16:24:24.648Z Reads: 72

```
[quote="ZachTetra, post:13, topic:89796"]
hella performance
[/quote]

5kg 🤔 thats 100 18650 cells 💁‍♂️ 10s10p maybe better in this case.

Don’t see that great performance if to compare it. Even the price isn’t better.
```

---
## \#15 Posted by: bilkenter Posted at: 2019-04-08T16:27:46.555Z Reads: 62

```
There are some seller on Aliexpress and Alibaba. This battery technology has some advantages and disadvantages over lithium ion. You should use or not according to your priority.
```

---
## \#16 Posted by: rusins Posted at: 2019-04-08T16:30:46.327Z Reads: 60

```
If my calculations are correct then 30Q has an energy density of 165.4Wh per litre, and the wikipedia page says that some lithium titanate batteries are reported to have 177Wh/L :slight_smile:
```

---
## \#17 Posted by: Vykku Posted at: 2019-04-08T16:38:40.705Z Reads: 56

```
Their main advantage are fast charging (Toshiba cells can handle full charge in about 11-12 mins), and high cycle count (90% capacity left after 10k cycles, again for the Toshiba SCiB cells). 

However the high end cells are not available for sale to the general public, and you can only source sketchy Aliexpress ones which haven't been tested extensively (and might be lying about the ratings). Also the Aliexpress ones have way lower density than lithium ion, so a similar battery would be much bulkier.

The technology itself does have a lot of potential for esk8 in the future, but I think that the cells available to the public are not good enough yet. If you do decide to go with the Aliexpress cells, make sure to make a thread about them since it would be an interesting experiment.
```

---
## \#18 Posted by: Andy87 Posted at: 2019-04-08T16:59:55.445Z Reads: 48

```
Very unlikely that i‘ll buy some sketchy AliExpress batteries. I even didn’t research about that kind of battery yet and for me a 5kg battery is way too heavy anyway. If I ever go that heavy a also don’t mind to charge for a longer time. To charge a 18650 with the max charge current they are rated is pretty quick as well. Just not so much of us charge with 16A a 4p pack. Anyway a cycle life of 10k sound very good. Very much hope we get some better batteries in future.
```

---
## \#19 Posted by: Vykku Posted at: 2019-04-08T17:21:31.600Z Reads: 45

```
Sorry, I was referring to OP here but forgot that my comment was a reply to yours:

[quote="Vykku, post:17, topic:89796"]
If you do decide to go with the Aliexpress cells, make sure to make a thread about them since it would be an interesting experiment.
[/quote]
```

---
