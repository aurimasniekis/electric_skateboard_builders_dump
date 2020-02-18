# 12s (2 x 6s Series) Charging question

### Replies: 9 Views: 1403

## \#1 Posted by: Sarky1 Posted at: 2017-01-06T17:24:42.722Z Reads: 127

```
Hey guys,

I think this will work but before I bang test it can someone confirm my sanity.

I have 2 6s 10000mah in Series and rather than adding a connector to disconnect each time I'm wondering if charging while hooked up like this is OK. I will also be connecting the balance connectors. I have 2 external chargers I will be using.

<img src="/uploads/db1493/original/3X/0/3/035ad581ba9bf3f4c3a007bbe1cef0c598d104b9.jpg" width="690" height="414">
```

---
## \#2 Posted by: abenny Posted at: 2017-01-06T17:39:04.556Z Reads: 117

```
you can buy balance leads for parallel charging for a couple of bucks, and if you make a parallel adapter, you can charge both batteries at once as a single 6s battery on your charger... im not sure if having both connected in series while trying to only charge 6 cells is a good idea, but im not really a wiz with batteries. my method will take longer to charge, but i have done it successfully with my 4s cells
```

---
## \#3 Posted by: TheImmortalJew Posted at: 2017-01-06T18:11:06.720Z Reads: 107

```
I don't think it will work the way you have it drawn. You have a permanent series connection between your XT60 charge plugs. In order for it to work you would have to disconnect that wire to charge at 6s and reconnect it to discharge in 12s.
```

---
## \#4 Posted by: Hummie Posted at: 2017-01-06T18:21:52.096Z Reads: 104

```
have to break the series chain and then do it parallel.  but maybe charge all in series and get a 12s bulk charger and you could put (2) 10$  6s balance chargers on the two battery balance leads
```

---
## \#5 Posted by: Sarky1 Posted at: 2017-01-07T23:01:28.588Z Reads: 83

```
Thanks Guys,

I already have dual 6s chargers thats why I'm trying to balance charge each at 6s. I'm not trying to parallel. 

Looks like the consensus is I have to break that series to charge. I didn't think I needed to as if I pick up voltage from these points I'm happily sitting at 6s voltages on both xt60's
```

---
## \#6 Posted by: Maxid Posted at: 2017-01-07T23:54:51.504Z Reads: 79

```
I think your thinking is right and it should work since you are not doing the common ground mistake.
However someone with a little more experience might want to chime in - @lowGuido maybe? ;)
I am not sure for example how your dual charger is internally wired and if the grounds are connected - that might make it unsafe.
```

---
## \#7 Posted by: lowGuido Posted at: 2017-01-08T01:34:59.043Z Reads: 74

```
You definitely can not parallel charge with the packs still connected in series.  But I dont see any reason you wouldnt be able to leave them connected with 2 seperate chargers.

I would be inclined to seperate them just in case.
```

---
## \#8 Posted by: PXSS Posted at: 2017-01-08T02:52:12.878Z Reads: 71

```
If you have a dual port charger, like an iCharger duo, you need to separate them. There cannot be any connection between the two channels or you'll blow the charger. If they are two separate chargers then you should be good
```

---
## \#9 Posted by: Sarky1 Posted at: 2017-01-08T16:03:32.228Z Reads: 62

```
Ah interesting. Well I have 2 separate chargers but they are using the same power supply.  Is my issue here a ground loop?
```

---
