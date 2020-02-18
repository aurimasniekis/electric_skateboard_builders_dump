# Building first battery pack

### Replies: 5 Views: 199

## \#1 Posted by: SmirnofficePapi Posted at: 2019-03-23T11:11:56.179Z Reads: 95

```
Hi everyone 

I'm putting together my first batterypack after the one i got from DIYeboards failed. I'm keeping the rest of the stuff from the kit i got from them. 

I will be building a 10s3p battery as that is what the enclosure allows size wise. 
and will be using samsung 30q cells. as they produce 15A and not the more popular 20A
this is because the ESC will allow "Current: Up to 120A for a few seconds or 50A continous"
as they write. 

I have the battery configuration in place, and i feel confidant so far, the main problem right now is picking out the BMS. I dont know what requirements i should have for it. since it's a 3p, that makes the continuous amps 45, withing the 50A continous that the ESC allows. Will i need to get a BMS that has those specification?
I've been looking at this bms currently:
https://m.banggood.com/37V-42V-10S-45A-Li-ion-Battery-Protection-Board-BMS-PCB-System-p-1177351.html?rmmds=search#popupStatedetail
But there are two problems with it, 
1: the charging current: 45A - that sounds crazy. i have a charger that charges with 2A, so 45 sounds bonkers 
2: that there is no P- on the BMS, it only seems to have a B- and C- 

I hope you guys can help me out. 
Best Wishes 
Ryan
```

---
## \#2 Posted by: rojitor Posted at: 2019-03-23T16:59:47.982Z Reads: 80

```
Has a shared port. Charge and discharge are the same. You can do continuous 60 amps with 30q 3p
I don't think It can deal with 45amps charge. Must be a mistake. Nevertheless you shouln't charge above 4.5a (0.5c)
```

---
## \#3 Posted by: SmirnofficePapi Posted at: 2019-03-24T12:22:09.448Z Reads: 62

```
Are you sure that they can draw 60A(20x3) continuous, cause this website 
https://eu.nkon.nl/samsung-inr-18650-30q-3000mah.html
says 45A (15x3) - or am in looking at the wrong place? 

Would that BMS work for these batteries, and limit the battery to 45A continuous? 
and would the board then need to be turned off to charge? 

thanks for the help by the way! :)
```

---
## \#4 Posted by: rojitor Posted at: 2019-03-24T12:38:59.015Z Reads: 56

```
Yes i am sure. I understand your confusion. They are indeed rated for 15a yet they have been reported by several communities to work flawlessly at 20a continuous. I have done some 3p packs myself and i have real life experience. They do not sweat pushing 2 6374 motors so it's true. You can count on 20a continuous from 30q.
That bms will work but maybe you want more amps.
Yes. You better turn It off to charge.
```

---
## \#5 Posted by: SmirnofficePapi Posted at: 2019-03-24T14:29:24.797Z Reads: 39

```
Cool, that's awesome, thanks for the help. I dont think my esc can handle more amps than the 45 the bms will limit it at, so that's perfect. 

thanks again for the advice, huge help. 
best wishes, Ryan.
```

---
