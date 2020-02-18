# Battery won&rsquo;t charge. BMS outputs lower voltage than battery total

### Replies: 11 Views: 1331

## \#1 Posted by: fuentesm15 Posted at: 2018-08-23T02:13:42.284Z Reads: 93

```
I need some help with my BMS. I have a 10s setup and this afternoon when I tried to charge my skateboard, the green light on my charger indicating it is not plugged in or fully charge would not change to red indicating it is charging. I check the voltage at the charger and the charge port of my skateboard. the charger was good as it read 42v however the charge port voltage is strange as it only reads about 33v while my battery total is measuring as approximately 37v. I have a feeling it is my BMS but it was charging perfectly find last night. please help!

I can post pictures and provide more info if necessary. In addition, I disconnected my balance leads and measured the voltages for each battery. Each measures as expected all totaling approximately 37v. the reason for the battery total being this is because my battery is approximately at 50% charge right now.
```

---
## \#2 Posted by: fuentesm15 Posted at: 2018-08-23T02:23:05.349Z Reads: 90

```
update: while troubleshooting, I accidentally plugged in the charger without the balance cable connected to the bms. I quickly realized my mistake and quickly unplugged however before doing so, I noticed the charger indicated the battery was charging. I then connected the balance cable again and also connected the charger only to have the green light on my charger still on indicating it was not charging.

I use this skateboard to commute daily how bad would it be to leave the balance cables disconnected and continue to charge until Friday when I can replace the bms? yes the cells will not be balance charged, but will they return to normal once I start balance charging them again with a new bms?
```

---
## \#3 Posted by: pjotr47 Posted at: 2018-08-23T02:30:15.441Z Reads: 87

```
Until Friday wouldn’t be a problem if you’re cells are in a good condition and have all the same voltage
```

---
## \#4 Posted by: fuentesm15 Posted at: 2018-08-23T02:33:45.072Z Reads: 79

```
assuming they go slightly out of wack, will they return to balance over time with balance charging via bms?
```

---
## \#5 Posted by: Jake2k17 Posted at: 2018-08-23T03:14:36.818Z Reads: 77

```
The reason that they are not charging may be because the balance wires are hot connected in the right order. Are you using li ion it Lipo?
```

---
## \#6 Posted by: fuentesm15 Posted at: 2018-08-23T03:42:53.937Z Reads: 75

```
lipos equaling 10s. This is an existing build, that was working fine for a  month. also to confirm this. I double checked the order of the balance wires and they are all in the proper order per the bms schematics.
```

---
## \#7 Posted by: Brdchris Posted at: 2018-08-23T03:46:24.874Z Reads: 78

```
Mine did the same thing. My bms fried and I ended up loosing a whole parallel group. Might want to check your battery out before doing anything else. My 12th group had zero volts and the bms would only charge to like 37.8 I think
```

---
## \#8 Posted by: fuentesm15 Posted at: 2018-08-23T03:49:36.403Z Reads: 71

```
specifically, I am using 2 4s 5000mah lipos and 1 2s 5000mah lipo in series. I find it strange that this is suddenly a problem. Initially I thought I maybe hit a bump to hard earlier today that may have caused something to disconnect or a solder joint to fail, but I've double checked all of the soldering points that I made and all is connected properly. I also removed the heat spreader from the bms to check for any black spots on the pcb that could indicate I fried something however the thing looks as new as when I got it. I suspect my bms is a lemon and I've ordered another to confirm this.
```

---
## \#9 Posted by: fuentesm15 Posted at: 2018-08-23T04:03:50.523Z Reads: 69

```
Brdchris, i checked each cell with the volt meter thankfully all are good.
```

---
## \#10 Posted by: fuentesm15 Posted at: 2018-08-25T04:01:15.570Z Reads: 55

```
Update: replaced bms with new model different from the first. Tested with a volt meter before install and got the full total of my batter outputted from the bms. will post pictures in time and will update as needed.
```

---
## \#11 Posted by: Sander Posted at: 2018-09-11T16:52:04.715Z Reads: 47

```
Hey, the same thing happened to me. So now my board won't charge. I have charged it 3 times before with no problem but now it wont charge. When I check the voltage at the charger port it says 33.4V, when I check voltage with the battery ground (B-) it shows 43.6V. When I disconnect the balance leads the voltage with the charger port shows (P-) 42.3V. Any idea how to fix it without buying a new one? When I check every cell with the balance leads via the charger ground(P-) it starts with -6.8V and the 12th wire is 33.4V and when you add them together the voltage is 40.2V. It shows only correct value when I use the battery ground (B-) not P-.

http://www.batterysupports.com/44v-48v-504v-12s-45a-12x-36v-lithium-ion-lipolymer-battery-bms-p-269.html

![image|690x384](upload://ebIe0em6bhTGfcKJVJBTlSYmHpP.jpg)
```

---
