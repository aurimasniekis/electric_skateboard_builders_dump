# Help! BMS/Charger overcharges my 10s

### Replies: 10 Views: 160

## \#1 Posted by: Guacamoleface Posted at: 2019-04-06T19:13:27.018Z Reads: 56

```
Hey, so I finished my third build today. 

I put the board on charge while finishing off the last pieces of the board. Thought it took long to charge and charger light never Went green. So I disconnect the charger and measure voltage from charge plug on the skateboard and it shows 44.5v. The bms is supposed to cut off after 42v and the charger supply 43.5 volt if measure it. 

I used this setup last summer, same charger and same batterypack&bms and only thing and never noticed any problem. 

I also dissembled the pack and measured from XT90 and was still to high. Im not sure but felt like voltage dropped abit over time. Went out and took a tour on the board and now the voltage is down to 40v again. 

Any idea? 

Thanks!
```

---
## \#2 Posted by: Andy87 Posted at: 2019-04-06T19:41:34.317Z Reads: 47

```
[quote="Guacamoleface, post:1, topic:89614"]
charger supply 43.5 volt
[/quote]

If your 10s charger output 43.5V than through it in the trash.

Idk what is wrong with your bms, but I would definitely measure the voltage of every p-pack now and look if one of the packs is out of the row.
```

---
## \#3 Posted by: Guacamoleface Posted at: 2019-04-06T19:44:02.101Z Reads: 45

```
Thanks for reply. Yeah gonna do that. But if one would be disconnected I feel like voltage would be lower and not higher since it balance.
```

---
## \#4 Posted by: Andy87 Posted at: 2019-04-06T19:49:13.951Z Reads: 43

```
Your charger shouldn’t charge over 42V in general. So even if your bms isn’t working the overall voltage of your battery shouldn’t exceed 42v as the charger would switch off by his own.
```

---
## \#5 Posted by: Sn4pz Posted at: 2019-04-06T19:51:25.087Z Reads: 41

```
Share a link to your charger so others can stay clear of it
```

---
## \#6 Posted by: pjotr47 Posted at: 2019-04-06T19:51:44.528Z Reads: 40

```
What charger are you using? You can maybe open it and set the correct voltage with the potentiometer
```

---
## \#7 Posted by: Guacamoleface Posted at: 2019-04-06T20:06:04.735Z Reads: 39

```
@Sn4pz @pjotr47 @Andy87 

Slight correction, missread the voltage, charger supply 42.3. 
I dont have a link but its a 2A 10s charger that say it supply 42.3 so thats correct.
Its an ebike charger for li-ion 10s4p package. using samsung cells.

I just measured the voltage on bms after draining battery abit - None of the paralells differ any in voltage.
```

---
## \#8 Posted by: Guacamoleface Posted at: 2019-04-06T21:38:07.607Z Reads: 31

```
This is the bms http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/BMS-D250.html
```

---
## \#9 Posted by: pjotr47 Posted at: 2019-04-06T21:49:11.194Z Reads: 30

```
The adapter must give 42v not more!
```

---
## \#10 Posted by: Guacamoleface Posted at: 2019-04-06T22:01:55.390Z Reads: 28

```
@pjotr47 but how can the bms reach higher voltage than the charging supply supplies?
```

---
