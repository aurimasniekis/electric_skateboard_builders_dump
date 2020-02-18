# How long will a 6s 10,000mah lipo last

### Replies: 21 Views: 2065

## \#1 Posted by: Orin635 Posted at: 2017-09-26T19:42:10.134Z Reads: 145

```
Hi, guys, I am wondering how many km/miles my board will last. If anyone knows a website calculator (like calc.esk8.it) to find the distance. or even just know from experience

Planned specs:
Motor: Turnigy 280kv
Battery: (2x 3s 5000mah lipo)
Wheels: 59mm
Belt: 3:1 ratio
ESC: 120a x-car beast series
(I'm not sure if anything else will affect the distance if you need more info please just comment)
```

---
## \#2 Posted by: mmaner Posted at: 2017-09-26T19:46:16.471Z Reads: 141

```
http://esk8.today/2016/12/28/how-far-can-i-ride/
<img src="/uploads/db1493/original/3X/1/c/1cb8bc0e271f1cbf6f0d15f213092399c41968a0.png" width="314" height="500">
```

---
## \#3 Posted by: MysticalDork Posted at: 2017-09-26T19:48:01.607Z Reads: 130

```
Well for one thing, you would need 4 of those 3s 5000mah batteries to get 6s 10000mah. To answer your question, it would be 3.7*6*10 to get watt-hours like, then divide that by 10, because most setups use around 10 watt-hours per km.
```

---
## \#4 Posted by: Orin635 Posted at: 2017-09-26T19:48:47.502Z Reads: 125

```
why would i need 4 of the batterys do they not double?)
```

---
## \#5 Posted by: MysticalDork Posted at: 2017-09-26T19:50:10.315Z Reads: 122

```
Two 3s 5000mah batteries in series gives you a 6s 5000mah battery.

Two 3s 5000mah batteries in parallel gives you a 3s 10000mah battery. To get both 6s and 10000mah, you need 4 packs.
```

---
## \#6 Posted by: Orin635 Posted at: 2017-09-26T19:53:36.031Z Reads: 117

```
Thank you very much
```

---
## \#7 Posted by: Orin635 Posted at: 2017-09-26T19:54:13.568Z Reads: 115

```
that does not make sense are you sure about that?
```

---
## \#8 Posted by: Brycehoosiers Posted at: 2017-09-26T19:55:50.525Z Reads: 112

```
never heard that either doesn't make sense
```

---
## \#9 Posted by: Orin635 Posted at: 2017-09-26T19:58:00.370Z Reads: 108

```
ye :P just watching some videos on that now it says nothing like that
```

---
## \#10 Posted by: Orin635 Posted at: 2017-09-26T19:59:46.818Z Reads: 104

```
I think you are getting confused with your amps, mah and cells
```

---
## \#11 Posted by: MysticalDork Posted at: 2017-09-26T20:09:27.830Z Reads: 96

```
Nope. When you add cells together, you either get more volts, or more mAh, not both. I've built my own battery packs, I know my way around volts amps and watts.
```

---
## \#12 Posted by: MysticalDork Posted at: 2017-09-26T20:22:11.197Z Reads: 92

```
Search around about series and parallel. With just two packs, you can't have both series and parallel at the same time.
```

---
## \#13 Posted by: hornet90 Posted at: 2017-09-26T20:30:13.636Z Reads: 90

```
Ill jump in with 2 setups i had that where 6s 2x3s 5000mha 1 setup 7 miles the other was 6 miles
```

---
## \#14 Posted by: GrecoMan Posted at: 2017-09-26T20:30:58.600Z Reads: 89

```
@MysticalDork is spot on, adding cells in series increases voltage, adding cells in parallel increases capacity (ah/mah)

YOU NEED 4 3S 5000MAH BATTERIES TO ACHIEVE 6S 10,000MAH
```

---
## \#15 Posted by: darkkevind Posted at: 2017-09-26T20:32:08.488Z Reads: 92

```
@MysticalDork is absolutely right. Look it up...

If you parallel batteries, you their AMP output, you also up their MAH capacity.

When you put batteries in series, all you're really doing is getting more volts, the MAH and AMP rating stay the same....
```

---
## \#16 Posted by: Orin635 Posted at: 2017-09-26T20:44:32.294Z Reads: 85

```
I apologise, So which should I do series or parallel
```

---
## \#17 Posted by: JdogAwesome Posted at: 2017-09-26T20:46:10.918Z Reads: 83

```
You need at least 6S and with 2x 3S 5Ah in series you'll have a 6S 5Ah and you'll get about 4-6 Mile's of range depending on how fast you go. I have a 6S 10Ah pack which is made up of 4x 3S 5Ah Zippy Compact packs and I get about 10-14 miles of range.
```

---
## \#18 Posted by: GrecoMan Posted at: 2017-09-26T20:46:22.544Z Reads: 83

```
Series, VESC cant run on 3s
```

---
## \#19 Posted by: bartroosen12 Posted at: 2017-09-26T21:11:30.784Z Reads: 78

```
I guess you will get around 15-18km with 6S 10Ah
```

---
## \#20 Posted by: hornet90 Posted at: 2017-09-26T21:14:33.733Z Reads: 78

```
Whats your top speed
```

---
## \#21 Posted by: JdogAwesome Posted at: 2017-09-26T21:27:02.499Z Reads: 72

```
Well my old top speed with my original Carvon V2 single hub was 32MPH but withy new dual Maytech hubs I only get 20mph top speeds, though WAY better torque. Planning on changing my battery config to 12S once my BMS gets here.
```

---
