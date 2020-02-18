# BMS not charging battery? (Solved)

### Replies: 7 Views: 1310

## \#1 Posted by: Brontech Posted at: 2018-05-25T23:21:51.274Z Reads: 100

```
I've just setup my 12s bms on my eboard, and so far, it was working. I could turn the whole board on with the bms with an E-switch and have the board move on its own, but when I plugged it in to charge, it was not charging...
My Charger showed a green light, but the pack was not fully charged.
I've followed this diagram, just with two lipos instead of lion batteries.
![41 AM|690x320](upload://lmopvMlmknRVkv7fH9v1oFycwNM.png)
Any help is greatly appreciated!
Also, I can provide photos of my setup if that helps.
EDIT: Accidentally wired negative wire that goes to the charge port to ground :roll_eyes:
```

---
## \#2 Posted by: Brontech Posted at: 2018-05-26T02:21:00.685Z Reads: 82

```
I connected the charge port negative to C- on the BMS and tapped into the main positive wire for the positive wire of the charge port.
I've measured all the balance leads and each cell is around 3.73-3.75.
The board runs perfectly, just wont charge.
This issue has really stumped me.. 
![|666x500](upload://ehlRh5YPcrYXQZ0RO6Py7pmgEN8.JPG)
![IMG_2410|375x500](upload://jTOxS77yvaKj514C7aGVciZ7H3e.JPG)
Here is how I wired the charge port. Black to C- and red to main positive wire.
![IMG_2411|375x500](upload://uCwIpowLOPi230pqWoSyhXFXj9X.JPG)
Here are how the balance ports are wired. I am quite sure however, that the batteries or balance wires are not to blame because I can read each voltage of the cell and no cells have a large voltage difference. (.02V at most)

Any insight about my issue would be greatly appreciated! :slight_smile:
```

---
## \#3 Posted by: Brontech Posted at: 2018-05-26T02:39:26.950Z Reads: 73

```
I've just measured the charger plug and I'm reading the proper voltage (50.4V) and when measuring the charger port that's connected to the bms, I get about 45V, which is the total voltage of my current pack.
```

---
## \#4 Posted by: kuphjr Posted at: 2018-10-25T14:22:58.782Z Reads: 50

```
You said you had this issue solved. May I ask what you did to fix it?
```

---
## \#5 Posted by: santi_illa Posted at: 2018-10-25T21:46:51.906Z Reads: 48

```
I know this not reply to your post but, I need to know if someone can tell me if I have for example 2 3s lipo batteries of 5500 each and 11.1v so 22.2v in total. Will a 24v esc work with it and a lower Amp and voltage bms can charge it like a 24v 18 amps. 

bms:https://tiendamia.com/e-product?ebay=v1|153176838256|453032095835&pName=Balanced-BMS-8S-24V-18A-25A-35A-45A-60A-lipo-battery
esc:https://tiendamia.com/producto?amz=B07GRW61K3&pName=SponsoredHobbysky-24V36V-Upgrade-Dual-Motor-Drive-ESC-Electric-Speed-Controller-with-Closed
```

---
## \#6 Posted by: santi_illa Posted at: 2018-10-25T21:47:27.769Z Reads: 46

```
batteries:https://articulo.mercadolibre.com.uy/MLU-457394021-floureon-2packs-3s-111v-5500mah-35-c-lipo-bateria-con-co-_JM
```

---
## \#7 Posted by: Brontech Posted at: 2018-10-26T01:25:30.690Z Reads: 45

```
[quote="Brontech, post:1, topic:56795"]
EDIT: Accidentally wired negative wire that goes to the charge port to ground :roll_eyes:
[/quote]

There are 3 terminals on my charge port. Negative, Ground, and positive. I accidentally wired my negative wire to ground.
```

---
