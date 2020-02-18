# Electric bell/horn modded to remote

### Replies: 9 Views: 973

## \#1 Posted by: Funkypumpkin Posted at: 2018-04-10T21:09:01.486Z Reads: 138

```
Been lurking around this forum for a while now and noticed that there aren't any bell/horn options I would consider viable for electric skateboards.

I had an idea of adding an electric bell on the the remote itself. This way you could, with a click of a button, notify pedestrians that you are coming.

[Rockbros bell](https://www.ebay.com/itm/ROCKBROS-Cycling-Electric-Horn-MTB-Bike-Road-Bicycle-Handlebar-Alarm-Bell-Ring/352241184199?_trkparms=aid%3D888007%26algo%3DDISC.MBE%26ao%3D1%26asc%3D20131227121020%26meid%3D7030d9daf4c8411dbd06b6ffee75ad1d%26pid%3D100009%26rk%3D1%26rkt%3D1%26sd%3D382250163259%26itm%3D352241184199&_trksid=p2047675.c100009.m1982) was posted on a thread that discussed bell in general. I noticed it uses two coin batteries which I assume give 3V voltage. 
Regarding the remote I could only find Boosted board remote battery information which was a 3,7V 450mAh battery. I won't be using that exact remote, but for the examples sake lets use these specifications.

So I have three questions:
1. Is this a totally crazy/stupid idea?

2. Is this diagram I made right? (resistor and voltage wise) 
![Remote mod diagram|690x296](upload://iOCXUvNDJC5iIlVOYvxebHOzZDd.png)

3. Could the remote battery be replaced with a bigger battery for example [this one](https://www.ebay.com/itm/2-x-3-7V-750mAh-o-Battery-for-MJX-RC-Quadcopter-X200-X300C-X400-X500-X800-J3O1/253285963284?hash=item3af9051614:g:eUQAAOSwT2daH5Pj)?

Now I understand that the bell won't fit into the remote even with the silicone striped of it, but I'm thinking of taking just the board, button and speaker from it. I would design and 3d print a new housing for the whole remote.
```

---
## \#2 Posted by: b264 Posted at: 2018-04-10T21:14:35.052Z Reads: 117

```
What remote will you be using?
```

---
## \#3 Posted by: Funkypumpkin Posted at: 2018-04-10T21:15:23.912Z Reads: 116

```
Wowgo 2s remote most likely
```

---
## \#4 Posted by: Funkypumpkin Posted at: 2018-04-12T17:54:32.880Z Reads: 92

```
![1|690x366](upload://uph0k2wY3cJJPLFFbYCr0DATw43.PNG)

Updated the diagram and made calculations regarding resistor.

Could someone confirm I calculated correctly?
```

---
## \#5 Posted by: b264 Posted at: 2018-04-12T17:55:43.204Z Reads: 88

```
It's not.  You can't regulate the load at 3V with one resistor.  The voltage drop over the resistor will change based on load current.
```

---
## \#6 Posted by: Funkypumpkin Posted at: 2018-04-12T18:43:55.560Z Reads: 83

```
So I need a (linear) voltage regulator in stead of a resistor right? Or should it just be a diode since the voltage drop is only 0,7V?

[Would this work?](https://www.digikey.com/product-detail/en/microchip-technology/TC1262-3.0VAB/TC1262-3.0VAB-ND/442714)

Sorry it's been quite a while (15 years) since I did this stuff in school.
```

---
## \#7 Posted by: b264 Posted at: 2018-04-12T20:30:16.412Z Reads: 67

```
That would work if you only need 1.5W max or a diode Vdrop or the part you're trying to run might be okay with 2.8V - 4.2V you'll have to check
```

---
## \#8 Posted by: SkaterBoy58 Posted at: 2018-04-12T23:42:28.284Z Reads: 60

```
@Funkypumpkin  Hi - we seem to on similar builds here on upgrading remotes  with batteries and bells  see my post [mini remote upgrade](http://www.electric-skateboard.builders/t/mini-remote-ugrade/51991)

I am using identical bell to you - have you measured the bell current at 225mA as per diagram above ?   . Seems a bit high to me but I don't have my bell yet to measure current.
```

---
## \#9 Posted by: Funkypumpkin Posted at: 2018-04-13T05:55:33.463Z Reads: 49

```
Sweet! Good luck! This is absolute great we can compare notes ;)

I haven't measured anything yet since missing both the bell and the remote :frowning:
So this is all speculation at this point.
```

---
