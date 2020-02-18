# Help making a custom battery charger

### Replies: 19 Views: 3525

## \#1 Posted by: smurf Posted at: 2016-10-31T21:12:56.892Z Reads: 226

```
I would like to make a custom battery charger with adjustable voltage. I understand the basics but I could definitely use some help or advice .
Not sure where to get a decent 36V ac/dc power supply.

https://www.amazon.com/gp/product/B00LGKE2GQ/ref=pd_sbs_147_2?ie=UTF8&psc=1&refRID=BJ96PDG90GRDS6PKTH5Z

http://www.banggood.com/600W-Digital-Control-DC-DC-Adjustable-Step-Up-Module-Constant-Voltage-Current-Solar-Charging-p-1082316.html?rmmds=category

https://www.amazon.com/gp/product/B01GFVI6R6/ref=s9_simh_gw_g23_i1_r?ie=UTF8&fpl=fresh&pf_rd_m=ATVPDKIKX0DER&pf_rd_s=&pf_rd_r=C9V7KM3CHX465MGQ1HS7&pf_rd_t=36701&pf_rd_p=b21f7431-0e6c-4207-b08b-cc9492e60b0f&pf_rd_i=desktop
```

---
## \#2 Posted by: fuelre Posted at: 2016-10-31T23:54:01.867Z Reads: 194

```
Search for "meanwell"
```

---
## \#3 Posted by: smurf Posted at: 2016-11-01T01:04:02.751Z Reads: 184

```
One of these?

http://www.meanwell.com/productPdf.aspx?i=457

Or

http://www.meanwell.com/productPdf.aspx?i=716
```

---
## \#4 Posted by: jmasta Posted at: 2016-11-01T01:25:17.511Z Reads: 176

```
I was actually looking at buying that same step-up regulator 

This is much cheaper ($13) and should also work:  [https://www.amazon.com/dp/B019W4C5IE](https://www.amazon.com/dp/B019W4C5IE)
It has two potentiometers: one each for voltage and current regulation (most only have one potentiometer for voltage).  But I would want to add in a display for voltage and maybe even current. So that adds about $8-18 to the cost.  At that point, you might as well buy the numerical control VR
```

---
## \#5 Posted by: smurf Posted at: 2016-11-01T02:28:04.122Z Reads: 170

```
I don't think that one has cc-cv that we need to charge battery's
```

---
## \#6 Posted by: Pantologist Posted at: 2016-11-01T03:59:23.523Z Reads: 159

```
If you are charging 10S Lithium Ion pack, you'll need a 42V output charger. MeanWell is a good PSU manufacturer. 

I found some on eBay. 

http://www.ebay.com/itm/Mean-Well-CEN-100-42-AC-DC-Power-Supply-Single-OUT-42V-2-28A-95-76WUS-Authorized-/112057719924?hash=item1a17291c74:g:h~YAAOSw7aBVBOFq

http://www.ebay.com/itm/Mean-Well-OWA-60U-42-Plug-In-Adapter-Single-OUT-42V-1-5A-63W-US-Authorized-/122046856757?hash=item1c6a8f3e35:g:gsMAAOSwwbdWGuBW

http://www.ebay.com/itm/Mean-Well-OWA-90U-42-Plug-In-Adapter-Single-OUT-42V-2-15A-90-3W-US-Authorized-/112057716862?hash=item1a1729107e:g:hxkAAOSwT5tWG~A7
```

---
## \#7 Posted by: jmasta Posted at: 2016-11-01T06:09:27.405Z Reads: 148

```
[quote="Pantologist, post:6, topic:12218, full:true"]
If you are charging 10S Lithium Ion pack, you'll need a 42V output charger. MeanWell is a good PSU manufacturer.
[/quote]

That's probably the best and easiest option.  But you could use almost any power supply of sufficient wattage, paired with a step-up voltage regulator.  That's basically all those are

A 12S 4A charger is $85 after shipping, and you have to wait a month.  You could make the same thing for less money if you have power supply laying around.  It's not really worth if you have to buy a PSU... or if you don't know what you're doing ;)

Granted.. the only reason I am even considering this option is because a Chinese eBay seller screwed me over.  I bought a 12S charger and received a 16S charger with a hand-written label to "change" the voltage to 50.4V  (12S).  Good thing I checked with a DVM first
```

---
## \#8 Posted by: smurf Posted at: 2016-11-01T06:14:33.037Z Reads: 138

```
The whole point is to be able to charge 9s 10s 12s 14s all in one and to slightly drop voltage to extend battery life.
For example charging 10s at 41V

http://www.electric-skateboard.builders/t/cheap-chargers-with-customizeable-end-of-charge-voltage/6902
```

---
## \#9 Posted by: SageTX Posted at: 2017-05-13T22:59:37.344Z Reads: 106

```
What power supply did you end up getting? I have the same drok cc/cv controller and want to make a much higher amp charger for my lipos.

Did you ever complete this charging box?  Any pics/tips?
```

---
## \#10 Posted by: smurf Posted at: 2017-05-14T00:29:54.451Z Reads: 103

```
I want to figure out how to mount the display on the case.

https://www.instagram.com/p/BNh6IlUj1mQ/

That's a 36v 400 watt power supply
```

---
## \#11 Posted by: smurf Posted at: 2017-05-14T00:46:17.500Z Reads: 100

```
Knowing what I know now I would have just got this instead of even starting the project.

https://www.amazon.com/gp/product/B015RXDR5Y/ref=ox_sc_sfl_title_24?ie=UTF8&psc=1&smid=AMH4W1K8OCGMX
```

---
## \#12 Posted by: SageTX Posted at: 2017-05-14T01:01:23.866Z Reads: 96

```
Yeah, i haven't decided whether to just put the converter in a small box to convert _any_ power to what i need,  or to enclose a power supply with it.  
 I was just going to strip down a 3-400 watt pc power supply and throw that in there. But that would not make it very portable. (I basically live on the road).  :unamused:
```

---
## \#13 Posted by: Lambjr088 Posted at: 2017-05-14T02:08:08.867Z Reads: 94

```
For that price I'd rather get one of these

http://www.ebikes.ca/shop/electric-bicycle-parts/chargers/cycle-satiator.html

http://www.ebikes.ca/shop/electric-bicycle-parts/chargers/cycle-satiator-72v-5a.html
```

---
## \#14 Posted by: Hummie Posted at: 2017-05-14T02:18:47.301Z Reads: 94

```
I got a cheap one from amazon that was much cheaper than a meanwell. I've had both and prefer my 500 watt cheap one as the adjustable voltage screw often needs to be adjusted if at a low voltage with the less powerful version, so u have to fiddle with the tiny screw in that case as it steps up to differen higher voltages.
```

---
## \#15 Posted by: smurf Posted at: 2017-05-14T04:56:24.734Z Reads: 89

```
If you're on the road all the time you can power up the drok off the cigarette lighter power
http://www.dcpwr.com/shop/images/C2P-X.JPG
```

---
## \#16 Posted by: smurf Posted at: 2017-05-14T05:50:56.551Z Reads: 81

```
That's a great charger for 16S4P battery
```

---
## \#17 Posted by: Lambjr088 Posted at: 2017-05-14T06:07:59.825Z Reads: 79

```
Yea but they can be adjusted to power a 12s 10s 8s battery pack @smurf
```

---
## \#18 Posted by: smurf Posted at: 2017-05-14T07:19:58.698Z Reads: 79

```
How to put a drok in a box that's the topic
```

---
## \#19 Posted by: progrock Posted at: 2017-10-20T13:09:11.488Z Reads: 54

```
I gotta ask, did this build workout?... I just started looking into a DIY option for a variable voltage charger for EVs primarily.  I won't lie, I think I'll be ordering the Cycle Satiator in the next day or two... but I still can't understand why they don't hav ea ton of competition.  I don't really see what is so special that other companies don't build variable voltage chargers.  After some investigating, and the fact that I want a charger that can hit at least 100v, I came across the same board you did here, the B900W (and only $17.20 shipped on aliexpress).  I figure pairing this with a decent 24v LED power supply (same ones I've been using to power custom 3D printers), and it shouldn't take much more to have a variable voltage power supply that can be used to charge a large range of electric vehicles.   As for a case/box... I plan to design and print one myself, easy enough with Fusion360 and one of my 3D printers.  But I am very interested in hearing if you fared well with this build, or found out it was a really bad idea for some reason.
```

---
