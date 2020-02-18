# What batteries are these? Lithium ions shaped like Lipos

### Replies: 5 Views: 297

## \#1 Posted by: mutantbass Posted at: 2018-06-12T11:52:43.846Z Reads: 124

```
Hey everyone. 

So I have a habit of cleaning out my laptop for dust to keep it running cool. Today, as I was cleaning I noticed the battery is lithium ION and not LIPO as i assumed it would be because of how thin it is.

 ![Photo%2012-06-2018%2C%2013%2033%2041|666x500](upload://dveD8bhvGZ7iZNyTcGsGATtTreA.jpg)![Photo%2012-06-2018%2C%2013%2033%2045|666x500](upload://kDVs9Xg0vPlfbUHBYIyQ5LTPS5D.jpg)![Photo%2012-06-2018%2C%2013%2033%2049|666x500](upload://pXS7iGN2xRyPbOLzpW3b8laKgR6.jpg)

The battery is no thicker than 7-8mm. What lithium ion cells are these? I see the discharge of the battery is only 6c but I am more interested in the form factor. I tried googling a few of the numbers on the battery but came up short. The laptop is xps 15 9550. 

Whats interesting is that the cells inside as you can see are square form factor.It also has a little bit of flex in it. 

These form factor could potentially make for smaller and denser batteries for our esk8s.

any ideas?
```

---
## \#2 Posted by: bevilacqua Posted at: 2018-06-12T12:00:59.768Z Reads: 116

```
Normal 18650 are rolled: Imagin a long paper stack of 3 sheets (Anode - Separator - Cathode) that you roll into a cigar like shape. 

Primatic Cells can be made out of stacked layers: 3 + 3 (on top) + 3 and so on (all connected in parallel)

Other prismatic cells like the Samsung ones on a BMW i3 are rolled like cylindrical cells but with a prismatic form factor ( Wide-Flat-Cigar).

Usually they are purpose made cells, so they are hard to buy and usually not very practical.

Hope this is helpful :)
```

---
## \#3 Posted by: willumpie82 Posted at: 2018-06-12T12:15:49.120Z Reads: 103

```
these batteries could be suitable but you will need a stiff enclosure, when the layers in the cell damage (because of to much flex) the battery will go b00m
interesting enough, 11,4v (=3s) but I see 4 cells, so it is probably an asymmetrical pack, 

Other than that, these cells are not made for high current demand. In case of a 10s3P of these cells (~730mah/cell) than still your peak amps are just 6c * 730mah * 3p = ~13A

I tried a 10s3p of old laptop batteries (18650s) ~2000mah, but they have only 2c, hence 12A did sag so much that my VESC brown-outed on just the slightest hill

If you want a custom form factor battery, Take apart a few big RC lipo's (60C) and rearrange the cells or use high discharge 18650's
```

---
## \#4 Posted by: mutantbass Posted at: 2018-06-12T12:31:36.960Z Reads: 83

```
thanks for the replies guys. I googled pristamic/pouch batteries but they all seem to be lifepo4 not li-ions.

DO you think this battery is mislabelled as lithium ion? Its Dell so I doubt a big company like this is mislabelling their batteries.

Sounds like it is a custom job afterall.

@willumpie82 its actually 3s2p. Its total 6 cells. I just didn't take a picture of the whole battery.
```

---
## \#5 Posted by: bevilacqua Posted at: 2018-06-12T15:46:54.366Z Reads: 49

```
I don't think they mislabeled it ;)
```

---
