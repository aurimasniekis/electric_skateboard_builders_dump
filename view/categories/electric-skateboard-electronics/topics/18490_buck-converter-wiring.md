# Buck Converter Wiring

### Replies: 10 Views: 1043

## \#1 Posted by: CaptainMerricka Posted at: 2017-03-03T00:50:34.703Z Reads: 137

```
Where do I need to switch the buck converter?
Can I leave it wired to the high voltage side and switch the low voltage side?
Or do I need to get a high voltage switch and switch the HV side?
```

---
## \#2 Posted by: Namasaki Posted at: 2017-03-03T01:15:57.784Z Reads: 133

```
If I'm not mistaken, the buck converter supplies 5v to the receiver.
For powering on and off you will need either a HV/HC E-Switch Like the Vedder switch or the one Torqueboards sells.
Or you will need to make a jumper with an XT90 aniti-spark connector.
```

---
## \#3 Posted by: smurf Posted at: 2017-03-03T19:44:55.709Z Reads: 109

```
Does it get warm if it is plugged in and not being used? If it is going to be mostly on switch the low voltage side with a cheap switch. But if it is going to be mostly off or gets hot switch before it.
```

---
## \#4 Posted by: Tampaesk8er Posted at: 2017-03-03T22:37:02.153Z Reads: 88

```
I bought this switch and im very happy with it.

diy-electric-skateboard-kits-parts/electric-skateboard-on-off-power-switch/
```

---
## \#5 Posted by: Stevemk14ebr Posted at: 2017-03-03T22:50:00.374Z Reads: 81

```
I bought the same switch and had it die. Just to show another side for an informed choice.
```

---
## \#6 Posted by: CaptainMerricka Posted at: 2017-03-04T21:54:57.651Z Reads: 68

```
I dont want the leds on all the time, only when it is dark so another switch is necessary. I would not use the vedder anti spark switch because another one would be overkill.  I did some math, and since the converter is 200W and I am running 36 volts, it only draws 6A max from the 36V side.  I found  this toggle rated for 16A at 250VDC but it is another 10 bucks shipped from mouser where as a 5v switch is easy to acquire. Sounds like I will need to get it though and switch the HV side since I imagine that they will be off most of the time. But since I also have head/taillights and another set of underglow leds I will add 2 5V switches to the LV side to switch between the two in addition to the main converter HV switch.
http://www.mouser.com/Search/ProductDetail.aspx?R=DK284-73virtualkey69100000virtualkey691-DK284-73
```

---
## \#7 Posted by: ninja Posted at: 2017-03-04T22:57:47.962Z Reads: 62

```
I have just a little 5A switch just before converter. 
I don't  want to converter work all the time, so i have switch before converter, and use it only when main switch is off. So if getting dark i turn off my board and then turn on that tiny converter switch, then turn on main switch(XT 90s or other anti spark switch). Main thing is not to use that small switch for LED lights while board is turned on. Never had issues with this 5A switch. Actually somebody told me that these LED lights with converter are not sucking much juice, so there is no spark anyway. All big bad ass current going to vesc. You can see that i'm talking truth, just take a volt meter/ indicator like what electric workers use, and connect it to battery while board is turned on- you will see that nothing sparks, even indicator wires are so tiny and not getting burned. So thing is that antis park is for main battery to vesc, rest things can be added with tiny wires and small switches. I had voltmeter on my board as well with 5a switch no sparks, nothing! :) 

But for me safer feeling is- that i operate those small switches when main power is off, and main power should be anti spark (XT90s super duper cheap and it really works, or other fancy anti spark switches that are too expensive for my opinion) ! 

Here is my converter:
 http://www.ebay.co.uk/itm/291692573003?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT

Here is my small switches (you can see 5a switch next to volt checker and other 5A switch to XT90s anti spark loop key:
<img src="/uploads/db1493/original/3X/9/8/98251b213434d562a19d3cd2f0a9aae928a8cf56.JPG" width="332" height="500"><img src="/uploads/db1493/original/3X/d/e/def389239aaaeb7a3f0be08e9bfcd0e525c19771.JPG" width="690" height="458">
```

---
## \#8 Posted by: CaptainMerricka Posted at: 2017-03-04T23:06:41.616Z Reads: 54

```
I got this converter. 
http://www.ebay.com/sch/i.html?_from=R40&_trksid=m570.l1313&_nkw=200W+15A+Voltage+Power+Buck+Converter+Step+Down+Module+DC-DC+8-60V+TO+1-36V+ZP&_sacat=0
```

---
## \#9 Posted by: smurf Posted at: 2017-03-05T00:45:44.812Z Reads: 52

```
Conversion efficiency: up to 94% :+1:
```

---
## \#10 Posted by: Redfire1 Posted at: 2018-03-23T16:54:28.318Z Reads: 32

```
@CaptainMerricka and any one who know I am very new trying to make my own skateboard,I bought a anti spark switch and want to adopt a on off switch to it with led 12v.I am going to used dual motor 2 3s lipo I 24v.I was to to is a resistor but can’t work out what resistor to us can anyone help please.these are my anti and on off switch ![image|230x500](upload://mYHgkQ73V1PhGFHS3rJxVgbMKhb.jpg)![image|374x500](upload://jGNChFdSIW6x60ZW6e1dchVpAa6.jpeg)
```

---
