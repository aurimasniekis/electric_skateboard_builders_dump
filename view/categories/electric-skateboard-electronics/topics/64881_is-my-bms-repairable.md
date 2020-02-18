# Is my BMS repairable?

### Replies: 13 Views: 390

## \#1 Posted by: Winfly Posted at: 2018-08-14T22:16:50.030Z Reads: 89

```
I have a Bestech D140 10S charge only BMS from @thisguyhere. I heard something popped when plugged in the charger the other day and it wouldn't charge anymore. Turns out some of the components on the BMS fried. Is my BMS repairable? here are some pics:
![image|304x500](upload://gtskHtZ2HjcmToS5L8vI2tSrBk5.jpg)
Pretty sure that resistor next to B5 shouldnt be covered with solder
![image|690x364](upload://3HeXmKExALILGEP0gojzOBCdiXH.jpg)
(upload://tYV3LZ7RVXXDQSOyj0Iy9cA0XHP.jpg)
This smd resistor blew, does anyone know what exactly I need to replace it? a link to mouser or digitkey would be nice.
![image|304x500](upload://nttRSIJQy26gNSGyg2HAeSmneou.jpg)
here's an original pic pulled from his [website](http://esk8life.com/bestech-d140-10s), which has a slightly different layout: 
![image|312x351](upload://cxIxBqLZugefVyTsR8CAzi7YZJi.jpg)
```

---
## \#2 Posted by: thisguyhere Posted at: 2018-08-14T22:23:37.401Z Reads: 82

```
if you know how to solder SMD and can source those same components, suppose it'd be possible.  it's certainly beyond my abilities.

as with the stock image, it's exactly that, just sample images.  because they revise and modify their modules over time, and also the version we got is not exactly the same as the stock image, it's going to have differences.

try emailing donna@bestech.com with the exact images, hell just link her back to here and see if they can make any recommendations.

otherwise, you'd probably have to replace it.
```

---
## \#3 Posted by: Winfly Posted at: 2018-08-14T22:56:33.130Z Reads: 73

```
is that the right email address? my email bounced.
```

---
## \#4 Posted by: ThermalM16 Posted at: 2018-08-14T23:08:07.044Z Reads: 69

```
Hey, you can just grab a multimeter and test one of the other resistors in any of those other rows to find the resistance value of it. For stuff like that, I just wick the old solder off, throw some flux on, the add some solder to the new resistor, it's super easy. The size and shape of the resistor technically doesn't matter, as long as it can handle the same power as the previous one. 

However, after taking a look at that photo, the circled component looks more like it might be an SMD fuse or capacitor. If the other ones measure a resistance value close to 0, it's a fuse and you can just bridge it if you need it working asap.
```

---
## \#5 Posted by: Winfly Posted at: 2018-08-14T23:12:57.571Z Reads: 61

```
yeah the first one is easy to clean up. I need more help on getting the blown component replaced.
```

---
## \#6 Posted by: thisguyhere Posted at: 2018-08-14T23:15:06.606Z Reads: 57

```
my bad

Donna@BesTechPower.com

or maybe even their support email, info@BesTechPower.com
```

---
## \#7 Posted by: ThermalM16 Posted at: 2018-08-14T23:19:28.070Z Reads: 56

```
Is there only one resistor mounted there on your model?
```

---
## \#8 Posted by: Winfly Posted at: 2018-08-14T23:20:21.406Z Reads: 57

```
yeah I think thats a resistor right? a research of R005 2512 package on digitkey show me this https://www.digikey.com/products/en/resistors/chip-resistor-surface-mount/52?FV=ffe00034&quantity=0&ColumnSort=0&page=1&pageSize=25&k=R005+2512&pkeyword=R005
Dont know which one to get.
```

---
## \#9 Posted by: ThermalM16 Posted at: 2018-08-14T23:21:09.364Z Reads: 57

```
Yes, those bigger rectangle shaped ones are resistors
```

---
## \#10 Posted by: ThermalM16 Posted at: 2018-08-14T23:25:15.611Z Reads: 56

```
I'm not sure on the wattage they were using, but those look like current sense resistors. These should do the trick

https://www.ebay.com/itm/2512-Metal-Alloy-SMD-SMT-Chip-Resistors-1-1W-2W-3W-Range-0-001-to-0-5/253809453654?hash=item3b1838ea56%3Am%3Amzlaqac10oVMs34pdmYSt4Q&var=553094273429&_sacat=0&_nkw=0.005+ohm+resistor&_from=R40&rt=nc&_trksid=m570.l1313

I would see if you can get an answer from Bestech first just to double check before ordering those though
```

---
## \#11 Posted by: Winfly Posted at: 2018-08-14T23:29:00.087Z Reads: 48

```
Thanks. and yeah i'll wait for them to reply. would you say getting a 3W rather than 1W is safer?
```

---
## \#12 Posted by: threebysix Posted at: 2018-08-15T04:52:37.328Z Reads: 41

```
I believe higher wattage rating should be fine as long as the foot print is correct size.
```

---
## \#13 Posted by: Winfly Posted at: 2018-08-15T05:31:53.620Z Reads: 39

```
I took a caliper and found it to be 2512 package.
```

---
