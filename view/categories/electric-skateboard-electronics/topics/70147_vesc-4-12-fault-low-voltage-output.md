# Vesc 4.12 FAULT low voltage output

### Replies: 8 Views: 230

## \#1 Posted by: RonnyFox Posted at: 2018-10-04T15:05:39.252Z Reads: 48

```
Hi guys, 
So still can’t work out what’s going on with one of my VESC 4s... everything seems to be as usual except the voltage output. Currently with 42V input, the output is only 26.4V. Does anyone have any ideas about WTF is going on here or how it can be fixed? I would really appreciate any assistance thanks y’all!
```

---
## \#2 Posted by: Benjamin899 Posted at: 2018-10-04T18:17:03.966Z Reads: 45

```
post screenshots of all your settings
```

---
## \#3 Posted by: RonnyFox Posted at: 2018-10-04T20:08:55.457Z Reads: 35

```
![16%20am|690x388](upload://AlAIF73HrrrWBWQ0M4ySsVaaRhA.png) ![00%20am|690x388](upload://AoAskQ8vVeF3aH9bOadQJ9Ng0Lt.png) ![19%20am|690x388](upload://mz3iuuhcnatZC3puHiAwYdTYrKi.png) ![55%20am|690x388](upload://5O5Q6cq2QeuQl62OmfNpBLpkB9t.png) ![54%20am|690x388](upload://tt6UkOxKZ7CojEfyjC3jqmPnQG6.png) ![27%20am|690x388](upload://lyvF0Y4GUlziXVwBMeC37yDBu7P.png) ![32%20am|690x388](upload://mygq1yiDNtM48tlxeo9u2f4qAvI.png) ![23%20am|690x388](upload://ykeFIRFJg34mEaKJcEFitJpkhd0.jpeg) ![08%20am|690x388](upload://cfibPWNtmhTaag6quKW0ZZ0yI9P.png) ![05%20am|690x388](upload://p0gapJc6QUeQaLnpFeUlRPNTxut.png) ![12%20am|690x388](upload://6Ib0TdRzFRb5KuJjTkaCYupIdrA.png) ![22%20am|690x388](upload://lwUIN9n6QIssUyR8ytL2j406ZPR.png) ![25%20am|690x388](upload://uZd03LBE1KNrtGnrchQcxyx1S8G.png) ![28%20am|690x388](upload://e7itWrAqXaCQPkgHjE7G62EFcJU.png) ![57%20am|690x388](upload://g3ikz9SS9HSZRwh24zP8VizkjUe.png) ![01%20am|690x388](upload://bAKTZnn9UVnqKrEOv40DQkQivaP.png)
```

---
## \#4 Posted by: Benjamin899 Posted at: 2018-10-04T20:24:01.450Z Reads: 27

```
there is a chance you fried that vesc.
First i dont know what type of battery you have, but -40 Amps seems a tad much, but depends on battery.
Second, 4.12 are not to keen on the 100k ERPM Limit, they are safer at 60k. So maybe something is fried and thats why you have that faulty reading ect.
```

---
## \#5 Posted by: RonnyFox Posted at: 2018-10-05T03:43:47.304Z Reads: 21

```
Ok thanks @Benjamin899 
Battery is a 10s6p vtc6 cell pack. What would you recommend for that setting?
```

---
## \#6 Posted by: Benjamin899 Posted at: 2018-10-05T11:40:41.932Z Reads: 13

```
well with that type of battery thats ok. depending if its a single or dual drive. if its dual battery amps have to be halved otherwise both vesc would dump 80 amps into the battery.
```

---
## \#7 Posted by: mynamesmatt Posted at: 2018-10-06T16:01:24.141Z Reads: 9

```
-12a will be just fine.

2 things
firstly, the vesc can only take 50a battery current MAXIMUM. so setting it at or over this is pushing your luck. try not to exceed 40a battery amps. motor amps however you can crank up to whatever your motor can take. eg i have 65a/-55a
secondly, does anything come up when you type "faults" into the terminal?
```

---
## \#8 Posted by: RonnyFox Posted at: 2018-10-13T21:24:01.455Z Reads: 7

```
Hi @mynamesmatt
Thanks for your advice there man, I didn’t even think about that!! I’ll change batt Amps to 40 on next vesc... and I’ve never used the vesc terminal...! I will have a look when I’m home and get back to you bro!
```

---
