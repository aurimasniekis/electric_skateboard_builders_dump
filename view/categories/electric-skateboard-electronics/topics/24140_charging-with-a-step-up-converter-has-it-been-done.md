# Charging with a step up converter, has it been done?

### Replies: 9 Views: 1539

## \#1 Posted by: Achmed20 Posted at: 2017-05-29T18:57:43.048Z Reads: 96

```
sooooo,
when i build my DIY board, i was going for a 9S setup (3x 3s 5000mah lipos). 
mostly because of size and easy replacement since those lipos are rather cheap. little did i know that having a 9s solution comes with its own set of problems. finding a 9S BMS for example (which i found). finding a 38V charger however with at least 2A  is a complete different story. i can only find 36V chargers which will charge my battery to something about 85%. 

so my idea right now is, using a 24V 3A charger and use a step up converter to boost it to 38V. 
Using a step down converter with a ~42V charger would probably be the better idea, but im kinda in the experiment mood and want to try this. stuff should arrive tomorrow.

so would it work? did anyone ever try that?
```

---
## \#2 Posted by: lowGuido Posted at: 2017-05-29T19:08:32.880Z Reads: 96

```
its been discussed.. its not something thats worth while.
I cant find the thread. you would be better off stepping down. look into the specs of your BMS and see if it regulates the charge input. you might get lucky.

or on the flipside get another cell and go 10S.
```

---
## \#3 Posted by: TSG_AU Posted at: 2017-05-29T19:16:52.209Z Reads: 92

```
Sure it's been done.
Here's a prototype in development:
http://raphaelchang.com/#projects/bms/
https://www.electric-skateboard.builders/t/raphael-chang-bms-and-esc/8952
```

---
## \#4 Posted by: Achmed20 Posted at: 2017-05-29T19:21:12.967Z Reads: 80

```
i know that project. its kinda why i came up with that idea he first place :)
I soooooo wish he would be finished by now because that BMS is just awesome.
```

---
## \#5 Posted by: Maxid Posted at: 2017-05-29T19:24:03.247Z Reads: 78

```
We have discussed this several times. I am using such a charging solution. I use a DROK and notebook PSU.
```

---
## \#6 Posted by: icon Posted at: 2017-05-29T19:27:00.133Z Reads: 75

```
Guessing it would work
http://www.ebay.com/itm/Intelligent-Smart-37-8V-2A-Charger-for-9S-32-4V-33-3V-Li-ion-Li-Po-Battery-EU-/221896623314?hash=item33aa11c4d2:g:KtUAAOSwHjNWBgfK
```

---
## \#7 Posted by: Namasaki Posted at: 2017-05-29T19:28:02.385Z Reads: 75

```
My charging solution is a Lab power supply. You can adjust the voltage and charge any size pack with a bms.
It also works better than any brick charger you can buy. It's not the cheapest solution though.

https://www.amazon.com/gp/product/B00AXL7UJA/ref=s9u_simh_gw_i1?ie=UTF8&fpl=fresh&pd_rd_i=B00AXL7UJA&pd_rd_r=H069Q0MAMFBJ7HAHVWM1&pd_rd_w=PSTIr&pd_rd_wg=ZpBkU&pf_rd_m=ATVPDKIKX0DER&pf_rd_s=&pf_rd_r=KK92HHN0JW2VJ7QD6JTD&pf_rd_t=36701&pf_rd_p=781f4767-b4d4-466b-8c26-2639359664eb&pf_rd_i=desktop
```

---
## \#8 Posted by: lowGuido Posted at: 2017-05-29T19:32:45.347Z Reads: 68

```
It will definitely work.
you just lose some efficiency stepping up. you are better off stepping down.
```

---
## \#9 Posted by: Achmed20 Posted at: 2017-05-30T18:29:55.808Z Reads: 53

```
well, the powerbrick arrived, so did the boost converters, 

but it it not working for me. but that seems to be a problem with the converter itself. it pretty much shuts down as soon its connected to the BMS / battery. i guess its because its getting voltage from the "output" side which it doesnt seem to like.
guess its missing a diode. meh...

back to plan b. i ordered the powerbrick @icon linked (thx by the way :)) and untill it arrives, i just go with a under charged battery.
```

---
