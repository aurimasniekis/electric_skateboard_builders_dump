# Unknown 120A Battery current limit in VESC Tool

### Replies: 9 Views: 120

## \#1 Posted by: AK1 Posted at: 2020-01-26T00:55:21.479Z Reads: 41

```
I have a 10S10P 30Q battery. Theoretically I should be able to pull 150A, and some sources even claim 200A is possible(although it is debatable). I am using the FSESC6.6 and everything is wired with 8 gauge high strand silicone wire using a QS8-S connector. The reason all of this is important is because the VESC Tool software only lets me use 120A of this potential.

When I set my "Battery Current Max" to any value, I get a message that "The following parameters were truncated because they were set outside of their allowed limits.". Why is this happening and am I able to increase my limit? 

*As a side note I did not see anyone else having this problem, and I also noticed that many users were able to set their battery current max higher than 120A. My motors are each set to 80A -50A limits which are within spec(to my knowledge). My FSESC firmware is upgraded too.

![IMG_9475|666x500](upload://lXHLgjP8zalzZ3FgGKpwgfoDX.jpeg)
```

---
## \#2 Posted by: AlanZhou Posted at: 2020-01-26T03:47:55.261Z Reads: 35

```
What vescs are you using
```

---
## \#3 Posted by: AK1 Posted at: 2020-01-26T04:12:36.736Z Reads: 33

```
VESC 6, here is the exact model

https://flipsky.net/collections/electronic-products/products/dual-fsesc6-6-based-upon-vesc6-with-aluminum-heatsink-1
```

---
## \#4 Posted by: AlanZhou Posted at: 2020-01-26T04:16:19.051Z Reads: 33

```
I think there should be a unlimited firmware version from flipsky
```

---
## \#5 Posted by: AlanZhou Posted at: 2020-01-26T04:16:56.919Z Reads: 33

```
Also 120a is per side I believe
```

---
## \#6 Posted by: Andy87 Posted at: 2020-01-26T04:57:23.345Z Reads: 31

```
Every vesc tool has a hw no limits fw version included.
Just need to flash that one to your vescs and you can set your limits how you want
```

---
## \#7 Posted by: Andy87 Posted at: 2020-01-26T05:03:32.249Z Reads: 31

```
And that is right too.
It’s not a unity where the battery max value is one value for both together.
If the batt max is set to 120A than it means 120A per vesc or 240A total.

Besides this it doesn’t make sense to set your bat max limit higher than you motor max because of 🤷‍♂️ Duty Cycle
```

---
## \#8 Posted by: AK1 Posted at: 2020-01-26T05:29:48.726Z Reads: 30

```
It appears that the “Battery Current Max” is for each VESC as @AlanZhou said. This means that my real “Battery Current Max” is currently 240A, so I will be changing that down to 200A(100A per VESC). 

I have seen the no hardware limit files before, but I felt something else was wrong as the manufacturer stated it was a 200A VESC, not 120A. Good to know. Thank you!
```

---
## \#9 Posted by: Santino Posted at: 2020-01-27T07:07:19.540Z Reads: 18

```
I think you have a constant discharge of 150, so 75 for each motor tops...and 75A for each vesc tops too... You could have a peak discharge of 200A, meaning 100A peak for each vesc setting, but it is just a peak, not constant... You could check over here your numbers to avoid damaging your system. 

https://calc.3dservisas.eu/?TZDBCsIwEET_JWeRxKStel2lJyUg2LvNIYKxhR7Ffzczjdbbm2F2NpuXuklUe_W4D0-1yuKchV3XmSe5ZDaa6BcUJLSexQHKVDMjtCkhlJqMI0os4G9u9HAdiUMgVtmKCLMm_or6KKWpj8dMW028YtyBk5SmxHc39PwAdsRlfxLaCIdu4mkNuD19rwlthzj-IWDbTqv3Bw==
```

---
