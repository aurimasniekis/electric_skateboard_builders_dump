# Should I Consider My 18650 Li-Ion Cells &ldquo;Healthy&rdquo;?

### Replies: 14 Views: 1045

## \#1 Posted by: BLeaCH Posted at: 2018-01-15T06:53:30.732Z Reads: 162

```
Hi I began opening notebook batteries to take his 18650 Li-ion cells and use them to make a few battery packs, i know a lot of people are against about it, but where i live it's a lot pricey buy here and so difficult to import (chile) :angry: 

So, i started charging the good cells that i take from the notebook batteries with a B6 Mini (A original one, with PC port) but when the charger finish the charge with "4.2"v i measure it with the charger's meter or/and a multimeter and the voltage drop to an "4.1x"v on some cases the value it's lower than "4.0"v

Several sites promotes to check the healt of the cell charging the 18650 cell and wait a week or more and check to see a voltaje drop but... can i put the "healty" tag to a battery who was just full charged and measured with voltage drop on 0.0x volts and continue checking the capacity?

Can be this considered a good cell to folllow the next steps or it must be just charged on 4.2v to go on? And for the "week self discharge test" how much difference is a good discharge value to pass the test??

thanks for any answer and sorry for my bad english, but is not my first language and it's quite rusty D:
```

---
## \#2 Posted by: SOICDIP Posted at: 2018-01-15T06:56:50.826Z Reads: 156

```
Voltage dropping right after charging indicates high internal resistance, which points to an old cell.

Are these laptop packs new? Your B6 Mini has a discharge function. Try measuring the capacity.
```

---
## \#3 Posted by: Namasaki Posted at: 2018-01-15T07:07:17.193Z Reads: 145

```
The problem with using laptop cells is that they will most likely not be able to handle the current draw in an Esk8 application.
So their voltage will sag excessively and they could overheat and even go into thermal runaway which could cause a fire.
https://youtu.be/24fYrV2vCPk
```

---
## \#4 Posted by: bimmer Posted at: 2018-01-15T07:19:38.426Z Reads: 131

```
People arent against it because of superficial reasons( batteries cheap or not the best) they are against it because Laptop batteries are rated for 5A discharge so even at 10P you cannot build a pack that will last long or be very safe. As batteries  age they form dendrites like the spikes at the top of a  cave once  the dendrites short anode the cathode there is a thermal  runaway and the batteries explodes. The formation of said  dendrites is  increased by over high drain applications.
![dendrites|690x326](upload://rKHPAnJoMyClWZgO0G5loDuaSPD.jpg)
```

---
## \#5 Posted by: rojitor Posted at: 2018-01-15T14:19:39.016Z Reads: 107

```
Don't do it bro. Look for used battery packs or lipo.
Used cells have more resistance so more heat. Laptop are low C so you will have a crappy battery in best case scenario and a fire in the worst.
```

---
## \#6 Posted by: Acido Posted at: 2018-01-15T14:31:16.164Z Reads: 105

```
Buy some used cells or pay someone buy them for you and ship it to chile with a low package value so you don't pay customs
```

---
## \#7 Posted by: The_Bob Posted at: 2018-01-15T21:03:18.690Z Reads: 83

```
What about power tool batteries? Do they have a high enough C?
```

---
## \#8 Posted by: BLeaCH Posted at: 2018-01-16T06:39:30.181Z Reads: 72

```
No @SOICDIP , these battery packs are not brand new. the notebooks bateries are principally taken from used notebooks where i work
```

---
## \#9 Posted by: BLeaCH Posted at: 2018-01-16T06:53:58.091Z Reads: 69

```
thanks @bimmer, more clear it can't be. now i know and can explain the "internal" reasons about it

also thanks @Namasaki and @rojitor, i will see the best cells and take and give  a "no power motor" use, maybe to power an arduino proyect


but, how about use it with a fuse wire? i will prevent the overdischarge and the overheat?
```

---
## \#10 Posted by: BLeaCH Posted at: 2018-01-16T07:00:19.821Z Reads: 60

```
@The_Bob are you saying buy something like these bateries?

![imagen|690x398](upload://8ClqOiarOAcQjX09BpaQraRZ8LL.jpg)

these batteries are made for heavy duty tasks, will it work taking their sells to make an 6s battery?
```

---
## \#11 Posted by: BLeaCH Posted at: 2018-01-16T07:07:44.817Z Reads: 54

```
that's a quite good idea @acido, but i was wondering about the customs limitations about this kind of batteries for sites who buys for you.

i was thinking of use a site/service called "socialbuyers" where i pay to extrangers who came to my country to buy for me and bring to me, for a extra.
```

---
## \#12 Posted by: bimmer Posted at: 2018-01-16T07:12:48.367Z Reads: 50

```
http://www.batterysupports.com/36v-37v-42v-6000mah-60ah-30a-lithium-ion-liion-battery-pack-p-376.html
Pretty sure they'll ship anywhere :smiley:
```

---
## \#13 Posted by: Acido Posted at: 2018-01-16T07:37:11.139Z Reads: 46

```
Buy the envelope or whatever you are going to put it in, package the batteries at home and ship them if they ask whats inside say electronics Ive done this with 700wh batteries for ebikes
```

---
## \#14 Posted by: The_Bob Posted at: 2018-01-16T20:19:53.947Z Reads: 34

```
yeah, I mean taking the cells.
```

---
