# Bms wiring with no (-c) charge port

### Replies: 11 Views: 1479

## \#1 Posted by: Shahar9320 Posted at: 2017-06-27T23:22:49.218Z Reads: 105

```
hey guys! im having trouble with the bms. 
bms: http://www.batterysupports.com/44v-48v-504v-12s-80a-12x-36v-lithium-ion-lipolymer-battery-bms-p-392.html
why is there no charge port? (-c). also, there are 2 wire coming out from both p- and b- and i dont know where they should go. please see my diagram and check for problems
<img src="/uploads/db1493/original/3X/b/e/be3177ef875081ea2a9902929b951c5ba5fc50b2.JPG" width="375" height="500">
thank you very much
```

---
## \#2 Posted by: Jinra Posted at: 2017-06-27T23:24:38.716Z Reads: 99

```
Charge is P-

It's explained in the schematic of the page

<img src="/uploads/db1493/original/3X/9/d/9daece86a352ff578df30238dc10de949f2ca820.png" width="597" height="500">http://i1098.photobucket.com/albums/g378/lilianleung/LOGO%20Connecting%20Chart.jpg~original

Your schematic looks good, though I think you're suppose to join one of the balance leads from each pack since its in series.
```

---
## \#3 Posted by: Shahar9320 Posted at: 2017-06-27T23:26:27.428Z Reads: 89

```
but in my diagram there is one wire that comes out from b- and is connected to nothing
```

---
## \#4 Posted by: Jinra Posted at: 2017-06-27T23:27:05.097Z Reads: 89

```
Just unsolder it, or join it to B- for redundancy and bandwidth
```

---
## \#5 Posted by: Shahar9320 Posted at: 2017-06-27T23:27:09.188Z Reads: 86

```
what is the balance leads?
```

---
## \#6 Posted by: Jinra Posted at: 2017-06-27T23:29:26.094Z Reads: 85

```
Well you should have 7 balance leads per lipo pack, not 6. 6 should go to each pack's cell positive and one should go to cell negative. You'll have to join the balance leads that represent the same S cell.
```

---
## \#7 Posted by: Shahar9320 Posted at: 2017-06-27T23:30:40.001Z Reads: 84

```
does this have 7 wires? https://hobbyking.com/en_us/graphene-6000mah-4s-65c-w-xt90.html
```

---
## \#8 Posted by: Jinra Posted at: 2017-06-27T23:31:32.494Z Reads: 81

```
That has 5 since it's 4s, you drew 6s on your schematic
```

---
## \#9 Posted by: Shahar9320 Posted at: 2017-06-27T23:34:09.181Z Reads: 80

```
thats a mistake.. this is the battery https://hobbyking.com/en_us/graphene-6000mah-6s-65c-w-xt90.html
```

---
## \#10 Posted by: Jinra Posted at: 2017-06-27T23:35:39.325Z Reads: 76

```
Yea that should have 7
```

---
## \#11 Posted by: Shahar9320 Posted at: 2017-06-27T23:36:17.959Z Reads: 80

```
so where do i connect the other 2 wires? the bms only have 12 of these
```

---
