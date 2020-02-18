# Problem with Alienpowersystems Esc

### Replies: 15 Views: 195

## \#1 Posted by: Louismxopen Posted at: 2018-08-13T07:00:51.795Z Reads: 78

```
Hey guys I got a big problem at my latest build, i got 2x2200W 270kv Aps motors with the Aps esc that was a Dual Motor set. My Power supply is an Aps 6s 16000mah 35C Lipo battery. After i wired everythink up it worked very good. But the esc dosent cut off at the minimum voltage so the battery was fully drowned and is now dead. But also i got a maximum Range of 4-5km did someone got an Idea how to improve the range? I could go up to 8s But i dont think that this would increase the Range so hard.
```

---
## \#2 Posted by: brenternet Posted at: 2018-08-13T07:07:29.757Z Reads: 77

```
Did you check the voltage of the battery at the start of just percentage?
```

---
## \#3 Posted by: mynamesmatt Posted at: 2018-08-13T07:08:59.217Z Reads: 76

```
Increasing the range would mean higher Mah my sir. Its the capacity so it determines how far you can ride :)
```

---
## \#4 Posted by: Louismxopen Posted at: 2018-08-13T07:12:57.561Z Reads: 73

```
Yes it was fully Charged at 22.2 Volts and all cells got the right voltage so the battery was okay
```

---
## \#5 Posted by: Louismxopen Posted at: 2018-08-13T07:15:37.624Z Reads: 62

```
Yes but I think 16000mAh were pretty much and i thougt it will give me a Range up to 10km of so
```

---
## \#6 Posted by: mynamesmatt Posted at: 2018-08-13T07:19:07.963Z Reads: 61

```
what battery pack were they?
```

---
## \#7 Posted by: Louismxopen Posted at: 2018-08-13T07:29:19.222Z Reads: 54

```
Alienpowersystems 16Ah 35C
```

---
## \#8 Posted by: mynamesmatt Posted at: 2018-08-13T07:36:13.028Z Reads: 53

```
How were you charging the battery?
```

---
## \#9 Posted by: Louismxopen Posted at: 2018-08-13T07:44:31.674Z Reads: 53

```
With an Turnigy reaktor 300w 23 A Charger i charged it with 1A and blancing mode
```

---
## \#10 Posted by: mynamesmatt Posted at: 2018-08-13T07:47:33.100Z Reads: 49

```
Strange, you did have all 3 plugs in right?
```

---
## \#11 Posted by: FredrikHems Posted at: 2018-08-13T07:53:37.408Z Reads: 46

```
[quote="Louismxopen, post:4, topic:64690"]
22.2
[/quote]
There you have your problem. Its not fully charged at 22,2 volts, but at 25,2 volts. 22,2v is the nominal charge.
```

---
## \#12 Posted by: Louismxopen Posted at: 2018-08-13T08:18:14.110Z Reads: 38

```
Ok than I will try this First
```

---
## \#13 Posted by: FredrikHems Posted at: 2018-08-13T09:10:13.701Z Reads: 33

```
Thats 100% your problem, as at 22.2v you only have about ~25% battery left. However, you said you ran your battery until it was dead, which means that your battery is probably ruined.
```

---
## \#14 Posted by: Louismxopen Posted at: 2018-08-13T11:47:13.110Z Reads: 31

```
Yes it is dead. So you mean 22.2 volts are just 25% of the hole capacity?
```

---
## \#15 Posted by: Louismxopen Posted at: 2018-08-13T13:42:01.020Z Reads: 25

```
Got one last question would it be possible to wire 2 4s 8000mah 30c in Series and 2 in parallel that I have an 8s 16000mah battery? How i have to connect these balancer wires? Also in parallel and Series as the positive and negative wires.
```

---
