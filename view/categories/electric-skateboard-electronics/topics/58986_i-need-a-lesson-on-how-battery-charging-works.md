# I need a lesson on how battery charging works

### Replies: 9 Views: 434

## \#1 Posted by: DeathByBacon Posted at: 2018-06-15T09:04:47.316Z Reads: 119

```
Is it possible to charge a battery with another battery? E.g. Battery A (30Q) charged by Battery B (30Q). How do you control and make sure that Battery B charges Battery A and not the other way around?

The idea is, I have a 10s4p on the board. I want to be able to carry a battery pack in my bag for emergency charging, a 10s2p  that I can plug to the charging port of the board. Is there something I need to do to make sure that the emergency battery charges the pack on the board and not the other way around?
```

---
## \#2 Posted by: solodros Posted at: 2018-06-15T09:25:30.403Z Reads: 113

```
You can use DC-DC boost module to increase the output voltage of battery B to 43v (more than 10*4.25=42.5v). Please pay attention to the heat dissipation of boost module. Also note that battery B requires BMS with undervoltage protection
```

---
## \#3 Posted by: DeathByBacon Posted at: 2018-06-15T09:41:07.319Z Reads: 104

```
Are all dc-dc boost module cccv capable? Does it even matter in this type of setup?
```

---
## \#4 Posted by: Genghis_Kuan Posted at: 2018-06-15T09:42:11.342Z Reads: 102

```
Hate to be generic and use the classic water example but basically if you connect the two batteries together there is a voltage difference (Water level height difference) the battery pack with the higher voltage will discharge it self (Water will flow from high to low) till both packs are at equilibrium (Water level height is the same). 

To discharge one battery completely and charge another you will need some sort of charging circuit which will mostly feature a boost converter as mentioned above.
```

---
## \#5 Posted by: Genghis_Kuan Posted at: 2018-06-15T09:47:45.456Z Reads: 83

```
If you think about it, you have a limited amount of power able to come from your battery unlike a wall socket which can output constant power. So it will be CV CC for as long as it can discharge at that level then they will most likely both drop (Not too sure) which is why youll need to design or buy a charging circuit which 'switches off' the battery doing the charging when it can no longer provide enough power
```

---
## \#6 Posted by: DeathByBacon Posted at: 2018-06-15T10:01:12.820Z Reads: 75

```
Do You  think  this setup will work? 

**Battery**: 10s2p or 8s4p

**DC-DC Step Up**: 
https://www.ebay.com/itm/DC-DC-10-40V-To-12-50V-6A-240W-CCCV-Boost-Converter-Step-up-Power-Supply-Module/262658050654?hash=item3d27a3ca5e:g:I48AAOSw0xRZpoZT

**BMS: For charging**, discharging, and low voltage cutoff
https://www.ebay.com/itm/Max-40A-Balance-Battery-Protection-Board-BMS-PCB-For-36V-10S-10Packs-Li-ion-Cell/311862435323?hash=item489c731dfb:g:yXoAAOSwX61ZCgP~

Is it possible to charge while riding? Or am I pushing it a bit too far?
```

---
## \#7 Posted by: Genghis_Kuan Posted at: 2018-06-16T00:31:08.158Z Reads: 50

```
Im not an expert just some kid that studies engineering and knows basic physics principles, but I think it would until like I said the packs come into equilibrium and water stops flowing. If your gonna have them charge while riding why not just make a bigger pack with more cells in parallel that you can disconnect when you dont need em?
```

---
## \#8 Posted by: Wilsonliang777 Posted at: 2018-06-16T01:58:40.204Z Reads: 45

```
Wouldn't be simpler to just made a enclosure bigger and put the 10s4p battery in the board and change the battery as needed.
```

---
## \#9 Posted by: LittleSheepz Posted at: 2018-06-16T02:49:43.386Z Reads: 41

```
Think of it as a phone battery charged with a portable charger. The phone battery is at 3.7 - 4.2V kept balanced by the BMS. While the portable charger is at constant 5V out(kept balanced by the BMS and an DC-DC Output board), 0V when the battery's juice ran out. Though charging efficiency is only avg at 70-90%. Once the phone is fully charged, when still connected, charging efficiency will be converted to heat waste.

Though the challenge here is to find a constant 42V output for the portable charger to charge your skateboard. Frankly, would be better off changing battery packs/carrying a Ac-DC Charger.

P.S There's no off-the-shelf 42V Constant output board. Most available are in 3.3v/5v/12V. If designing your own 42V Constant output board and considering the heat dissipation needed for the board. It would feel like I'm carrying a tank of heatsinks. NOT PRACTICAL.
```

---
