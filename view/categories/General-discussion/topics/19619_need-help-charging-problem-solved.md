# Need help! - Charging problem\[solved\]

### Replies: 11 Views: 867

## \#1 Posted by: Guacamoleface Posted at: 2017-03-24T12:44:03.016Z Reads: 88

```
Okay, Sun arrived to sweden, decided to put together my temporary charging solution for my board so I got to ride some while sun is here for the weekend.

Set my Imax B6 up with my power supply(16v).. Hook my battery up with it, connected balance cable and power cables.(My battery pack is a split 10s4p - 6s4p and 4s4p both with balance connectors.

I go into my menu of imax set it to lilon and 6s balance charge. I start it detects cells - it finds 5...

I figured it was my balance cable that come off or something.Tried it with my external balance checker - it fins 6, I measure it with multimeter - I find 6. 

So I try it again but my imax still only detects 5 cells.. 
I tried to see so it was plugged in all the way - it was. 
I tried with my 4s - it works fine. Finds 4cells.
I checked all my cells all at 3,4 volts

Im at the point where I consider going buying a E-bike with same setups charger and charge it without balancing it until I get a bms.

The charger is genuine so its not a copy.
Anyone got an idea of what the problem could be or is it just that I got another shitty imax?
```

---
## \#2 Posted by: Guacamoleface Posted at: 2017-03-24T14:04:28.449Z Reads: 74

```
Update: Still doesnt detect the cells when it runs the detection before you start charging it. If I click continue eventhough they advice you not to if it doesnt show the correct amount of cells and it starts charging - in the overview of cells it display voltages for each cell(all 6).

Also if I choose only to charge(no balance) - it still detects 5 out of 6 cells - No balance cable attached.
```

---
## \#3 Posted by: saul Posted at: 2017-03-24T15:03:56.187Z Reads: 69

```
Why wouldn't you split it 5 and 5 and charge in parallel!????

It could be the charger.
Or if the cells are low. Near 3v or so. The charger would see it as 5s. But It should see them with balance mode.

If this is the case you can charge for a bit till they get to about 20v. Then stop and switch to 6s. Continue. 

But careful. It would really suck to damage a 50cell pack because of a $30 charger and impatientience.
```

---
## \#4 Posted by: Guacamoleface Posted at: 2017-03-24T15:27:29.575Z Reads: 56

```
The reason for that is because I got a flexy board and 2 enclosures - it would be way to big for the vesc side of my board. 

Its just a temporary solution for now. - will be a bms charging it in the future.

it still charges it as 6s voltage - and I can still see all cells voltage (3,4v as for now) on the display if I check.

Should be fine I guess aslong as I monitor the voltage aslong. 
It makes me wonder - does it detect the cells according to the voltage power cable or the balance cable - to me it seems like its from the power cable as it still detects it in normal charge(none-balanced)
```

---
## \#5 Posted by: Namasaki Posted at: 2017-03-25T03:58:06.791Z Reads: 42

```
Does the balance connector from the 6s section have 7 pins and are you plugging it into the 7 pin socket?
Can you post some pictures of it?
```

---
## \#6 Posted by: makevoid Posted at: 2017-03-25T08:11:50.139Z Reads: 35

```
it could be that the voltage is so low that it detects a lower S battery. what voltage do you get? a possible solution would be to charge at 5s for some minutes  (set the amps of the charger very low like 0.5A and charge for 2-5 min, w/o balance lead connected ). Then if I'm correct you should be able to balance charge at 6s as normal because the voltage rose enough. I suggest to charge them slowly if they were this low. 

Anyway you can post pics or write: total voltage detected + volts per cell so we can have more insight but I'm pretty sure my tip will fix your issue
```

---
## \#7 Posted by: Guacamoleface Posted at: 2017-03-25T09:18:37.854Z Reads: 33

```
@makevoid 
Thanks for the tips - When I was looking around I saw someone doing that and it worked but that was because his battery was low.
My batteries are not low - they are all pretty much in balance right now (0.05volt difference max). 

All cells are at 3.4volts  - the total voltage displays at 20,4volt

it will let me charge at 6s if I click continue but it say on detection it could only see 5 cells. In overview of voltage if I click continue it will display 6 cells however. 
So it seems like the detection is not going from what balance cable gives it but more or less the total voltage or something like that. 
it just feels abit sketchy to me - oh well its a cheap charger. - aslong as I can monitor each cell it should be fine one would think :)



@Namasaki  
- The pins on both charger and my battery is 7 pins and the negative is correctly placed when its plugged in.
```

---
## \#8 Posted by: makevoid Posted at: 2017-03-25T09:53:58.785Z Reads: 32

```
could be a bad balance cable/connector, anyway if it detects 6s it's strange that it starts to charge at 5s, try to charge very slowly for some minutes (5) at low amps (0.5), disconnect reconnect and see if it goes back to normal is my advice

edit: you can use a multimeter/tester to check the cable/connections, every cell voltage to see if everything is correct if you haven't done it already
```

---
## \#9 Posted by: Guacamoleface Posted at: 2017-03-25T10:01:23.556Z Reads: 30

```
It doesnt start charging at 5s. It still charges at 6s voltage. But in the detection it does it shows you that it only detects a 5s battery.
And everything seem to be fine cable wise. Pins seem to get full contact aswell.
Multimeter gets connection everywhere.
So does my balance checker.

Yeah considering trying that, but might just try and charge my total ( since its 6s4p and 4s4p connected to a 10s4p) with an ebike/hoverboard charger if I can get hold of one and then see if balance charger detects(as I wanna keep both packs at same volt and if it fails, one will be at higher voltage)
```

---
## \#10 Posted by: Namasaki Posted at: 2017-03-25T13:03:13.254Z Reads: 28

```
Sounds like your balance charger has a defect.
```

---
## \#11 Posted by: Guacamoleface Posted at: 2017-03-25T17:31:33.595Z Reads: 23

```
update: it was as I suspected, it seem to detect from total voltage so when its under nominal voltage it detects as a 5s instead of 6s. 

what @makevoid said helped. gave me error when it reached nominal voltage but restart and worked fine.
now fully charged and everything turned out balanced and charged.

thanks for the help guys!
```

---
