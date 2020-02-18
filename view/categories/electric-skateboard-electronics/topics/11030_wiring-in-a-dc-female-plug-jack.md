# Wiring in a DC Female Plug/Jack

### Replies: 6 Views: 1413

## \#1 Posted by: johnny_261 Posted at: 2016-10-12T19:19:30.244Z Reads: 124

```
Hello,

I am just finish the wiring on my build and had a noob question about wiring in the charging jack.  I have the jack as in the link below.

http://www.ebay.com/itm/391532615616?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT

As I understand it, the outside barrel is negative and the pin in the middle is positive.  So I should just use a multimeter to figure out which lead is which, and then connect the lead for the pin in the middle to the positive wire on my battery pack.  Then lead for the outside barrel should be connected to the P-/CH- on the BMS?

I've never done this before, so wanted to get confirmation so I don't start a fire!
```

---
## \#2 Posted by: stealth71 Posted at: 2016-10-12T19:21:08.142Z Reads: 120

```
What charger are you using?  My charger came with it's own plug.
```

---
## \#3 Posted by: johnny_261 Posted at: 2016-10-12T19:21:56.394Z Reads: 118

```
https://www.aliexpress.com/item/1Pcs-Fast-Charging-Electric-Motor-Car-Battery-Charger-Li-ion-Battery-Packs-AC-25-2V-2A/32650153446.html

Didn't come with a plug which is why I had to buy some on ebay.
```

---
## \#4 Posted by: stealth71 Posted at: 2016-10-12T19:27:22.850Z Reads: 112

```
The picture on the charger is as you described.  Positive in the center and negative outside.

Here is a diagram from a supower BMS:
http://i1098.photobucket.com/albums/g378/lilianleung/13Slogo.jpg
```

---
## \#5 Posted by: johnny_261 Posted at: 2016-10-12T19:31:07.346Z Reads: 108

```
Thanks for confirming.  This is the wiring diagram I made.  Everything is wired up and tested except for the meter and the charging plug.  Just wanted to be really careful with it since this part is uncharted territory for me.

<img src="/uploads/db1493/original/3X/a/5/a5ffc810b6fe9304799519085fe8e35715927fa7.jpg" width="333" height="500">
```

---
## \#6 Posted by: Jcullinan09 Posted at: 2018-09-25T01:14:09.476Z Reads: 34

```
In the picture by @stealth71, the balance connector for channel 1 is connected to the first bridge from the whole batteries negative contact. 

HOWEVER, in @johnny_261's image the balance connector for channel 1 is connected to the ultimate negative contact of the whole battery.

Whose diagram is correct, and which one should I wire a 10s BMS to??
![50%20PM|334x500](upload://eQyDogBliDGpWumHqA9ixY7PU5J.png)![02%20PM|690x483](upload://3e2NtwlJc12rVJDM1ieEoYVRN0i.jpeg)
```

---
