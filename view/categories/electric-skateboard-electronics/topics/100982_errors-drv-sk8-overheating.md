# Errors drv -Sk8 overheating

### Replies: 13 Views: 236

## \#1 Posted by: Djawho Posted at: 2019-08-28T11:40:10.000Z Reads: 95

```
hello guys.
 I just received and test my new engines, sk8. I put one on my focbox, waiting for unity. So last night I went around the house, barely 1 km, without slope. And suddenly, i've losted acceleration and brake ?? !! So I 've take my smartphone, and launched ackmaniac, and ...... The engine time was + 80 ° c :thinking:  So it seems obvious to me that this is the problem ...
Mon précédent moteur n'avait pas de thermistance , donc c'est nouveau pour moi . Sauriez vous si il y'a une sorte d’étalonnage ou quelque chose à faire ?? 
Je roule en 10s4P 10a , MAX moteur 60 (ils encaissent 80 normalement) max batt 60 , min moteur 55 , Min batt 16 . ET je pése 70kg tout mouillé.
 THX :sweat_smile:
```

---
## \#2 Posted by: mynamesmatt Posted at: 2019-08-28T14:11:18.599Z Reads: 87

```
can you actually touch the motor? i doubt it's getting that hot. if it's not hot to touch, the temp sensor is faulty.
```

---
## \#3 Posted by: Djawho Posted at: 2019-08-28T15:01:07.611Z Reads: 78

```
Yep the motor is hot but i can touch it
```

---
## \#4 Posted by: Djawho Posted at: 2019-08-28T17:30:13.474Z Reads: 66

```
@mynamesmatt  do you know , by what's changed "Beta Value for motor thermistor" value ?
```

---
## \#5 Posted by: mynamesmatt Posted at: 2019-08-28T21:13:42.884Z Reads: 54

```
no idea, honestly with the sk8 disregard the motor temps. i dont think the temp you have there is correct. mine constantly read -78°C so there's defs no working sensor there
```

---
## \#6 Posted by: Djawho Posted at: 2019-08-28T23:33:56.248Z Reads: 46

```
s#it drv error , i don't know how to repare ! The temps fault can to be this ?! It's not the abs , clic on picture pls.
![Capture|208x500](upload://3sRx5zHRAPY9gLbVImkRb3CkjH.png)
```

---
## \#7 Posted by: Andy87 Posted at: 2019-08-29T12:47:18.800Z Reads: 33

```
Check your connections. Abs overcurrent can come from a lose wire or bad solder join.
```

---
## \#8 Posted by: Djawho Posted at: 2019-08-29T12:48:58.876Z Reads: 33

```
the résitance "R6" is out , do you know the REF ??
the C1 08 ET C1 07 , and the C1 02 ET C1 03 , are soldered together .
After to have separated this,the value of R36 -R30 -R46 are 37.5k … But i dont know the REF of R6 and what 'is a impact of to have lost this
```

---
## \#10 Posted by: Santino Posted at: 2019-08-29T20:07:21.236Z Reads: 21

```
It seems you fried something...I would message the vendor of your ESC to ask him for the best solution...Also check every connection, and solder joints, to avoid repeating the situation after fixing the issue...If he can not help you, might be a good idea to give a try to any person that fix electronics of your neighborhood...And flash back the firmware after fix....If it is too expensive, you might need to buy another ECS...Just my thoughts...
```

---
## \#11 Posted by: Andy87 Posted at: 2019-08-29T20:12:37.078Z Reads: 20

```
Not sure about the values, but maybe @seaborder can. He also does vesc repair in case it is needed.
```

---
## \#12 Posted by: Djawho Posted at: 2019-08-29T20:50:50.416Z Reads: 19

```
I would especially need the component reference "R6" on the focbox . I just resoldered the USB port of the focbox (and it works now :blush: ) . And I noticed that the component named R6 has disappeared :scream: But i don't know what'is this part ?
```

---
## \#13 Posted by: Jumpman Posted at: 2019-08-29T21:18:27.131Z Reads: 18

```
I think it R6 is 0 ohm resistor, but it is not needed.  So, it is normal for it to be missing.
```

---
## \#14 Posted by: Djawho Posted at: 2019-08-29T23:06:54.278Z Reads: 18

```
Thanks @Jumpman i have just find this information :upside_down_face:
```

---
